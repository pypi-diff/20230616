# Comparing `tmp/argtoml-0.1.2.tar.gz` & `tmp/argtoml-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argtoml-0.1.2.tar", last modified: Thu Jun 15 22:08:14 2023, max compression
+gzip compressed data, was "argtoml-0.1.3.tar", last modified: Thu Jun 15 22:16:30 2023, max compression
```

## Comparing `argtoml-0.1.2.tar` & `argtoml-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:08:14.253219 argtoml-0.1.2/
--rw-r--r--   0 gum       (1000) gum       (1000)     1069 2023-06-10 10:02:47.000000 argtoml-0.1.2/LICENSE
--rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-15 22:08:14.249886 argtoml-0.1.2/PKG-INFO
--rw-r--r--   0 gum       (1000) gum       (1000)     1522 2023-06-07 09:20:09.000000 argtoml-0.1.2/README.md
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:08:14.246552 argtoml-0.1.2/argtoml/
--rw-r--r--   0 gum       (1000) gum       (1000)       92 2023-06-05 13:46:56.000000 argtoml-0.1.2/argtoml/__init__.py
--rw-r--r--   0 gum       (1000) gum       (1000)     7788 2023-06-15 22:03:48.000000 argtoml-0.1.2/argtoml/main.py
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:08:14.249886 argtoml-0.1.2/argtoml/tests/
--rw-r--r--   0 gum       (1000) gum       (1000)       25 2023-06-09 12:19:14.000000 argtoml-0.1.2/argtoml/tests/__init__.py
--rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.2/argtoml/tests/test_main.py
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:08:14.246552 argtoml-0.1.2/argtoml.egg-info/
--rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-15 22:08:14.000000 argtoml-0.1.2/argtoml.egg-info/PKG-INFO
--rw-r--r--   0 gum       (1000) gum       (1000)      273 2023-06-15 22:08:14.000000 argtoml-0.1.2/argtoml.egg-info/SOURCES.txt
--rw-r--r--   0 gum       (1000) gum       (1000)        1 2023-06-15 22:08:14.000000 argtoml-0.1.2/argtoml.egg-info/dependency_links.txt
--rw-r--r--   0 gum       (1000) gum       (1000)        8 2023-06-15 22:08:14.000000 argtoml-0.1.2/argtoml.egg-info/top_level.txt
--rw-r--r--   0 gum       (1000) gum       (1000)      939 2023-06-15 22:07:57.000000 argtoml-0.1.2/pyproject.toml
--rw-r--r--   0 gum       (1000) gum       (1000)       38 2023-06-15 22:08:14.253219 argtoml-0.1.2/setup.cfg
--rw-r--r--   0 gum       (1000) gum       (1000)       61 2023-06-07 07:31:31.000000 argtoml-0.1.2/setup.py
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:08:14.249886 argtoml-0.1.2/tests/
--rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.2/tests/test_main.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:16:30.603556 argtoml-0.1.3/
+-rw-r--r--   0 gum       (1000) gum       (1000)     1069 2023-06-10 10:02:47.000000 argtoml-0.1.3/LICENSE
+-rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-15 22:16:30.603556 argtoml-0.1.3/PKG-INFO
+-rw-r--r--   0 gum       (1000) gum       (1000)     1522 2023-06-07 09:20:09.000000 argtoml-0.1.3/README.md
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:16:30.600223 argtoml-0.1.3/argtoml/
+-rw-r--r--   0 gum       (1000) gum       (1000)       92 2023-06-05 13:46:56.000000 argtoml-0.1.3/argtoml/__init__.py
+-rw-r--r--   0 gum       (1000) gum       (1000)     7832 2023-06-15 22:16:08.000000 argtoml-0.1.3/argtoml/main.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:16:30.603556 argtoml-0.1.3/argtoml/tests/
+-rw-r--r--   0 gum       (1000) gum       (1000)       25 2023-06-09 12:19:14.000000 argtoml-0.1.3/argtoml/tests/__init__.py
+-rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.3/argtoml/tests/test_main.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:16:30.603556 argtoml-0.1.3/argtoml.egg-info/
+-rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-15 22:16:30.000000 argtoml-0.1.3/argtoml.egg-info/PKG-INFO
+-rw-r--r--   0 gum       (1000) gum       (1000)      273 2023-06-15 22:16:30.000000 argtoml-0.1.3/argtoml.egg-info/SOURCES.txt
+-rw-r--r--   0 gum       (1000) gum       (1000)        1 2023-06-15 22:16:30.000000 argtoml-0.1.3/argtoml.egg-info/dependency_links.txt
+-rw-r--r--   0 gum       (1000) gum       (1000)        8 2023-06-15 22:16:30.000000 argtoml-0.1.3/argtoml.egg-info/top_level.txt
+-rw-r--r--   0 gum       (1000) gum       (1000)      939 2023-06-15 22:16:20.000000 argtoml-0.1.3/pyproject.toml
+-rw-r--r--   0 gum       (1000) gum       (1000)       38 2023-06-15 22:16:30.603556 argtoml-0.1.3/setup.cfg
+-rw-r--r--   0 gum       (1000) gum       (1000)       61 2023-06-07 07:31:31.000000 argtoml-0.1.3/setup.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:16:30.603556 argtoml-0.1.3/tests/
+-rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.3/tests/test_main.py
```

### Comparing `argtoml-0.1.2/LICENSE` & `argtoml-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `argtoml-0.1.2/PKG-INFO` & `argtoml-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.1.2
+Version: 0.1.3
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <jono-dev.6psuo@simplelogin.com>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `argtoml-0.1.2/README.md` & `argtoml-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `argtoml-0.1.2/argtoml/main.py` & `argtoml-0.1.3/argtoml/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             )
 
         arg_value = args[key_str] if key_str in args else None
 
         # Fill in the default value from the toml file.
         if arg_value is None:
             if type(value) == dict:
-                setattr(namespace, key, fill_toml_args(args, value, key, filled))
+                setattr(namespace, key, fill_toml_args(args, value, key, filled, path=path))
             # Check whether both boolean arguments are empty before filling in the default.
             elif type(value) == bool:
                 if args[alt_key_str] is None:
                     setattr(namespace, key, value)  # Fill in the default.
                 else:
                     setattr(namespace, key, False)  # The anti-argument was called.
                     del args[alt_key_str]
@@ -159,22 +159,22 @@
                 match type(value):
                     case builtins.list:
                         arg_value = literal_eval(arg_value)
                         assert type(arg_value) == list
                         for i, arg in enumerate(arg_value):
                             if type(arg) == dict:
                                 # TODO; I might need to check for whether any values are filled twice.
-                                arg_value[i] = fill_toml_args(args, arg, key, filled)
+                                arg_value[i] = fill_toml_args(args, arg, key, filled, path=path)
 
                     case builtins.dict:
                         # Check if values are not filled twice.
-                        fill_toml_args(args, value, key, True)
+                        fill_toml_args(args, value, key, True, path=path)
                         arg_value = literal_eval(arg_value)
                         assert type(arg_value) == dict
-                        arg_value = fill_toml_args(args, arg_value, key, filled)
+                        arg_value = fill_toml_args(args, arg_value, key, filled, path=path)
 
                     case builtins.bool:
                         assert type(arg_value) == bool
                         if args[alt_key_str] is not None:
                             raise ValueError(f"Do not call --{key_str} and --{alt_key_str} simultaneously.")
                     case builtins.str:
                         assert type(arg_value) == str
```

### Comparing `argtoml-0.1.2/argtoml.egg-info/PKG-INFO` & `argtoml-0.1.3/argtoml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.1.2
+Version: 0.1.3
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <jono-dev.6psuo@simplelogin.com>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `argtoml-0.1.2/pyproject.toml` & `argtoml-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "argtoml"
-version = "0.1.2"
+version = "0.1.3"
 description = "Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file."
 dynamic = ["readme"]
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

