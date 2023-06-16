# Comparing `tmp/thipstercli-0.2.2.tar.gz` & `tmp/thipstercli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipstercli-0.2.2.tar", last modified: Fri Jun 16 08:16:57 2023, max compression
+gzip compressed data, was "thipstercli-0.3.0.tar", last modified: Fri Jun 16 09:38:10 2023, max compression
```

## Comparing `thipstercli-0.2.2.tar` & `thipstercli-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:16:57.647420 thipstercli-0.2.2/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-16 08:16:54.000000 thipstercli-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-16 08:16:57.643420 thipstercli-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4516 2023-06-16 08:16:54.000000 thipstercli-0.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1350 2023-06-16 08:16:54.000000 thipstercli-0.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 08:16:57.647420 thipstercli-0.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1818 2023-06-16 08:16:55.000000 thipstercli-0.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:16:57.643420 thipstercli-0.2.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 08:16:54.000000 thipstercli-0.2.2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1981 2023-06-16 08:16:54.000000 thipstercli-0.2.2/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3844 2023-06-16 08:16:54.000000 thipstercli-0.2.2/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     2786 2023-06-16 08:16:54.000000 thipstercli-0.2.2/tests/test_providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:16:57.643420 thipstercli-0.2.2/thipstercli/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      108 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/cli.py
--rw-r--r--   0 root         (0) root         (0)     2017 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/config.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/constants.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/display.py
--rw-r--r--   0 root         (0) root         (0)     2665 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/helpers.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-06-16 08:16:54.000000 thipstercli-0.2.2/thipstercli/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:16:57.643420 thipstercli-0.2.2/thipstercli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-16 08:16:57.000000 thipstercli-0.2.2/thipstercli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2023-06-16 08:16:57.000000 thipstercli-0.2.2/thipstercli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 08:16:57.000000 thipstercli-0.2.2/thipstercli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-16 08:16:57.000000 thipstercli-0.2.2/thipstercli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-16 08:16:57.000000 thipstercli-0.2.2/thipstercli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-16 08:16:57.000000 thipstercli-0.2.2/thipstercli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:38:10.049243 thipstercli-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-16 09:38:06.000000 thipstercli-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-16 09:38:10.049243 thipstercli-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-06-16 09:38:06.000000 thipstercli-0.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-06-16 09:38:06.000000 thipstercli-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 09:38:10.049243 thipstercli-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-06-16 09:38:07.000000 thipstercli-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:38:10.045243 thipstercli-0.3.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 09:38:06.000000 thipstercli-0.3.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-16 09:38:06.000000 thipstercli-0.3.0/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-06-16 09:38:06.000000 thipstercli-0.3.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-06-16 09:38:06.000000 thipstercli-0.3.0/tests/test_providers.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-06-16 09:38:06.000000 thipstercli-0.3.0/tests/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:38:10.045243 thipstercli-0.3.0/thipstercli/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6116 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/config.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/display.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/providers.py
+-rw-r--r--   0 root         (0) root         (0)     3438 2023-06-16 09:38:06.000000 thipstercli-0.3.0/thipstercli/repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:38:10.049243 thipstercli-0.3.0/thipstercli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-16 09:38:10.000000 thipstercli-0.3.0/thipstercli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      567 2023-06-16 09:38:10.000000 thipstercli-0.3.0/thipstercli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 09:38:10.000000 thipstercli-0.3.0/thipstercli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-16 09:38:10.000000 thipstercli-0.3.0/thipstercli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-16 09:38:10.000000 thipstercli-0.3.0/thipstercli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-16 09:38:10.000000 thipstercli-0.3.0/thipstercli.egg-info/top_level.txt
```

### Comparing `thipstercli-0.2.2/LICENSE` & `thipstercli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thipstercli-0.2.2/PKG-INFO` & `thipstercli-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.2.2
+Version: 0.3.0
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
-Metadata-Version: 2.1 Name: thipstercli Version: 0.2.2 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.3.0 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.2.2/README.md` & `thipstercli-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `thipstercli-0.2.2/pyproject.toml` & `thipstercli-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     "C4",
     "EM",
     "EXE",
     "ISC",
     "ICN",
     "INP",
     "PYI",
+    "PTH",
     "Q",
     "RSE",
     "RET",
     "SIM",
     "TID",
     "ARG",
     "RUF",
```

### Comparing `thipstercli-0.2.2/setup.py` & `thipstercli-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('.').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.2.2'
+__version__ = '0.3.0'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as f:
     long_description = f.read()
 
@@ -54,11 +54,11 @@
     install_requires=required,
     packages=find_packages(
         exclude=['ci'],
     ),
     extras_require=get_extra_requires(),
     entry_points={
         'console_scripts': [
-            'thipster = thipstercli.cli:app',
+            'thipster = thipstercli.cli:main_app',
         ],
     },
 )
```

### Comparing `thipstercli-0.2.2/tests/conftest.py` & `thipstercli-0.3.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,21 +60,13 @@
 def empty_config_file(create_config_file):
     """Create an empty user config file."""
     create_config_file.write_text("""{}""")
     init_parameters()
     yield
 
 
-@pytest.fixture
-def config_file_wrong_provider(create_config_file):
-    """Create a user config file with the auth provider set to 'notfound'."""
-    create_config_file.write_text("""{"auth_provider": "notfound"}""")
-    init_parameters()
-    yield
-
-
 def get_config_file() -> dict[str, object]:
     """Return the user config file as a dictionary."""
     return json.loads(
         (Path(get_app_dir(constants.APP_NAME)) / constants.CONFIG_FILE_NAME)
         .read_text(),
     )
```

### Comparing `thipstercli-0.2.2/tests/test_cli.py` & `thipstercli-0.3.0/tests/test_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from importlib.metadata import version as get_version
 from pathlib import Path
 
 from typer import get_app_dir
 from typer.testing import CliRunner
 
-from thipstercli.cli import app
+from thipstercli.cli import main_app
 from thipstercli.config import state
 
 AUTH_FILE_PATH = 'tests/credentials.json'
 
 runner = CliRunner(mix_stderr=False)
 
 
@@ -47,76 +47,74 @@
 
         return res
     return wrapper
 
 
 def test_version():
     """Test the version command."""
-    result = runner.invoke(app, ['version'])
+    result = runner.invoke(main_app, ['version'])
     version = get_version('thipstercli')
     assert result.exit_code == 0
     assert 'THipster-cli' and version in result.output
 
 
 def test_version_thipster():
     """Test the version command with thipster."""
-    result = runner.invoke(app, ['version', '--thipster'])
+    result = runner.invoke(main_app, ['version', '--thipster'])
     version = get_version('thipstercli')
     assert result.exit_code == 0
     assert 'THipster-cli' and version in result.output
     version = get_version('thipster')
     assert 'THipster' and version in result.output
 
 
 def test_run_wrong_local_repository():
     """Test the run command with a wrong local repository path."""
     result = runner.invoke(
-        app, ['run', 'tests/resources/bucket.thips', '--local', 'wrong_path'],
+        main_app, ['run', 'tests/resources/bucket.thips', '-rl', 'wrong_path'],
     )
     assert result.exit_code != 0
-    assert 'Error : No such file or directory :' \
-        in result.stderr
-    assert 'wrong_path' in result.stderr
+    assert "Couldn't find wrong_path local repository" in result.stderr
 
 
 def test_run_wrong_file_path():
-    """Test the run command with a wrong input file path."""
-    result = runner.invoke(app, ['run', 'wrong_path'])
+    """Test the run command with a wrong local repository path."""
+    result = runner.invoke(main_app, ['run', 'wrong_path'])
     assert result.exit_code != 0
     assert 'Error : Path not found :' in result.stderr
     assert 'wrong_path' in result.stderr
 
 
 @auth_test
 def test_run_bucket():
     """Test the run command with a gcp bucket resource."""
     result = runner.invoke(
-        app, [
+        main_app, [
             'run', 'tests/resources/bucket.thips',
-            '-l', 'tests/resources/models',
+            '-rl', 'tests/resources/models',
         ],
     )
 
     assert result.exit_code == 0
     assert 'thipster_cli_test_bucket' in result.output
     assert 'Terraform will perform the following actions' in result.output
 
 
 def test_config_file_verbose(config_file):
     """Test if the value of verbose is correctly set from the config file."""
     _ = config_file
-    runner.invoke(app, ['--help'])
+    runner.invoke(main_app, ['--help'])
     assert state.get('verbose', False) is True
 
 
 def test_config_file_input_dir(config_file):
     """Test if the value of input_dir is correctly set from the config file."""
     _ = config_file
-    runner.invoke(app, ['--help'])
+    runner.invoke(main_app, ['--help'])
     assert state.get('input_dir', None) == 'test/input_directory'
 
 
 def test_config_file_output_dir(config_file):
     """Test if the value of output_dir is correctly set from the config file."""
     _ = config_file
-    runner.invoke(app, ['--help'])
+    runner.invoke(main_app, ['--help'])
     assert state.get('output_dir', None) == 'test/output_directory'
```

### Comparing `thipstercli-0.2.2/tests/test_providers.py` & `thipstercli-0.3.0/tests/test_providers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,74 @@
 """Test the providers.py module."""
+import pytest
 from typer.testing import CliRunner
 
-from thipstercli.config import state
+from thipstercli.config import init_parameters, state
 from thipstercli.helpers import get_auth_provider_class
-from thipstercli.providers import app, check_provider_exists
+from thipstercli.providers import check_provider_exists, provider_app
 
 from .conftest import get_config_file
 
 runner = CliRunner(mix_stderr=False)
 
 providers = [
     'google',
 ]
 
 
+@pytest.fixture
+def config_file_wrong_provider(create_config_file):
+    """Create a user config file with the auth provider set to 'notfound'."""
+    create_config_file.write_text("""{"auth_provider": "notfound"}""")
+    init_parameters()
+    yield
+
+
 def test_list_providers():
     """Test the list command."""
-    result = runner.invoke(app, ['list'])
+    result = runner.invoke(provider_app, ['list'])
     assert result.exit_code == 0
     for provider in providers:
         assert provider in result.stdout.lower()
 
 
 def test_info_provider():
     """Test the info command for 'google'."""
-    result = runner.invoke(app, ['info', 'google'])
+    result = runner.invoke(provider_app, ['info', 'google'])
     assert result.exit_code == 0
     assert 'google' in result.stdout.lower()
     assert 'gcloud' in result.stdout.lower()
 
 
 def test_info_provider_not_found():
     """Test the info command for wrong provider 'notfound'."""
-    result = runner.invoke(app, ['info', 'notfound'])
+    result = runner.invoke(provider_app, ['info', 'notfound'])
     assert result.exit_code == 1
     assert 'provider notfound not found.' in result.stdout.lower()
 
 
 def test_set_provider():
     """Test the set command for 'google'."""
-    result = runner.invoke(app, ['set', 'google'])
+    result = runner.invoke(provider_app, ['set', 'google'])
     assert result.exit_code == 0
     assert 'google' in result.stdout.lower()
     assert 'provider set to' in result.stdout.lower()
 
 
 def test_set_provider_not_found():
     """Test the set command for wrong provider 'notfound'."""
-    result = runner.invoke(app, ['set', 'notfound'])
+    result = runner.invoke(provider_app, ['set', 'notfound'])
     assert result.exit_code == 1
     assert 'provider notfound not found.' in result.stdout.lower()
 
 
 def test_display_provider(config_file):
     """Test the display command for the 'google' provider set in the config file."""
     _ = config_file
-    result = runner.invoke(app, ['display'])
+    result = runner.invoke(provider_app, ['display'])
     assert result.exit_code == 0
     assert 'provider set to' in result.stdout.lower()
     assert 'google' in result.stdout.lower()
 
 
 def test_get_provider_class():
     """Test the get_auth_provider_class function."""
@@ -72,16 +81,16 @@
     provider = check_provider_exists('google')
     assert provider == 'google'
 
 
 def test_set_provider_config_file(config_file_wrong_provider):
     """Test if the set command sets the provider in the config file."""
     _ = config_file_wrong_provider
-    runner.invoke(app, ['set', 'google'])
-    assert get_config_file().get('auth_provider', None) == 'google'
+    runner.invoke(provider_app, ['set', 'google'])
+    assert get_config_file().get('auth_provider') == 'google'
 
 
 def test_wrong_provider_config_file(config_file_wrong_provider):
     """Test the behavior of the app when the config file has a wrong provider."""
     _ = config_file_wrong_provider
-    runner.invoke(app, ['--help'])
-    assert state.get('auth_provider', None) is None
+    runner.invoke(provider_app, ['--help'])
+    assert state.get('auth_provider') is None
```

### Comparing `thipstercli-0.2.2/thipstercli/config.py` & `thipstercli-0.3.0/thipstercli/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 """Configuration module for the application."""
 import json
 from pathlib import Path
 
 from rich import print
 from typer import get_app_dir
 
-import thipstercli.constants as constants
-from thipstercli.helpers import check_thipster_module_exists
+from . import constants
+from .helpers import check_thipster_module_exists
 
 state = {}
 
 app_dir = get_app_dir(constants.APP_NAME)
-config_path: Path = Path(app_dir) / constants.CONFIG_FILE_NAME
+config_file: Path = Path(app_dir) / constants.CONFIG_FILE_NAME
 
 
 def init_parameters() -> None:
     """Initialize the state of the application."""
-    if not config_path.is_file():
+    if not config_file.is_file():
         set_default_config()
-        config_path.parent.mkdir(parents=True, exist_ok=True)
-        config_path.write_text(json.dumps(state, sort_keys=True, indent=4))
+        config_file.parent.mkdir(parents=True, exist_ok=True)
+        config_file.write_text(json.dumps(state, sort_keys=True, indent=4))
         return
 
-    state.update(json.loads(config_path.read_text()))
+    state.update(json.loads(config_file.read_text()))
 
     if not state.get('auth_provider'):
         return
 
     if not check_thipster_module_exists('auth', state['auth_provider']):
         print(f':rotating_light: User set Auth Provider [red]{state["auth_provider"]}\
 [/red] not found')
         state.pop('auth_provider')
 
 
 def set_default_config() -> None:
     """Set the default values for the user configuration file."""
     state['app_name'] = constants.APP_NAME
     state['verbose'] = constants.VERBOSE
-    state['models_repository_provider'] = constants.MODELS_REPOSITORY_PROVIDER
+    state['repository_recovery_mode'] = constants.REPOSITORY_RECOVERY_MODE
     state['models_repository'] = constants.MODELS_REPOSITORY
     state['models_repository_branch'] = constants.MODELS_REPOSITORY_BRANCH
-    state['local_models_repository_path'] = constants.LOCAL_MODELS_REPOSITORY_PATH
     state['input_dir'] = constants.INPUT_DIR
     state['output_dir'] = constants.OUTPUT_DIR
 
 
 def update_config_file(parameters: dict[str, object]) -> None:
     """Update the config file with the given parameters."""
-    if config_path.is_file():
-        config_file: dict[str, object] = json.loads(config_path.read_text())
-        config_file.update(parameters)
+    if config_file.is_file():
+        config: dict[str, object] = json.loads(config_file.read_text())
+        config.update(parameters)
     else:
-        config_path.parent.mkdir(parents=True, exist_ok=True)
-        config_file = parameters
+        config_file.parent.mkdir(parents=True, exist_ok=True)
+        config = parameters
 
-    config_path.write_text(json.dumps(config_file, sort_keys=True, indent=4))
+    config_file.write_text(json.dumps(config, sort_keys=True, indent=4))
```

### Comparing `thipstercli-0.2.2/thipstercli/display.py` & `thipstercli-0.3.0/thipstercli/display.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 def error(*args, **kwargs):
     """Print an error message and exit the program."""
     print('[bold][red]Error :[/red][/bold]', *args, file=sys.stderr, **kwargs)
     sys.stderr.flush()
     raise typer.Exit(1)
 
 
+def warn(*args, **kwargs):
+    """Print a warning message."""
+    print(
+        '[bold][yellow]Warning :[/yellow][/bold]',
+        *args, file=sys.stdout, **kwargs,
+    )
+    sys.stdin.flush()
+
+
 def print_if_verbose(text: str):
     """Print the given text if the verbose flag is set."""
     print(text) if state.get('verbose', False) else None
 
 
 def print_start_if_verbose(text: str):
     """Print ' :arrow_forward: {text}... ' if the verbose flag is set."""
```

### Comparing `thipstercli-0.2.2/thipstercli/helpers.py` & `thipstercli-0.3.0/thipstercli/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Functions to get thipster classes and modules."""
 import importlib
 import os
+from pathlib import Path
 
 
 def get_thipster_class(
     parent_module_name: str,
     module_name: str,
     class_name_extension: str,
 ) -> type:
@@ -73,15 +74,15 @@
     list[str]
         The list of classes contained in the module.
     """
     module = importlib.import_module(
         f'thipster.{module_name.lower()}',
     )
     module_class_list = []
-    with os.scandir(os.path.dirname(module.__file__)) as entries:
+    with os.scandir(Path(module.__file__).parent) as entries:
         for entry in entries:
             if entry.is_file() and entry.name.endswith('.py') and not \
                     entry.name.startswith('__'):
                 module_class = entry.name.capitalize() if entry.name.islower() else \
                     entry.name
                 module_class_list.append(module_class)
     return module_class_list
```

### Comparing `thipstercli-0.2.2/thipstercli/providers.py` & `thipstercli-0.3.0/thipstercli/providers.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,51 +6,51 @@
 from thipstercli.config import state, update_config_file
 from thipstercli.helpers import (
     check_thipster_module_exists,
     get_auth_provider_class,
     get_thipster_module_class_list,
 )
 
-app = typer.Typer(no_args_is_help=True)
+provider_app = typer.Typer(no_args_is_help=True)
 
 
-@app.command('list')
+@provider_app.command('list')
 def _list():
     """List all the supported providers."""
     state['providers'] = get_thipster_module_class_list('auth')
     provider_display = ''
     for provider in state['providers']:
         provider_display += f'[green]{provider[:-3]}[/green]\n'
     print(Panel(provider_display, title='Providers'))
     __more_info_provider()
 
 
-@app.command('info')
+@provider_app.command('info')
 def info(provider: str):
     """Get information about a provider."""
     provider = check_provider_exists(provider)
 
     provider_class = get_auth_provider_class(provider)
     print(Panel(provider_class.__doc__, title=provider))
 
 
-@app.command('set')
+@provider_app.command('set')
 def set_auth_provider(provider: str):
     """Set the provider to use for the auth."""
     provider = check_provider_exists(provider)
 
     update_config_file(
         {'auth_provider': provider},
     )
 
     print(f'Provider set to [green]{provider}[/green]')
     __more_info_provider()
 
 
-@app.command('display')
+@provider_app.command('display')
 def display():
     """Display the current provider."""
     if not state.get('auth_provider', None):
         print('No provider set.\nPlease use [bold]thipster providers set <provider>\
 [/bold] to set a provider')
         return
     print(f"Provider set to [green]{state['auth_provider']}[/green]")
@@ -71,8 +71,8 @@
     print(
         Panel('For more information about a provider, run: thipster providers info \
 <provider>'),
     ) if state.get('verbose') else None
 
 
 if __name__ == '__main__':
-    app()
+    provider_app()
```

### Comparing `thipstercli-0.2.2/thipstercli.egg-info/PKG-INFO` & `thipstercli-0.3.0/thipstercli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.2.2
+Version: 0.3.0
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
-Metadata-Version: 2.1 Name: thipstercli Version: 0.2.2 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.3.0 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.2.2/thipstercli.egg-info/SOURCES.txt` & `thipstercli-0.3.0/thipstercli.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 README.md
 pyproject.toml
 setup.py
 tests/__init__.py
 tests/conftest.py
 tests/test_cli.py
 tests/test_providers.py
+tests/test_repository.py
 thipstercli/__init__.py
 thipstercli/__main__.py
 thipstercli/cli.py
 thipstercli/config.py
 thipstercli/constants.py
 thipstercli/display.py
 thipstercli/helpers.py
 thipstercli/providers.py
+thipstercli/repository.py
 thipstercli.egg-info/PKG-INFO
 thipstercli.egg-info/SOURCES.txt
 thipstercli.egg-info/dependency_links.txt
 thipstercli.egg-info/entry_points.txt
 thipstercli.egg-info/requires.txt
 thipstercli.egg-info/top_level.txt
```

