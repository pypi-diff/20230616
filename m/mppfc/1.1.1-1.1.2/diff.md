# Comparing `tmp/mppfc-1.1.1.tar.gz` & `tmp/mppfc-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mppfc-1.1.1.tar", max compression
+gzip compressed data, was "mppfc-1.1.2.tar", max compression
```

## Comparing `mppfc-1.1.1.tar` & `mppfc-1.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-01-03 11:43:04.716668 mppfc-1.1.1/LICENSE
--rw-r--r--   0        0        0     6384 2023-02-02 17:20:24.570224 mppfc-1.1.1/README.md
--rw-r--r--   0        0        0      265 2023-02-02 11:20:34.630027 mppfc-1.1.1/mppfc/__init__.py
--rw-r--r--   0        0        0    21966 2023-02-02 17:13:58.437077 mppfc-1.1.1/mppfc/cache.py
--rw-r--r--   0        0        0    23819 2023-02-02 11:52:06.656988 mppfc-1.1.1/mppfc/mppfc.py
--rw-r--r--   0        0        0      617 2023-02-02 17:19:11.407524 mppfc-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     7221 1970-01-01 00:00:00.000000 mppfc-1.1.1/setup.py
--rw-r--r--   0        0        0     7069 1970-01-01 00:00:00.000000 mppfc-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-01-03 11:43:04.716668 mppfc-1.1.2/LICENSE
+-rw-r--r--   0        0        0     6384 2023-02-02 17:20:24.570224 mppfc-1.1.2/README.md
+-rw-r--r--   0        0        0      265 2023-02-02 11:20:34.630027 mppfc-1.1.2/mppfc/__init__.py
+-rw-r--r--   0        0        0    23319 2023-06-16 07:10:56.280947 mppfc-1.1.2/mppfc/cache.py
+-rw-r--r--   0        0        0    23819 2023-06-16 07:10:56.260947 mppfc-1.1.2/mppfc/mppfc.py
+-rw-r--r--   0        0        0      617 2023-06-16 07:09:01.542969 mppfc-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7221 1970-01-01 00:00:00.000000 mppfc-1.1.2/setup.py
+-rw-r--r--   0        0        0     7069 1970-01-01 00:00:00.000000 mppfc-1.1.2/PKG-INFO
```

### Comparing `mppfc-1.1.1/LICENSE` & `mppfc-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mppfc-1.1.1/README.md` & `mppfc-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mppfc-1.1.1/mppfc/cache.py` & `mppfc-1.1.2/mppfc/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # python imports
-from functools import partial
 import hashlib
 import inspect
+import warnings
 from inspect import signature
 import logging
 import os
 import pathlib
 import pickle
+from time import perf_counter_ns
 from typing import Any, Callable, Union
 from types import FunctionType
 
 # third party imports
 import binfootprint
 
 hex_alphabet = "0123456789abcdef"
 
 log = logging.getLogger(__name__)
 log.setLevel("DEBUG")
 
 
 class CacheFileBased:
+    cache_flags = ["no_cache", "update", "has_key", "cache_only"]
+
     def __init__(
         self,
         fnc: FunctionType,
         path: Union[str, pathlib.Path] = ".cache",
         include_module_name: bool = True,
     ):
         """
@@ -175,28 +178,33 @@
         """
         try:
             return f_name.exists()
         except FileNotFoundError:
             return False
 
     @staticmethod
-    def _write_item(f_name: pathlib.Path, item: Any) -> None:
+    def _write_item(f_name: pathlib.Path, item: Any, delta_t: float = None) -> None:
         """
         writes item to disk at location f_name
 
+        Optionally write also the time it took to do the calculation.
+
         Removes partially written file on InterruptError.
 
         Args:
             f_name: Path object, where to dump the item
             item: the python object to be dumped
+            delta_t: time it took to do the calculation
         """
         f_name.parent.mkdir(parents=True, exist_ok=True)
         try:
             with open(f_name, "wb") as f:
                 pickle.dump(item, f)
+                if delta_t is not None:
+                    pickle.dump(delta_t, f)
         except Exception:
             os.remove(f_name)
             raise
 
     def __call__(
         self, *args: Any, _cache_flag: Union[str, None] = None, **kwargs: Any
     ) -> Any:
@@ -209,14 +217,19 @@
                 'update': Call `fnc` and update the cache with recent return value.
                 'has_key': Return `True` if the call has already been cached, otherwise `False`.
                 'cache_only': Return result from cache. Raises a `KeyError` if the result has not been cached yet.
 
         Returns:
             The result of `fnc(*args, **kwargs)`. If `_cache_flag == 'has_key'` return a boolean.
         """
+        if _cache_flag and _cache_flag not in self.cache_flags:
+            raise ValueError(
+                f"_cache_flag has unknown value '{_cache_flag}', expect one out of {self.cache_flags}  "
+            )
+
         if _cache_flag == "no_cache":
             return self.fnc(*args, **kwargs)
         else:
             f_name = self.get_f_name(*args, **kwargs)
             item_exists = self.item_exists(f_name)
 
             if _cache_flag == "has_key":
@@ -227,16 +240,18 @@
                         "Item not found in cache! (File '{}' does not exist.)".format(
                             f_name
                         )
                     )
                 with open(f_name, "rb") as f:
                     return pickle.load(f)
             elif (not item_exists) or (_cache_flag == "update"):
+                t_0 = perf_counter_ns()
                 r = self.fnc(*args, **kwargs)
-                self._write_item(f_name=f_name, item=r)
+                delta_t_in_sec = (perf_counter_ns() - t_0) / 10**9
+                self._write_item(f_name=f_name, item=r, delta_t=delta_t_in_sec)
                 return r
             else:
                 with open(f_name, "rb") as f:
                     return pickle.load(f)
 
     def set_result(
         self,
@@ -260,14 +275,34 @@
             raise ValueError(
                 "Result has already been cached! "
                 + "Set '_cache_overwrite' to True to force an update."
             )
         f_name.parent.mkdir(parents=True, exist_ok=True)
         self._write_item(f_name=f_name, item=_cache_result)
 
+    def get_calculation_time(self, *args: Any, **kwargs: Any) -> [float, None]:
+        """
+        return the time it took to do the calculation
+
+        If no data is available return None
+        """
+        f_name = self.get_f_name(*args, **kwargs)
+        item_exists = self.item_exists(f_name)
+        if not item_exists:
+            raise KeyError(
+                "Item not found in cache! (File '{}' does not exist.)".format(f_name)
+            )
+
+        with open(f_name, "rb") as f:
+            pickle.load(f)
+            try:
+                return pickle.load(f)
+            except EOFError:
+                warnings.warn("no information for the calculation time stored!")
+
 
 class CacheFileBasedDec:
     """
     Provides a decorator to cache the return values of a function to disk.
     """
 
     def __init__(
```

### Comparing `mppfc-1.1.1/mppfc/mppfc.py` & `mppfc-1.1.2/mppfc/mppfc.py`

 * *Files identical despite different names*

### Comparing `mppfc-1.1.1/pyproject.toml` & `mppfc-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mppfc"
-version = "1.1.1"
+version = "1.1.2"
 description = "multi-processing persistent function cache"
 authors = ["Richard Hartmann <richard_hartmann@gmx.de>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `mppfc-1.1.1/setup.py` & `mppfc-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['binfootprint>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'mppfc',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'multi-processing persistent function cache',
     'long_description': '# mppfc - Multi-Processing Persistent Function Cache\n\n[![PyPI version](https://badge.fury.io/py/mppfc.svg)](https://badge.fury.io/py/mppfc)\n\nThe `mppfc` module allows to speed up the evaluation of computationally \nexpansive functions by \na) processing several arguments in parallel and \nb) persistent caching of the results to disk.\nPersistent caching becomes available by simply decorating a given function.\nWith no more than two extra lines of code, parallel evaluation is realized.\n\nHere is a [minimal example](https://github.com/richard-hartmann/mppfc/blob/main/examples/minimal.py):\n\n```python\nimport mppfc\n\n@mppfc.MultiProcCachedFunctionDec()\ndef slow_function(x):\n    # complicated stuff\n    return x\n\nslow_function.start_mp()\nfor x in some_range:\n    y = slow_function(x)\nslow_function.wait()\n```\nThe first time you run this script, all `y` are `None`, since the evaluation \nis done by several background processes.\nOnce `wait()` returns, all parameters have been cached to disk.\nSo calling the script a second time yields (almost immediately) the\ndesired results in `y`.\n\nEvaluating only the `for` loop in a jupyter notebook cell\nwill give you partial results if the background processes are still doing some work.\nIn that way you can already show successfully retrieved results.\n(see the examples [simple.ipynb](https://github.com/richard-hartmann/mppfc/blob/main/examples/simple.ipynb) \nand [live_update.ipynb](https://github.com/richard-hartmann/mppfc/blob/main/examples/live_update.ipynb))\n\nFor a nearly exhaustive example see [full.py](https://github.com/richard-hartmann/mppfc/blob/main/examples/full.py).\n\n### caching class instantiation\n\n*new in Version 1.1*\n\nWhen class instantiation, i.e. calling `__init__(...)` takes very long, you can cache the instantiation\nby subclassing from `mppfc.CacheInit`.\n\n```python\nclass SomeClass(mppfc.CacheInit):\n    """instantiation is being cached simply by subclassing from `CacheInit`"""\n    def __init__(self, a, t=1):\n        time.sleep(t)\n        self.a = a\n```\n\nNote that subclassing such a cached class is not supported.\nIf you try that, a `CacheInitSubclassError` is raised.\nHowever, you can simply circumvent this problem by creating a dummy class for caching, e.g.\n\n```python\nclass S0:\n    s0 = \'s0\'\n\nclass S1(S0):\n    s1 = \'s1\'\n    def __init__(self, s):\n        self.s = s\n\nclass S1Cached(mppfc.CacheInit, S1):\n    """dummy \'subclass\' of S1 with caching"""\n    def __init__(self, s):\n        super().__init__(s)\n\nclass S2(mppfc.CacheInit, S1):\n    """S2 inherits from S1 AND is being cached"""\n    s2 = "s2"\n    def __init__(self, s):\n        super().__init__(s)\n```\n\nWhen subclassing from `CacheInit` the following extra keyword arguments can be used\nto control the Cache\n\n* `_CacheInit_serializer`: a function which serializes an object to binary data\n    (default is binfootprint.dump).\n* `_CacheInit_path`: the path where to put the cache data (default is \'.CacheInit\')\n* `_CacheInit_include_module_name`: if `True` (default) include the name of module where the class\n   is defined into the path where the instances will be cached.\n   (useful during development stage where Classes might be moved around or module name are still\n   under debate)\n\n### pitfalls\n\nNote that arguments are distinguished by their binary representation obtained from the \n[binfootprint](https://github.com/richard-hartmann/binfootprint) module.\nThis implies that the integer `1` and the float `1.0` are treated as different arguments, even though\nin many numeric situations the result does not differ.\n\n```python\nimport mppfc\nimport math\n\n@mppfc.MultiProcCachedFunctionDec()\ndef pitfall_1(x):\n    return math.sqrt(x)\n\nx = 1\nprint("pitfall_1(x={}) = {}".format(x, pitfall_1(x=x)))\n# pitfall_1(x=1) = 1.0\nx = 1.0\nprint("BUT, x={} in cache: {}".format(x, pitfall_1(x=x, _cache_flag="has_key")))\n# BUT, x=1.0 in cache: False\nprint("and obviously: pitfall_1(x={}) = {}".format(x, pitfall_1(x=x, _cache_flag="no_cache")))\n# and obviously: pitfall_1(x=1.0) = 1.0\n```\n\nThe same holds true for lists and tuples.\n\n```python\nimport mppfc\nimport math\n\n@mppfc.MultiProcCachedFunctionDec()\ndef pitfall_2(arr):\n    return sum(arr)\n\narr = [1, 2, 3]\nprint("pitfall_2(arr={}) = {}".format(arr, pitfall_2(arr=arr)))\n# pitfall_2(arr=[1, 2, 3]) = 6\narr = (1, 2, 3)\nprint("BUT, arr={} in cache: {}".format(arr, pitfall_2(arr=arr, _cache_flag="has_key")))\n# BUT, arr=(1, 2, 3) in cache: False\nprint("and obviously: pitfall_1(arr={}) = {}".format(arr, pitfall_2(arr=arr, _cache_flag="no_cache")))\n# and obviously: pitfall_1(arr=(1, 2, 3)) = 6\n```\n\nFor more details see [binfootprint\'s README](https://github.com/richard-hartmann/binfootprint).\n\n## ToDo\n\n- Set the signature of the wrapper `_cached_init` to the signature of `cls.__init__` (if possible).\n  Probably requires some MetaClass programming.\n- Create online documentation with mkdocs.\n\n\n## Installation\n\n### pip\n\n    pip install mppfc\n\n### poetry\n\nUsing poetry allows you to include this package in your project as a dependency.\n\n### git\n\ncheck out the code from github\n\n    git clone https://github.com/richard-hartmann/mppfc.git\n\n## Dependencies\n\n - requires at least python 3.8\n - uses [`binfootprint`](https://github.com/richard-hartmann/binfootprint) \n   to serialize and hash the arguments of a function \n\n## Licence\n\n### MIT licence\nCopyright (c) 2023 Richard Hartmann\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n',
     'author': 'Richard Hartmann',
     'author_email': 'richard_hartmann@gmx.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mppfc-1.1.1/PKG-INFO` & `mppfc-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mppfc
-Version: 1.1.1
+Version: 1.1.2
 Summary: multi-processing persistent function cache
 License: MIT
 Author: Richard Hartmann
 Author-email: richard_hartmann@gmx.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

