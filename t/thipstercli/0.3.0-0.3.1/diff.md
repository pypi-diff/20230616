# Comparing `tmp/thipstercli-0.3.0.tar.gz` & `tmp/thipstercli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipstercli-0.3.0.tar", last modified: Fri Jun 16 09:38:10 2023, max compression
+gzip compressed data, was "thipstercli-0.3.1.tar", last modified: Fri Jun 16 12:09:36 2023, max compression
```

## Comparing `thipstercli-0.3.0.tar` & `thipstercli-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:38:10.049243 thipstercli-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-16 09:38:06.000000 thipstercli-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-16 09:38:10.049243 thipstercli-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4516 2023-06-16 09:38:06.000000 thipstercli-0.3.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1361 2023-06-16 09:38:06.000000 thipstercli-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 09:38:10.049243 thipstercli-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1823 2023-06-16 09:38:07.000000 thipstercli-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:38:10.045243 thipstercli-0.3.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 09:38:06.000000 thipstercli-0.3.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-06-16 09:38:06.000000 thipstercli-0.3.0/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3847 2023-06-16 09:38:06.000000 thipstercli-0.3.0/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     3137 2023-06-16 09:38:06.000000 thipstercli-0.3.0/tests/test_providers.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-06-16 09:38:06.000000 thipstercli-0.3.0/tests/test_repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:38:10.045243 thipstercli-0.3.0/thipstercli/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6116 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/cli.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/config.py
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/constants.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/display.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/helpers.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/providers.py
--rw-r--r--   0 root         (0) root         (0)     3438 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:38:10.049243 thipstercli-0.3.0/thipstercli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-16 09:38:10.000000 thipstercli-0.3.0/thipstercli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      567 2023-06-16 09:38:10.000000 thipstercli-0.3.0/thipstercli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 09:38:10.000000 thipstercli-0.3.0/thipstercli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-16 09:38:10.000000 thipstercli-0.3.0/thipstercli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      265 2023-06-16 09:38:10.000000 thipstercli-0.3.0/thipstercli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-16 09:38:10.000000 thipstercli-0.3.0/thipstercli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:09:36.107291 thipstercli-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-16 12:09:32.000000 thipstercli-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-16 12:09:36.107291 thipstercli-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-06-16 12:09:32.000000 thipstercli-0.3.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-06-16 12:09:32.000000 thipstercli-0.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 12:09:36.107291 thipstercli-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-06-16 12:09:33.000000 thipstercli-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:09:36.107291 thipstercli-0.3.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 12:09:32.000000 thipstercli-0.3.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-16 12:09:32.000000 thipstercli-0.3.1/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-06-16 12:09:32.000000 thipstercli-0.3.1/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-06-16 12:09:32.000000 thipstercli-0.3.1/tests/test_providers.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-06-16 12:09:32.000000 thipstercli-0.3.1/tests/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:09:36.107291 thipstercli-0.3.1/thipstercli/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6108 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/config.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/display.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/providers.py
+-rw-r--r--   0 root         (0) root         (0)     3438 2023-06-16 12:09:32.000000 thipstercli-0.3.1/thipstercli/repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:09:36.107291 thipstercli-0.3.1/thipstercli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-16 12:09:36.000000 thipstercli-0.3.1/thipstercli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      567 2023-06-16 12:09:36.000000 thipstercli-0.3.1/thipstercli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:09:36.000000 thipstercli-0.3.1/thipstercli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-16 12:09:36.000000 thipstercli-0.3.1/thipstercli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-16 12:09:36.000000 thipstercli-0.3.1/thipstercli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-16 12:09:36.000000 thipstercli-0.3.1/thipstercli.egg-info/top_level.txt
```

### Comparing `thipstercli-0.3.0/LICENSE` & `thipstercli-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.0/PKG-INFO` & `thipstercli-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.3.0 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.3.1 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.3.0/README.md` & `thipstercli-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.0/pyproject.toml` & `thipstercli-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.0/setup.py` & `thipstercli-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('.').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as f:
     long_description = f.read()
```

### Comparing `thipstercli-0.3.0/tests/conftest.py` & `thipstercli-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.0/tests/test_cli.py` & `thipstercli-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.0/tests/test_providers.py` & `thipstercli-0.3.1/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.0/tests/test_repository.py` & `thipstercli-0.3.1/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.0/thipstercli/cli.py` & `thipstercli-0.3.1/thipstercli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """THipster CLI."""
 from pathlib import Path
 
 import typer
 from rich import print
 from thipster import Engine as ThipsterEngine
 from thipster.auth import Google
-from thipster.engine.exceptions import THipsterException
+from thipster.engine.exceptions import THipsterError
 from thipster.parser import ParserFactory
 from thipster.repository import GithubRepo, LocalRepo
 from thipster.terraform import Terraform
 
 import thipstercli.constants as constants
 from thipstercli import providers, repository
 from thipstercli.config import app_dir, init_parameters, state
@@ -141,15 +141,15 @@
 
         if apply:
             print("Type 'yes' to apply the changes : ")
             print(engine._apply_terraform())
 
         print_if_verbose('Done! :tada:')
 
-    except THipsterException as e:
+    except THipsterError as e:
         error(e.message)
     except FileNotFoundError as e:
         error(
             f'No such file or directory : [bold][red]{e.filename}[/red][/bold]',
         )
     except Exception as e:
         error(*e.args)
```

### Comparing `thipstercli-0.3.0/thipstercli/config.py` & `thipstercli-0.3.1/thipstercli/config.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.0/thipstercli/display.py` & `thipstercli-0.3.1/thipstercli/display.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.0/thipstercli/helpers.py` & `thipstercli-0.3.1/thipstercli/helpers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.0/thipstercli/providers.py` & `thipstercli-0.3.1/thipstercli/providers.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,19 @@
     get_auth_provider_class,
     get_thipster_module_class_list,
 )
 
 provider_app = typer.Typer(no_args_is_help=True)
 
 
+@provider_app.callback()
+def _callback():
+    """Manage authentification providers."""
+
+
 @provider_app.command('list')
 def _list():
     """List all the supported providers."""
     state['providers'] = get_thipster_module_class_list('auth')
     provider_display = ''
     for provider in state['providers']:
         provider_display += f'[green]{provider[:-3]}[/green]\n'
```

### Comparing `thipstercli-0.3.0/thipstercli/repository.py` & `thipstercli-0.3.1/thipstercli/repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.0/thipstercli.egg-info/PKG-INFO` & `thipstercli-0.3.1/thipstercli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.3.0 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.3.1 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.3.0/thipstercli.egg-info/SOURCES.txt` & `thipstercli-0.3.1/thipstercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

