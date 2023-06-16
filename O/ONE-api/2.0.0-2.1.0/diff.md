# Comparing `tmp/ONE-api-2.0.0.tar.gz` & `tmp/ONE-api-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ONE-api-2.0.0.tar", last modified: Thu May 11 16:59:38 2023, max compression
+gzip compressed data, was "ONE-api-2.1.0.tar", last modified: Fri Jun 16 10:42:32 2023, max compression
```

## Comparing `ONE-api-2.0.0.tar` & `ONE-api-2.1.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 16:59:38.912708 ONE-api-2.0.0/
--rw-rw-rw-   0        0        0       26 2021-05-11 13:53:45.000000 ONE-api-2.0.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-11 16:59:38.778852 ONE-api-2.0.0/ONE_api.egg-info/
--rw-rw-rw-   0        0        0     4464 2023-05-11 16:59:37.000000 ONE-api-2.0.0/ONE_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1380 2023-05-11 16:59:37.000000 ONE-api-2.0.0/ONE_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 16:59:37.000000 ONE-api-2.0.0/ONE_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-05-11 16:59:37.000000 ONE-api-2.0.0/ONE_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-11 16:59:37.000000 ONE-api-2.0.0/ONE_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4464 2023-05-11 16:59:38.911711 ONE-api-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3453 2023-05-11 16:58:57.000000 ONE-api-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 16:59:38.822092 ONE-api-2.0.0/one/
--rw-rw-rw-   0        0        0       77 2023-05-11 16:58:57.000000 ONE-api-2.0.0/one/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:59:38.838173 ONE-api-2.0.0/one/alf/
--rw-rw-rw-   0        0        0       70 2021-09-13 19:50:22.000000 ONE-api-2.0.0/one/alf/__init__.py
--rw-rw-rw-   0        0        0    11896 2022-11-09 13:54:50.000000 ONE-api-2.0.0/one/alf/cache.py
--rw-rw-rw-   0        0        0     3185 2022-11-09 13:45:11.000000 ONE-api-2.0.0/one/alf/exceptions.py
--rw-rw-rw-   0        0        0    14801 2023-05-11 16:58:57.000000 ONE-api-2.0.0/one/alf/files.py
--rw-rw-rw-   0        0        0    28418 2023-05-11 16:58:57.000000 ONE-api-2.0.0/one/alf/io.py
--rw-rw-rw-   0        0        0    18656 2023-05-11 16:58:57.000000 ONE-api-2.0.0/one/alf/spec.py
--rw-rw-rw-   0        0        0   118317 2023-05-11 16:58:57.000000 ONE-api-2.0.0/one/api.py
--rw-rw-rw-   0        0        0    26479 2023-05-11 16:58:57.000000 ONE-api-2.0.0/one/converters.py
--rw-rw-rw-   0        0        0    13362 2023-02-28 15:23:52.000000 ONE-api-2.0.0/one/params.py
--rw-rw-rw-   0        0        0    33596 2023-05-11 16:58:57.000000 ONE-api-2.0.0/one/registration.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:59:38.849341 ONE-api-2.0.0/one/remote/
--rw-rw-rw-   0        0        0       40 2022-11-09 13:45:11.000000 ONE-api-2.0.0/one/remote/__init__.py
--rw-rw-rw-   0        0        0     8957 2023-04-21 11:35:55.000000 ONE-api-2.0.0/one/remote/aws.py
--rw-rw-rw-   0        0        0     4566 2023-01-20 12:25:51.000000 ONE-api-2.0.0/one/remote/base.py
--rw-rw-rw-   0        0        0    21865 2023-05-11 16:58:57.000000 ONE-api-2.0.0/one/remote/globus.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:59:38.691715 ONE-api-2.0.0/one/tests/
-drwxrwxrwx   0        0        0        0 2023-05-11 16:59:38.865435 ONE-api-2.0.0/one/tests/fixtures/
--rw-rw-rw-   0        0        0    29918 2021-05-13 19:38:01.000000 ONE-api-2.0.0/one/tests/fixtures/datasets.pqt
-drwxrwxrwx   0        0        0        0 2023-05-11 16:59:38.878401 ONE-api-2.0.0/one/tests/fixtures/params/
--rw-rw-rw-   0        0        0      140 2021-09-13 19:50:22.000000 ONE-api-2.0.0/one/tests/fixtures/params/.caches
--rw-rw-rw-   0        0        0      276 2022-04-25 08:39:47.000000 ONE-api-2.0.0/one/tests/fixtures/params/.test.alyx.internationalbrainlab.org
-drwxrwxrwx   0        0        0        0 2023-05-11 16:59:38.907723 ONE-api-2.0.0/one/tests/fixtures/rest_responses/
--rw-rw-rw-   0        0        0      283 2021-09-13 19:50:22.000000 ONE-api-2.0.0/one/tests/fixtures/rest_responses/1f187d80fd59677b395fcdb18e68e4401bfa1cc9
--rw-rw-rw-   0        0        0      427 2022-11-09 13:45:11.000000 ONE-api-2.0.0/one/tests/fixtures/rest_responses/3f51aa2e0baa42438467906f56a457c91a221898
--rw-rw-rw-   0        0        0     1370 2021-09-13 19:50:22.000000 ONE-api-2.0.0/one/tests/fixtures/rest_responses/47893cf67c985e6361cdee009334963f49fb0746
--rw-rw-rw-   0        0        0     1451 2021-09-13 19:50:22.000000 ONE-api-2.0.0/one/tests/fixtures/rest_responses/535d0e9a1e2c1efbdeba0d673b131e00361a2edb
--rw-rw-rw-   0        0        0      313 2022-11-09 13:45:11.000000 ONE-api-2.0.0/one/tests/fixtures/rest_responses/5618bea3484a52cd893616f07903f0e49e023ba1
--rw-rw-rw-   0        0        0     8066 2022-11-09 13:45:11.000000 ONE-api-2.0.0/one/tests/fixtures/rest_responses/6dc96f7e9bcc6ac2e7581489b9580a6cd3f28293
--rw-rw-rw-   0        0        0      210 2021-09-13 19:50:22.000000 ONE-api-2.0.0/one/tests/fixtures/rest_responses/db1731fb8df0208944ae85f76718430813a8bf50
--rw-rw-rw-   0        0        0      417 2022-11-09 13:45:11.000000 ONE-api-2.0.0/one/tests/fixtures/rest_responses/dcce48259bb929661f60a02a48563f70aa6185b3
--rw-rw-rw-   0        0        0    22531 2021-05-12 14:50:16.000000 ONE-api-2.0.0/one/tests/fixtures/rest_responses/f530d6022f61cdc9e38cc66beb3cb71f3003c9a1
--rw-rw-rw-   0        0        0     6916 2021-05-13 19:38:01.000000 ONE-api-2.0.0/one/tests/fixtures/sessions.pqt
--rw-rw-rw-   0        0        0      324 2021-09-16 15:52:39.000000 ONE-api-2.0.0/one/tests/fixtures/test_dbs.json
--rw-rw-rw-   0        0        0   828598 2021-09-13 19:50:22.000000 ONE-api-2.0.0/one/tests/fixtures/test_img.png
--rw-rw-rw-   0        0        0    21620 2023-05-11 16:58:57.000000 ONE-api-2.0.0/one/util.py
--rw-rw-rw-   0        0        0    47614 2023-05-11 16:58:57.000000 ONE-api-2.0.0/one/webclient.py
--rw-rw-rw-   0        0        0       42 2023-05-11 16:59:38.912708 ONE-api-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1679 2022-11-09 13:45:11.000000 ONE-api-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.292338 ONE-api-2.1.0/
+-rw-rw-rw-   0        0        0       26 2021-05-11 13:53:45.000000 ONE-api-2.1.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.216002 ONE-api-2.1.0/ONE_api.egg-info/
+-rw-rw-rw-   0        0        0     4464 2023-06-16 10:42:31.000000 ONE-api-2.1.0/ONE_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1380 2023-06-16 10:42:31.000000 ONE-api-2.1.0/ONE_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 10:42:31.000000 ONE-api-2.1.0/ONE_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-06-16 10:42:31.000000 ONE-api-2.1.0/ONE_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-16 10:42:31.000000 ONE-api-2.1.0/ONE_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4464 2023-06-16 10:42:32.288348 ONE-api-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3453 2023-05-12 08:59:29.000000 ONE-api-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.232519 ONE-api-2.1.0/one/
+-rw-rw-rw-   0        0        0       77 2023-06-16 09:54:18.000000 ONE-api-2.1.0/one/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.243882 ONE-api-2.1.0/one/alf/
+-rw-rw-rw-   0        0        0       70 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/alf/__init__.py
+-rw-rw-rw-   0        0        0    11896 2023-06-16 08:46:55.000000 ONE-api-2.1.0/one/alf/cache.py
+-rw-rw-rw-   0        0        0     3186 2023-06-16 09:25:42.000000 ONE-api-2.1.0/one/alf/exceptions.py
+-rw-rw-rw-   0        0        0    14801 2023-05-12 08:59:29.000000 ONE-api-2.1.0/one/alf/files.py
+-rw-rw-rw-   0        0        0    28696 2023-06-16 09:54:18.000000 ONE-api-2.1.0/one/alf/io.py
+-rw-rw-rw-   0        0        0    18659 2023-06-16 09:54:18.000000 ONE-api-2.1.0/one/alf/spec.py
+-rw-rw-rw-   0        0        0   118319 2023-06-16 09:25:42.000000 ONE-api-2.1.0/one/api.py
+-rw-rw-rw-   0        0        0    26479 2023-05-12 08:59:29.000000 ONE-api-2.1.0/one/converters.py
+-rw-rw-rw-   0        0        0    13362 2023-02-28 15:23:52.000000 ONE-api-2.1.0/one/params.py
+-rw-rw-rw-   0        0        0    33596 2023-05-12 08:59:29.000000 ONE-api-2.1.0/one/registration.py
+drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.253463 ONE-api-2.1.0/one/remote/
+-rw-rw-rw-   0        0        0       40 2022-11-09 13:45:11.000000 ONE-api-2.1.0/one/remote/__init__.py
+-rw-rw-rw-   0        0        0     8957 2023-04-21 11:35:55.000000 ONE-api-2.1.0/one/remote/aws.py
+-rw-rw-rw-   0        0        0     4566 2023-01-20 12:25:51.000000 ONE-api-2.1.0/one/remote/base.py
+-rw-rw-rw-   0        0        0    21865 2023-05-12 08:59:29.000000 ONE-api-2.1.0/one/remote/globus.py
+drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.199498 ONE-api-2.1.0/one/tests/
+drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.263268 ONE-api-2.1.0/one/tests/fixtures/
+-rw-rw-rw-   0        0        0    29918 2021-05-13 19:38:01.000000 ONE-api-2.1.0/one/tests/fixtures/datasets.pqt
+drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.269251 ONE-api-2.1.0/one/tests/fixtures/params/
+-rw-rw-rw-   0        0        0      140 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/tests/fixtures/params/.caches
+-rw-rw-rw-   0        0        0      276 2022-04-25 08:39:47.000000 ONE-api-2.1.0/one/tests/fixtures/params/.test.alyx.internationalbrainlab.org
+drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.286354 ONE-api-2.1.0/one/tests/fixtures/rest_responses/
+-rw-rw-rw-   0        0        0      283 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/1f187d80fd59677b395fcdb18e68e4401bfa1cc9
+-rw-rw-rw-   0        0        0      427 2022-11-09 13:45:11.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/3f51aa2e0baa42438467906f56a457c91a221898
+-rw-rw-rw-   0        0        0     1370 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/47893cf67c985e6361cdee009334963f49fb0746
+-rw-rw-rw-   0        0        0     1451 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/535d0e9a1e2c1efbdeba0d673b131e00361a2edb
+-rw-rw-rw-   0        0        0      313 2022-11-09 13:45:11.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/5618bea3484a52cd893616f07903f0e49e023ba1
+-rw-rw-rw-   0        0        0     8066 2022-11-09 13:45:11.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/6dc96f7e9bcc6ac2e7581489b9580a6cd3f28293
+-rw-rw-rw-   0        0        0      210 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/db1731fb8df0208944ae85f76718430813a8bf50
+-rw-rw-rw-   0        0        0      417 2022-11-09 13:45:11.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/dcce48259bb929661f60a02a48563f70aa6185b3
+-rw-rw-rw-   0        0        0    22531 2021-05-12 14:50:16.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/f530d6022f61cdc9e38cc66beb3cb71f3003c9a1
+-rw-rw-rw-   0        0        0     6916 2021-05-13 19:38:01.000000 ONE-api-2.1.0/one/tests/fixtures/sessions.pqt
+-rw-rw-rw-   0        0        0      324 2021-09-16 15:52:39.000000 ONE-api-2.1.0/one/tests/fixtures/test_dbs.json
+-rw-rw-rw-   0        0        0   828598 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/tests/fixtures/test_img.png
+-rw-rw-rw-   0        0        0    21620 2023-05-12 08:59:29.000000 ONE-api-2.1.0/one/util.py
+-rw-rw-rw-   0        0        0    47614 2023-05-12 08:59:29.000000 ONE-api-2.1.0/one/webclient.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 10:42:32.292338 ONE-api-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1679 2022-11-09 13:45:11.000000 ONE-api-2.1.0/setup.py
```

### Comparing `ONE-api-2.0.0/ONE_api.egg-info/PKG-INFO` & `ONE-api-2.1.0/ONE_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ONE-api
-Version: 2.0.0
+Version: 2.1.0
 Summary: Open Neurophysiology Environment
 Home-page: https://github.com/int-brain-lab/ONE
 Author: IBL Staff
 License: MIT
 Description: # Open Neurophysiology Environment
         [![Coverage Status](https://coveralls.io/repos/github/int-brain-lab/ONE/badge.svg?branch=main)](https://coveralls.io/github/int-brain-lab/ONE?branch=main)
         ![CI workflow](https://github.com/int-brain-lab/ONE/actions/workflows/main.yaml/badge.svg?branch=main)
```

### Comparing `ONE-api-2.0.0/ONE_api.egg-info/SOURCES.txt` & `ONE-api-2.1.0/ONE_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/PKG-INFO` & `ONE-api-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ONE-api
-Version: 2.0.0
+Version: 2.1.0
 Summary: Open Neurophysiology Environment
 Home-page: https://github.com/int-brain-lab/ONE
 Author: IBL Staff
 License: MIT
 Description: # Open Neurophysiology Environment
         [![Coverage Status](https://coveralls.io/repos/github/int-brain-lab/ONE/badge.svg?branch=main)](https://coveralls.io/github/int-brain-lab/ONE?branch=main)
         ![CI workflow](https://github.com/int-brain-lab/ONE/actions/workflows/main.yaml/badge.svg?branch=main)
```

### Comparing `ONE-api-2.0.0/README.md` & `ONE-api-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/alf/cache.py` & `ONE-api-2.1.0/one/alf/cache.py`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/alf/exceptions.py` & `ONE-api-2.1.0/one/alf/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""ALyx File related errors
+"""ALyx File related errors.
 
 A set of Alyx and ALF related error classes which provide a more verbose description of the raised
 issues.
 """
 
 
 class ALFError(Exception):
```

### Comparing `ONE-api-2.0.0/one/alf/files.py` & `ONE-api-2.1.0/one/alf/files.py`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/alf/io.py` & `ONE-api-2.1.0/one/alf/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,15 +282,15 @@
     Parameters
     ----------
     fil : str, pathlib.Path
         File to read
 
     Returns
     -------
-    any
+    Any
         Array/json/pandas dataframe depending on format
     """
     if not fil:
         return
     fil = Path(fil)
     if fil.stat().st_size == 0:
         return
@@ -312,14 +312,21 @@
     if fil.suffix == '.ssv':
         return pd.read_csv(fil, delimiter=' ').squeeze('columns')
     if fil.suffix in ('.tsv', '.htsv'):
         return pd.read_csv(fil, delimiter='\t').squeeze('columns')
     if fil.suffix in ('.yml', '.yaml'):
         with open(fil, 'r') as _fil:
             return yaml.safe_load(_fil)
+    if fil.suffix == '.sparse_npz':
+        try:
+            import sparse
+            return sparse.load_npz(fil)
+        except ModuleNotFoundError:
+            warnings.warn(f'{Path(fil).name} requires the pydata sparse package to load.')
+            return Path(fil)
     return Path(fil)
 
 
 def _ls(alfpath, object=None, **kwargs) -> (list, tuple):
     """
     Given a path, an object and a filter, returns all files and associated attributes
```

### Comparing `ONE-api-2.0.0/one/alf/spec.py` & `ONE-api-2.1.0/one/alf/spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,19 +103,19 @@
 """str: The collection, revision and filename specification pattern"""
 
 FULL_SPEC = f'{SESSION_SPEC}/{REL_PATH_SPEC}'
 """str: The full ALF path specification pattern"""
 
 _DEFAULT = (
     ('lab', r'\w+'),
-    ('subject', r'[\w-]+'),
+    ('subject', r'[\w.-]+'),
     ('date', r'\d{4}-\d{2}-\d{2}'),
     ('number', r'\d{1,3}'),
-    ('collection', r'[\w/-]+'),
-    ('revision', r'[\w-]+'),  # brackets
+    ('collection', r'[\w./-]+'),
+    ('revision', r'[\w.-]+'),  # brackets
     # to include underscores: r'(?P<namespace>(?:^_)\w+(?:_))?'
     ('namespace', '(?<=_)[a-zA-Z0-9]+'),  # brackets
     ('object', r'\w+'),
     # to treat _times and _intervals as timescale: (?P<attribute>[a-zA-Z]+)_?
     # (?:_[a-z]+_)? allows attribute level namespaces (deprecated)
     ('attribute', r'(?:_[a-z]+_)?[a-zA-Z0-9]+(?:_times(?=[_.])|_intervals(?=[_.]))?'),  # brackets
     ('timescale', r'\w+'),  # brackets
```

### Comparing `ONE-api-2.0.0/one/api.py` & `ONE-api-2.1.0/one/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1925,14 +1925,15 @@
         Notes
         -----
         - This method does not use the local cache and therefore can not work in 'local' mode.
 
         Examples
         --------
         List the insertions associated with a given data release
+
         >>> tag = '2022_Q2_IBL_et_al_RepeatedSite'
         ... ins = one.search_insertions(django='datasets__tags__name,' + tag)
         """
         query_type = query_type or self.mode
         if query_type == 'local' and 'insertions' not in self._cache.keys():
             raise NotImplementedError('Searching on insertions required remote connection')
         elif query_type == 'auto':
```

### Comparing `ONE-api-2.0.0/one/converters.py` & `ONE-api-2.1.0/one/converters.py`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/params.py` & `ONE-api-2.1.0/one/params.py`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/registration.py` & `ONE-api-2.1.0/one/registration.py`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/remote/aws.py` & `ONE-api-2.1.0/one/remote/aws.py`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/remote/base.py` & `ONE-api-2.1.0/one/remote/base.py`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/remote/globus.py` & `ONE-api-2.1.0/one/remote/globus.py`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/tests/fixtures/datasets.pqt` & `ONE-api-2.1.0/one/tests/fixtures/datasets.pqt`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/tests/fixtures/rest_responses/47893cf67c985e6361cdee009334963f49fb0746` & `ONE-api-2.1.0/one/tests/fixtures/rest_responses/47893cf67c985e6361cdee009334963f49fb0746`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/tests/fixtures/rest_responses/535d0e9a1e2c1efbdeba0d673b131e00361a2edb` & `ONE-api-2.1.0/one/tests/fixtures/rest_responses/535d0e9a1e2c1efbdeba0d673b131e00361a2edb`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/tests/fixtures/rest_responses/6dc96f7e9bcc6ac2e7581489b9580a6cd3f28293` & `ONE-api-2.1.0/one/tests/fixtures/rest_responses/6dc96f7e9bcc6ac2e7581489b9580a6cd3f28293`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/tests/fixtures/rest_responses/f530d6022f61cdc9e38cc66beb3cb71f3003c9a1` & `ONE-api-2.1.0/one/tests/fixtures/rest_responses/f530d6022f61cdc9e38cc66beb3cb71f3003c9a1`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/tests/fixtures/sessions.pqt` & `ONE-api-2.1.0/one/tests/fixtures/sessions.pqt`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/tests/fixtures/test_img.png` & `ONE-api-2.1.0/one/tests/fixtures/test_img.png`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/util.py` & `ONE-api-2.1.0/one/util.py`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/one/webclient.py` & `ONE-api-2.1.0/one/webclient.py`

 * *Files identical despite different names*

### Comparing `ONE-api-2.0.0/setup.py` & `ONE-api-2.1.0/setup.py`

 * *Files identical despite different names*

