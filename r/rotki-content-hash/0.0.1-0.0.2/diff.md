# Comparing `tmp/rotki-content-hash-0.0.1.tar.gz` & `tmp/rotki-content-hash-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotki-content-hash-0.0.1.tar", last modified: Thu Jun 15 21:48:42 2023, max compression
+gzip compressed data, was "rotki-content-hash-0.0.2.tar", last modified: Thu Jun 15 22:26:41 2023, max compression
```

## Comparing `rotki-content-hash-0.0.1.tar` & `rotki-content-hash-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/
--rw-r--r--   0 lefteris  (1000) users      (100)     1092 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/LICENSE
--rw-r--r--   0 lefteris  (1000) users      (100)      192 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/MANIFEST.in
--rw-r--r--   0 lefteris  (1000) users      (100)     7441 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/PKG-INFO
--rw-r--r--   0 lefteris  (1000) users      (100)     6537 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/README.md
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.024845 rotki-content-hash-0.0.1/content_hash/
--rw-r--r--   0 lefteris  (1000) users      (100)     1214 2023-06-15 20:14:33.000000 rotki-content-hash-0.0.1/content_hash/__init__.py
--rw-r--r--   0 lefteris  (1000) users      (100)     2407 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/content_hash/__main__.py
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/content_hash/decodes/
--rw-r--r--   0 lefteris  (1000) users      (100)      514 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/content_hash/decodes/__init__.py
--rw-r--r--   0 lefteris  (1000) users      (100)      319 2023-06-15 20:56:47.000000 rotki-content-hash-0.0.1/content_hash/decodes/b58_multi_hash.py
--rw-r--r--   0 lefteris  (1000) users      (100)      299 2023-06-15 21:35:43.000000 rotki-content-hash-0.0.1/content_hash/decodes/hex_multi_hash.py
--rw-r--r--   0 lefteris  (1000) users      (100)      211 2023-06-15 20:04:42.000000 rotki-content-hash-0.0.1/content_hash/decodes/utf8.py
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/content_hash/encodes/
--rw-r--r--   0 lefteris  (1000) users      (100)      515 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/content_hash/encodes/__init__.py
--rw-r--r--   0 lefteris  (1000) users      (100)      466 2023-06-15 21:32:49.000000 rotki-content-hash-0.0.1/content_hash/encodes/ipfs.py
--rw-r--r--   0 lefteris  (1000) users      (100)      440 2023-06-15 21:35:54.000000 rotki-content-hash-0.0.1/content_hash/encodes/swarm.py
--rw-r--r--   0 lefteris  (1000) users      (100)      209 2023-06-15 21:30:09.000000 rotki-content-hash-0.0.1/content_hash/encodes/utf8.py
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/content_hash/profiles/
--rw-r--r--   0 lefteris  (1000) users      (100)     1876 2023-06-15 20:24:43.000000 rotki-content-hash-0.0.1/content_hash/profiles/__init__.py
--rw-r--r--   0 lefteris  (1000) users      (100)      249 2023-06-15 21:33:00.000000 rotki-content-hash-0.0.1/content_hash/utils.py
--rw-r--r--   0 lefteris  (1000) users      (100)      719 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/example.py
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/
--rw-r--r--   0 lefteris  (1000) users      (100)     7441 2023-06-15 21:48:42.000000 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/PKG-INFO
--rw-r--r--   0 lefteris  (1000) users      (100)      749 2023-06-15 21:48:42.000000 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/SOURCES.txt
--rw-r--r--   0 lefteris  (1000) users      (100)        1 2023-06-15 21:48:42.000000 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/dependency_links.txt
--rw-r--r--   0 lefteris  (1000) users      (100)       66 2023-06-15 21:48:42.000000 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/entry_points.txt
--rw-r--r--   0 lefteris  (1000) users      (100)       98 2023-06-15 21:48:42.000000 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/requires.txt
--rw-r--r--   0 lefteris  (1000) users      (100)       13 2023-06-15 21:48:42.000000 rotki-content-hash-0.0.1/rotki_content_hash.egg-info/top_level.txt
--rw-r--r--   0 lefteris  (1000) users      (100)       38 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/setup.cfg
--rw-r--r--   0 lefteris  (1000) users      (100)     1603 2023-06-15 21:47:47.000000 rotki-content-hash-0.0.1/setup.py
-drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 21:48:42.028179 rotki-content-hash-0.0.1/tests/
--rw-r--r--   0 lefteris  (1000) users      (100)     1018 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/tests/test_command_program.py
--rw-r--r--   0 lefteris  (1000) users      (100)      477 2023-06-15 20:35:10.000000 rotki-content-hash-0.0.1/tests/test_content_hash.py
--rw-r--r--   0 lefteris  (1000) users      (100)      785 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.1/tests/test_profile.py
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 22:26:41.340281 rotki-content-hash-0.0.2/
+-rw-r--r--   0 lefteris  (1000) users      (100)     1092 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.2/LICENSE
+-rw-r--r--   0 lefteris  (1000) users      (100)      192 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.2/MANIFEST.in
+-rw-r--r--   0 lefteris  (1000) users      (100)     7441 2023-06-15 22:26:41.340281 rotki-content-hash-0.0.2/PKG-INFO
+-rw-r--r--   0 lefteris  (1000) users      (100)     6537 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.2/README.md
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 22:26:41.336948 rotki-content-hash-0.0.2/content_hash/
+-rw-r--r--   0 lefteris  (1000) users      (100)     1214 2023-06-15 20:14:33.000000 rotki-content-hash-0.0.2/content_hash/__init__.py
+-rw-r--r--   0 lefteris  (1000) users      (100)     2407 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.2/content_hash/__main__.py
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 22:26:41.336948 rotki-content-hash-0.0.2/content_hash/decodes/
+-rw-r--r--   0 lefteris  (1000) users      (100)      514 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.2/content_hash/decodes/__init__.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      319 2023-06-15 20:56:47.000000 rotki-content-hash-0.0.2/content_hash/decodes/b58_multi_hash.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      299 2023-06-15 21:35:43.000000 rotki-content-hash-0.0.2/content_hash/decodes/hex_multi_hash.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      211 2023-06-15 20:04:42.000000 rotki-content-hash-0.0.2/content_hash/decodes/utf8.py
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 22:26:41.340281 rotki-content-hash-0.0.2/content_hash/encodes/
+-rw-r--r--   0 lefteris  (1000) users      (100)      515 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.2/content_hash/encodes/__init__.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      466 2023-06-15 21:32:49.000000 rotki-content-hash-0.0.2/content_hash/encodes/ipfs.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      440 2023-06-15 21:35:54.000000 rotki-content-hash-0.0.2/content_hash/encodes/swarm.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      209 2023-06-15 21:30:09.000000 rotki-content-hash-0.0.2/content_hash/encodes/utf8.py
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 22:26:41.340281 rotki-content-hash-0.0.2/content_hash/profiles/
+-rw-r--r--   0 lefteris  (1000) users      (100)     1876 2023-06-15 20:24:43.000000 rotki-content-hash-0.0.2/content_hash/profiles/__init__.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      249 2023-06-15 21:33:00.000000 rotki-content-hash-0.0.2/content_hash/utils.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      719 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.2/example.py
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 22:26:41.340281 rotki-content-hash-0.0.2/rotki_content_hash.egg-info/
+-rw-r--r--   0 lefteris  (1000) users      (100)     7441 2023-06-15 22:26:41.000000 rotki-content-hash-0.0.2/rotki_content_hash.egg-info/PKG-INFO
+-rw-r--r--   0 lefteris  (1000) users      (100)      749 2023-06-15 22:26:41.000000 rotki-content-hash-0.0.2/rotki_content_hash.egg-info/SOURCES.txt
+-rw-r--r--   0 lefteris  (1000) users      (100)        1 2023-06-15 22:26:41.000000 rotki-content-hash-0.0.2/rotki_content_hash.egg-info/dependency_links.txt
+-rw-r--r--   0 lefteris  (1000) users      (100)       66 2023-06-15 22:26:41.000000 rotki-content-hash-0.0.2/rotki_content_hash.egg-info/entry_points.txt
+-rw-r--r--   0 lefteris  (1000) users      (100)       98 2023-06-15 22:26:41.000000 rotki-content-hash-0.0.2/rotki_content_hash.egg-info/requires.txt
+-rw-r--r--   0 lefteris  (1000) users      (100)       13 2023-06-15 22:26:41.000000 rotki-content-hash-0.0.2/rotki_content_hash.egg-info/top_level.txt
+-rw-r--r--   0 lefteris  (1000) users      (100)       38 2023-06-15 22:26:41.340281 rotki-content-hash-0.0.2/setup.cfg
+-rw-r--r--   0 lefteris  (1000) users      (100)     1636 2023-06-15 22:26:24.000000 rotki-content-hash-0.0.2/setup.py
+drwxr-xr-x   0 lefteris  (1000) users      (100)        0 2023-06-15 22:26:41.340281 rotki-content-hash-0.0.2/tests/
+-rw-r--r--   0 lefteris  (1000) users      (100)     1018 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.2/tests/test_command_program.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      477 2023-06-15 20:35:10.000000 rotki-content-hash-0.0.2/tests/test_content_hash.py
+-rw-r--r--   0 lefteris  (1000) users      (100)      785 2023-06-15 12:17:55.000000 rotki-content-hash-0.0.2/tests/test_profile.py
```

### Comparing `rotki-content-hash-0.0.1/LICENSE` & `rotki-content-hash-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.1/PKG-INFO` & `rotki-content-hash-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotki-content-hash
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python implementation of EIP 1577 content hash
 Home-page: https://github.com/filips123/ContentHashPy/
 Author: Filip Š
 Author-email: projects@filips.si
 License: MIT
 Keywords: ethereum,ethereum-name-service,ens,eip1577,web3,decentralized
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rotki-content-hash-0.0.1/README.md` & `rotki-content-hash-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.1/content_hash/__init__.py` & `rotki-content-hash-0.0.2/content_hash/__init__.py`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.1/content_hash/__main__.py` & `rotki-content-hash-0.0.2/content_hash/__main__.py`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.1/content_hash/decodes/__init__.py` & `rotki-content-hash-0.0.2/content_hash/decodes/__init__.py`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.1/content_hash/encodes/__init__.py` & `rotki-content-hash-0.0.2/content_hash/encodes/__init__.py`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.1/content_hash/profiles/__init__.py` & `rotki-content-hash-0.0.2/content_hash/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.1/example.py` & `rotki-content-hash-0.0.2/example.py`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.1/rotki_content_hash.egg-info/PKG-INFO` & `rotki-content-hash-0.0.2/rotki_content_hash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotki-content-hash
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python implementation of EIP 1577 content hash
 Home-page: https://github.com/filips123/ContentHashPy/
 Author: Filip Š
 Author-email: projects@filips.si
 License: MIT
 Keywords: ethereum,ethereum-name-service,ens,eip1577,web3,decentralized
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rotki-content-hash-0.0.1/rotki_content_hash.egg-info/SOURCES.txt` & `rotki-content-hash-0.0.2/rotki_content_hash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.1/setup.py` & `rotki-content-hash-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup(
     name = 'rotki-content-hash',
     description = 'Python implementation of EIP 1577 content hash',
     long_description = readme(),
     long_description_content_type='text/markdown',
     license = 'MIT',
-    version='0.0.1',
+    version='0.0.2',
     setup_requires = ['setuptools-git-version'],
 
     packages = ['content_hash'],
 
     entry_points = {
         'console_scripts': ['rotki-content-hash=content_hash.__main__:main'],
     },
@@ -46,8 +46,9 @@
         'Programming Language :: Python :: 3',
         'Topic :: Internet :: Name Service (DNS)',
         'Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator',
         'Topic :: Security :: Cryptography',
         'Topic :: Software Development :: Libraries',
         'Topic :: Utilities',
     ],
+    include_package_data = True,
 )
```

### Comparing `rotki-content-hash-0.0.1/tests/test_command_program.py` & `rotki-content-hash-0.0.2/tests/test_command_program.py`

 * *Files identical despite different names*

### Comparing `rotki-content-hash-0.0.1/tests/test_profile.py` & `rotki-content-hash-0.0.2/tests/test_profile.py`

 * *Files identical despite different names*

