# Comparing `tmp/props2yaml-0.1.1.tar.gz` & `tmp/props2yaml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "props2yaml-0.1.1.tar", last modified: Thu Jun 15 16:36:44 2023, max compression
+gzip compressed data, was "props2yaml-0.1.2.tar", last modified: Thu Jun 15 22:07:38 2023, max compression
```

## Comparing `props2yaml-0.1.1.tar` & `props2yaml-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:36:44.812393 props2yaml-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:36:44.812393 props2yaml-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:36:44.812393 props2yaml-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-15 16:36:35.000000 props2yaml-0.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-15 16:36:35.000000 props2yaml-0.1.1/.github/workflows/staging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-15 16:36:35.000000 props2yaml-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 16:36:35.000000 props2yaml-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-15 16:36:44.812393 props2yaml-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-15 16:36:35.000000 props2yaml-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-15 16:36:35.000000 props2yaml-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:36:44.812393 props2yaml-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:36:44.812393 props2yaml-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:36:44.812393 props2yaml-0.1.1/src/props2yaml/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 16:36:35.000000 props2yaml-0.1.1/src/props2yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-15 16:36:35.000000 props2yaml-0.1.1/src/props2yaml/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1598 2023-06-15 16:36:35.000000 props2yaml-0.1.1/src/props2yaml/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:36:44.812393 props2yaml-0.1.1/src/props2yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-15 16:36:44.000000 props2yaml-0.1.1/src/props2yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-15 16:36:44.000000 props2yaml-0.1.1/src/props2yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:36:44.000000 props2yaml-0.1.1/src/props2yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 16:36:44.000000 props2yaml-0.1.1/src/props2yaml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 16:36:44.000000 props2yaml-0.1.1/src/props2yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 16:36:44.000000 props2yaml-0.1.1/src/props2yaml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:38.532318 props2yaml-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:38.532318 props2yaml-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:38.532318 props2yaml-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-15 22:07:25.000000 props2yaml-0.1.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-15 22:07:25.000000 props2yaml-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-15 22:07:25.000000 props2yaml-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 22:07:25.000000 props2yaml-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-15 22:07:38.532318 props2yaml-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-15 22:07:25.000000 props2yaml-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-15 22:07:25.000000 props2yaml-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:07:38.532318 props2yaml-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:38.532318 props2yaml-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:38.532318 props2yaml-0.1.2/src/props2yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-15 22:07:25.000000 props2yaml-0.1.2/src/props2yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 22:07:25.000000 props2yaml-0.1.2/src/props2yaml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-15 22:07:25.000000 props2yaml-0.1.2/src/props2yaml/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-15 22:07:25.000000 props2yaml-0.1.2/src/props2yaml/converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-06-15 22:07:25.000000 props2yaml-0.1.2/src/props2yaml/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:38.532318 props2yaml-0.1.2/src/props2yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-15 22:07:38.000000 props2yaml-0.1.2/src/props2yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-15 22:07:38.000000 props2yaml-0.1.2/src/props2yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:07:38.000000 props2yaml-0.1.2/src/props2yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 22:07:38.000000 props2yaml-0.1.2/src/props2yaml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:07:38.000000 props2yaml-0.1.2/src/props2yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 22:07:38.000000 props2yaml-0.1.2/src/props2yaml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:38.532318 props2yaml-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-15 22:07:25.000000 props2yaml-0.1.2/tests/test_converter.py
```

### Comparing `props2yaml-0.1.1/.github/workflows/release.yml` & `props2yaml-0.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `props2yaml-0.1.1/.gitignore` & `props2yaml-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `props2yaml-0.1.1/LICENSE` & `props2yaml-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `props2yaml-0.1.1/PKG-INFO` & `props2yaml-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,58 @@
 Metadata-Version: 2.1
 Name: props2yaml
-Version: 0.1.1
+Version: 0.1.2
 Summary: Convert .properties files into .yaml
 Author-email: "Jorge F. Sánchez" <props2yaml@jfsanchez.net>
 License: MIT
 Project-URL: Homepage, https://github.com/jfsanchez91/props2yaml
 Project-URL: Bug Tracker, https://github.com/jfsanchez91/props2yaml/issues
 Keywords: yaml,properties,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 # props2yaml
+
 Convert `.properties` files into `.yaml`
 
 ## install
+
 ```bash
 pip install -U props2yaml
-p2y --version
+props2yaml --version
 ```
 
-## usage
- - ```bash
-   p2y -i config.properties -o config.yml            # (1)
+## cli usage
+
+- ```bash
+   props2yaml config.properties -o config.yml          # (1)
    ```
- - ```bash
-   p2y -i config.properties > config.yml             # (2)
+- ```bash
+   props2yaml config.properties > config.yml           # (2)
    ```
- - ```bash
-   cat config.properties | p2y -i - -o config.yml    # (3)
+- ```bash
+   cat config.properties | props2yaml -o config.yml    # (3)
    ```
- - ```bash
-   cat config.properties | p2y -i - > config.yml     # (4)
+- ```bash
+   cat config.properties | props2yaml > config.yml     # (4)
    ```
+
+## python usage
+
+```python3
+from props2yaml import convert_properties_to_yaml
+
+converted = convert_properties_to_yaml("config.prop.value=50")
+print(converted)
+```
+_output:_
+```yaml
+config:
+  prop:
+    value: '50'
+```
```

### Comparing `props2yaml-0.1.1/pyproject.toml` & `props2yaml-0.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -20,27 +20,47 @@
 dependencies = [
     "pyyaml",
 ]
 dynamic = [
     "version",
 ]
 
+[project.optional-dependencies]
+dev = [
+    "black",
+]
+test = [
+    "pytest",
+]
+
 [build-system]
 requires = [
     "setuptools>=45",
     "setuptools_scm[toml]>=7.1"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 version_scheme = "no-guess-dev"
-local_scheme="no-local-version"
+local_scheme = "no-local-version"
 
 [project.urls]
 "Homepage" = "https://github.com/jfsanchez91/props2yaml"
 "Bug Tracker" = "https://github.com/jfsanchez91/props2yaml/issues"
 
 [project.scripts]
-p2y = "props2yaml:main"
+props2yaml = "props2yaml.main:main"
 
 [tool.black]
 line-length = 120
+
+[tool.pytest.ini_options]
+pythonpath = [
+  ".", "src",
+]
+log_cli = true
+log_cli_level = "ERROR"
+
+log_file = "pytest.log"
+log_file_level = "INFO"
+log_file_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
+log_file_date_format = "%Y-%m-%d %H:%M:%S"
```

### Comparing `props2yaml-0.1.1/src/props2yaml/main.py` & `props2yaml-0.1.2/src/props2yaml/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,46 @@
 #!/usr/bin/env python3
 
-import sys
 import argparse
-import re
-import yaml
-
-from props2yaml.__version__ import __version__
-
+import sys
 
-def convert_properties_to_yaml(properties_file):
-    properties = {}
-    with properties_file as in_file:
-        for line in in_file:
-            line = line.strip()
-            if line and not line.startswith("#"):
-                key, value = re.split(r"\s*=\s*", line, maxsplit=1)
-                nested_keys = key.split(".")
-                nested_dict = properties
-                for nested_key in nested_keys[:-1]:
-                    nested_dict = nested_dict.setdefault(nested_key, {})
-                nested_dict[nested_keys[-1]] = value
-    return properties
+from props2yaml import __version__
+from props2yaml import convert_properties_to_yaml
 
 
 def main():
-    parser = argparse.ArgumentParser(description="Convert .properties files into .yaml.")
-    parser.add_argument('-v', '--version', action='version', version="%(prog)s " + __version__)
+    parser = argparse.ArgumentParser(
+        prog="props2yaml",
+        description="Convert .properties files into .yaml.",
+        epilog="Example: %(prog)s config1.properties config2.properties -o config.yml",
+    )
+    parser.add_argument("-v", "--version", action="version", version="%(prog)s " + __version__)
     parser.add_argument(
-        "-i",
-        "--input-file",
+        "input_files",
+        metavar="INPUT_FILE",
         type=argparse.FileType("r"),
-        help=f"Input properties filename",
-        required=True,
+        nargs="*",
+        help="Input properties filename. Default stdin.",
+        default=[sys.stdin],
     )
     parser.add_argument(
         "-o",
         "--output-file",
         type=argparse.FileType("w"),
-        help=f"Output yaml filename",
+        help=f"Output yaml filename. Default stdout.",
         required=False,
+        default=sys.stdout,
     )
     args = parser.parse_args()
 
-    converted = convert_properties_to_yaml(properties_file=args.input_file)
-
-    if args.output_file:
-        with args.output_file as out_file:
-            yaml.dump(converted, out_file, default_flow_style=False)
-    else:
-        yaml.dump(converted, sys.stdout, default_flow_style=False)
+    with args.output_file as output_file:
+        for input_file in args.input_files:
+            with input_file as file:
+                properties = file.read()
+                converted = convert_properties_to_yaml(properties)
+                if file.fileno() != 0:
+                    output_file.write(f"#{file.name}\n")
+                output_file.write(f"{converted}\n")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `props2yaml-0.1.1/src/props2yaml.egg-info/PKG-INFO` & `props2yaml-0.1.2/src/props2yaml.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,58 @@
 Metadata-Version: 2.1
 Name: props2yaml
-Version: 0.1.1
+Version: 0.1.2
 Summary: Convert .properties files into .yaml
 Author-email: "Jorge F. Sánchez" <props2yaml@jfsanchez.net>
 License: MIT
 Project-URL: Homepage, https://github.com/jfsanchez91/props2yaml
 Project-URL: Bug Tracker, https://github.com/jfsanchez91/props2yaml/issues
 Keywords: yaml,properties,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 # props2yaml
+
 Convert `.properties` files into `.yaml`
 
 ## install
+
 ```bash
 pip install -U props2yaml
-p2y --version
+props2yaml --version
 ```
 
-## usage
- - ```bash
-   p2y -i config.properties -o config.yml            # (1)
+## cli usage
+
+- ```bash
+   props2yaml config.properties -o config.yml          # (1)
    ```
- - ```bash
-   p2y -i config.properties > config.yml             # (2)
+- ```bash
+   props2yaml config.properties > config.yml           # (2)
    ```
- - ```bash
-   cat config.properties | p2y -i - -o config.yml    # (3)
+- ```bash
+   cat config.properties | props2yaml -o config.yml    # (3)
    ```
- - ```bash
-   cat config.properties | p2y -i - > config.yml     # (4)
+- ```bash
+   cat config.properties | props2yaml > config.yml     # (4)
    ```
+
+## python usage
+
+```python3
+from props2yaml import convert_properties_to_yaml
+
+converted = convert_properties_to_yaml("config.prop.value=50")
+print(converted)
+```
+_output:_
+```yaml
+config:
+  prop:
+    value: '50'
+```
```

