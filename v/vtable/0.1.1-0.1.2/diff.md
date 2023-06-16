# Comparing `tmp/vtable-0.1.1.tar.gz` & `tmp/vtable-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtable-0.1.1.tar", max compression
+gzip compressed data, was "vtable-0.1.2.tar", max compression
```

## Comparing `vtable-0.1.1.tar` & `vtable-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-06-16 17:21:26.072295 vtable-0.1.1/LICENSE
--rw-r--r--   0        0        0       46 2023-06-16 17:21:26.072295 vtable-0.1.1/README.md
--rw-r--r--   0        0        0      367 2023-06-16 20:37:24.320728 vtable-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 20:35:50.836724 vtable-0.1.1/vtable/__init__.py
--rw-r--r--   0        0        0     4316 2023-06-16 17:58:42.164378 vtable-0.1.1/vtable/checkablecombo.py
--rw-r--r--   0        0        0     6865 2023-06-16 18:13:56.268411 vtable-0.1.1/vtable/colfilters.py
--rw-r--r--   0        0        0      972 2023-06-16 18:48:26.596487 vtable-0.1.1/vtable/loaders.py
--rw-r--r--   0        0        0     1985 2023-06-16 18:40:40.912470 vtable-0.1.1/vtable/main.py
--rw-r--r--   0        0        0     3610 2023-06-16 17:59:08.676379 vtable-0.1.1/vtable/newtable.py
--rw-r--r--   0        0        0     1704 2023-06-16 17:59:18.176379 vtable-0.1.1/vtable/selector.py
--rw-r--r--   0        0        0     2205 2023-06-16 18:12:30.236408 vtable-0.1.1/vtable/supertable.py
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 vtable-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-16 17:21:26.072295 vtable-0.1.2/LICENSE
+-rw-r--r--   0        0        0       46 2023-06-16 17:21:26.072295 vtable-0.1.2/README.md
+-rw-r--r--   0        0        0      367 2023-06-16 20:40:59.712736 vtable-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 20:35:50.836724 vtable-0.1.2/vtable/__init__.py
+-rw-r--r--   0        0        0     4316 2023-06-16 17:58:42.164378 vtable-0.1.2/vtable/checkablecombo.py
+-rw-r--r--   0        0        0     6866 2023-06-16 20:40:38.636735 vtable-0.1.2/vtable/colfilters.py
+-rw-r--r--   0        0        0      972 2023-06-16 18:48:26.596487 vtable-0.1.2/vtable/loaders.py
+-rw-r--r--   0        0        0     1999 2023-06-16 20:40:38.624735 vtable-0.1.2/vtable/main.py
+-rw-r--r--   0        0        0     3610 2023-06-16 17:59:08.676379 vtable-0.1.2/vtable/newtable.py
+-rw-r--r--   0        0        0     1704 2023-06-16 17:59:18.176379 vtable-0.1.2/vtable/selector.py
+-rw-r--r--   0        0        0     2219 2023-06-16 20:40:52.680735 vtable-0.1.2/vtable/supertable.py
+-rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 vtable-0.1.2/PKG-INFO
```

### Comparing `vtable-0.1.1/LICENSE` & `vtable-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vtable-0.1.1/vtable/checkablecombo.py` & `vtable-0.1.2/vtable/checkablecombo.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.1/vtable/colfilters.py` & `vtable-0.1.2/vtable/colfilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import re
 
 
 import PyQt5.QtWidgets as QtWidget
 import PyQt5.QtCore as QtCore
 
-from checkablecombo import CheckableComboBox
+from .checkablecombo import CheckableComboBox
 
 
 """
 Abstract and concreate column filter classes. 
 
 These are QWidget objects that also encode the logic of which rows should be filtered in and out 
 """
```

### Comparing `vtable-0.1.1/vtable/loaders.py` & `vtable-0.1.2/vtable/loaders.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.1/vtable/main.py` & `vtable-0.1.2/vtable/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import PyQt5.QtWidgets as QtWidget
 import PyQt5.QtWidgets
 
 import pandas as pd
-import supertable
-import selector
+from . import supertable
+from . import selector
 
 
 """
 Sketches at initialising a set of filters 
 """
```

### Comparing `vtable-0.1.1/vtable/newtable.py` & `vtable-0.1.2/vtable/newtable.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.1/vtable/selector.py` & `vtable-0.1.2/vtable/selector.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.1/vtable/supertable.py` & `vtable-0.1.2/vtable/supertable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import PyQt5.QtWidgets as QtWidget
 
 import numpy as np
-import colfilters
-import newtable
+from . import colfilters
+from . import newtable
 
 class SuperTableWidget(QtWidget.QDialog):
     def __init__(self, df, num=1000, parent=None):
         QtWidget.QMainWindow.__init__(self, parent)
         self.df = df
         self.ncol = len(df.columns)
```

### Comparing `vtable-0.1.1/PKG-INFO` & `vtable-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtable
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Qt based table viewer for Python
 License: GPL 3.0
 Author: fergal
 Author-email: fergal.mullally@gmail.com
 Requires-Python: >3.6
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

