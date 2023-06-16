# Comparing `tmp/openi-beta-0.1.1.tar.gz` & `tmp/openi-beta-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.1.1.tar", last modified: Fri Jun 16 06:35:14 2023, max compression
+gzip compressed data, was "openi-beta-0.1.2.tar", last modified: Fri Jun 16 06:49:33 2023, max compression
```

## Comparing `openi-beta-0.1.1.tar` & `openi-beta-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.677532 openi-beta-0.1.1/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-16 06:35:14.677402 openi-beta-0.1.1/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-16 06:34:35.000000 openi-beta-0.1.1/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-16 06:35:14.677575 openi-beta-0.1.1/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-16 06:35:01.000000 openi-beta-0.1.1/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.674694 openi-beta-0.1.1/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.675449 openi-beta-0.1.1/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-16 06:34:35.000000 openi-beta-0.1.1/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      358 2023-06-16 06:34:50.000000 openi-beta-0.1.1/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.675953 openi-beta-0.1.1/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.1/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    10813 2023-06-16 06:34:35.000000 openi-beta-0.1.1/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.676173 openi-beta-0.1.1/src/openi/utils/
--rw-r--r--   0 jochen10518   (501) staff       (20)      418 2023-06-16 06:34:35.000000 openi-beta-0.1.1/src/openi/utils/logger.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.676993 openi-beta-0.1.1/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-16 06:35:14.000000 openi-beta-0.1.1/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-16 06:35:14.000000 openi-beta-0.1.1/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-16 06:35:14.000000 openi-beta-0.1.1/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-16 06:35:14.000000 openi-beta-0.1.1/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-16 06:35:14.000000 openi-beta-0.1.1/src/openi_beta.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:35:14.677140 openi-beta-0.1.1/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-16 06:34:35.000000 openi-beta-0.1.1/test/test_upload_multi.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.690150 openi-beta-0.1.2/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-16 06:49:33.690011 openi-beta-0.1.2/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-16 06:44:09.000000 openi-beta-0.1.2/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-16 06:49:33.690199 openi-beta-0.1.2/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-16 06:49:19.000000 openi-beta-0.1.2/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.687357 openi-beta-0.1.2/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.688134 openi-beta-0.1.2/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-16 06:44:09.000000 openi-beta-0.1.2/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      358 2023-06-16 06:44:09.000000 openi-beta-0.1.2/src/openi/constants.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.688624 openi-beta-0.1.2/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.2/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    10839 2023-06-16 06:48:18.000000 openi-beta-0.1.2/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.688866 openi-beta-0.1.2/src/openi/utils/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      418 2023-06-16 06:44:09.000000 openi-beta-0.1.2/src/openi/utils/logger.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.689630 openi-beta-0.1.2/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-16 06:49:33.000000 openi-beta-0.1.2/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-16 06:49:33.000000 openi-beta-0.1.2/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-16 06:49:33.000000 openi-beta-0.1.2/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-16 06:49:33.000000 openi-beta-0.1.2/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-16 06:49:33.000000 openi-beta-0.1.2/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 06:49:33.689780 openi-beta-0.1.2/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-16 06:44:09.000000 openi-beta-0.1.2/test/test_upload_multi.py
```

### Comparing `openi-beta-0.1.1/PKG-INFO` & `openi-beta-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.1
+Version: 0.1.2
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.1/README.md` & `openi-beta-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-0.1.1/setup.py` & `openi-beta-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.1.1',
+    version='0.1.2',
     description='A test package for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openi-beta-0.1.1/src/openi/dataset/dataset.py` & `openi-beta-0.1.2/src/openi/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,17 @@
 
     def getDatasetID(self):
         params = {"access_token": self.token}
         x = requests.get('{}datasets/{}/{}/'.format(self.app_url, self.username, self.repo), params=params)
         if x.status_code == 200:
             try:
                 self.dataset_id = x.json()["data"][0]["id"]
-            except:
+            except Exception as e:
                 logging.error(f'{x} {x.reason} {x.text} | FileObject: {self.__dict__}')
-                print(
+                raise ValueError(
                     f'❌ repo [{self.username}/{self.repo}]: dataset does not exist, please create dataset before uploading files.')
         else:
             logging.error(f'{x} {x.reason} | FileObject: {self.__dict__}')
             raise ConnectionRefusedError(
                 f'❌ <{x.status_code} {x.reason}>')
 
     def newMultipart(self):
```

### Comparing `openi-beta-0.1.1/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-0.1.2/src/openi_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.1
+Version: 0.1.2
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.1/test/test_upload_multi.py` & `openi-beta-0.1.2/test/test_upload_multi.py`

 * *Files identical despite different names*

