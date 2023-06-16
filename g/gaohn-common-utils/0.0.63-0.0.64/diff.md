# Comparing `tmp/gaohn-common-utils-0.0.63.tar.gz` & `tmp/gaohn-common-utils-0.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.63.tar", last modified: Thu Jun 15 13:31:27 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.64.tar", last modified: Fri Jun 16 01:44:26 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.63.tar` & `gaohn-common-utils-0.0.64.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:27.540728 gaohn-common-utils-0.0.63/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 13:31:27.540728 gaohn-common-utils-0.0.63/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:27.540728 gaohn-common-utils-0.0.63/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:27.540728 gaohn-common-utils-0.0.63/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:27.536728 gaohn-common-utils-0.0.63/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:27.540728 gaohn-common-utils-0.0.63/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:27.540728 gaohn-common-utils-0.0.63/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:27.540728 gaohn-common-utils-0.0.63/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:27.540728 gaohn-common-utils-0.0.63/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:27.540728 gaohn-common-utils-0.0.63/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:27.536728 gaohn-common-utils-0.0.63/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:27.540728 gaohn-common-utils-0.0.63/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:27.540728 gaohn-common-utils-0.0.63/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:31:27.540728 gaohn-common-utils-0.0.63/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 13:31:27.000000 gaohn-common-utils-0.0.63/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 13:31:27.000000 gaohn-common-utils-0.0.63/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:31:27.000000 gaohn-common-utils-0.0.63/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 13:31:27.000000 gaohn-common-utils-0.0.63/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 13:31:27.000000 gaohn-common-utils-0.0.63/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-15 13:31:07.000000 gaohn-common-utils-0.0.63/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 13:31:27.540728 gaohn-common-utils-0.0.63/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:26.235289 gaohn-common-utils-0.0.64/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-16 01:44:26.235289 gaohn-common-utils-0.0.64/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:26.231289 gaohn-common-utils-0.0.64/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:26.231289 gaohn-common-utils-0.0.64/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:26.231289 gaohn-common-utils-0.0.64/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:26.231289 gaohn-common-utils-0.0.64/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:26.231289 gaohn-common-utils-0.0.64/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:26.235289 gaohn-common-utils-0.0.64/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:26.235289 gaohn-common-utils-0.0.64/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:26.235289 gaohn-common-utils-0.0.64/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:26.231289 gaohn-common-utils-0.0.64/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:26.235289 gaohn-common-utils-0.0.64/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:26.235289 gaohn-common-utils-0.0.64/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:44:26.235289 gaohn-common-utils-0.0.64/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-16 01:44:26.000000 gaohn-common-utils-0.0.64/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-16 01:44:26.000000 gaohn-common-utils-0.0.64/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:44:26.000000 gaohn-common-utils-0.0.64/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-16 01:44:26.000000 gaohn-common-utils-0.0.64/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 01:44:26.000000 gaohn-common-utils-0.0.64/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-16 01:44:02.000000 gaohn-common-utils-0.0.64/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 01:44:26.235289 gaohn-common-utils-0.0.64/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.63/LICENSE` & `gaohn-common-utils-0.0.64/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.63/PKG-INFO` & `gaohn-common-utils-0.0.64/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.63
+Version: 0.0.64
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.63/README.md` & `gaohn-common-utils-0.0.64/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.63/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.64/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.63/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.64/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.63/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.64/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.63/common_utils/core/base.py` & `gaohn-common-utils-0.0.64/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.63/common_utils/core/common.py` & `gaohn-common-utils-0.0.64/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.63/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.64/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.63/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.64/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.63/common_utils/core/logger.py` & `gaohn-common-utils-0.0.64/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.63/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.64/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.63/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.64/common_utils/versioning/dvc/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,78 @@
 import hashlib
 import json
 import shutil
 from pathlib import Path
-from typing import Dict
+from typing import Dict, Optional
 
 from common_utils.core.base import Storage
 
 
 # pylint: disable=line-too-long
 class SimpleDVC:
     """
     # TODO: try to see if we can make it work for local storage as well.
 
-    LOCAL TREE
+    Local Scenario 1:
     pipeline-training/data
     ├── interim
     ├── processed
     └── raw
         ├── filtered_movies_incremental.csv             # filename
         └── filtered_movies_incremental.csv.json        # metadata for filename
 
+    This scenario handles the workflow whereby user will dump the below stores folder
+    into remote storage during runtime. For example, if user chooses not to store
+    the actual data and just the .csv.json metadata file, then the below will be dumped
+    into say, a GCS bucket or MLFlow artifact store.
+    Of course, ideally, the metadata store in the same location as the actual data
+    so git can track it.
+    Local Scenario 2:
+    /pipeline-training/stores/<UNIQUE_RUN_ID>
+    |── logs
+    |── registry
+    |── artifacts
+    └── blobs
+        ├── raw
+        |   ├── filtered_movies_incremental.csv.json         # metadata for filename
+
+
+    So in this case:
+    - data_dir = /pipeline-training/data
+    - metadata_dir = /pipeline-training/stores/<UNIQUE_RUN_ID>/blobs/raw
+
     REMOTE DVC TREE
     gaohn/                                              # remote_bucket_name
     └── imdb                                            # remote_bucket_project_name
         └── gaohn-dvc                                   # remote_dvc_dir_name
             ├── 1234567890                              # md5 hash for raw/filtered_movies_incremental.csv
             └── filtered_movies_incremental.csv.json
     """
 
     def __init__(
         self,
         storage: Storage,
         remote_bucket_project_name: str,
         data_dir: str = "./data",
         cache_dir: str = ".cache",
+        metadata_dir: Optional[
+            str
+        ] = None,  # new parameter for the location of metadata
     ) -> None:
         self.storage = storage
         self._remote_bucket_project_name = remote_bucket_project_name
 
         self.data_dir = Path(data_dir)
-        self.cache_dir = Path(cache_dir)
 
+        self.cache_dir = Path(cache_dir)
         self.cache_dir.mkdir(parents=True, exist_ok=True)
 
+        # if metadata_dir is None, then metadata_dir = data_dir
+        self.metadata_dir = Path(metadata_dir) if metadata_dir else self.data_dir
+
         self.metadata_file: Path
 
     @property
     def remote_dvc_dir_name(self) -> str:
         """Always fixed to gaohn-dvc. Immutable just like how dvc always uses .dvc."""
         return "gaohn-dvc"
 
@@ -82,15 +108,15 @@
 
         Args:
             filename (str): Name of the file.
 
         Returns:
             Path: Path object for the metadata file in the data directory.
         """
-        return self.data_dir / f"{filename}.json"
+        return self.metadata_dir / f"{filename}.json"
 
     def _load_metadata(self, filename: str) -> Dict[str, str]:
         """
         Loads the metadata for a file from its metadata JSON file.
 
         Args:
             filename (str): Name of the file.
@@ -105,39 +131,39 @@
     def _calculate_md5(self, filepath: str) -> str:
         hash_md5 = hashlib.md5()
         with open(filepath, "rb") as file:
             for chunk in iter(lambda: file.read(4096), b""):
                 hash_md5.update(chunk)
         return hash_md5.hexdigest()
 
-    def add(self, filepath: str, save_metadata: bool = True) -> Dict[str, str]:
+    def add(self, filepath: str) -> Dict[str, str]:
         filepath = Path(filepath)
         filename = filepath.name
         extension = filepath.suffix
 
         md5 = self._calculate_md5(str(filepath))
         cache_filepath = self.cache_dir / md5
 
         shutil.copy(filepath, cache_filepath)
 
         metadata = {
             "filename": filename,
             "filepath": str(cache_filepath),
             "data_dir": str(self.data_dir),
+            "metadata_dir": str(self.metadata_dir),
             "extension": extension,
             "remote_bucket_name": self.remote_bucket_name,
             "remote_bucket_project_name": self.remote_bucket_project_name,
             "remote_dvc_dir_name": self.remote_dvc_dir_name,
             "md5": md5,
         }
 
-        if save_metadata:
-            self.metadata_file = self.data_dir / f"{filename}.json"
-            with self.metadata_file.open("w") as file:
-                json.dump(metadata, file, indent=4)
+        self.metadata_file = self._get_metadata_file_path(filename)
+        with self.metadata_file.open("w") as file:
+            json.dump(metadata, file, indent=4)
 
         self._create_gitignore(filename)
 
         return metadata
 
     def push(self, filepath: str) -> None:
         filepath = Path(filepath)
```

### Comparing `gaohn-common-utils-0.0.63/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.64/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.63/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.64/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.63
+Version: 0.0.64
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.63/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.64/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.63/pyproject.toml` & `gaohn-common-utils-0.0.64/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.63"
+version = "0.0.64"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

