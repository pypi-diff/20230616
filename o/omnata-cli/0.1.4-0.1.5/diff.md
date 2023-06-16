# Comparing `tmp/omnata_cli-0.1.4.tar.gz` & `tmp/omnata_cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_cli-0.1.4.tar", max compression
+gzip compressed data, was "omnata_cli-0.1.5.tar", max compression
```

## Comparing `omnata_cli-0.1.4.tar` & `omnata_cli-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    26526 2023-06-05 22:18:59.884947 omnata_cli-0.1.4/LICENSE
--rw-r--r--   0        0        0       49 2023-06-05 22:18:59.884947 omnata_cli-0.1.4/README.md
--rw-r--r--   0        0        0      534 2023-06-05 22:18:59.884947 omnata_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1130 2023-06-05 22:18:59.884947 omnata_cli-0.1.4/src/omnata_cli/__init__.py
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 omnata_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-16 03:18:22.000814 omnata_cli-0.1.5/LICENSE
+-rw-r--r--   0        0        0       49 2023-06-16 03:18:22.000814 omnata_cli-0.1.5/README.md
+-rw-r--r--   0        0        0      534 2023-06-16 03:18:22.000814 omnata_cli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1039 2023-06-16 03:18:22.000814 omnata_cli-0.1.5/src/omnata_cli/__init__.py
+-rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 omnata_cli-0.1.5/PKG-INFO
```

### Comparing `omnata_cli-0.1.4/LICENSE` & `omnata_cli-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_cli-0.1.4/pyproject.toml` & `omnata_cli-0.1.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omnata-cli"
-version = "0.1.4"
+version = "0.1.5"
 description = "A command line interface for Omnata"
 authors = ["James Weakley <james.weakley@omnata.com>"]
 readme = "README.md"
 packages = [{include = "omnata_cli", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `omnata_cli-0.1.4/src/omnata_cli/__init__.py` & `omnata_cli-0.1.5/src/omnata_cli/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-from pathlib import Path
 import typer
 from snowcli import config
 from snowcli.config import AppConfig
 
 
 app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
 
 @app.command()
 def docs():
     """Open the Omnata CLI documentation in your browser."""
     typer.launch("https://docs.omnata.com")
 try:
-    from omnata_plugin_devkit import cli # 
-
+    from omnata_plugin_devkit import cli # pylint: disable=import-error
     # If the import is successful, we can add its commands to our application
-    # Assume `external_command` is the command you want to include from the external package
     app.add_typer(cli.app, name="plugin_dev")
 
 except ImportError:
     @app.command()
     def plugin_dev():
-        "To use the plugin-dev subcommand, run `pip install omnata_plugin_devkit`."
-        print("To use the plugin-dev subcommand, run `pip install omnata_plugin_devkit`.")
+        "To use the plugin-dev subcommand, run `pip install omnata-plugin-devkit`."
+        print("To use the plugin-dev subcommand, run `pip install omnata-plugin-devkit`.")
         raise typer.Abort()
 
 
 def check_env_conf(env_conf,environment):
     if env_conf is None:
         print(
             f"The {environment} environment is not configured in app.toml "
```

### Comparing `omnata_cli-0.1.4/PKG-INFO` & `omnata_cli-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnata-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: A command line interface for Omnata
 Author: James Weakley
 Author-email: james.weakley@omnata.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

