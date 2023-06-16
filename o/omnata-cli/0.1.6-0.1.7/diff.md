# Comparing `tmp/omnata_cli-0.1.6.tar.gz` & `tmp/omnata_cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_cli-0.1.6.tar", max compression
+gzip compressed data, was "omnata_cli-0.1.7.tar", max compression
```

## Comparing `omnata_cli-0.1.6.tar` & `omnata_cli-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    26526 2023-06-16 03:30:20.863293 omnata_cli-0.1.6/LICENSE
--rw-r--r--   0        0        0       49 2023-06-16 03:30:20.863293 omnata_cli-0.1.6/README.md
--rw-r--r--   0        0        0      534 2023-06-16 03:30:20.863293 omnata_cli-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1039 2023-06-16 03:30:20.863293 omnata_cli-0.1.6/src/omnata_cli/__init__.py
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 omnata_cli-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-16 03:46:24.872951 omnata_cli-0.1.7/LICENSE
+-rw-r--r--   0        0        0       49 2023-06-16 03:46:24.872951 omnata_cli-0.1.7/README.md
+-rw-r--r--   0        0        0      534 2023-06-16 03:46:24.872951 omnata_cli-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1039 2023-06-16 03:46:24.872951 omnata_cli-0.1.7/src/omnata_cli/__init__.py
+-rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 omnata_cli-0.1.7/PKG-INFO
```

### Comparing `omnata_cli-0.1.6/LICENSE` & `omnata_cli-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_cli-0.1.6/pyproject.toml` & `omnata_cli-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omnata-cli"
-version = "0.1.6"
+version = "0.1.7"
 description = "A command line interface for Omnata"
 authors = ["James Weakley <james.weakley@omnata.com>"]
 readme = "README.md"
 packages = [{include = "omnata_cli", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `omnata_cli-0.1.6/src/omnata_cli/__init__.py` & `omnata_cli-0.1.7/src/omnata_cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # If the import is successful, we can add its commands to our application
     app.add_typer(cli.app, name="plugin_dev")
 
 except ImportError:
     @app.command()
     def plugin_dev():
         "To use the plugin-dev subcommand, run `pip install omnata-plugin-devkit`."
-        print("To use the plugin-dev subcommand, run `pip install omnata-plugin-devkit`.")
+        print("To use the plugin_dev subcommand, run `pip install omnata-plugin-devkit`.")
         raise typer.Abort()
 
 
 def check_env_conf(env_conf,environment):
     if env_conf is None:
         print(
             f"The {environment} environment is not configured in app.toml "
```

### Comparing `omnata_cli-0.1.6/PKG-INFO` & `omnata_cli-0.1.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnata-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: A command line interface for Omnata
 Author: James Weakley
 Author-email: james.weakley@omnata.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

