# Comparing `tmp/heyang-test-0.0.3.tar.gz` & `tmp/heyang-test-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heyang-test-0.0.3.tar", last modified: Fri Jun 16 07:44:47 2023, max compression
+gzip compressed data, was "heyang-test-0.1.0.tar", last modified: Fri Jun 16 08:10:36 2023, max compression
```

## Comparing `heyang-test-0.0.3.tar` & `heyang-test-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 07:44:47.099351 heyang-test-0.0.3/
--rw-rw-rw-   0        0        0     1073 2023-06-16 07:33:44.000000 heyang-test-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2877 2023-06-16 07:44:47.099351 heyang-test-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2053 2023-06-16 07:33:44.000000 heyang-test-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 07:44:47.083334 heyang-test-0.0.3/hanlingzhi/
--rw-rw-rw-   0        0        0        0 2023-06-16 07:33:44.000000 heyang-test-0.0.3/hanlingzhi/__init__.py
--rw-rw-rw-   0        0        0      104 2023-06-16 07:33:44.000000 heyang-test-0.0.3/hanlingzhi/math_h.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:44:47.099351 heyang-test-0.0.3/heyang_test.egg-info/
--rw-rw-rw-   0        0        0     2877 2023-06-16 07:44:46.000000 heyang-test-0.0.3/heyang_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-06-16 07:44:46.000000 heyang-test-0.0.3/heyang_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 07:44:46.000000 heyang-test-0.0.3/heyang_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-16 07:44:46.000000 heyang-test-0.0.3/heyang_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-16 07:44:46.000000 heyang-test-0.0.3/heyang_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 07:44:47.099351 heyang-test-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2065 2023-06-16 07:44:44.000000 heyang-test-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:44:47.099351 heyang-test-0.0.3/string_h/
--rw-rw-rw-   0        0        0        0 2023-06-16 07:33:44.000000 heyang-test-0.0.3/string_h/__init__.py
--rw-rw-rw-   0        0        0       48 2023-06-16 07:33:44.000000 heyang-test-0.0.3/string_h/reverse.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:10:36.145200 heyang-test-0.1.0/
+-rw-rw-rw-   0        0        0     1073 2023-06-16 07:33:44.000000 heyang-test-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2877 2023-06-16 08:10:36.145200 heyang-test-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2053 2023-06-16 07:33:44.000000 heyang-test-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 08:10:36.109167 heyang-test-0.1.0/hanlingzhi/
+-rw-rw-rw-   0        0        0        0 2023-06-16 07:33:44.000000 heyang-test-0.1.0/hanlingzhi/__init__.py
+-rw-rw-rw-   0        0        0      104 2023-06-16 07:33:44.000000 heyang-test-0.1.0/hanlingzhi/math_h.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:10:36.137200 heyang-test-0.1.0/heyang_test.egg-info/
+-rw-rw-rw-   0        0        0     2877 2023-06-16 08:10:35.000000 heyang-test-0.1.0/heyang_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-06-16 08:10:35.000000 heyang-test-0.1.0/heyang_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0    72534 2023-06-15 08:35:04.000000 heyang-test-0.1.0/heyang_test.egg-info/ciku-main.zip
+-rw-rw-rw-   0        0        0        1 2023-06-16 08:10:35.000000 heyang-test-0.1.0/heyang_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-16 08:10:35.000000 heyang-test-0.1.0/heyang_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-16 08:10:35.000000 heyang-test-0.1.0/heyang_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 08:10:36.145200 heyang-test-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2065 2023-06-16 08:09:28.000000 heyang-test-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:10:36.141205 heyang-test-0.1.0/string_h/
+-rw-rw-rw-   0        0        0        0 2023-06-16 07:33:44.000000 heyang-test-0.1.0/string_h/__init__.py
+-rw-rw-rw-   0        0        0       48 2023-06-16 07:33:44.000000 heyang-test-0.1.0/string_h/reverse.py
```

### Comparing `heyang-test-0.0.3/LICENSE.txt` & `heyang-test-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `heyang-test-0.0.3/PKG-INFO` & `heyang-test-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heyang-test
-Version: 0.0.3
+Version: 0.1.0
 Summary: 验证打包功能的测试包, 请勿下载
 Author: heyang
 Author-email: hey505442@gmail.com
 License: MIT
 Keywords: hanlingzhi package demo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `heyang-test-0.0.3/README.md` & `heyang-test-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `heyang-test-0.0.3/heyang_test.egg-info/PKG-INFO` & `heyang-test-0.1.0/heyang_test.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heyang-test
-Version: 0.0.3
+Version: 0.1.0
 Summary: 验证打包功能的测试包, 请勿下载
 Author: heyang
 Author-email: hey505442@gmail.com
 License: MIT
 Keywords: hanlingzhi package demo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `heyang-test-0.0.3/setup.py` & `heyang-test-0.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包名
     name="heyang-test",
     # 版本(也可以用日期表示 2020.3.1 这样每次提交不需要在改版本)
-    version="0.0.3",
+    version="0.1.0",
     # 作者
     author="heyang",
     # 作者邮箱
     author_email="hey505442@gmail.com",
     # 包的说明(这个要正规,会展示出来, 列表页灰色横幅可见)
     description="验证打包功能的测试包, 请勿下载",
     # 项目描述
```

