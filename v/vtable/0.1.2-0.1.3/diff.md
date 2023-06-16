# Comparing `tmp/vtable-0.1.2.tar.gz` & `tmp/vtable-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtable-0.1.2.tar", max compression
+gzip compressed data, was "vtable-0.1.3.tar", max compression
```

## Comparing `vtable-0.1.2.tar` & `vtable-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-06-16 17:21:26.072295 vtable-0.1.2/LICENSE
--rw-r--r--   0        0        0       46 2023-06-16 17:21:26.072295 vtable-0.1.2/README.md
--rw-r--r--   0        0        0      367 2023-06-16 20:40:59.712736 vtable-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 20:35:50.836724 vtable-0.1.2/vtable/__init__.py
--rw-r--r--   0        0        0     4316 2023-06-16 17:58:42.164378 vtable-0.1.2/vtable/checkablecombo.py
--rw-r--r--   0        0        0     6866 2023-06-16 20:40:38.636735 vtable-0.1.2/vtable/colfilters.py
--rw-r--r--   0        0        0      972 2023-06-16 18:48:26.596487 vtable-0.1.2/vtable/loaders.py
--rw-r--r--   0        0        0     1999 2023-06-16 20:40:38.624735 vtable-0.1.2/vtable/main.py
--rw-r--r--   0        0        0     3610 2023-06-16 17:59:08.676379 vtable-0.1.2/vtable/newtable.py
--rw-r--r--   0        0        0     1704 2023-06-16 17:59:18.176379 vtable-0.1.2/vtable/selector.py
--rw-r--r--   0        0        0     2219 2023-06-16 20:40:52.680735 vtable-0.1.2/vtable/supertable.py
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 vtable-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-16 17:21:26.072295 vtable-0.1.3/LICENSE
+-rw-r--r--   0        0        0       46 2023-06-16 17:21:26.072295 vtable-0.1.3/README.md
+-rw-r--r--   0        0        0      367 2023-06-16 20:47:45.588750 vtable-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-06-16 20:44:32.180743 vtable-0.1.3/vtable/__init__.py
+-rw-r--r--   0        0        0     4316 2023-06-16 17:58:42.164378 vtable-0.1.3/vtable/checkablecombo.py
+-rw-r--r--   0        0        0     6803 2023-06-16 20:45:26.756745 vtable-0.1.3/vtable/colfilters.py
+-rw-r--r--   0        0        0      972 2023-06-16 18:48:26.596487 vtable-0.1.3/vtable/loaders.py
+-rw-r--r--   0        0        0     2046 2023-06-16 20:46:04.212747 vtable-0.1.3/vtable/main.py
+-rw-r--r--   0        0        0     3610 2023-06-16 17:59:08.676379 vtable-0.1.3/vtable/newtable.py
+-rw-r--r--   0        0        0     1704 2023-06-16 17:59:18.176379 vtable-0.1.3/vtable/selector.py
+-rw-r--r--   0        0        0     2219 2023-06-16 20:40:52.680735 vtable-0.1.3/vtable/supertable.py
+-rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 vtable-0.1.3/PKG-INFO
```

### Comparing `vtable-0.1.2/LICENSE` & `vtable-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vtable-0.1.2/vtable/checkablecombo.py` & `vtable-0.1.3/vtable/checkablecombo.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.2/vtable/colfilters.py` & `vtable-0.1.3/vtable/colfilters.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,14 @@
 
         print( np.all(self.col.astype(str) == '0'))
         print(np.sum(self.col.astype(str) == '0'))
         print(np.sum(self.col.astype(str) == '1'))
         print(np.where(idx == False))
         print(idx)
 
-        #import pdb; pdb.set_trace()
-        # print(idx[:10])
         try:
             self.idx = idx.values
         except AttributeError:
             self.idx = idx
         print('Debug', self.col.name, np.sum(idx))
         self.changed.emit()
```

### Comparing `vtable-0.1.2/vtable/loaders.py` & `vtable-0.1.3/vtable/loaders.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.2/vtable/main.py` & `vtable-0.1.3/vtable/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import PyQt5.QtWidgets as QtWidget
 import PyQt5.QtWidgets
 
 import pandas as pd
 from . import supertable
 from . import selector
+from . import loaders
+
 
 
 """
 Sketches at initialising a set of filters 
 """
 
 
@@ -48,30 +50,31 @@
     def process_key_press(self, eventQKeyEvent):
         key = eventQKeyEvent.key()
         if key == 81:  #The letter [q]
             self.hide()
             self.close()
 
 
-import loaders
-import sys
 def future_main(path):
     app = PyQt5.QtWidgets.QApplication.instance()
     if app is None:
         app = PyQt5.QtWidgets.QApplication([])
 
     loader = loaders.Loaders()
     df = loader.load(path)
 
     win = MainWin(df)
     win.show()
     return win
 
 
 def main():
+    import sys
+
+    #Does this bleong in __init__
     app = PyQt5.QtWidgets.QApplication.instance()
     if app is None:
         app = PyQt5.QtWidgets.QApplication([])
 
 
     df = pd.read_csv('../../orig/a01.csv', index_col=0)
     win = MainWin(df)
```

### Comparing `vtable-0.1.2/vtable/newtable.py` & `vtable-0.1.3/vtable/newtable.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.2/vtable/selector.py` & `vtable-0.1.3/vtable/selector.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.2/vtable/supertable.py` & `vtable-0.1.3/vtable/supertable.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.2/PKG-INFO` & `vtable-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtable
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Qt based table viewer for Python
 License: GPL 3.0
 Author: fergal
 Author-email: fergal.mullally@gmail.com
 Requires-Python: >3.6
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

