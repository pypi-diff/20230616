# Comparing `tmp/featherplot-0.0.1.tar.gz` & `tmp/featherplot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featherplot-0.0.1.tar", last modified: Fri Jun 16 18:02:57 2023, max compression
+gzip compressed data, was "featherplot-0.0.2.tar", last modified: Fri Jun 16 19:09:07 2023, max compression
```

## Comparing `featherplot-0.0.1.tar` & `featherplot-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 18:02:57.673818 featherplot-0.0.1/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 featherplot-0.0.1/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 featherplot-0.0.1/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     1788 2023-06-16 18:02:57.673689 featherplot-0.0.1/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1181 2023-06-16 13:10:42.000000 featherplot-0.0.1/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 18:02:57.672045 featherplot-0.0.1/featherplot/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-16 17:59:21.000000 featherplot-0.0.1/featherplot/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    17002 2023-06-16 17:59:21.000000 featherplot-0.0.1/featherplot/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     1574 2023-06-16 17:59:21.000000 featherplot-0.0.1/featherplot/commands.py
--rw-r--r--   0 solst      (501) staff       (20)      209 2023-06-16 17:59:21.000000 featherplot-0.0.1/featherplot/constants.py
--rw-r--r--   0 solst      (501) staff       (20)      406 2023-06-16 11:36:56.000000 featherplot-0.0.1/featherplot/dataclasses.py
--rw-r--r--   0 solst      (501) staff       (20)     4366 2023-06-16 17:59:21.000000 featherplot-0.0.1/featherplot/deepscatter.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-16 17:59:21.000000 featherplot-0.0.1/featherplot/files.py
--rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-16 17:59:21.000000 featherplot-0.0.1/featherplot/paths.py
--rw-r--r--   0 solst      (501) staff       (20)      241 2023-06-16 17:59:21.000000 featherplot-0.0.1/featherplot/rich.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-16 17:59:21.000000 featherplot-0.0.1/featherplot/typer.py
--rw-r--r--   0 solst      (501) staff       (20)     6173 2023-06-16 17:59:21.000000 featherplot-0.0.1/featherplot/types.py
--rw-r--r--   0 solst      (501) staff       (20)    19929 2023-06-16 17:59:21.000000 featherplot-0.0.1/featherplot/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 18:02:57.673480 featherplot-0.0.1/featherplot.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     1788 2023-06-16 18:02:57.000000 featherplot-0.0.1/featherplot.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      572 2023-06-16 18:02:57.000000 featherplot-0.0.1/featherplot.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 18:02:57.000000 featherplot-0.0.1/featherplot.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)      115 2023-06-16 18:02:57.000000 featherplot-0.0.1/featherplot.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 11:34:58.000000 featherplot-0.0.1/featherplot.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-16 18:02:57.000000 featherplot-0.0.1/featherplot.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)       12 2023-06-16 18:02:57.000000 featherplot-0.0.1/featherplot.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)     1066 2023-06-16 17:53:09.000000 featherplot-0.0.1/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-16 18:02:57.673860 featherplot-0.0.1/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 featherplot-0.0.1/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 19:09:07.774103 featherplot-0.0.2/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 featherplot-0.0.2/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 featherplot-0.0.2/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     1788 2023-06-16 19:09:07.773965 featherplot-0.0.2/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1181 2023-06-16 13:10:42.000000 featherplot-0.0.2/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 19:09:07.772621 featherplot-0.0.2/featherplot/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    17256 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     1574 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)      209 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/constants.py
+-rw-r--r--   0 solst      (501) staff       (20)      406 2023-06-16 11:36:56.000000 featherplot-0.0.2/featherplot/dataclasses.py
+-rw-r--r--   0 solst      (501) staff       (20)     4366 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/deepscatter.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/files.py
+-rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/paths.py
+-rw-r--r--   0 solst      (501) staff       (20)      241 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)     6565 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/types.py
+-rw-r--r--   0 solst      (501) staff       (20)    20001 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 19:09:07.773766 featherplot-0.0.2/featherplot.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     1788 2023-06-16 19:09:07.000000 featherplot-0.0.2/featherplot.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      572 2023-06-16 19:09:07.000000 featherplot-0.0.2/featherplot.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 19:09:07.000000 featherplot-0.0.2/featherplot.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)      115 2023-06-16 19:09:07.000000 featherplot-0.0.2/featherplot.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 11:34:58.000000 featherplot-0.0.2/featherplot.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-16 19:09:07.000000 featherplot-0.0.2/featherplot.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)       12 2023-06-16 19:09:07.000000 featherplot-0.0.2/featherplot.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      870 2023-06-16 19:08:48.000000 featherplot-0.0.2/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-16 19:09:07.774144 featherplot-0.0.2/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 featherplot-0.0.2/setup.py
```

### Comparing `featherplot-0.0.1/LICENSE` & `featherplot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.1/PKG-INFO` & `featherplot-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featherplot
-Version: 0.0.1
+Version: 0.0.2
 Summary: featherplot
 Home-page: https://github.com/dsm-72/featherplot-py
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `featherplot-0.0.1/README.md` & `featherplot-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.1/featherplot/_modidx.py` & `featherplot-0.0.2/featherplot/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,16 @@
                                          'featherplot.deepscatter.parse_args': ( 'deepscatter.html#parse_args',
                                                                                  'featherplot/deepscatter.py')},
             'featherplot.files': {},
             'featherplot.paths': {},
             'featherplot.rich': {},
             'featherplot.typer': {},
             'featherplot.types': { 'featherplot.types.BaseChannel': ('types.html#basechannel', 'featherplot/types.py'),
+                                   'featherplot.types.BaseChannel.export_tuple_as_list': ( 'types.html#basechannel.export_tuple_as_list',
+                                                                                           'featherplot/types.py'),
                                    'featherplot.types.BaseChannel.to_dict': ('types.html#basechannel.to_dict', 'featherplot/types.py'),
                                    'featherplot.types.BaseChannel.to_meta': ('types.html#basechannel.to_meta', 'featherplot/types.py'),
                                    'featherplot.types.BasicBooleanChannel': ('types.html#basicbooleanchannel', 'featherplot/types.py'),
                                    'featherplot.types.BasicChannel': ('types.html#basicchannel', 'featherplot/types.py'),
                                    'featherplot.types.BasicChannelError': ('types.html#basicchannelerror', 'featherplot/types.py'),
                                    'featherplot.types.BasicColorChannel': ('types.html#basiccolorchannel', 'featherplot/types.py'),
                                    'featherplot.types.CategoricalChannel': ('types.html#categoricalchannel', 'featherplot/types.py'),
```

### Comparing `featherplot-0.0.1/featherplot/commands.py` & `featherplot-0.0.2/featherplot/commands.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.1/featherplot/deepscatter.py` & `featherplot-0.0.2/featherplot/deepscatter.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.1/featherplot/paths.py` & `featherplot-0.0.2/featherplot/paths.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.1/featherplot/types.py` & `featherplot-0.0.2/featherplot/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
            'TransformTypeGuard', 'QuadFeatherColumnTypeGuard', 'BaseChannel', 'ConditionalChannel', 'LambdaChannel',
            'ConstantBool', 'ConstantNumber', 'ConstantColor', 'BasicChannel', 'BasicBooleanChannel',
            'CategoricalChannel', 'BasicColorChannel', 'CategoricalColorChannel']
 
 # %% ../nbs/03_types.ipynb 3
 from rich.repr import auto as rich_auto
 from dataclasses import dataclass, field, asdict
-from typing import Optional, Union, Any, List, TypeAlias, Literal, Tuple, get_args
+from typing import Optional, Union, Any, List, TypeAlias, Literal, Tuple, get_args, Dict
 
 # %% ../nbs/03_types.ipynb 4
 #| export
 
 
 # %% ../nbs/03_types.ipynb 5
 QUADFEATHER_REQUIRED_COLUMNS: TypeAlias = Literal['x', 'y']
@@ -120,17 +120,29 @@
 
 Conditional: TypeAlias = Union[SingleArgumentConditonal, TwoArgumentConditional]
 
 @rich_auto
 @dataclass
 class BaseChannel:
     field: str
+
+    def export_tuple_as_list(self, d:Dict[str, Any], key:str) -> Dict[str, Any]:
+        val = d.get(key, None)
+        if val is not None:
+            if type(val) == tuple:
+                d[key] = list(val)
+        return d
     
     def to_dict(self) -> dict:
         d = asdict(self)
+
+        d = self.export_tuple_as_list(d, 'range')
+        d = self.export_tuple_as_list(d, 'domain')
+        d = self.export_tuple_as_list(d, 'categories')
+
         if 'human' in d and d['human'] is None:
             del d['human']
         if 'categories' in d and d['categories'] is None:
             del d['categories']
         return d
     
     def to_meta(self) -> dict:
```

### Comparing `featherplot-0.0.1/featherplot/utils.py` & `featherplot-0.0.2/featherplot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,17 +109,17 @@
 # %% ../nbs/04_utils.ipynb 10
 def create_lambda_channel(field: str, col:pd.Series, **kwargs) -> LambdaChannel:
     lfunc = kwargs.get('lfunc', None)
     if lfunc is None:
         raise MissingKwargsError('Must provide lfunc (lambda function))')
     try:
         # attempt to create LambdaChannel
-        domain = (col.min(), col.max())
+        domain = (col.min().tolist(), col.max().tolist())
         mapped = col.map(lfunc)
-        range = (mapped.min(), mapped.max())
+        range = (mapped.min().tolist(), mapped.max().tolist())
         channel = LambdaChannel(field=field, lfunc=lfunc, range=range, domain=domain, **kwargs)
     except:
         raise LambdaChannelError('Could not create LambdaChannel')
     return channel
 
 def create_conditional_channel(field: str, col:pd.Series, **kwargs) -> ConditionalChannel:
      # NOTE: for ConditionalChannel
@@ -207,15 +207,15 @@
     if dtype == 'object':
         col = col.astype('category')
         dtype = col.dtype.name
 
     try:
         if dtype == 'category':
             col = col.cat.as_ordered()
-            domain = int(col.cat.codes.min()), int(col.cat.codes.max())
+            domain = int(col.cat.codes.min().tolist()), int(col.cat.codes.max().tolist())
 
             cats = col.cat.categories.tolist() if len(col.cat.categories) <= 10 else None
             channel = CategoricalColorChannel(field=field, domain=domain, categories=cats, **kwargs)        
             return channel
         
     except:
         raise CategoricalChannelError('Could not create CategoricalColorChannel')
@@ -238,15 +238,15 @@
         # NOTE: this forces strings to be categories
         case 'object':
             channel = create_color_channel(field, col, **kwargs)
         
         case _:
             # NOTE: not a bool, not a category, not a string, must be numeric
             # pd.api.types.is_number(a)
-            channel = BasicChannel(field=field, domain=(col.min(), col.max()), **kwargs)            
+            channel = BasicChannel(field=field, domain=(col.min().tolist(), col.max().tolist()), **kwargs)            
     
     if channel is None:
         raise ChannelCreationError('Could not create RootChannel')
     return channel
 
 @rich_auto
 @dataclass
```

### Comparing `featherplot-0.0.1/featherplot.egg-info/PKG-INFO` & `featherplot-0.0.2/featherplot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featherplot
-Version: 0.0.1
+Version: 0.0.2
 Summary: featherplot
 Home-page: https://github.com/dsm-72/featherplot-py
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `featherplot-0.0.1/featherplot.egg-info/SOURCES.txt` & `featherplot-0.0.2/featherplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.1/setup.py` & `featherplot-0.0.2/setup.py`

 * *Files identical despite different names*

