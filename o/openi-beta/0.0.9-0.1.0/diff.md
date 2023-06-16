# Comparing `tmp/openi-beta-0.0.9.tar.gz` & `tmp/openi-beta-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.0.9.tar", last modified: Thu Jun 15 03:56:11 2023, max compression
+gzip compressed data, was "openi-beta-0.1.0.tar", last modified: Fri Jun 16 01:47:14 2023, max compression
```

## Comparing `openi-beta-0.0.9.tar` & `openi-beta-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.825851 openi-beta-0.0.9/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-15 03:56:11.825730 openi-beta-0.0.9/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-15 01:12:38.000000 openi-beta-0.0.9/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-15 03:56:11.825898 openi-beta-0.0.9/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)      967 2023-06-15 03:56:11.000000 openi-beta-0.0.9/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.823413 openi-beta-0.0.9/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.824155 openi-beta-0.0.9/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-15 01:12:38.000000 openi-beta-0.0.9/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      357 2023-06-15 02:29:50.000000 openi-beta-0.0.9/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.824554 openi-beta-0.0.9/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.9/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    10840 2023-06-15 03:54:20.000000 openi-beta-0.0.9/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.824702 openi-beta-0.0.9/src/openi/utils/
--rw-r--r--   0 jochen10518   (501) staff       (20)      417 2023-06-15 03:06:17.000000 openi-beta-0.0.9/src/openi/utils/logger.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.825401 openi-beta-0.0.9/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-15 03:56:11.000000 openi-beta-0.0.9/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-15 03:56:11.000000 openi-beta-0.0.9/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-15 03:56:11.000000 openi-beta-0.0.9/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-15 03:56:11.000000 openi-beta-0.0.9/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-15 03:56:11.000000 openi-beta-0.0.9/src/openi_beta.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.825551 openi-beta-0.0.9/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-15 01:13:48.000000 openi-beta-0.0.9/test/test_upload_multi.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.195110 openi-beta-0.1.0/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-16 01:47:14.194970 openi-beta-0.1.0/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-16 01:09:47.000000 openi-beta-0.1.0/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-16 01:47:14.195157 openi-beta-0.1.0/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-16 01:46:31.000000 openi-beta-0.1.0/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.192192 openi-beta-0.1.0/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.192971 openi-beta-0.1.0/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-16 01:09:47.000000 openi-beta-0.1.0/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      357 2023-06-16 01:09:47.000000 openi-beta-0.1.0/src/openi/constants.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.193457 openi-beta-0.1.0/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.0/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    10813 2023-06-16 01:36:15.000000 openi-beta-0.1.0/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.193697 openi-beta-0.1.0/src/openi/utils/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      418 2023-06-16 01:14:21.000000 openi-beta-0.1.0/src/openi/utils/logger.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.194600 openi-beta-0.1.0/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-16 01:47:14.000000 openi-beta-0.1.0/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-16 01:47:14.000000 openi-beta-0.1.0/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-16 01:47:14.000000 openi-beta-0.1.0/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-16 01:47:14.000000 openi-beta-0.1.0/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-16 01:47:14.000000 openi-beta-0.1.0/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-16 01:47:14.194744 openi-beta-0.1.0/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-16 01:09:47.000000 openi-beta-0.1.0/test/test_upload_multi.py
```

### Comparing `openi-beta-0.0.9/PKG-INFO` & `openi-beta-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.0.9
+Version: 0.1.0
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.0.9/README.md` & `openi-beta-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-0.0.9/setup.py` & `openi-beta-0.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # python setup.py sdist bdist_wheel
-#
+# twine upload dist/*
+# twine upload --repository testpypi dist/*
+# pip install -i https://test.pypi.org/pypi/ --extra-index-url https://pypi.org/simple <your_package_in_testpypi>
 
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.0.9',
+    version='0.1.0',
     description='A test package for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openi-beta-0.0.9/src/openi/dataset/dataset.py` & `openi-beta-0.1.0/src/openi/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,29 +170,28 @@
     """
 
     def stdOut(self, message=""):
         asctime = datetime.now().strftime("%H:%M:%S")
         return (f'{asctime}|{self.filename}|{self.cluster}|{message}')
 
     def filePreprocess(self):
+        self.getDatasetID()
         if self.size == 0:
             logging.error(f'[{self.filename}] File size is 0 | FileObject: {self.__dict__}')
             raise ValueError(
                 f'❌ [{self.filename}] File size is 0')
         if self.size > MAX_FILE_SIZE:
             logging.error(f'[{self.filename}] File size exceeds 200GB | FileObject: {self.__dict__}')
             raise ValueError(
                 f'❌ [{self.filename}] File size exceeds 200GB')
 
         chunk_size = SMALL_FILE_CHUNK_SIZE if self.size < SMALL_FILE_SIZE else LARGE_FILE_CHUNK_SIZE
         self.total_chunk_counts = math.ceil(self.size / chunk_size)
         self.chunks = {n: (n - 1) * chunk_size for n in range(1, self.total_chunk_counts + 1)}
-
         self.calculateMD5()
-        self.getDatasetID()
 
     def calculateMD5(self):
         with open(self.filepath, 'rb') as f:
             data = f.read()
         self.md5 = hashlib.md5(data).hexdigest()
 
     """
@@ -228,15 +227,15 @@
         self.filePreprocess()
         # checking upload status
         self.getChunks()
 
         # upload starts
         if self.uuid != '':
             if self.uploaded:
-                logging.error(f'Upload failed: [{self.filename} - {self.cluster}], already exists, cannot be uploaded again. | File size exceeds 200GB | FileObject: {self.__dict__}')
+                logging.error(f'Upload failed: [{self.filename} - {self.cluster}], already exists, cannot be uploaded again. | FileObject: {self.__dict__}')
                 raise ValueError(
                     f'❌ Upload failed: [{self.filename} - {self.cluster}], already exists, cannot be uploaded again.')
             else:
                 print(self.stdOut('continue upload...'))
                 uploaded_chunks = [int(i.split('-')[0]) for i in self.uploaded_chunks.split(',') if i != '']
                 continue_chunks = {i: self.chunks[i] for i in self.chunks if i not in uploaded_chunks}
                 # re-upload last chunk from checkpoint
```

### Comparing `openi-beta-0.0.9/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-0.1.0/src/openi_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.0.9
+Version: 0.1.0
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.0.9/test/test_upload_multi.py` & `openi-beta-0.1.0/test/test_upload_multi.py`

 * *Files identical despite different names*

