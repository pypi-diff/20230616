# Comparing `tmp/logdir-0.9.2.tar.gz` & `tmp/logdir-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logdir-0.9.2.tar", last modified: Thu Jan 21 06:29:03 2021, max compression
+gzip compressed data, was "logdir-0.9.3.tar", max compression
```

## Comparing `logdir-0.9.2.tar` & `logdir-0.9.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1053 2021-01-21 06:28:32.357547 logdir-0.9.2/LICENSE
--rw-r--r--   0        0        0     3625 2021-01-21 06:28:32.357547 logdir-0.9.2/README.md
--rw-r--r--   0        0        0     9242 2021-01-21 06:28:32.357547 logdir-0.9.2/logdir/__init__.py
--rw-r--r--   0        0        0     1320 2021-01-21 06:28:32.357547 logdir-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     4382 2021-01-21 06:29:03.780722 logdir-0.9.2/setup.py
--rw-r--r--   0        0        0     4512 2021-01-21 06:29:03.781068 logdir-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1053 2021-02-25 06:47:21.561026 logdir-0.9.3/LICENSE
+-rw-r--r--   0        0        0     3703 2021-02-25 06:47:21.561026 logdir-0.9.3/README.md
+-rw-r--r--   0        0        0     9242 2021-02-25 06:47:21.561026 logdir-0.9.3/logdir/__init__.py
+-rw-r--r--   0        0        0     1320 2021-02-25 06:47:21.561026 logdir-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     4466 2021-02-25 06:47:56.273084 logdir-0.9.3/setup.py
+-rw-r--r--   0        0        0     4590 2021-02-25 06:47:56.273455 logdir-0.9.3/PKG-INFO
```

### Comparing `logdir-0.9.2/LICENSE` & `logdir-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `logdir-0.9.2/README.md` & `logdir-0.9.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
 To install from PyPI, run:
 
 ```bash
 pip install logdir
 ```
 
+To install from Conda, run:
+
+```bash
+conda install -c conda-forge logdir
+```
+
 To install from source, clone this repo, cd into it, and run:
 
 ```bash
 pip install .
 ```
 
 logdir is tested on Python 3.7+. Earlier Python versions may work but are not
```

### Comparing `logdir-0.9.2/logdir/__init__.py` & `logdir-0.9.3/logdir/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """A utility for managing logging directories."""
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 __all__ = [
     "LogDir",
 ]
 
 import datetime
 import json
```

### Comparing `logdir-0.9.2/pyproject.toml` & `logdir-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "logdir"
-version = "0.9.2"
+version = "0.9.3"
 description = "A utility for managing logging directories."
 authors = ["Bryon Tjanaka <bryon@btjanaka.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://logdir.btjanka.net"
 repository = "https://github.com/btjanaka/logdir"
 documentation = "https://logdir.btjanaka.net"
```

### Comparing `logdir-0.9.2/setup.py` & `logdir-0.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['dulwich>=0.20.0', 'ruamel.yaml>0.15', 'toml>=0.10']
 
 setup_kwargs = {
     'name': 'logdir',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'A utility for managing logging directories.',
-    'long_description': '# LogDir\n\nA utility for managing logging directories.\n\n|                    Source                    |                                                  PyPI                                                  |                                                                                             CI/CD                                                                                             |                        Docs                        |                                                                         Docs Status                                                                         |\n| :------------------------------------------: | :----------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------: |\n| [GitHub](https://github.com/btjanaka/logdir) | [![PyPI](https://img.shields.io/pypi/v/logdir?style=flat&color=blue)](https://pypi.org/project/logdir) | [![Test and Deploy](https://github.com/btjanaka/logdir/workflows/Test%20and%20Deploy/badge.svg?branch=master)](https://github.com/btjanaka/logdir/actions?query=workflow%3A"Test+and+Deploy") | [logdir.btjanaka.net](https://logdir.btjanaka.net) | [![Netlify Status](https://api.netlify.com/api/v1/badges/b3cdff86-dfcf-4b62-9a64-ab431bc5040f/deploy-status)](https://app.netlify.com/sites/logdir/deploys) |\n\n## Installation\n\nTo install from PyPI, run:\n\n```bash\npip install logdir\n```\n\nTo install from source, clone this repo, cd into it, and run:\n\n```bash\npip install .\n```\n\nlogdir is tested on Python 3.7+. Earlier Python versions may work but are not\nguaranteed.\n\n## Usage\n\nIf your experiment is called `My Experiment`, you can create a logging directory\nfor it with:\n\n```python\nfrom logdir import LogDir\n\nlogdir = LogDir("My Experiment")\n```\n\nThis will create a logging directory of the form\n`./logs/YYYY-MM-DD_HH-MM-SS_my-experiment-dir`; you can change `./logs` by\npassing in a second argument for the root directory when initializing `LogDir`,\ni.e. `LogDir("My Experiment", "./different-log-dir")`.\n\nYou now have access to useful methods for creating files and saving data in the\ndirectory. For example, start writing to a file `new.txt` in the directory with:\n\n```python\nwith logdir.pfile("new.txt").open() as file:\n    file.write("Hello World!")\n```\n\nThis takes advantage of the [pfile()](/api/#logdir.LogDir.pfile) method, which\ncreates a `pathlib.Path` to the new file. It also uses `pathlib.Path.open()`.\n\n`pfile()` will also create intermediate directories, so this will work even if\n`foo/bar/` does not exist in the logging directory already:\n\n```python\nwith logdir.pfile("foo/bar/new.txt").open() as file:\n    file.write("Hello World!")\n```\n\nThere is also [save_data()](/api/#logdir.LogDir.save_data), which saves data to\na file. JSON, YAML, TOML, and pickle files are currently supported.\n\n```python\nlogdir.save_data({"a": 1, "b": 2, "c": 3}, "file.json")\n```\n\nFinally, [readme()](/api/#logdir.LogDir.readme) adds a README.md to the\ndirectory with multiple pieces of information. For instance, this command:\n\n```python\nlogdir.readme(date=True, git_commit=True)\n```\n\nWill create something like:\n\n```md\n# My Experiment\n\n- Date: 2020-10-04 23:04:05\n- Git Commit: e3rftyt543rt5y67jhtgr4yhju\n```\n',
+    'long_description': '# LogDir\n\nA utility for managing logging directories.\n\n|                    Source                    |                                                  PyPI                                                  |                                                                                             CI/CD                                                                                             |                        Docs                        |                                                                         Docs Status                                                                         |\n| :------------------------------------------: | :----------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------: |\n| [GitHub](https://github.com/btjanaka/logdir) | [![PyPI](https://img.shields.io/pypi/v/logdir?style=flat&color=blue)](https://pypi.org/project/logdir) | [![Test and Deploy](https://github.com/btjanaka/logdir/workflows/Test%20and%20Deploy/badge.svg?branch=master)](https://github.com/btjanaka/logdir/actions?query=workflow%3A"Test+and+Deploy") | [logdir.btjanaka.net](https://logdir.btjanaka.net) | [![Netlify Status](https://api.netlify.com/api/v1/badges/b3cdff86-dfcf-4b62-9a64-ab431bc5040f/deploy-status)](https://app.netlify.com/sites/logdir/deploys) |\n\n## Installation\n\nTo install from PyPI, run:\n\n```bash\npip install logdir\n```\n\nTo install from Conda, run:\n\n```bash\nconda install -c conda-forge logdir\n```\n\nTo install from source, clone this repo, cd into it, and run:\n\n```bash\npip install .\n```\n\nlogdir is tested on Python 3.7+. Earlier Python versions may work but are not\nguaranteed.\n\n## Usage\n\nIf your experiment is called `My Experiment`, you can create a logging directory\nfor it with:\n\n```python\nfrom logdir import LogDir\n\nlogdir = LogDir("My Experiment")\n```\n\nThis will create a logging directory of the form\n`./logs/YYYY-MM-DD_HH-MM-SS_my-experiment-dir`; you can change `./logs` by\npassing in a second argument for the root directory when initializing `LogDir`,\ni.e. `LogDir("My Experiment", "./different-log-dir")`.\n\nYou now have access to useful methods for creating files and saving data in the\ndirectory. For example, start writing to a file `new.txt` in the directory with:\n\n```python\nwith logdir.pfile("new.txt").open() as file:\n    file.write("Hello World!")\n```\n\nThis takes advantage of the [pfile()](/api/#logdir.LogDir.pfile) method, which\ncreates a `pathlib.Path` to the new file. It also uses `pathlib.Path.open()`.\n\n`pfile()` will also create intermediate directories, so this will work even if\n`foo/bar/` does not exist in the logging directory already:\n\n```python\nwith logdir.pfile("foo/bar/new.txt").open() as file:\n    file.write("Hello World!")\n```\n\nThere is also [save_data()](/api/#logdir.LogDir.save_data), which saves data to\na file. JSON, YAML, TOML, and pickle files are currently supported.\n\n```python\nlogdir.save_data({"a": 1, "b": 2, "c": 3}, "file.json")\n```\n\nFinally, [readme()](/api/#logdir.LogDir.readme) adds a README.md to the\ndirectory with multiple pieces of information. For instance, this command:\n\n```python\nlogdir.readme(date=True, git_commit=True)\n```\n\nWill create something like:\n\n```md\n# My Experiment\n\n- Date: 2020-10-04 23:04:05\n- Git Commit: e3rftyt543rt5y67jhtgr4yhju\n```\n',
     'author': 'Bryon Tjanaka',
     'author_email': 'bryon@btjanaka.net',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://logdir.btjanka.net',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `logdir-0.9.2/PKG-INFO` & `logdir-0.9.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logdir
-Version: 0.9.2
+Version: 0.9.3
 Summary: A utility for managing logging directories.
 Home-page: https://logdir.btjanka.net
 License: MIT
 Keywords: log,logging,utilities
 Author: Bryon Tjanaka
 Author-email: bryon@btjanaka.net
 Requires-Python: >=3.7,<4.0
@@ -35,14 +35,20 @@
 
 To install from PyPI, run:
 
 ```bash
 pip install logdir
 ```
 
+To install from Conda, run:
+
+```bash
+conda install -c conda-forge logdir
+```
+
 To install from source, clone this repo, cd into it, and run:
 
 ```bash
 pip install .
 ```
 
 logdir is tested on Python 3.7+. Earlier Python versions may work but are not
```

