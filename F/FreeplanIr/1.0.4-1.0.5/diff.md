# Comparing `tmp/FreeplanIr-1.0.4.tar.gz` & `tmp/FreeplanIr-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeplanIr-1.0.4.tar", last modified: Mon Jun  5 06:52:46 2023, max compression
+gzip compressed data, was "FreeplanIr-1.0.5.tar", last modified: Fri Jun 16 09:26:57 2023, max compression
```

## Comparing `FreeplanIr-1.0.4.tar` & `FreeplanIr-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 06:52:46.796779 FreeplanIr-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-06-05 06:52:46.785751 FreeplanIr-1.0.4/FreeplanIr/
--rw-rw-rw-   0        0        0       47 2023-05-24 09:10:22.000000 FreeplanIr-1.0.4/FreeplanIr/__init__.py
--rw-rw-rw-   0        0        0     4038 2023-06-05 06:50:24.000000 FreeplanIr-1.0.4/FreeplanIr/main.py
-drwxrwxrwx   0        0        0        0 2023-06-05 06:52:46.793749 FreeplanIr-1.0.4/FreeplanIr.egg-info/
--rw-rw-rw-   0        0        0     1706 2023-06-05 06:52:46.000000 FreeplanIr-1.0.4/FreeplanIr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-06-05 06:52:46.000000 FreeplanIr-1.0.4/FreeplanIr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 06:52:46.000000 FreeplanIr-1.0.4/FreeplanIr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-05 06:52:46.000000 FreeplanIr-1.0.4/FreeplanIr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-05 06:52:46.000000 FreeplanIr-1.0.4/FreeplanIr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2023-05-24 08:32:25.000000 FreeplanIr-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1706 2023-06-05 06:52:46.795748 FreeplanIr-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-06-05 06:41:44.000000 FreeplanIr-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 06:52:46.796779 FreeplanIr-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      766 2023-06-05 06:41:44.000000 FreeplanIr-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:26:57.577169 FreeplanIr-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-06-16 09:26:57.567169 FreeplanIr-1.0.5/FreeplanIr/
+-rw-rw-rw-   0        0        0       47 2023-05-24 09:10:22.000000 FreeplanIr-1.0.5/FreeplanIr/__init__.py
+-rw-rw-rw-   0        0        0     3980 2023-06-16 09:23:23.000000 FreeplanIr-1.0.5/FreeplanIr/main.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:26:57.574167 FreeplanIr-1.0.5/FreeplanIr.egg-info/
+-rw-rw-rw-   0        0        0     1706 2023-06-16 09:26:57.000000 FreeplanIr-1.0.5/FreeplanIr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-06-16 09:26:57.000000 FreeplanIr-1.0.5/FreeplanIr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 09:26:57.000000 FreeplanIr-1.0.5/FreeplanIr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-16 09:26:57.000000 FreeplanIr-1.0.5/FreeplanIr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 09:26:57.000000 FreeplanIr-1.0.5/FreeplanIr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2023-05-24 08:32:25.000000 FreeplanIr-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1706 2023-06-16 09:26:57.576168 FreeplanIr-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-06-05 06:41:44.000000 FreeplanIr-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 09:26:57.577169 FreeplanIr-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      766 2023-06-16 09:23:49.000000 FreeplanIr-1.0.5/setup.py
```

### Comparing `FreeplanIr-1.0.4/FreeplanIr/main.py` & `FreeplanIr-1.0.5/FreeplanIr/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         mind_map = Et.parse(self.file_path)
         self.root = mind_map.getroot()
 
     def plan_test(self) -> List[List[str]]:
         data_list = []
 
         def traverse_nodes(node: Element, data: List[str]):
-            text = node.get('TEXT').replace('\n', '\\n')
             data.append(node.get('TEXT'))
             for child_node in node.findall('node'):
                 self._count += 1
                 if self._count > self._max_num:
                     self._max_num = self._count
                 traverse_nodes(child_node, data.copy())
```

### Comparing `FreeplanIr-1.0.4/FreeplanIr.egg-info/PKG-INFO` & `FreeplanIr-1.0.5/FreeplanIr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeplanIr
-Version: 1.0.4
+Version: 1.0.5
 Summary: 一个可以解析freeplan *.mm格式文件的工具
 Home-page: https://github.com/leslie110
 Author: wangdashuai
 Author-email: hanchaodaming@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FreeplanIr-1.0.4/LICENSE.txt` & `FreeplanIr-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FreeplanIr-1.0.4/PKG-INFO` & `FreeplanIr-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeplanIr
-Version: 1.0.4
+Version: 1.0.5
 Summary: 一个可以解析freeplan *.mm格式文件的工具
 Home-page: https://github.com/leslie110
 Author: wangdashuai
 Author-email: hanchaodaming@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FreeplanIr-1.0.4/README.md` & `FreeplanIr-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `FreeplanIr-1.0.4/setup.py` & `FreeplanIr-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="FreeplanIr",
-    version="1.0.4",
+    version="1.0.5",
     author="wangdashuai",
     author_email="hanchaodaming@outlook.com",
     description="一个可以解析freeplan *.mm格式文件的工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/leslie110",
     packages=setuptools.find_packages(),
```

