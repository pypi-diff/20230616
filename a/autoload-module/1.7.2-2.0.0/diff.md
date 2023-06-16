# Comparing `tmp/autoload-module-1.7.2.tar.gz` & `tmp/autoload_module-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoload-module-1.7.2.tar", max compression
+gzip compressed data, was "autoload_module-2.0.0.tar", max compression
```

## Comparing `autoload-module-1.7.2.tar` & `autoload_module-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1070 2021-07-07 05:39:29.087584 autoload-module-1.7.2/LICENSE
--rw-r--r--   0        0        0     7847 2021-07-07 05:39:29.087584 autoload-module-1.7.2/README.md
--rw-r--r--   0        0        0      177 2021-07-07 05:39:29.087584 autoload-module-1.7.2/autoload/__init__.py
--rw-r--r--   0        0        0     1422 2021-07-07 05:39:29.087584 autoload-module-1.7.2/autoload/_context.py
--rw-r--r--   0        0        0      276 2021-07-07 05:39:29.087584 autoload-module-1.7.2/autoload/_globals.py
--rw-r--r--   0        0        0     5433 2021-07-07 05:39:29.087584 autoload-module-1.7.2/autoload/_import.py
--rw-r--r--   0        0        0      466 2021-07-07 05:39:29.087584 autoload-module-1.7.2/autoload/decorator.py
--rw-r--r--   0        0        0      128 2021-07-07 05:39:29.087584 autoload-module-1.7.2/autoload/exception.py
--rw-r--r--   0        0        0    11059 2021-07-07 05:39:29.087584 autoload-module-1.7.2/autoload/module_loader.py
--rw-r--r--   0        0        0     1277 2021-07-07 05:39:29.087584 autoload-module-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     8787 2021-07-07 05:39:35.316035 autoload-module-1.7.2/setup.py
--rw-r--r--   0        0        0     9014 2021-07-07 05:39:35.316693 autoload-module-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-16 07:17:01.066935 autoload_module-2.0.0/LICENSE
+-rw-r--r--   0        0        0     7857 2023-06-16 07:17:01.066935 autoload_module-2.0.0/README.md
+-rw-r--r--   0        0        0      177 2023-06-16 07:17:01.066935 autoload_module-2.0.0/autoload/__init__.py
+-rw-r--r--   0        0        0     1422 2023-06-16 07:17:01.066935 autoload_module-2.0.0/autoload/_context.py
+-rw-r--r--   0        0        0      276 2023-06-16 07:17:01.066935 autoload_module-2.0.0/autoload/_globals.py
+-rw-r--r--   0        0        0     5433 2023-06-16 07:17:01.066935 autoload_module-2.0.0/autoload/_import.py
+-rw-r--r--   0        0        0      466 2023-06-16 07:17:01.066935 autoload_module-2.0.0/autoload/decorator.py
+-rw-r--r--   0        0        0      128 2023-06-16 07:17:01.066935 autoload_module-2.0.0/autoload/exception.py
+-rw-r--r--   0        0        0    10960 2023-06-16 07:17:01.066935 autoload_module-2.0.0/autoload/module_loader.py
+-rw-r--r--   0        0        0     1202 2023-06-16 07:17:01.066935 autoload_module-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9076 1970-01-01 00:00:00.000000 autoload_module-2.0.0/PKG-INFO
```

### Comparing `autoload-module-1.7.2/LICENSE` & `autoload_module-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoload-module-1.7.2/README.md` & `autoload_module-2.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 ### Methods
 #### load_classes
 ```
 load_classes(
     src: str,
     excludes: Iterable[str] = (),
     recursive: bool = False,
-) -> Tuple[Type]:
+) -> Tuple[Type, ...]:
 ```
 This method read the Python package or module and return the tuple of class objects.
 
 - Directory
 ```
 pkg/
  ├ example.py
@@ -199,15 +199,15 @@
 
 #### load_functions
 ```
 load_functions(
     src: str,
     excludes: Iterable[str] = (),
     recursive: bool = False,
-) -> Tuple[Callable]:
+) -> Tuple[Callable, ...]:
 ```
 This method read the Python package or module and return the tuple of functions.
 The usage is the same as `load_classes`.
 
 ##### NOTE
 - To search class or function, **You must match the name of file, and the one of class or function.**
 For example, if you named the file `test_module.py`, you must name the class `TestModule` or the function `test_module`.
```

### Comparing `autoload-module-1.7.2/autoload/_context.py` & `autoload_module-2.0.0/autoload/_context.py`

 * *Files identical despite different names*

### Comparing `autoload-module-1.7.2/autoload/_import.py` & `autoload_module-2.0.0/autoload/_import.py`

 * *Files identical despite different names*

### Comparing `autoload-module-1.7.2/autoload/module_loader.py` & `autoload_module-2.0.0/autoload/module_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ._import import ImportableFactory, ImportOption
 
 __all__ = ("ModuleLoader", "ModuleLoaderSetting")
 
 from .exception import LoaderStrictModeError
 
 
-class __Private:
+class _Private:
     """Private namespace.
     If you do not want to expose, define here as much as possible.
     """
 
     THIS_FILE = os_path.basename(__file__)
     DEFAULT_EXCLUDES = ("__init__.py", THIS_FILE, "__pycache__")
 
@@ -42,18 +42,14 @@
         if base_path == "":
             return "/"
         if base_path.endswith("/"):
             return base_path[:-1]
         return base_path
 
 
-def _access_private():
-    return __Private
-
-
 @dataclass(frozen=True)
 class ModuleLoaderSetting:
     base_path: Optional[str] = None
     strict: bool = False
     singleton: bool = False
 
 
@@ -86,15 +82,15 @@
             return cls._instance
         base_path, strict = list(args) + [None] * (cls._INSTANCE_VAL_COUNT - len(args))
         base_path = kwargs.get("base_path") if base_path is None else base_path
         strict = kwargs.get("strict") if strict is None else strict
         if base_path is None:
             global_base_path = cls._setting.base_path
             base_path = (
-                _access_private().init_base_url(base_path)
+                _Private.init_base_url(base_path)
                 if global_base_path is None
                 else global_base_path
             )
         if strict is None:
             strict = cls._setting.strict
         ci = cls._instance
         if ci.base_path != base_path or ci.strict != strict:
@@ -116,15 +112,15 @@
         setting = ModuleLoader._setting
         if setting.singleton is True and hasattr(
             self, f"__{self.__class__.__name__}_base_path"
         ):
             return
         global_base_path, global_strict = setting.base_path, setting.strict
         self.__base_path: str = (
-            _access_private().init_base_url(base_path)
+            _Private.init_base_url(base_path)
             if global_base_path is None
             else global_base_path
         )
         self.__strict: bool = global_strict if strict is None else strict
 
     @property
     def base_path(self) -> str:
@@ -254,17 +250,16 @@
         excludes: Iterable[str] = (),
         recursive: bool = False,
     ) -> Tuple[Class_Or_Func, ...]:
         if src is None:
             raise TypeError("'src' parameter is required.")
         if not isinstance(src, str):
             raise TypeError("src variable must be string.")
-        private = _access_private()
-        exclude_files = list(private.DEFAULT_EXCLUDES)
-        exclude_files.append(os_path.basename(private.detect_call_path()))
+        exclude_files = list(_Private.DEFAULT_EXCLUDES)
+        exclude_files.append(os_path.basename(_Private.detect_call_path()))
         if excludes:
             if not iter(excludes):
                 raise TypeError("excludes variable must be iterable.")
             for exclude in excludes:
                 if not isinstance(exclude, str):
                     raise TypeError("The contents of the excludes must all be strings")
                 exclude_files.append(exclude)
```

### Comparing `autoload-module-1.7.2/pyproject.toml` & `autoload_module-2.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoload-module"
-version = "1.7.2"
+version = "2.0.0"
 description = "Python Autoload Module"
 authors = ["Hiroki Miyaji <nukoprogramming@gmail.com>"]
 license = "MIT"
 maintainers = ["Hiroki Miyaji <nukoprogramming@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/hiroki0525/autoload_module"
 repository = "https://github.com/hiroki0525/autoload_module"
@@ -21,22 +21,18 @@
     'Programming Language :: Python :: Implementation :: PyPy',
 ]
 packages = [
     { include = "autoload" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-flake8 = "^3.9.2"
-black = "^21.5b1"
-isort = "^5.8.0"
-mypy = "^0.812"
-pre-commit = "^2.12.1"
+pre-commit = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `autoload-module-1.7.2/setup.py` & `autoload_module-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,333 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: autoload-module
+Version: 2.0.0
+Summary: Python Autoload Module
+Home-page: https://github.com/hiroki0525/autoload_module
+License: MIT
+Keywords: python,import,autoload,autoload_module,metaprogramming,dynamic import
+Author: Hiroki Miyaji
+Author-email: nukoprogramming@gmail.com
+Maintainer: Hiroki Miyaji
+Maintainer-email: nukoprogramming@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries
+Project-URL: Documentation, https://github.com/hiroki0525/autoload_module
+Project-URL: Repository, https://github.com/hiroki0525/autoload_module
+Description-Content-Type: text/markdown
 
-packages = \
-['autoload']
+# autoload_module
+[![PyPI version](https://badge.fury.io/py/autoload-module.svg)](https://badge.fury.io/py/autoload-module)
+[![Test](https://github.com/hiroki0525/autoload_module/actions/workflows/test.yml/badge.svg)](https://github.com/hiroki0525/autoload_module/actions/workflows/test.yml)
+[![Downloads](https://pepy.tech/badge/autoload-module)](https://pepy.tech/project/autoload-module)
+<img src="https://img.shields.io/badge/license-MIT-blue.svg?style=flat" alt="MIT License image">
 
-package_data = \
-{'': ['*']}
+This library will give you comfortable Python metaprogramming.  
+The following is a plain example.
 
-setup_kwargs = {
-    'name': 'autoload-module',
-    'version': '1.7.2',
-    'description': 'Python Autoload Module',
-    'long_description': '# autoload_module\n[![PyPI version](https://badge.fury.io/py/autoload-module.svg)](https://badge.fury.io/py/autoload-module)\n[![Test](https://github.com/hiroki0525/autoload_module/actions/workflows/test.yml/badge.svg)](https://github.com/hiroki0525/autoload_module/actions/workflows/test.yml)\n[![Downloads](https://pepy.tech/badge/autoload-module)](https://pepy.tech/project/autoload-module)\n<img src="https://img.shields.io/badge/license-MIT-blue.svg?style=flat" alt="MIT License image">\n\nThis library will give you comfortable Python metaprogramming.  \nThe following is a plain example.\n\n- Directory\n```\nproject/\n ├ example.py\n └ validator/\n   ├ validator_a.py\n   ├ validator_b.py\n   └ validator_c.py\n```\n- example.py\n```python\nfrom autoload import ModuleLoader\n\ninput = "foo bar baz"\nloader = ModuleLoader()\n\n# Automatically import modules and return class objects\nvalidator_classes = loader.load_classes("validator")\ntry:\n    # initialize and execute method\n    [clazz().validate(input) for clazz in validator_classes]\nexcept:\n    print("input is invalid!!")\n```\n## Install\n```\npip install autoload-module\n```\n## Usage\n### Constructor\n```\nModuleLoader(\n  base_path: Optional[str] = None,\n  strict: bool = False\n)\n```\nThe ModuleLoader can be generated with no parameters.\nIn that case, the instance has the absolute path where\nit was initialized.  \n- Directory\n```\n/usr/local/src/project/\n  ├ example.py\n  └ validator/\n    ├ validator_a.py\n    ├ validator_b.py\n    └ validator_c.py\n```\n- example.py\n```python\nfrom autoload import ModuleLoader\n\n# The instance has \'/usr/local/src/project/\'\nloader = ModuleLoader()\n\n# load modules in the directory; \'/usr/local/src/project/validator/\'\nvalidator_classes = loader.load_classes("validator")\n```\nIf you want to change the base path, you must generate the ModuleLoader with an absolute path parameter.\n```python\nloader = ModuleLoader(\'/user/local/src/custom\')\n```\n\nAbout strict parameter, please see [here](#NOTE) .\n\nYou can also create global setting and initialize singleton object.\n```python\nfrom autoload import ModuleLoader\nimport os\n\n# global setting\nModuleLoader.set_setting(base_path=os.getcwd(), strict=True)\n\nloader_a = ModuleLoader()\nloader_b = ModuleLoader()\n\nprint(loader_a.base_path)\n# -> /Users/user1/abc\nprint(loader_b.base_path)\n# -> /Users/user1/abc\n\n# singleton setting\nModuleLoader.set_setting(singleton=True)\n\nloader_c = ModuleLoader()\nloader_d = ModuleLoader()\nloader_e = ModuleLoader(\'/test\')\n\nassert loader_c is loader_d # OK\nassert loader_c is loader_e # OK\n\n# The base_path is \'/Users/user1/abc\'\nassert loader_c.base_path is loader_e.base_path # OK\n```\n\n### Methods\n#### load_classes\n```\nload_classes(\n    src: str,\n    excludes: Iterable[str] = (),\n    recursive: bool = False,\n) -> Tuple[Type]:\n```\nThis method read the Python package or module and return the tuple of class objects.\n\n- Directory\n```\npkg/\n ├ example.py\n ├ __init__.py\n ├ config.yaml\n └ main/\n     ├ validator_a.py\n     ├ validator_b.py\n     ├ validator_c.py\n     └ sub/\n        ├ validator_d.py\n        └ validator_e.py\n```\n- validator_a.py\n```python\nclass ValidatorA:\n    def validate(self):\n        print("validateA!!")\n```\n- example.py\n```python\nloader = ModuleLoader()\n\n# Automatically read modules without \'__init__.py\', not py file, and this file.\n# return the tuple of ValidateA, ValidatorB, and ValidatorC class objects\nvalidator_classes = loader.load_classes("main")\n\n# initialize and execute method\n[clazz().validate() for clazz in validator_classes]\n# -> validateA!!\n# -> validateB!!\n# -> validateC!!\n```\nYou can also load only specific modules using `excludes` variable or `load_config` decorator as below.\n```python\n# Pattern1: \'excludes\'\n# \'excludes\' is a iterable object like tuple, list.\n# You must specify module names in \'excludes\'.\nvalidator_classes = loader.load_classes("main", ["validator_a"])\n\n[clazz().validate() for clazz in validator_classes]\n# -> validateB!!\n# -> validateC!!\n\n# Pattern2: \'load_config\'\nfrom autoload import load_config\n\n@load_config(load=False)\nclass ValidatorA:\n  def validate(self):\n    print("validateA!!")\n\nvalidator_classes = loader.load_classes("main")\n\n[clazz().validate() for clazz in validator_classes]\n# -> validateB!!\n# -> validateC!!\n```\nThis function will check directory structure recursively if you specify `recursive=True`. \n```python\n# \'recursive=False\' is default.\n# In this case, the loader will also check \'pkg/main/sub/\'.\nvalidator_classes = loader.load_classes("main", recursive=True)\n\n[clazz().validate() for clazz in validator_classes]\n# -> validateA!!\n# -> validateB!!\n# -> validateC!!\n# -> validateD!!\n# -> validateE!!\n```\nYou can specify `src` as below.\n```python\nloader.load_classes("main/validator_a.py")\nloader.load_classes("main.validator_a")\nloader.load_classes("./main/validator_a")\nloader.load_classes(".main.validator_a")\nloader.load_classes("main.sub.validator_d")\nloader.load_classes("./main/sub/validator_d")\nloader.load_classes("../otherpkg")\nloader.load_classes("..otherpkg")\n```\n\n#### load_functions\n```\nload_functions(\n    src: str,\n    excludes: Iterable[str] = (),\n    recursive: bool = False,\n) -> Tuple[Callable]:\n```\nThis method read the Python package or module and return the tuple of functions.\nThe usage is the same as `load_classes`.\n\n##### NOTE\n- To search class or function, **You must match the name of file, and the one of class or function.**\nFor example, if you named the file `test_module.py`, you must name the class `TestModule` or the function `test_module`.\nWhen you want to customize their name, use `@load_config` decorator.\n    - validator_a.py\n    ```python\n    from autoload import load_config\n  \n    @load_config()\n    class CustomValidator:\n        def validate(self):\n            print("validateA!!")\n    ```\n- You can also control the order of loaded class objects using `@load_config` decorator.\n    - validator_a.py\n    ```python\n    from autoload import load_config\n  \n    # sort in ascending order\n    @load_config(order=1)\n    class ValidatorA:\n        def validate(self):\n            print("validateA!!")\n    ```\n- If you decorate some classes or functions with `@load_config`, the loader will load them.\n  However, initialized `strict=True`, the loader denies multiple loading as below.\n  - pkg/validator_a.py\n  ```python\n  from autoload import load_config\n\n  # This will be loaded because of name\'s rule.\n  class ValidatorA:\n    def validate(self):\n        print("validateA!!")\n  \n  # Anything goes.\n  @load_config(order=2)\n  class Foo:\n    pass\n  ```\n  \n  - main.py\n  ```python\n  from autoload import ModuleLoader\n  from autoload.exception import LoaderStrictModeError\n  \n  loader = ModuleLoader()\n  # return ValidatorA and Foo class objects.\n  classes = loader.load_classes("pkg")\n\n  # ModuleLoader strictly try to load a class or function object\n  # per a Python module on a basis of its name.\n  strict_loader = ModuleLoader(strict=True)\n  try:\n    classes = strict_loader.load_classes("pkg")\n  except LoaderStrictModeError as e:\n    print(e)\n  # -> Loader can only load a \'ValidatorA\' class in validator_a module.\n  # -> Please check \'Foo\' in validator_a module.\n  ```\n#### load_class\n```\nload_class(file_name: str)\n```\nThis method read the Python file and return the class object.\n- Directory\n```\nproject/\n  ├ example.py\n  └ validator.py\n```\n- validator.py\n```python\nclass Validator:\n    def validate(self):\n        print("validate!!")\n```\n- example.py\n```python\nloader = ModuleLoader()\nclazz = loader.load_class("validator")\nclazz().validate()\n# -> validate!!\n```\nHow to specify `file_name` is the same as that of `load_classes`.\n\n#### load_function\n```\nload_function(file_name: str)\n```\nThis method read the Python file and return a function object.\nThe usage is the same as `load_class`.\n\n## License\nReleased under the MIT license.',
-    'author': 'Hiroki Miyaji',
-    'author_email': 'nukoprogramming@gmail.com',
-    'maintainer': 'Hiroki Miyaji',
-    'maintainer_email': 'nukoprogramming@gmail.com',
-    'url': 'https://github.com/hiroki0525/autoload_module',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.7,<4.0',
-}
+- Directory
+```
+project/
+ ├ example.py
+ └ validator/
+   ├ validator_a.py
+   ├ validator_b.py
+   └ validator_c.py
+```
+- example.py
+```python
+from autoload import ModuleLoader
 
+input = "foo bar baz"
+loader = ModuleLoader()
 
-setup(**setup_kwargs)
+# Automatically import modules and return class objects
+validator_classes = loader.load_classes("validator")
+try:
+    # initialize and execute method
+    [clazz().validate(input) for clazz in validator_classes]
+except:
+    print("input is invalid!!")
+```
+## Install
+```
+pip install autoload-module
+```
+## Usage
+### Constructor
+```
+ModuleLoader(
+  base_path: Optional[str] = None,
+  strict: bool = False
+)
+```
+The ModuleLoader can be generated with no parameters.
+In that case, the instance has the absolute path where
+it was initialized.  
+- Directory
+```
+/usr/local/src/project/
+  ├ example.py
+  └ validator/
+    ├ validator_a.py
+    ├ validator_b.py
+    └ validator_c.py
+```
+- example.py
+```python
+from autoload import ModuleLoader
+
+# The instance has '/usr/local/src/project/'
+loader = ModuleLoader()
+
+# load modules in the directory; '/usr/local/src/project/validator/'
+validator_classes = loader.load_classes("validator")
+```
+If you want to change the base path, you must generate the ModuleLoader with an absolute path parameter.
+```python
+loader = ModuleLoader('/user/local/src/custom')
+```
+
+About strict parameter, please see [here](#NOTE) .
+
+You can also create global setting and initialize singleton object.
+```python
+from autoload import ModuleLoader
+import os
+
+# global setting
+ModuleLoader.set_setting(base_path=os.getcwd(), strict=True)
+
+loader_a = ModuleLoader()
+loader_b = ModuleLoader()
+
+print(loader_a.base_path)
+# -> /Users/user1/abc
+print(loader_b.base_path)
+# -> /Users/user1/abc
+
+# singleton setting
+ModuleLoader.set_setting(singleton=True)
+
+loader_c = ModuleLoader()
+loader_d = ModuleLoader()
+loader_e = ModuleLoader('/test')
+
+assert loader_c is loader_d # OK
+assert loader_c is loader_e # OK
+
+# The base_path is '/Users/user1/abc'
+assert loader_c.base_path is loader_e.base_path # OK
+```
+
+### Methods
+#### load_classes
+```
+load_classes(
+    src: str,
+    excludes: Iterable[str] = (),
+    recursive: bool = False,
+) -> Tuple[Type, ...]:
+```
+This method read the Python package or module and return the tuple of class objects.
+
+- Directory
+```
+pkg/
+ ├ example.py
+ ├ __init__.py
+ ├ config.yaml
+ └ main/
+     ├ validator_a.py
+     ├ validator_b.py
+     ├ validator_c.py
+     └ sub/
+        ├ validator_d.py
+        └ validator_e.py
+```
+- validator_a.py
+```python
+class ValidatorA:
+    def validate(self):
+        print("validateA!!")
+```
+- example.py
+```python
+loader = ModuleLoader()
+
+# Automatically read modules without '__init__.py', not py file, and this file.
+# return the tuple of ValidateA, ValidatorB, and ValidatorC class objects
+validator_classes = loader.load_classes("main")
+
+# initialize and execute method
+[clazz().validate() for clazz in validator_classes]
+# -> validateA!!
+# -> validateB!!
+# -> validateC!!
+```
+You can also load only specific modules using `excludes` variable or `load_config` decorator as below.
+```python
+# Pattern1: 'excludes'
+# 'excludes' is a iterable object like tuple, list.
+# You must specify module names in 'excludes'.
+validator_classes = loader.load_classes("main", ["validator_a"])
+
+[clazz().validate() for clazz in validator_classes]
+# -> validateB!!
+# -> validateC!!
+
+# Pattern2: 'load_config'
+from autoload import load_config
+
+@load_config(load=False)
+class ValidatorA:
+  def validate(self):
+    print("validateA!!")
+
+validator_classes = loader.load_classes("main")
+
+[clazz().validate() for clazz in validator_classes]
+# -> validateB!!
+# -> validateC!!
+```
+This function will check directory structure recursively if you specify `recursive=True`. 
+```python
+# 'recursive=False' is default.
+# In this case, the loader will also check 'pkg/main/sub/'.
+validator_classes = loader.load_classes("main", recursive=True)
+
+[clazz().validate() for clazz in validator_classes]
+# -> validateA!!
+# -> validateB!!
+# -> validateC!!
+# -> validateD!!
+# -> validateE!!
+```
+You can specify `src` as below.
+```python
+loader.load_classes("main/validator_a.py")
+loader.load_classes("main.validator_a")
+loader.load_classes("./main/validator_a")
+loader.load_classes(".main.validator_a")
+loader.load_classes("main.sub.validator_d")
+loader.load_classes("./main/sub/validator_d")
+loader.load_classes("../otherpkg")
+loader.load_classes("..otherpkg")
+```
+
+#### load_functions
+```
+load_functions(
+    src: str,
+    excludes: Iterable[str] = (),
+    recursive: bool = False,
+) -> Tuple[Callable, ...]:
+```
+This method read the Python package or module and return the tuple of functions.
+The usage is the same as `load_classes`.
+
+##### NOTE
+- To search class or function, **You must match the name of file, and the one of class or function.**
+For example, if you named the file `test_module.py`, you must name the class `TestModule` or the function `test_module`.
+When you want to customize their name, use `@load_config` decorator.
+    - validator_a.py
+    ```python
+    from autoload import load_config
+  
+    @load_config()
+    class CustomValidator:
+        def validate(self):
+            print("validateA!!")
+    ```
+- You can also control the order of loaded class objects using `@load_config` decorator.
+    - validator_a.py
+    ```python
+    from autoload import load_config
+  
+    # sort in ascending order
+    @load_config(order=1)
+    class ValidatorA:
+        def validate(self):
+            print("validateA!!")
+    ```
+- If you decorate some classes or functions with `@load_config`, the loader will load them.
+  However, initialized `strict=True`, the loader denies multiple loading as below.
+  - pkg/validator_a.py
+  ```python
+  from autoload import load_config
+
+  # This will be loaded because of name's rule.
+  class ValidatorA:
+    def validate(self):
+        print("validateA!!")
+  
+  # Anything goes.
+  @load_config(order=2)
+  class Foo:
+    pass
+  ```
+  
+  - main.py
+  ```python
+  from autoload import ModuleLoader
+  from autoload.exception import LoaderStrictModeError
+  
+  loader = ModuleLoader()
+  # return ValidatorA and Foo class objects.
+  classes = loader.load_classes("pkg")
+
+  # ModuleLoader strictly try to load a class or function object
+  # per a Python module on a basis of its name.
+  strict_loader = ModuleLoader(strict=True)
+  try:
+    classes = strict_loader.load_classes("pkg")
+  except LoaderStrictModeError as e:
+    print(e)
+  # -> Loader can only load a 'ValidatorA' class in validator_a module.
+  # -> Please check 'Foo' in validator_a module.
+  ```
+#### load_class
+```
+load_class(file_name: str)
+```
+This method read the Python file and return the class object.
+- Directory
+```
+project/
+  ├ example.py
+  └ validator.py
+```
+- validator.py
+```python
+class Validator:
+    def validate(self):
+        print("validate!!")
+```
+- example.py
+```python
+loader = ModuleLoader()
+clazz = loader.load_class("validator")
+clazz().validate()
+# -> validate!!
+```
+How to specify `file_name` is the same as that of `load_classes`.
+
+#### load_function
+```
+load_function(file_name: str)
+```
+This method read the Python file and return a function object.
+The usage is the same as `load_class`.
+
+## License
+Released under the MIT license.
```

