# Comparing `tmp/thipstercli-0.2.1.tar.gz` & `tmp/thipstercli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipstercli-0.2.1.tar", last modified: Thu Jun 15 13:09:05 2023, max compression
+gzip compressed data, was "thipstercli-0.2.2.tar", last modified: Fri Jun 16 08:16:57 2023, max compression
```

## Comparing `thipstercli-0.2.1.tar` & `thipstercli-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:09:05.759597 thipstercli-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-15 13:09:02.000000 thipstercli-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4982 2023-06-15 13:09:05.755597 thipstercli-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4294 2023-06-15 13:09:02.000000 thipstercli-0.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)      919 2023-06-15 13:09:02.000000 thipstercli-0.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 13:09:05.759597 thipstercli-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-15 13:09:03.000000 thipstercli-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:09:05.755597 thipstercli-0.2.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 13:09:02.000000 thipstercli-0.2.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1615 2023-06-15 13:09:02.000000 thipstercli-0.2.1/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-06-15 13:09:02.000000 thipstercli-0.2.1/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     2156 2023-06-15 13:09:02.000000 thipstercli-0.2.1/tests/test_providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:09:05.755597 thipstercli-0.2.1/thipstercli/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-15 13:09:02.000000 thipstercli-0.2.1/thipstercli/__init__.py
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-15 13:09:02.000000 thipstercli-0.2.1/thipstercli/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4848 2023-06-15 13:09:02.000000 thipstercli-0.2.1/thipstercli/cli.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-06-15 13:09:02.000000 thipstercli-0.2.1/thipstercli/config.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-06-15 13:09:02.000000 thipstercli-0.2.1/thipstercli/constants.py
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-15 13:09:02.000000 thipstercli-0.2.1/thipstercli/display.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-06-15 13:09:02.000000 thipstercli-0.2.1/thipstercli/helpers.py
--rw-r--r--   0 root         (0) root         (0)     2110 2023-06-15 13:09:02.000000 thipstercli-0.2.1/thipstercli/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:09:05.755597 thipstercli-0.2.1/thipstercli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4982 2023-06-15 13:09:05.000000 thipstercli-0.2.1/thipstercli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2023-06-15 13:09:05.000000 thipstercli-0.2.1/thipstercli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 13:09:05.000000 thipstercli-0.2.1/thipstercli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-15 13:09:05.000000 thipstercli-0.2.1/thipstercli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-15 13:09:05.000000 thipstercli-0.2.1/thipstercli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-15 13:09:05.000000 thipstercli-0.2.1/thipstercli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:16:57.647420 thipstercli-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-16 08:16:54.000000 thipstercli-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-16 08:16:57.643420 thipstercli-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-06-16 08:16:54.000000 thipstercli-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1350 2023-06-16 08:16:54.000000 thipstercli-0.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 08:16:57.647420 thipstercli-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-16 08:16:55.000000 thipstercli-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:16:57.643420 thipstercli-0.2.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 08:16:54.000000 thipstercli-0.2.2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-06-16 08:16:54.000000 thipstercli-0.2.2/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3844 2023-06-16 08:16:54.000000 thipstercli-0.2.2/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-06-16 08:16:54.000000 thipstercli-0.2.2/tests/test_providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:16:57.643420 thipstercli-0.2.2/thipstercli/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      108 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/config.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/display.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:16:57.643420 thipstercli-0.2.2/thipstercli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-16 08:16:57.000000 thipstercli-0.2.2/thipstercli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2023-06-16 08:16:57.000000 thipstercli-0.2.2/thipstercli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 08:16:57.000000 thipstercli-0.2.2/thipstercli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-16 08:16:57.000000 thipstercli-0.2.2/thipstercli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-16 08:16:57.000000 thipstercli-0.2.2/thipstercli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-16 08:16:57.000000 thipstercli-0.2.2/thipstercli.egg-info/top_level.txt
```

### Comparing `thipstercli-0.2.1/LICENSE` & `thipstercli-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thipstercli-0.2.1/PKG-INFO` & `thipstercli-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.2.1
+Version: 0.2.2
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
@@ -26,23 +26,26 @@
 
 Written entirely in Python, it leverages the Python CDK for Terraform to create Terraform files and apply them to the chosen provider.
 
 <p align="center">
   <a href="https://github.com/THipster/THipster-cli/blob/main/LICENSE" target="_blank" alt="License">
     <img src="https://img.shields.io/github/license/THipster/THipster-cli" alt="License">
   </a>
-  <a href="https://thipstercli.readthedocs.io/en/latest/?badge=latest" target="_blank" alt="Read the docs documentation">
-    <img src="https://readthedocs.org/projects/thipstercli/badge/?version=latest" alt="Read the docs documentation">
+  <a href="https://thipster-cli.readthedocs.io/en/latest/?badge=latest" target="_blank" alt="Read the docs documentation">
+    <img src="https://readthedocs.org/projects/thipster-cli/badge/?version=latest" alt="Read the docs documentation">
   </a>
   <a href="https://pypi.org/project/thipstercli/" target="_blank" alt="PyPi package">
     <img src="https://img.shields.io/pypi/v/thipstercli?color=brightgreen&label=pypi%20package" alt="Package version">
   </a>
   <a href="https://pypi.org/project/thipstercli/" target="_blank" alt="PyPi package">
     <img src="https://img.shields.io/pypi/pyversions/thipstercli?color=brightgreen" alt="Supported Python versions">
   </a>
+  <a href="https://github.com/astral-sh/ruff">
+    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff" style="max-width:100%;">
+  </a>
 </p>
 
 ## Technology Stack
 Written in Python 3.11, thipster-cli is build using [Typer](https://typer.tiangolo.com/).
 
 ## Project Status
 THipster-cli is currently in an active development state. If you want to know more, please check the [CHANGELOG](https://github.com/THipster/THipster-cli/blob/main/CHANGELOG.md) for more details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.2.1 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.2.2 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
@@ -11,15 +11,15 @@
 github.com/THipster/THipster), build with [Typer](https://typer.tiangolo.com/).
 THipster is a tool dedicated to simplifying the ordeal associated with writing
 Terraform files. It allows users to write infrastructure as code in a
 simplified format, using either YAML (with JINJA) or the dedicated Thipster
 DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
 create Terraform files and apply them to the chosen provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
-                                   versions]
+                               versions] [Ruff]
 ## Technology Stack Written in Python 3.11, thipster-cli is build using [Typer]
 (https://typer.tiangolo.com/). ## Project Status THipster-cli is currently in
 an active development state. If you want to know more, please check the
 [CHANGELOG](https://github.com/THipster/THipster-cli/blob/main/CHANGELOG.md)
 for more details. ## Dependencies To use the CLI, you will need to have all the
 required THipster dependencies installed on your machine. Please refer to the
 [THipster documentation](https://github.com/THipster/THipster#dependencies) for
```

### Comparing `thipstercli-0.2.1/README.md` & `thipstercli-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 
 Written entirely in Python, it leverages the Python CDK for Terraform to create Terraform files and apply them to the chosen provider.
 
 <p align="center">
   <a href="https://github.com/THipster/THipster-cli/blob/main/LICENSE" target="_blank" alt="License">
     <img src="https://img.shields.io/github/license/THipster/THipster-cli" alt="License">
   </a>
-  <a href="https://thipstercli.readthedocs.io/en/latest/?badge=latest" target="_blank" alt="Read the docs documentation">
-    <img src="https://readthedocs.org/projects/thipstercli/badge/?version=latest" alt="Read the docs documentation">
+  <a href="https://thipster-cli.readthedocs.io/en/latest/?badge=latest" target="_blank" alt="Read the docs documentation">
+    <img src="https://readthedocs.org/projects/thipster-cli/badge/?version=latest" alt="Read the docs documentation">
   </a>
   <a href="https://pypi.org/project/thipstercli/" target="_blank" alt="PyPi package">
     <img src="https://img.shields.io/pypi/v/thipstercli?color=brightgreen&label=pypi%20package" alt="Package version">
   </a>
   <a href="https://pypi.org/project/thipstercli/" target="_blank" alt="PyPi package">
     <img src="https://img.shields.io/pypi/pyversions/thipstercli?color=brightgreen" alt="Supported Python versions">
   </a>
+  <a href="https://github.com/astral-sh/ruff">
+    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff" style="max-width:100%;">
+  </a>
 </p>
 
 ## Technology Stack
 Written in Python 3.11, thipster-cli is build using [Typer](https://typer.tiangolo.com/).
 
 ## Project Status
 THipster-cli is currently in an active development state. If you want to know more, please check the [CHANGELOG](https://github.com/THipster/THipster-cli/blob/main/CHANGELOG.md) for more details.
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 THipster/THipster), build with [Typer](https://typer.tiangolo.com/). THipster
 is a tool dedicated to simplifying the ordeal associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Written entirely
 in Python, it leverages the Python CDK for Terraform to create Terraform files
 and apply them to the chosen provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
-                                   versions]
+                               versions] [Ruff]
 ## Technology Stack Written in Python 3.11, thipster-cli is build using [Typer]
 (https://typer.tiangolo.com/). ## Project Status THipster-cli is currently in
 an active development state. If you want to know more, please check the
 [CHANGELOG](https://github.com/THipster/THipster-cli/blob/main/CHANGELOG.md)
 for more details. ## Dependencies To use the CLI, you will need to have all the
 required THipster dependencies installed on your machine. Please refer to the
 [THipster documentation](https://github.com/THipster/THipster#dependencies) for
```

### Comparing `thipstercli-0.2.1/setup.py` & `thipstercli-0.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+"""Setup file for the THipster-cli package."""
 from pathlib import Path
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 
 def get_extra_requires() -> dict[str, list[str]]:
+    """Get the extra requirements from the requirements-*.txt files."""
     extras_require = {}
     for req_file in Path('.').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 
-with open('requirements.txt') as f:
+with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
-with open('README.md') as f:
+with Path('README.md').open() as f:
     long_description = f.read()
 
 setup(
     name='thipstercli',
     version=__version__,
     license='MIT',
     description='CLI interface build with typer, designed to use the thipster package',
```

### Comparing `thipstercli-0.2.1/tests/conftest.py` & `thipstercli-0.2.2/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,48 @@
-import os
+"""Pytest configuration file."""
 import json
-import pytest
 from pathlib import Path
+
+import pytest
 from typer import get_app_dir
+
 import thipstercli.constants as constants
 from thipstercli.config import init_parameters
 
 
 @pytest.fixture
 def init_app_state():
+    """Initialize the app state."""
     init_parameters()
     yield
 
 
 @pytest.fixture
 def config_path():
+    """Return the user config file path."""
     return Path(get_app_dir(constants.APP_NAME)) / constants.CONFIG_FILE_NAME
 
 
 @pytest.fixture
 def create_config_file(config_path):
-    if not os.path.exists(config_path):
+    """Create a user config file."""
+    if not config_path.exists():
         config_path.parent.mkdir(parents=True, exist_ok=True)
 
     yield config_path
 
-    if os.path.exists(config_path):
-        os.remove(config_path)
+    if config_path.exists():
+        Path(config_path).unlink()
 
 
 @pytest.fixture
 def config_file(
     create_config_file,
 ):
+    """Create a user config file with default values."""
     create_config_file.write_text("""{
         "app_name": "thipstercli",
         "auth_provider": "google",
         "input_dir": "test/input_directory",
         "local_models_repository_path": "models",
         "models_repository": "THipster/models",
         "models_repository_branch": "main",
@@ -48,24 +54,27 @@
     init_parameters()
 
     yield
 
 
 @pytest.fixture
 def empty_config_file(create_config_file):
+    """Create an empty user config file."""
     create_config_file.write_text("""{}""")
     init_parameters()
     yield
 
 
 @pytest.fixture
 def config_file_wrong_provider(create_config_file):
+    """Create a user config file with the auth provider set to 'notfound'."""
     create_config_file.write_text("""{"auth_provider": "notfound"}""")
     init_parameters()
     yield
 
 
 def get_config_file() -> dict[str, object]:
+    """Return the user config file as a dictionary."""
     return json.loads(
         (Path(get_app_dir(constants.APP_NAME)) / constants.CONFIG_FILE_NAME)
         .read_text(),
     )
```

### Comparing `thipstercli-0.2.1/tests/test_cli.py` & `thipstercli-0.2.2/tests/test_cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,111 +1,122 @@
+"""Test the cli.py module."""
 import os
 from importlib.metadata import version as get_version
+from pathlib import Path
 
+from typer import get_app_dir
 from typer.testing import CliRunner
-from thipstercli.config import state
+
 from thipstercli.cli import app
+from thipstercli.config import state
 
 AUTH_FILE_PATH = 'tests/credentials.json'
 
 runner = CliRunner(mix_stderr=False)
 
 
 def auth_test(func):
+    """Create a temporary credentials file for testing."""
     def wrapper(*args, **kwargs):
         delete_credentials = False
         if (
-            not os.path.exists(
-                os.path.join(
-                    os.getenv('HOME'),
-                    '.config/gcloud/application_default_credentials.json',
-                ),
+            not Path.exists(
+                Path(get_app_dir('gcloud')) /
+                'application_default_credentials.json',
             )
             and (
                 os.getenv('GOOGLE_APPLICATION_CREDENTIALS') is not None
                 or os.getenv('GOOGLE_APPLICATION_CREDENTIALS') != ''
             )
         ):
 
             delete_credentials = True
             if os.getenv('GOOGLE_APPLICATION_CREDENTIALS_CONTENT') is None:
-                raise Exception('No credentials available')
+                no_credentials = 'No credentials available'
+                raise Exception(no_credentials)
 
-            with open(AUTH_FILE_PATH, 'w') as auth_file:
+            with Path(AUTH_FILE_PATH).open('w') as auth_file:
                 auth_file.write(
                     os.environ['GOOGLE_APPLICATION_CREDENTIALS_CONTENT'],
                 )
             os.environ['GOOGLE_APPLICATION_CREDENTIALS'] = AUTH_FILE_PATH
 
         res = func(*args, **kwargs)
 
         if delete_credentials:
-            os.remove(AUTH_FILE_PATH)
+            Path(AUTH_FILE_PATH).unlink()
 
         return res
     return wrapper
 
 
 def test_version():
+    """Test the version command."""
     result = runner.invoke(app, ['version'])
     version = get_version('thipstercli')
     assert result.exit_code == 0
     assert 'THipster-cli' and version in result.output
 
 
 def test_version_thipster():
+    """Test the version command with thipster."""
     result = runner.invoke(app, ['version', '--thipster'])
     version = get_version('thipstercli')
     assert result.exit_code == 0
     assert 'THipster-cli' and version in result.output
     version = get_version('thipster')
     assert 'THipster' and version in result.output
 
 
 def test_run_wrong_local_repository():
+    """Test the run command with a wrong local repository path."""
     result = runner.invoke(
         app, ['run', 'tests/resources/bucket.thips', '--local', 'wrong_path'],
     )
     assert result.exit_code != 0
     assert 'Error : No such file or directory :' \
         in result.stderr
     assert 'wrong_path' in result.stderr
 
 
 def test_run_wrong_file_path():
+    """Test the run command with a wrong input file path."""
     result = runner.invoke(app, ['run', 'wrong_path'])
     assert result.exit_code != 0
     assert 'Error : Path not found :' in result.stderr
     assert 'wrong_path' in result.stderr
 
 
 @auth_test
 def test_run_bucket():
-
+    """Test the run command with a gcp bucket resource."""
     result = runner.invoke(
         app, [
             'run', 'tests/resources/bucket.thips',
             '-l', 'tests/resources/models',
         ],
     )
 
     assert result.exit_code == 0
     assert 'thipster_cli_test_bucket' in result.output
     assert 'Terraform will perform the following actions' in result.output
 
 
 def test_config_file_verbose(config_file):
+    """Test if the value of verbose is correctly set from the config file."""
     _ = config_file
     runner.invoke(app, ['--help'])
     assert state.get('verbose', False) is True
 
 
 def test_config_file_input_dir(config_file):
+    """Test if the value of input_dir is correctly set from the config file."""
     _ = config_file
     runner.invoke(app, ['--help'])
     assert state.get('input_dir', None) == 'test/input_directory'
 
 
 def test_config_file_output_dir(config_file):
+    """Test if the value of output_dir is correctly set from the config file."""
     _ = config_file
     runner.invoke(app, ['--help'])
     assert state.get('output_dir', None) == 'test/output_directory'
```

### Comparing `thipstercli-0.2.1/tests/test_providers.py` & `thipstercli-0.2.2/tests/test_providers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,87 @@
-from .conftest import get_config_file
+"""Test the providers.py module."""
 from typer.testing import CliRunner
+
 from thipstercli.config import state
 from thipstercli.helpers import get_auth_provider_class
 from thipstercli.providers import app, check_provider_exists
 
+from .conftest import get_config_file
+
 runner = CliRunner(mix_stderr=False)
 
 providers = [
     'google',
 ]
 
 
 def test_list_providers():
+    """Test the list command."""
     result = runner.invoke(app, ['list'])
     assert result.exit_code == 0
     for provider in providers:
         assert provider in result.stdout.lower()
 
 
 def test_info_provider():
+    """Test the info command for 'google'."""
     result = runner.invoke(app, ['info', 'google'])
     assert result.exit_code == 0
     assert 'google' in result.stdout.lower()
     assert 'gcloud' in result.stdout.lower()
 
 
 def test_info_provider_not_found():
+    """Test the info command for wrong provider 'notfound'."""
     result = runner.invoke(app, ['info', 'notfound'])
     assert result.exit_code == 1
     assert 'provider notfound not found.' in result.stdout.lower()
 
 
 def test_set_provider():
+    """Test the set command for 'google'."""
     result = runner.invoke(app, ['set', 'google'])
     assert result.exit_code == 0
     assert 'google' in result.stdout.lower()
     assert 'provider set to' in result.stdout.lower()
 
 
 def test_set_provider_not_found():
+    """Test the set command for wrong provider 'notfound'."""
     result = runner.invoke(app, ['set', 'notfound'])
     assert result.exit_code == 1
     assert 'provider notfound not found.' in result.stdout.lower()
 
 
 def test_display_provider(config_file):
+    """Test the display command for the 'google' provider set in the config file."""
     _ = config_file
     result = runner.invoke(app, ['display'])
     assert result.exit_code == 0
     assert 'provider set to' in result.stdout.lower()
     assert 'google' in result.stdout.lower()
 
 
 def test_get_provider_class():
+    """Test the get_auth_provider_class function."""
     provider = get_auth_provider_class('Google')
     assert provider.__name__ == 'GoogleAuth'
 
 
 def test_check_provider_exists():
+    """Test the check_provider_exists function."""
     provider = check_provider_exists('google')
     assert provider == 'google'
 
 
 def test_set_provider_config_file(config_file_wrong_provider):
+    """Test if the set command sets the provider in the config file."""
     _ = config_file_wrong_provider
     runner.invoke(app, ['set', 'google'])
     assert get_config_file().get('auth_provider', None) == 'google'
 
 
 def test_wrong_provider_config_file(config_file_wrong_provider):
+    """Test the behavior of the app when the config file has a wrong provider."""
     _ = config_file_wrong_provider
     runner.invoke(app, ['--help'])
     assert state.get('auth_provider', None) is None
```

### Comparing `thipstercli-0.2.1/thipstercli/cli.py` & `thipstercli-0.2.2/thipstercli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+"""THipster CLI."""
 import typer
-import thipstercli.constants as constants
 from rich import print
 from thipster import Engine as ThipsterEngine
 from thipster.auth import Google
+from thipster.engine.exceptions import THipsterException
 from thipster.parser import ParserFactory
 from thipster.repository import GithubRepo, LocalRepo
 from thipster.terraform import Terraform
-from thipster.engine.exceptions import THipsterException
 
+import thipstercli.constants as constants
 from thipstercli import providers
+from thipstercli.config import init_parameters, state
 from thipstercli.display import (
     error,
     print_if_verbose,
     print_package_version,
     print_start_if_verbose,
     print_success_if_verbose,
 )
-from thipstercli.config import init_parameters, state
 
 init_parameters()
 
 app = typer.Typer(
     name=state.get(
         'app_name', constants.APP_NAME,
     ), no_args_is_help=True,
@@ -32,32 +33,31 @@
 def _callback(
     verbose: bool = typer.Option(
         state.get('verbose', constants.VERBOSE),
         '--verbose', '-v',
         help='Prints more information about the execution of the THipster CLI',
     ),
 ):
-    """THipster CLI
+    """THipster CLI.
 
     THipster is a tool that allows you to generate Terraform code
-from a simple DSL or yaml file.
+    from a simple DSL or yaml file.
     """
     state['verbose'] = verbose
 
 
 @app.command('version')
 def _version(
     thipster: bool = typer.Option(
         False,
         '--thipster', '-t',
         help='Prints the version of the THipster tool',
     ),
 ):
-    """Prints the version of the THipster CLI
-    """
+    """Print the version of the THipster CLI."""
     print_package_version('thipstercli')
 
     if thipster:
         print_package_version('thipster')
 
 
 @app.command('run')
@@ -67,22 +67,14 @@
         help='Path to the file or directory to run',
     ),
     local: str = typer.Option(
         None,
         '--local', '-l',
         help='Runs the THipster Tool locally, importing models from the given path',
     ),
-    repository_provider: str = typer.Option(
-        state.get(
-            'models_repository_provider',
-            constants.MODELS_REPOSITORY_PROVIDER,
-        ),
-        '--repository-provider', '-rp',
-        help='Runs the THipster Tool using the given model repository provider',
-    ),
     repository: str = typer.Option(
         state.get('models_repository', constants.MODELS_REPOSITORY),
         '--repository-name', '-rn',
         help='Runs the THipster Tool using the given model repository',
     ),
     repository_branch: str = typer.Option(
         state.get(
@@ -99,16 +91,15 @@
     ),
     apply: bool = typer.Option(
         False,
         '--apply', '-a',
         help='Applies the generated Terraform code',
     ),
 ):
-    """Runs the THipster Tool on the given path
-    """
+    """Run the THipster Tool on the given path."""
     print_if_verbose(f'Running THipster on {path}')
 
     authentification_provider = providers.get_auth_provider_class(
         providers.check_provider_exists(provider),
     ) if provider else Google
 
     print_if_verbose(
```

### Comparing `thipstercli-0.2.1/thipstercli/config.py` & `thipstercli-0.2.2/thipstercli/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+"""Configuration module for the application."""
 import json
-from rich import print
 from pathlib import Path
+
+from rich import print
 from typer import get_app_dir
+
 import thipstercli.constants as constants
 from thipstercli.helpers import check_thipster_module_exists
 
 state = {}
 
 app_dir = get_app_dir(constants.APP_NAME)
 config_path: Path = Path(app_dir) / constants.CONFIG_FILE_NAME
 
 
 def init_parameters() -> None:
-    """Initializes the state
-    """
+    """Initialize the state of the application."""
     if not config_path.is_file():
         set_default_config()
         config_path.parent.mkdir(parents=True, exist_ok=True)
         config_path.write_text(json.dumps(state, sort_keys=True, indent=4))
         return
 
     state.update(json.loads(config_path.read_text()))
@@ -28,29 +30,27 @@
     if not check_thipster_module_exists('auth', state['auth_provider']):
         print(f':rotating_light: User set Auth Provider [red]{state["auth_provider"]}\
 [/red] not found')
         state.pop('auth_provider')
 
 
 def set_default_config() -> None:
-    """Sets the default configuration
-    """
+    """Set the default values for the user configuration file."""
     state['app_name'] = constants.APP_NAME
     state['verbose'] = constants.VERBOSE
     state['models_repository_provider'] = constants.MODELS_REPOSITORY_PROVIDER
     state['models_repository'] = constants.MODELS_REPOSITORY
     state['models_repository_branch'] = constants.MODELS_REPOSITORY_BRANCH
     state['local_models_repository_path'] = constants.LOCAL_MODELS_REPOSITORY_PATH
     state['input_dir'] = constants.INPUT_DIR
     state['output_dir'] = constants.OUTPUT_DIR
 
 
 def update_config_file(parameters: dict[str, object]) -> None:
-    """Updates the config file
-    """
+    """Update the config file with the given parameters."""
     if config_path.is_file():
         config_file: dict[str, object] = json.loads(config_path.read_text())
         config_file.update(parameters)
     else:
         config_path.parent.mkdir(parents=True, exist_ok=True)
         config_file = parameters
```

### Comparing `thipstercli-0.2.1/thipstercli/providers.py` & `thipstercli-0.2.2/thipstercli/providers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,67 @@
+"""Commands to manage the auth providers."""
 import typer
-from rich.panel import Panel
 from rich import print
+from rich.panel import Panel
+
 from thipstercli.config import state, update_config_file
 from thipstercli.helpers import (
+    check_thipster_module_exists,
     get_auth_provider_class,
     get_thipster_module_class_list,
-    check_thipster_module_exists,
 )
 
 app = typer.Typer(no_args_is_help=True)
 
 
 @app.command('list')
 def _list():
-    """List all the supported providers
-    """
+    """List all the supported providers."""
     state['providers'] = get_thipster_module_class_list('auth')
     provider_display = ''
     for provider in state['providers']:
         provider_display += f'[green]{provider[:-3]}[/green]\n'
     print(Panel(provider_display, title='Providers'))
     __more_info_provider()
 
 
 @app.command('info')
 def info(provider: str):
-    """Get information about a provider
-    """
+    """Get information about a provider."""
     provider = check_provider_exists(provider)
 
     provider_class = get_auth_provider_class(provider)
     print(Panel(provider_class.__doc__, title=provider))
 
 
 @app.command('set')
-def set(provider: str):
-    """Set the provider to use
-    """
+def set_auth_provider(provider: str):
+    """Set the provider to use for the auth."""
     provider = check_provider_exists(provider)
 
     update_config_file(
         {'auth_provider': provider},
     )
 
     print(f'Provider set to [green]{provider}[/green]')
     __more_info_provider()
 
 
 @app.command('display')
 def display():
-    """Display the current provider
-    """
+    """Display the current provider."""
     if not state.get('auth_provider', None):
         print('No provider set.\nPlease use [bold]thipster providers set <provider>\
 [/bold] to set a provider')
         return
     print(f"Provider set to [green]{state['auth_provider']}[/green]")
 
 
 def check_provider_exists(provider: str) -> str:
-    """Checks if the given provider exists in the providers list
-    """
+    """Check if the given provider exists in the providers list."""
     if not check_thipster_module_exists('auth', provider):
         print(f'Provider [red]{provider.capitalize()}[/red] not found. \
 Please use one of the following providers:')
         _list()
         raise typer.Exit(1)
 
     return provider
```

### Comparing `thipstercli-0.2.1/thipstercli.egg-info/PKG-INFO` & `thipstercli-0.2.2/thipstercli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.2.1
+Version: 0.2.2
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
@@ -26,23 +26,26 @@
 
 Written entirely in Python, it leverages the Python CDK for Terraform to create Terraform files and apply them to the chosen provider.
 
 <p align="center">
   <a href="https://github.com/THipster/THipster-cli/blob/main/LICENSE" target="_blank" alt="License">
     <img src="https://img.shields.io/github/license/THipster/THipster-cli" alt="License">
   </a>
-  <a href="https://thipstercli.readthedocs.io/en/latest/?badge=latest" target="_blank" alt="Read the docs documentation">
-    <img src="https://readthedocs.org/projects/thipstercli/badge/?version=latest" alt="Read the docs documentation">
+  <a href="https://thipster-cli.readthedocs.io/en/latest/?badge=latest" target="_blank" alt="Read the docs documentation">
+    <img src="https://readthedocs.org/projects/thipster-cli/badge/?version=latest" alt="Read the docs documentation">
   </a>
   <a href="https://pypi.org/project/thipstercli/" target="_blank" alt="PyPi package">
     <img src="https://img.shields.io/pypi/v/thipstercli?color=brightgreen&label=pypi%20package" alt="Package version">
   </a>
   <a href="https://pypi.org/project/thipstercli/" target="_blank" alt="PyPi package">
     <img src="https://img.shields.io/pypi/pyversions/thipstercli?color=brightgreen" alt="Supported Python versions">
   </a>
+  <a href="https://github.com/astral-sh/ruff">
+    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff" style="max-width:100%;">
+  </a>
 </p>
 
 ## Technology Stack
 Written in Python 3.11, thipster-cli is build using [Typer](https://typer.tiangolo.com/).
 
 ## Project Status
 THipster-cli is currently in an active development state. If you want to know more, please check the [CHANGELOG](https://github.com/THipster/THipster-cli/blob/main/CHANGELOG.md) for more details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.2.1 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.2.2 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
@@ -11,15 +11,15 @@
 github.com/THipster/THipster), build with [Typer](https://typer.tiangolo.com/).
 THipster is a tool dedicated to simplifying the ordeal associated with writing
 Terraform files. It allows users to write infrastructure as code in a
 simplified format, using either YAML (with JINJA) or the dedicated Thipster
 DSL. Written entirely in Python, it leverages the Python CDK for Terraform to
 create Terraform files and apply them to the chosen provider.
   [License] [Read_the_docs_documentation] [Package_version] [Supported_Python
-                                   versions]
+                               versions] [Ruff]
 ## Technology Stack Written in Python 3.11, thipster-cli is build using [Typer]
 (https://typer.tiangolo.com/). ## Project Status THipster-cli is currently in
 an active development state. If you want to know more, please check the
 [CHANGELOG](https://github.com/THipster/THipster-cli/blob/main/CHANGELOG.md)
 for more details. ## Dependencies To use the CLI, you will need to have all the
 required THipster dependencies installed on your machine. Please refer to the
 [THipster documentation](https://github.com/THipster/THipster#dependencies) for
```

### Comparing `thipstercli-0.2.1/thipstercli.egg-info/SOURCES.txt` & `thipstercli-0.2.2/thipstercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

