# Comparing `tmp/yet-another-json-config-0.0.3.tar.gz` & `tmp/yet-another-json-config-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet-another-json-config-0.0.3.tar", last modified: Tue Mar 14 03:27:16 2023, max compression
+gzip compressed data, was "yet-another-json-config-0.0.4.tar", last modified: Fri Jun 16 02:54:36 2023, max compression
```

## Comparing `yet-another-json-config-0.0.3.tar` & `yet-another-json-config-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 03:27:16.107981 yet-another-json-config-0.0.3/
--rw-rw-rw-   0        0        0     1087 2023-03-14 02:31:51.000000 yet-another-json-config-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     5024 2023-03-14 03:27:16.106643 yet-another-json-config-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4408 2023-03-14 03:17:31.000000 yet-another-json-config-0.0.3/README.md
--rw-rw-rw-   0        0        0      692 2023-03-14 03:22:54.000000 yet-another-json-config-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-14 03:27:16.107981 yet-another-json-config-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-14 03:27:16.088643 yet-another-json-config-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-03-14 03:27:16.098647 yet-another-json-config-0.0.3/src/yet_another_json_config/
--rw-rw-rw-   0        0        0       43 2023-03-14 02:31:51.000000 yet-another-json-config-0.0.3/src/yet_another_json_config/__init__.py
--rw-rw-rw-   0        0        0     6210 2023-03-14 02:46:53.000000 yet-another-json-config-0.0.3/src/yet_another_json_config/yet_another_json_config.py
-drwxrwxrwx   0        0        0        0 2023-03-14 03:27:16.103643 yet-another-json-config-0.0.3/src/yet_another_json_config.egg-info/
--rw-rw-rw-   0        0        0     5024 2023-03-14 03:27:16.000000 yet-another-json-config-0.0.3/src/yet_another_json_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-03-14 03:27:16.000000 yet-another-json-config-0.0.3/src/yet_another_json_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 03:27:16.000000 yet-another-json-config-0.0.3/src/yet_another_json_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-03-14 03:27:16.000000 yet-another-json-config-0.0.3/src/yet_another_json_config.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-14 03:27:16.105643 yet-another-json-config-0.0.3/tests/
--rw-rw-rw-   0        0        0     4939 2023-03-14 02:39:28.000000 yet-another-json-config-0.0.3/tests/test_config.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:54:36.682004 yet-another-json-config-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-03-14 02:31:51.000000 yet-another-json-config-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5024 2023-06-16 02:54:36.682004 yet-another-json-config-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4408 2023-03-14 03:17:31.000000 yet-another-json-config-0.0.4/README.md
+-rw-rw-rw-   0        0        0      692 2023-06-16 02:53:04.000000 yet-another-json-config-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 02:54:36.682004 yet-another-json-config-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 02:54:36.651382 yet-another-json-config-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:54:36.666804 yet-another-json-config-0.0.4/src/yet_another_json_config/
+-rw-rw-rw-   0        0        0       43 2023-03-14 02:31:51.000000 yet-another-json-config-0.0.4/src/yet_another_json_config/__init__.py
+-rw-rw-rw-   0        0        0     6185 2023-06-16 02:52:51.000000 yet-another-json-config-0.0.4/src/yet_another_json_config/yet_another_json_config.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:54:36.680003 yet-another-json-config-0.0.4/src/yet_another_json_config.egg-info/
+-rw-rw-rw-   0        0        0     5024 2023-06-16 02:54:36.000000 yet-another-json-config-0.0.4/src/yet_another_json_config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-06-16 02:54:36.000000 yet-another-json-config-0.0.4/src/yet_another_json_config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 02:54:36.000000 yet-another-json-config-0.0.4/src/yet_another_json_config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-16 02:54:36.000000 yet-another-json-config-0.0.4/src/yet_another_json_config.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 02:54:36.681005 yet-another-json-config-0.0.4/tests/
+-rw-rw-rw-   0        0        0     4939 2023-03-14 02:39:28.000000 yet-another-json-config-0.0.4/tests/test_config.py
```

### Comparing `yet-another-json-config-0.0.3/LICENSE` & `yet-another-json-config-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yet-another-json-config-0.0.3/PKG-INFO` & `yet-another-json-config-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yet-another-json-config
-Version: 0.0.3
+Version: 0.0.4
 Summary: Reads and write json files as a configuration file, supports nested json values.
 Author-email: engmtcdrm <gabif54409@rolenot.com>
 Project-URL: Homepage, https://github.com/engmtcdrm/yet-another-json-config
 Project-URL: Bug Tracker, https://github.com/engmtcdrm/yet-another-json-config/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yet-another-json-config-0.0.3/README.md` & `yet-another-json-config-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `yet-another-json-config-0.0.3/pyproject.toml` & `yet-another-json-config-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "yet-another-json-config"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="engmtcdrm", email="gabif54409@rolenot.com" },
 ]
 description = "Reads and write json files as a configuration file, supports nested json values."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `yet-another-json-config-0.0.3/src/yet_another_json_config/yet_another_json_config.py` & `yet-another-json-config-0.0.4/src/yet_another_json_config/yet_another_json_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,14 @@
             action_text = action[:-1]
 
         if keys == ():
             raise KeyError(f'No key specified to {action_text}.')
 
         # Convert based on being a tuple or not
         if type(keys[0]) == tuple:
-            print(keys)
             keys_list = list(*keys)
         else:
             keys_list = list(keys)
 
         if len(keys_list) == 0:
             raise KeyError(f'No key specified to {action_text}.')
```

### Comparing `yet-another-json-config-0.0.3/src/yet_another_json_config.egg-info/PKG-INFO` & `yet-another-json-config-0.0.4/src/yet_another_json_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yet-another-json-config
-Version: 0.0.3
+Version: 0.0.4
 Summary: Reads and write json files as a configuration file, supports nested json values.
 Author-email: engmtcdrm <gabif54409@rolenot.com>
 Project-URL: Homepage, https://github.com/engmtcdrm/yet-another-json-config
 Project-URL: Bug Tracker, https://github.com/engmtcdrm/yet-another-json-config/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yet-another-json-config-0.0.3/tests/test_config.py` & `yet-another-json-config-0.0.4/tests/test_config.py`

 * *Files identical despite different names*

