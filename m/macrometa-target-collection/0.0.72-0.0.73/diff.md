# Comparing `tmp/macrometa-target-collection-0.0.72.tar.gz` & `tmp/macrometa-target-collection-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.72.tar", last modified: Fri Jun 16 20:03:17 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.73.tar", last modified: Fri Jun 16 20:20:06 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.72.tar` & `macrometa-target-collection-0.0.73.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:03:17.172677 macrometa-target-collection-0.0.72/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 20:02:54.000000 macrometa-target-collection-0.0.72/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 20:03:17.172677 macrometa-target-collection-0.0.72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 20:02:54.000000 macrometa-target-collection-0.0.72/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:03:17.172677 macrometa-target-collection-0.0.72/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 20:02:54.000000 macrometa-target-collection-0.0.72/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16931 2023-06-16 20:02:54.000000 macrometa-target-collection-0.0.72/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:03:17.172677 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 20:03:17.000000 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 20:03:17.000000 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:03:17.000000 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 20:03:17.000000 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 20:03:17.000000 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 20:03:17.000000 macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 20:02:54.000000 macrometa-target-collection-0.0.72/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 20:03:17.172677 macrometa-target-collection-0.0.72/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:20:06.775015 macrometa-target-collection-0.0.73/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 20:19:47.000000 macrometa-target-collection-0.0.73/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 20:20:06.775015 macrometa-target-collection-0.0.73/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 20:19:47.000000 macrometa-target-collection-0.0.73/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:20:06.775015 macrometa-target-collection-0.0.73/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 20:19:47.000000 macrometa-target-collection-0.0.73/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17082 2023-06-16 20:19:47.000000 macrometa-target-collection-0.0.73/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:20:06.775015 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 20:20:06.000000 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 20:20:06.000000 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:20:06.000000 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 20:20:06.000000 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 20:20:06.000000 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 20:20:06.000000 macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 20:19:47.000000 macrometa-target-collection-0.0.73/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 20:20:06.775015 macrometa-target-collection-0.0.73/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.72/LICENSE` & `macrometa-target-collection-0.0.73/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.72/PKG-INFO` & `macrometa-target-collection-0.0.73/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.72
+Version: 0.0.73
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.72/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.73/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.72/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.73/macrometa_target_collection/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,15 @@
             # if batch has records that need to be processed but haven't reached batch size then process them.
             try_upsert(collection, record_batch, force=True)
         if count > 20:
             logger.warn("process batch exception raised..")
             raise Exception("process batch stopped.")
 
 
-async def main():
+async def main_impl():
     parser = argparse.ArgumentParser()
     parser.add_argument('-c', '--config', help='Config file')
     args = parser.parse_args()
     if args.config:
         with open(args.config) as input_json:
             config = json.load(input_json)
     else:
@@ -383,9 +383,18 @@
     if response.status_code == 200:
         json_data = response.json()
         if json_data["data"]["result"] and len(json_data["data"]["result"]) > 0:
             return True
     return False
 
 
+def main():
+    """Main entry point"""
+    try:
+        asyncio.run(main_impl())
+    except Exception as exc:
+        logger.critical(exc)
+        raise exc
+
+
 if __name__ == '__main__':
-    asyncio.run(main())
+    main()
```

### Comparing `macrometa-target-collection-0.0.72/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.73/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.72
+Version: 0.0.73
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.72/pyproject.toml` & `macrometa-target-collection-0.0.73/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.72"
+version = "0.0.73"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

