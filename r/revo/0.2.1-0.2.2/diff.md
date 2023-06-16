# Comparing `tmp/revo-0.2.1-py3-none-any.whl.zip` & `tmp/revo-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6509 bytes, number of entries: 7
+Zip file size: 6735 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       24 b- defN 23-May-29 11:26 revo/__init__.py
--rw-r--r--  2.0 unx     5479 b- defN 23-Jun-14 05:36 revo/_revo.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jun-14 05:41 revo-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6672 b- defN 23-Jun-14 05:41 revo-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 05:41 revo-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-14 05:41 revo-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      511 b- defN 23-Jun-14 05:41 revo-0.2.1.dist-info/RECORD
-7 files, 13851 bytes uncompressed, 5609 bytes compressed:  59.5%
+-rw-r--r--  2.0 unx     5647 b- defN 23-Jun-16 03:25 revo/_revo.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-16 03:29 revo-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7233 b- defN 23-Jun-16 03:29 revo-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 03:29 revo-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-16 03:29 revo-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      511 b- defN 23-Jun-16 03:29 revo-0.2.2.dist-info/RECORD
+7 files, 14580 bytes uncompressed, 5835 bytes compressed:  60.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: revo/__init__.py
 Comment: 
 
 Filename: revo/_revo.py
 Comment: 
 
-Filename: revo-0.2.1.dist-info/LICENSE
+Filename: revo-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: revo-0.2.1.dist-info/METADATA
+Filename: revo-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: revo-0.2.1.dist-info/WHEEL
+Filename: revo-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: revo-0.2.1.dist-info/top_level.txt
+Filename: revo-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: revo-0.2.1.dist-info/RECORD
+Filename: revo-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## revo/_revo.py

```diff
@@ -1,14 +1,15 @@
 ################################################################################
 # revo --- Referenced Values in Objects
 ################################################################################
 __all__ = ['Revo']
 
 import re
 import ast
+from copy import deepcopy
 try:
     from collections.abc import MutableMapping
 except:
     from collections import MutableMapping
 
 
 def _parse_literal(spec):
@@ -42,27 +43,27 @@
         return obj
     key = path[0]
     if isinstance(key, str) and key not in obj:
         raise KeyError(f'path "{"/".join(orig_path)}" not found')
     return _revo_get(obj[key], path[1:], orig_path)
 
 
-def _revo_set(obj, path, val, orig_path=None):
+def _revo_set(obj, path, val, extend=True, orig_path=None):
     if not isinstance(path, list):
-        _revo_set(obj, _revo_path(path), val)
+        _revo_set(obj, _revo_path(path), val, extend)
         return
     if not orig_path:
         orig_path = path
     key = path[0]
     if len(path) == 1:
-        if isinstance(key, str) and key not in obj:
+        if not extend and isinstance(key, str) and key not in obj:
             raise KeyError(f'path "{"/".join(orig_path)}" not found')
         obj[key] = val
     else:
-        _revo_set(obj[key], path[1:], val, orig_path)
+        _revo_set(obj[key], path[1:], val, extend, orig_path)
 
 
 def _revo_del(obj, path):
     if not isinstance(path, list):
         return _revo_del(obj, _revo_path(path))
     if len(path) == 1:
         del obj[path[0]]
@@ -84,22 +85,23 @@
     else:
         yield (None, obj)
 
 
 class Revo(MutableMapping):
 
     def __init__(self, obj, overrides=None, *,
-                 mercy=False, absorb=False, retain=True):
-        self.val = obj
+                 mercy=False, absorb=False, retain=True, extend=True):
+        self.val = deepcopy(obj)
         if not isinstance(obj, (list, dict)):
             raise TypeError('Only list or dict object allowed')
 
         self.mercy  = mercy   # allow unresolved or illegal references
         self.absorb = absorb  # merge definitions into the tree
         self.retain = retain  # try to keep reference value type
+        self.extend = extend  # allow extending new leaf nodes
 
         # top-level overrides not found in original object are definitions
         self.defs = []
 
         if overrides:
             self.resolve(overrides)
 
@@ -165,16 +167,15 @@
 
 
     def melt(self):
         return _revo_melt(self.val)
 
 
     def __getitem__(self, key): return _revo_get(self.val, key)
-    def __setitem__(self, key, val): _revo_set(self.val, key, val)
+    def __setitem__(self, key, val): _revo_set(self.val, key, val, self.extend)
     def __delitem__(self, key): _revo_del(self.val, key)
     def __iter__(self): return iter(self.val)
     def __len__(self): return len(self.val)
     def __str__(self): return str(self.val)
     def __repr__(self): return repr(self.val)
 
-
 ### revo.py ends here
```

## Comparing `revo-0.2.1.dist-info/LICENSE` & `revo-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `revo-0.2.1.dist-info/METADATA` & `revo-0.2.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revo
-Version: 0.2.1
+Version: 0.2.2
 Summary: Referenced Values in Objects.
 Author-email: Sun Yijiang <sunyijiang@gmail.com>
 Project-URL: Homepage, https://github.com/sunyj/revo
 Project-URL: Bug Tracker, https://github.com/sunyj/revo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -151,27 +151,49 @@
 
 It defaults to `False`.  When `mercy=True`, unresolved or partially-resolved
 values are left in the object.
 
 
 ## Definition merging
 
-Overrides may contain variables that are not in the object under resolve, for
-example:
+Top-level overrides may contain variables that are not in the object under
+resolve, for example:
 
 ```python
 import revo
 conf = revo.Revo({'name': 'hello $(date)'}, ['date=20220101'])
 conf['name'] # 'hello 20220101'
 conf['date'] # what do you expect?
 ```
 
-Such overrides are called *definitions*.  Definitions may stay in the object
-after the resolution.  Keyword-only boolean argument `absorb` controls this,
-it defaults to `False`.
+Such top-level overrides are called *definitions*.  Definitions may stay in
+the object after the resolution.  Keyword-only boolean argument `absorb`
+controls this, it defaults to `False`.
+
+
+## Definition extending
+
+Overrides may also contain variables with new leaf-node values, for example:
+
+```python
+import revo
+obj = {'data': {'name': 'foo'}}
+conf = revo.Revo(obj, overrides=['data/func=bar'])
+
+# good, as 'func' is a leaf node
+obj['data']['func'] # 'bar'
+
+# not good if extend is turned off
+conf = revo.Revo(obj, overrides=['data/func=bar'], extend=False)
+
+# error, as new is NOT a leaf node
+conf = revo.Revo(obj, overrides=['new/func=bar'])
+```
+
+Keyword-only boolean argument `extend` controls this, it defaults to `True`.
 
 
 ## Type retaining
 
 Keyword-only boolean argument `retain` controls if **revo** tries to keep
 variable value type in substitutions.
```

