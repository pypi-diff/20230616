# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.0.6.tar.gz` & `tmp/hyutils-hyutil-hoyun-lab-0.0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.tar", last modified: Thu Jun 15 02:11:46 2023, max compression
+gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.1.tar", last modified: Fri Jun 16 04:54:57 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.0.6.tar` & `hyutils-hyutil-hoyun-lab-0.0.6.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 02:11:46.138114 hyutils-hyutil-hoyun-lab-0.0.6/
--rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      598 2023-06-15 02:11:46.137415 hyutils-hyutil-hoyun-lab-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 02:11:46.138373 hyutils-hyutil-hoyun-lab-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      850 2023-06-15 02:11:17.000000 hyutils-hyutil-hoyun-lab-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 02:11:46.113129 hyutils-hyutil-hoyun-lab-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 02:11:46.129974 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/
--rw-rw-rw-   0        0        0      345 2023-06-15 02:11:17.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/__init__.py
--rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/appcontrol.py
--rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/date_time.py
--rw-rw-rw-   0        0        0     1155 2023-06-15 01:43:34.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/dirjob.py
--rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/hashing.py
--rw-rw-rw-   0        0        0    13711 2023-06-09 05:56:06.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/tfrecrod_utils.py
--rw-rw-rw-   0        0        0     3842 2023-06-08 04:01:29.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/xml_util.py
-drwxrwxrwx   0        0        0        0 2023-06-15 02:11:46.135135 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutils_hyutil_hoyun_lab.egg-info/
--rw-rw-rw-   0        0        0      598 2023-06-15 02:11:46.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-06-15 02:11:46.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 02:11:46.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-15 02:11:46.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 04:54:57.087312 hyutils-hyutil-hoyun-lab-0.0.6.1/
+-rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      600 2023-06-16 04:54:57.086813 hyutils-hyutil-hoyun-lab-0.0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 04:54:57.087312 hyutils-hyutil-hoyun-lab-0.0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-06-16 04:54:15.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:54:57.068184 hyutils-hyutil-hoyun-lab-0.0.6.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 04:54:57.081185 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      347 2023-06-16 04:54:05.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0     1144 2023-06-15 02:19:32.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/filejob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0    13711 2023-06-09 05:56:06.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/tfrecrod_utils.py
+-rw-rw-rw-   0        0        0     4046 2023-06-16 04:49:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/xml_util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:54:57.085184 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutils_hyutil_hoyun_lab.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-06-16 04:54:57.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2023-06-16 04:54:57.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 04:54:57.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-16 04:54:57.000000 hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6
+Version: 0.0.6.1
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6/setup.py` & `hyutils-hyutil-hoyun-lab-0.0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
     name="hyutils-hyutil-hoyun-lab",
-    version="0.0.6",
+    version="0.0.6.1",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/date_time.py` & `hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/dirjob.py` & `hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/dirjob.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,21 +12,20 @@
     for file in os.listdir(path):
         if os.path.isfile(os.path.join(path, file)):
             extension = os.path.splitext(file)[1]
             if extension == ext:
                 yield file
 
 def files_ext_sub(path, ext):
-    result = []
     for root, dirs, files in os.walk(path):
         for file in files:
             extension = os.path.splitext(file)[1]
             if extension == ext:
                 file_path = os.path.join(root, file)
-                yield file_path
+                yield file_path, root
 
 def dirs(path):
     for file in os.listdir(path):
         if os.path.isdir(os.path.join(path, file)):
             yield file
 
 def get_entry_count(path):
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/hashing.py` & `hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/tfrecrod_utils.py` & `hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/tfrecrod_utils.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/xml_util.py` & `hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutil_hoyun_lab/xml_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -96,8 +96,15 @@
         element1_2 = ET.SubElement(element1_1, 'ymin')
         element1_2.text = cls[5]
         element1_2 = ET.SubElement(element1_1, 'ymax')
         element1_2.text = cls[7]
 
     is_ok = True
 
-    return is_ok, data
+    return is_ok, data
+
+def write_xml(path, xml_data):
+    indent(xml_data, level=0)  # xml 들여쓰기
+    b_xml = ET.tostring(xml_data)
+    # 주석(xml)기록
+    with open(path, 'wb') as f:
+        f.write(b_xml)
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6.1/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6
+Version: 0.0.6.1
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

