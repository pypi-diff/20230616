# Comparing `tmp/argtoml-0.1.1.tar.gz` & `tmp/argtoml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argtoml-0.1.1.tar", last modified: Thu Jun 15 19:37:43 2023, max compression
+gzip compressed data, was "argtoml-0.1.2.tar", last modified: Thu Jun 15 22:08:14 2023, max compression
```

## Comparing `argtoml-0.1.1.tar` & `argtoml-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 19:37:43.578075 argtoml-0.1.1/
--rw-r--r--   0 gum       (1000) gum       (1000)     1069 2023-06-10 10:02:47.000000 argtoml-0.1.1/LICENSE
--rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-15 19:37:43.578075 argtoml-0.1.1/PKG-INFO
--rw-r--r--   0 gum       (1000) gum       (1000)     1522 2023-06-07 09:20:09.000000 argtoml-0.1.1/README.md
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 19:37:43.571408 argtoml-0.1.1/argtoml/
--rw-r--r--   0 gum       (1000) gum       (1000)       92 2023-06-05 13:46:56.000000 argtoml-0.1.1/argtoml/__init__.py
--rw-r--r--   0 gum       (1000) gum       (1000)     6630 2023-06-15 19:35:31.000000 argtoml-0.1.1/argtoml/main.py
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 19:37:43.574742 argtoml-0.1.1/argtoml/tests/
--rw-r--r--   0 gum       (1000) gum       (1000)       25 2023-06-09 12:19:14.000000 argtoml-0.1.1/argtoml/tests/__init__.py
--rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.1/argtoml/tests/test_main.py
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 19:37:43.574742 argtoml-0.1.1/argtoml.egg-info/
--rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-15 19:37:43.000000 argtoml-0.1.1/argtoml.egg-info/PKG-INFO
--rw-r--r--   0 gum       (1000) gum       (1000)      273 2023-06-15 19:37:43.000000 argtoml-0.1.1/argtoml.egg-info/SOURCES.txt
--rw-r--r--   0 gum       (1000) gum       (1000)        1 2023-06-15 19:37:43.000000 argtoml-0.1.1/argtoml.egg-info/dependency_links.txt
--rw-r--r--   0 gum       (1000) gum       (1000)        8 2023-06-15 19:37:43.000000 argtoml-0.1.1/argtoml.egg-info/top_level.txt
--rw-r--r--   0 gum       (1000) gum       (1000)      939 2023-06-15 19:37:25.000000 argtoml-0.1.1/pyproject.toml
--rw-r--r--   0 gum       (1000) gum       (1000)       38 2023-06-15 19:37:43.578075 argtoml-0.1.1/setup.cfg
--rw-r--r--   0 gum       (1000) gum       (1000)       61 2023-06-07 07:31:31.000000 argtoml-0.1.1/setup.py
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 19:37:43.574742 argtoml-0.1.1/tests/
--rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.1/tests/test_main.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:08:14.253219 argtoml-0.1.2/
+-rw-r--r--   0 gum       (1000) gum       (1000)     1069 2023-06-10 10:02:47.000000 argtoml-0.1.2/LICENSE
+-rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-15 22:08:14.249886 argtoml-0.1.2/PKG-INFO
+-rw-r--r--   0 gum       (1000) gum       (1000)     1522 2023-06-07 09:20:09.000000 argtoml-0.1.2/README.md
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:08:14.246552 argtoml-0.1.2/argtoml/
+-rw-r--r--   0 gum       (1000) gum       (1000)       92 2023-06-05 13:46:56.000000 argtoml-0.1.2/argtoml/__init__.py
+-rw-r--r--   0 gum       (1000) gum       (1000)     7788 2023-06-15 22:03:48.000000 argtoml-0.1.2/argtoml/main.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:08:14.249886 argtoml-0.1.2/argtoml/tests/
+-rw-r--r--   0 gum       (1000) gum       (1000)       25 2023-06-09 12:19:14.000000 argtoml-0.1.2/argtoml/tests/__init__.py
+-rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.2/argtoml/tests/test_main.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:08:14.246552 argtoml-0.1.2/argtoml.egg-info/
+-rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-15 22:08:14.000000 argtoml-0.1.2/argtoml.egg-info/PKG-INFO
+-rw-r--r--   0 gum       (1000) gum       (1000)      273 2023-06-15 22:08:14.000000 argtoml-0.1.2/argtoml.egg-info/SOURCES.txt
+-rw-r--r--   0 gum       (1000) gum       (1000)        1 2023-06-15 22:08:14.000000 argtoml-0.1.2/argtoml.egg-info/dependency_links.txt
+-rw-r--r--   0 gum       (1000) gum       (1000)        8 2023-06-15 22:08:14.000000 argtoml-0.1.2/argtoml.egg-info/top_level.txt
+-rw-r--r--   0 gum       (1000) gum       (1000)      939 2023-06-15 22:07:57.000000 argtoml-0.1.2/pyproject.toml
+-rw-r--r--   0 gum       (1000) gum       (1000)       38 2023-06-15 22:08:14.253219 argtoml-0.1.2/setup.cfg
+-rw-r--r--   0 gum       (1000) gum       (1000)       61 2023-06-07 07:31:31.000000 argtoml-0.1.2/setup.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 22:08:14.249886 argtoml-0.1.2/tests/
+-rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.2/tests/test_main.py
```

### Comparing `argtoml-0.1.1/LICENSE` & `argtoml-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `argtoml-0.1.1/PKG-INFO` & `argtoml-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.1.1
+Version: 0.1.2
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <jono-dev.6psuo@simplelogin.com>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `argtoml-0.1.1/README.md` & `argtoml-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `argtoml-0.1.1/argtoml/main.py` & `argtoml-0.1.2/argtoml/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,29 +8,50 @@
 import builtins
 import os
 import tomllib
 from argparse import ArgumentParser
 from ast import literal_eval
 from pathlib import Path
 from types import SimpleNamespace
+from typing import Optional, Union
 
 import __main__
 
 TOML_PATH = ""
 
-
 class Struct:
     def __init__(self, **entries):
         self.__dict__.update(entries)
 
     def __repr__(self):
         return "<%s>" % str(
             "\n ".join("%s : %s" % (k, repr(v)) for (k, v) in self.__dict__.items())
         )
 
+def string_to_path(string: str, prefix: Path = Path.cwd()):
+    """
+    Convert a string to a Path object.
+    """
+    if string == "~":
+        return Path.home()
+    elif string == ".":
+        return prefix
+    elif string == "..":
+        return prefix.parent
+    elif len(string) > 0 and string[0] == "/":
+        return Path(string)
+    elif len(string) > 1 and string[0:2] == "~/":
+        return Path.home() / string[2:]
+    elif len(string) > 1 and string[0:2] == "./":
+        return prefix / string[2:]
+    elif len(string) > 2 and string[0:3] == "../":
+        return prefix.parent / string[3:]
+    else:
+        return string
+
 
 def locate_toml():
     """
     Locate the toml file in the current directory.
     """
     # The toml file can be named config.toml or have the same name as the main file..
     main_file = Path(__main__.__file__)
@@ -45,15 +66,15 @@
             toml_file_names.append(dir.parent.name + ".toml")
         else:
             toml_file_names.append(dir.name + ".toml")
 
     # Search for the toml file in the current directory.
     for file in os.listdir("."):
         if file in toml_file_names:
-            return file
+            return str(Path.cwd() / file)
 
     # Search for the toml file in the project directory or its parents.
     while dir.name != "":
         for file in os.listdir(dir):
             if file in toml_file_names:
                 return os.path.join(dir, file)
         dir = dir.parent
@@ -89,15 +110,15 @@
                 f"--{prefix}{key}",
                 required=False,
                 type=type_,
                 help=f"defaults to {value}",
             )
 
 
-def fill_toml_args(args, toml, prefix="", filled=False):
+def fill_toml_args(args, toml, prefix="", filled=False, path: Optional[Path]=None):
     namespace = SimpleNamespace()
     for raw_key, value in toml.items():
         # Check if the user provided the same key but with dashes instead of underscores.
         key = raw_key.replace("-", "_")
         key_str = prefix + "." + key if prefix else key
         # Boolean variables have 2 arguments.
         alt_key_str = prefix + ".no_" + key if prefix else "no_" + key
@@ -116,14 +137,17 @@
             # Check whether both boolean arguments are empty before filling in the default.
             elif type(value) == bool:
                 if args[alt_key_str] is None:
                     setattr(namespace, key, value)  # Fill in the default.
                 else:
                     setattr(namespace, key, False)  # The anti-argument was called.
                     del args[alt_key_str]
+
+            elif path is not None and type(value) == str:
+                setattr(namespace, key, string_to_path(value, path))
                 
             else:
                 setattr(namespace, key, value)
 
         # Fill in the value from the command line.
         else:
             if filled:
@@ -148,14 +172,17 @@
                         assert type(arg_value) == dict
                         arg_value = fill_toml_args(args, arg_value, key, filled)
 
                     case builtins.bool:
                         assert type(arg_value) == bool
                         if args[alt_key_str] is not None:
                             raise ValueError(f"Do not call --{key_str} and --{alt_key_str} simultaneously.")
+                    case builtins.str:
+                        assert type(arg_value) == str
+                        arg_value = string_to_path(arg_value, path) if path is not None else arg_value
 
                     case _:
                         assert type(value) == type(arg_value)
 
             except AssertionError:
                 raise TypeError(
                     f"Type mismatch for {key_str}: the type from {TOML_PATH} is {type(value)}, but the CLI got a {type(arg_value)}"
@@ -163,31 +190,34 @@
 
             setattr(namespace, key, arg_value)
             del args[key_str]
 
     return namespace
 
 
-def parse_args(parser=ArgumentParser(), toml=None):
+def parse_args(parser=ArgumentParser(), toml=None, path: Union[Path, bool]=False):
     """
     Add the content of a toml file as argument with default values
     to an ArgumentParser object.
     """
 
     # Locate the toml file.
     global TOML_PATH
     if toml is None:
         toml = locate_toml()
         TOML_PATH = toml
 
+    if path == True:
+        path = Path(toml).parent
+
     # Add the keys from the toml file as arguments.
     with open(toml, "rb") as f:
         toml = tomllib.load(f)
     add_toml_args(parser, toml)
     args = vars(parser.parse_args())
 
-    namespace = fill_toml_args(args, toml)
+    namespace = fill_toml_args(args, toml, path=path if path else None)
     for key, value in args.items():
         if value is not None:
             setattr(namespace, key, value)
 
     return namespace
```

### Comparing `argtoml-0.1.1/argtoml.egg-info/PKG-INFO` & `argtoml-0.1.2/argtoml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.1.1
+Version: 0.1.2
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <jono-dev.6psuo@simplelogin.com>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `argtoml-0.1.1/pyproject.toml` & `argtoml-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "argtoml"
-version = "0.1.1"
+version = "0.1.2"
 description = "Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file."
 dynamic = ["readme"]
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

