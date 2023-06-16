# Comparing `tmp/pytk_net-0.2.0.tar.gz` & `tmp/pytk_net-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytk_net-0.2.0.tar", last modified: Fri Jun 16 08:56:34 2023, max compression
+gzip compressed data, was "dist\pytk_net-0.2.1.tar", last modified: Fri Jun 16 09:00:08 2023, max compression
```

## Comparing `pytk_net-0.2.0.tar` & `pytk_net-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 08:56:34.704525 pytk_net-0.2.0/
--rw-rw-rw-   0        0        0      966 2023-06-16 08:56:34.703528 pytk_net-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-06-14 06:03:47.000000 pytk_net-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 08:56:34.684329 pytk_net-0.2.0/pytk_net/
--rw-rw-rw-   0        0        0        0 2023-06-09 06:16:51.000000 pytk_net-0.2.0/pytk_net/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:56:34.695624 pytk_net-0.2.0/pytk_net/ext/
--rw-rw-rw-   0        0        0        0 2023-06-15 09:25:02.000000 pytk_net-0.2.0/pytk_net/ext/__init__.py
--rw-rw-rw-   0        0        0      183 2023-06-16 08:37:51.000000 pytk_net-0.2.0/pytk_net/ext/baseframe.py
--rw-rw-rw-   0        0        0      582 2023-06-16 07:33:50.000000 pytk_net-0.2.0/pytk_net/ext/icon.py
--rw-rw-rw-   0        0        0     3208 2023-06-16 08:55:34.000000 pytk_net-0.2.0/pytk_net/ext/navmenu.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:56:34.698540 pytk_net-0.2.0/pytk_net/icons/
--rw-rw-rw-   0        0        0    49971 2023-05-31 05:59:23.000000 pytk_net-0.2.0/pytk_net/icons/bootstrap-icons.json
--rw-rw-rw-   0        0        0   164360 2023-05-31 05:59:30.000000 pytk_net-0.2.0/pytk_net/icons/bootstrap-icons.woff
-drwxrwxrwx   0        0        0        0 2023-06-16 08:56:34.702530 pytk_net-0.2.0/pytk_net/overwrite/
--rw-rw-rw-   0        0        0     2435 2023-06-14 03:32:19.000000 pytk_net-0.2.0/pytk_net/overwrite/DateEntry.py
--rw-rw-rw-   0        0        0        0 2023-06-14 14:24:28.000000 pytk_net-0.2.0/pytk_net/overwrite/__init__.py
--rw-rw-rw-   0        0        0     2215 2023-06-16 08:55:48.000000 pytk_net-0.2.0/pytk_net/utils.py
--rw-rw-rw-   0        0        0      207 2023-06-16 06:24:00.000000 pytk_net-0.2.0/pytk_net/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:56:34.690635 pytk_net-0.2.0/pytk_net.egg-info/
--rw-rw-rw-   0        0        0      966 2023-06-16 08:56:34.000000 pytk_net-0.2.0/pytk_net.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-06-16 08:56:34.000000 pytk_net-0.2.0/pytk_net.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 08:56:34.000000 pytk_net-0.2.0/pytk_net.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-16 08:56:34.000000 pytk_net-0.2.0/pytk_net.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 08:56:34.704525 pytk_net-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-06-16 08:47:05.000000 pytk_net-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:00:08.110841 pytk_net-0.2.1/
+-rw-rw-rw-   0        0        0      966 2023-06-16 09:00:08.110841 pytk_net-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-06-14 06:03:47.000000 pytk_net-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 09:00:08.090591 pytk_net-0.2.1/pytk_net/
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:16:51.000000 pytk_net-0.2.1/pytk_net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:00:08.102780 pytk_net-0.2.1/pytk_net/ext/
+-rw-rw-rw-   0        0        0        0 2023-06-15 09:25:02.000000 pytk_net-0.2.1/pytk_net/ext/__init__.py
+-rw-rw-rw-   0        0        0      183 2023-06-16 08:37:51.000000 pytk_net-0.2.1/pytk_net/ext/baseframe.py
+-rw-rw-rw-   0        0        0      582 2023-06-16 07:33:50.000000 pytk_net-0.2.1/pytk_net/ext/icon.py
+-rw-rw-rw-   0        0        0     3217 2023-06-16 08:59:48.000000 pytk_net-0.2.1/pytk_net/ext/navmenu.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:00:08.106402 pytk_net-0.2.1/pytk_net/icons/
+-rw-rw-rw-   0        0        0    49971 2023-05-31 05:59:23.000000 pytk_net-0.2.1/pytk_net/icons/bootstrap-icons.json
+-rw-rw-rw-   0        0        0   164360 2023-05-31 05:59:30.000000 pytk_net-0.2.1/pytk_net/icons/bootstrap-icons.woff
+drwxrwxrwx   0        0        0        0 2023-06-16 09:00:08.109394 pytk_net-0.2.1/pytk_net/overwrite/
+-rw-rw-rw-   0        0        0     2435 2023-06-14 03:32:19.000000 pytk_net-0.2.1/pytk_net/overwrite/DateEntry.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 14:24:28.000000 pytk_net-0.2.1/pytk_net/overwrite/__init__.py
+-rw-rw-rw-   0        0        0     2215 2023-06-16 08:55:48.000000 pytk_net-0.2.1/pytk_net/utils.py
+-rw-rw-rw-   0        0        0      207 2023-06-16 06:24:00.000000 pytk_net-0.2.1/pytk_net/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:00:08.096702 pytk_net-0.2.1/pytk_net.egg-info/
+-rw-rw-rw-   0        0        0      966 2023-06-16 09:00:07.000000 pytk_net-0.2.1/pytk_net.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-06-16 09:00:07.000000 pytk_net-0.2.1/pytk_net.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 09:00:07.000000 pytk_net-0.2.1/pytk_net.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-16 09:00:07.000000 pytk_net-0.2.1/pytk_net.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 09:00:08.111841 pytk_net-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-06-16 09:00:00.000000 pytk_net-0.2.1/setup.py
```

### Comparing `pytk_net-0.2.0/PKG-INFO` & `pytk_net-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytk_net
-Version: 0.2.0
+Version: 0.2.1
 Summary: TkinterHelper布局助手官方拓展和工具库
 Home-page: https://www.pytk.net
 Author: iamxcd
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 TkinterHelper布局助手官方拓展和工具库
```

### Comparing `pytk_net-0.2.0/README.md` & `pytk_net-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.0/pytk_net/ext/icon.py` & `pytk_net-0.2.1/pytk_net/ext/icon.py`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.0/pytk_net/ext/navmenu.py` & `pytk_net-0.2.1/pytk_net/ext/navmenu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from tkinter import Label, X, LEFT, TOP
 from typing import List
 
 from ttkbootstrap import Frame, DARK, SECONDARY, WARNING
 
 from pytk_net.ext.baseframe import BaseFrame
 from pytk_net.ext.icon import Icon
-from utils import get_color
+from pytk_net.utils import get_color
 
 
 class NavMenuItem:
     def __init__(self, icon, text, side=TOP):
         self.side = side
         self.icon = icon
         self.text = text
```

### Comparing `pytk_net-0.2.0/pytk_net/icons/bootstrap-icons.json` & `pytk_net-0.2.1/pytk_net/icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.0/pytk_net/icons/bootstrap-icons.woff` & `pytk_net-0.2.1/pytk_net/icons/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.0/pytk_net/overwrite/DateEntry.py` & `pytk_net-0.2.1/pytk_net/overwrite/DateEntry.py`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.0/pytk_net/utils.py` & `pytk_net-0.2.1/pytk_net/utils.py`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.0/pytk_net.egg-info/PKG-INFO` & `pytk_net-0.2.1/pytk_net.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytk-net
-Version: 0.2.0
+Version: 0.2.1
 Summary: TkinterHelper布局助手官方拓展和工具库
 Home-page: https://www.pytk.net
 Author: iamxcd
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 TkinterHelper布局助手官方拓展和工具库
```

