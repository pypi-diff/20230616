# Comparing `tmp/kasa_crypt-0.0.0.tar.gz` & `tmp/kasa_crypt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kasa_crypt-0.0.0.tar", max compression
+gzip compressed data, was "kasa_crypt-0.1.0.tar", max compression
```

## Comparing `kasa_crypt-0.0.0.tar` & `kasa_crypt-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11345 2023-06-16 00:45:41.195356 kasa_crypt-0.0.0/LICENSE
--rw-r--r--   0        0        0     3261 2023-06-16 00:45:41.190281 kasa_crypt-0.0.0/README.md
--rw-r--r--   0        0        0     1177 2023-06-16 01:49:16.324980 kasa_crypt-0.0.0/build_ext.py
--rw-r--r--   0        0        0     1986 2023-06-16 01:00:13.874191 kasa_crypt-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      463 2023-06-16 02:56:51.551865 kasa_crypt-0.0.0/src/kasa_crypt/__init__.py
--rw-r--r--   0        0        0   126395 2023-06-16 02:56:26.669381 kasa_crypt-0.0.0/src/kasa_crypt/_crypt_impl.c
--rw-r--r--   0        0        0      876 2023-06-16 02:55:33.491675 kasa_crypt-0.0.0/src/kasa_crypt/_crypt_impl.pyx
--rw-r--r--   0        0        0      723 2023-06-16 02:55:33.491897 kasa_crypt-0.0.0/src/kasa_crypt/crypt_wrapper.h
--rw-r--r--   0        0        0        0 2023-06-16 00:45:41.216068 kasa_crypt-0.0.0/src/kasa_crypt/py.typed
--rw-r--r--   0        0        0      584 2023-06-16 01:50:16.315066 kasa_crypt-0.0.0/src/kasa_crypt/python_impl.py
--rw-r--r--   0        0        0     3970 1970-01-01 00:00:00.000000 kasa_crypt-0.0.0/setup.py
--rw-r--r--   0        0        0     4347 1970-01-01 00:00:00.000000 kasa_crypt-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-06-16 03:35:26.032303 kasa_crypt-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3455 2023-06-16 03:35:26.032303 kasa_crypt-0.1.0/README.md
+-rw-r--r--   0        0        0     1183 2023-06-16 03:35:26.032303 kasa_crypt-0.1.0/build_ext.py
+-rw-r--r--   0        0        0     2046 2023-06-16 03:35:26.980307 kasa_crypt-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      463 2023-06-16 03:35:26.936307 kasa_crypt-0.1.0/src/kasa_crypt/__init__.py
+-rw-r--r--   0        0        0      876 2023-06-16 03:35:26.036303 kasa_crypt-0.1.0/src/kasa_crypt/_crypt_impl.pyx
+-rw-r--r--   0        0        0      723 2023-06-16 03:35:26.036303 kasa_crypt-0.1.0/src/kasa_crypt/crypt_wrapper.h
+-rw-r--r--   0        0        0        0 2023-06-16 03:35:26.036303 kasa_crypt-0.1.0/src/kasa_crypt/py.typed
+-rw-r--r--   0        0        0      584 2023-06-16 03:35:26.036303 kasa_crypt-0.1.0/src/kasa_crypt/python_impl.py
+-rw-r--r--   0        0        0     4176 1970-01-01 00:00:00.000000 kasa_crypt-0.1.0/setup.py
+-rw-r--r--   0        0        0     4541 1970-01-01 00:00:00.000000 kasa_crypt-0.1.0/PKG-INFO
```

### Comparing `kasa_crypt-0.0.0/LICENSE` & `kasa_crypt-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kasa_crypt-0.0.0/README.md` & `kasa_crypt-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,24 @@
 
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install kasa-crypt`
 
+## Example usage
+
+```python
+from kasa_crypt import encrypt, decrypt
+
+encrypted = encrypt('{"hello":"world"}')
+decrypted = decrypt(encrypted[4:])  # Always a 4 byte header
+print (decrypted)
+```
+
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- markdownlint-disable -->
```

#### html2text {}

```diff
@@ -1,12 +1,15 @@
 # kasa-crypt
                     [CI_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 Fast kasa crypt ## Installation Install this via pip (or your favourite package
-manager): `pip install kasa-crypt` ## Contributors â¨ Thanks goes to these
-wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-This project follows the [all-contributors](https://github.com/all-
-contributors/all-contributors) specification. Contributions of any kind
-welcome! ## Credits This package was created with [Copier](https://
-copier.readthedocs.io/) and the [browniebroke/pypackage-template](https://
-github.com/browniebroke/pypackage-template) project template.
+manager): `pip install kasa-crypt` ## Example usage ```python from kasa_crypt
+import encrypt, decrypt encrypted = encrypt('{"hello":"world"}') decrypted =
+decrypt(encrypted[4:]) # Always a 4 byte header print (decrypted) ``` ##
+Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
+allcontributors.org/docs/en/emoji-key)):       This project follows the [all-
+contributors](https://github.com/all-contributors/all-contributors)
+specification. Contributions of any kind welcome! ## Credits This package was
+created with [Copier](https://copier.readthedocs.io/) and the [browniebroke/
+pypackage-template](https://github.com/browniebroke/pypackage-template) project
+template.
```

### Comparing `kasa_crypt-0.0.0/build_ext.py` & `kasa_crypt-0.1.0/build_ext.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Build optional cython modules."""
 
 import contextlib
 import os
 from distutils.command.build_ext import build_ext
 from os.path import join
-from typing import Any
+from typing import Any, Dict
 
 try:
     from setuptools import Extension
 except ImportError:
     from distutils.core import Extension
 
 kasa_crypt_module = Extension(
@@ -22,15 +22,15 @@
 
 class BuildExt(build_ext):
     def build_extensions(self) -> None:
         with contextlib.suppress(Exception):
             super().build_extensions()
 
 
-def build(setup_kwargs: dict[Any, Any]) -> None:
+def build(setup_kwargs: Dict[Any, Any]) -> None:
     if os.environ.get("SKIP_CYTHON", False):
         return
     try:
         from Cython.Build import cythonize
 
         setup_kwargs.update(
             dict(
```

### Comparing `kasa_crypt-0.0.0/pyproject.toml` & `kasa_crypt-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kasa-crypt"
-version = "0.0.0"
+version = "0.1.0"
 description = "Fast kasa crypt"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/kasa-crypt"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -28,14 +28,18 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
 
+
+[tool.poetry.group.test.dependencies]
+cython = "^0.29.35"
+
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/kasa_crypt/__init__.py:__version__"
 build_command = "pip install poetry && poetry build"
 
 [tool.pytest.ini_options]
```

### Comparing `kasa_crypt-0.0.0/src/kasa_crypt/_crypt_impl.pyx` & `kasa_crypt-0.1.0/src/kasa_crypt/_crypt_impl.pyx`

 * *Files identical despite different names*

### Comparing `kasa_crypt-0.0.0/src/kasa_crypt/crypt_wrapper.h` & `kasa_crypt-0.1.0/src/kasa_crypt/crypt_wrapper.h`

 * *Files identical despite different names*

### Comparing `kasa_crypt-0.0.0/src/kasa_crypt/python_impl.py` & `kasa_crypt-0.1.0/src/kasa_crypt/python_impl.py`

 * *Files identical despite different names*

### Comparing `kasa_crypt-0.0.0/setup.py` & `kasa_crypt-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 ['kasa_crypt']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'kasa-crypt',
-    'version': '0.0.0',
+    'version': '0.1.0',
     'description': 'Fast kasa crypt',
-    'long_description': '# kasa-crypt\n\n<p align="center">\n  <a href="https://github.com/bdraco/kasa-crypt/actions/workflows/ci.yml?query=branch%3Amain">\n    <img src="https://img.shields.io/github/actions/workflow/status/bdraco/kasa-crypt/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://codecov.io/gh/bdraco/kasa-crypt">\n    <img src="https://img.shields.io/codecov/c/github/bdraco/kasa-crypt.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/kasa-crypt/">\n    <img src="https://img.shields.io/pypi/v/kasa-crypt.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/kasa-crypt.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/kasa-crypt.svg?style=flat-square" alt="License">\n</p>\n\nFast kasa crypt\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install kasa-crypt`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)\nproject template.\n',
+    'long_description': '# kasa-crypt\n\n<p align="center">\n  <a href="https://github.com/bdraco/kasa-crypt/actions/workflows/ci.yml?query=branch%3Amain">\n    <img src="https://img.shields.io/github/actions/workflow/status/bdraco/kasa-crypt/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://codecov.io/gh/bdraco/kasa-crypt">\n    <img src="https://img.shields.io/codecov/c/github/bdraco/kasa-crypt.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/kasa-crypt/">\n    <img src="https://img.shields.io/pypi/v/kasa-crypt.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/kasa-crypt.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/kasa-crypt.svg?style=flat-square" alt="License">\n</p>\n\nFast kasa crypt\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install kasa-crypt`\n\n## Example usage\n\n```python\nfrom kasa_crypt import encrypt, decrypt\n\nencrypted = encrypt(\'{"hello":"world"}\')\ndecrypted = decrypt(encrypted[4:])  # Always a 4 byte header\nprint (decrypted)\n```\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'nick@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bdraco/kasa-crypt',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,22 +1,25 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['kasa_crypt'] package_data = \ {'': ['*']} setup_kwargs =
-{ 'name': 'kasa-crypt', 'version': '0.0.0', 'description': 'Fast kasa crypt',
+{ 'name': 'kasa-crypt', 'version': '0.1.0', 'description': 'Fast kasa crypt',
 'long_description': '# kasa-crypt\n\n
             \n \n_[CI_Status]\n\n \n_[Test_coverage_percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
 \n\nFast kasa crypt\n\n## Installation\n\nInstall this via pip (or your
-favourite package manager):\n\n`pip install kasa-crypt`\n\n## Contributors
-â¨\n\nThanks goes to these wonderful people ([emoji key](https://
-allcontributors.org/docs/en/emoji-key)):\n\n\n\n\n\n\n\n\nThis project follows
-the [all-contributors](https://github.com/all-contributors/all-contributors)
-specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package
-was created with\n[Copier](https://copier.readthedocs.io/) and the\n
-[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-
-template)\nproject template.\n', 'author': 'J. Nick Koston', 'author_email':
-'nick@koston.org', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'https://github.com/bdraco/kasa-crypt', 'package_dir': package_dir, 'packages':
-packages, 'package_data': package_data, 'python_requires': '>=3.7,<4.0', } from
-build_ext import * build(setup_kwargs) setup(**setup_kwargs)
+favourite package manager):\n\n`pip install kasa-crypt`\n\n## Example
+usage\n\n```python\nfrom kasa_crypt import encrypt, decrypt\n\nencrypted =
+encrypt(\'{"hello":"world"}\')\ndecrypted = decrypt(encrypted[4:]) # Always a 4
+byte header\nprint (decrypted)\n```\n\n## Contributors â¨\n\nThanks goes to
+these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-
+key)):\n\n\n\n\n\n\n\n\nThis project follows the [all-contributors](https://
+github.com/all-contributors/all-contributors) specification. Contributions of
+any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier]
+(https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template]
+(https://github.com/browniebroke/pypackage-template)\nproject template.\n',
+'author': 'J. Nick Koston', 'author_email': 'nick@koston.org', 'maintainer':
+'None', 'maintainer_email': 'None', 'url': 'https://github.com/bdraco/kasa-
+crypt', 'package_dir': package_dir, 'packages': packages, 'package_data':
+package_data, 'python_requires': '>=3.7,<4.0', } from build_ext import * build
+(setup_kwargs) setup(**setup_kwargs)
```

### Comparing `kasa_crypt-0.0.0/PKG-INFO` & `kasa_crypt-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kasa-crypt
-Version: 0.0.0
+Version: 0.1.0
 Summary: Fast kasa crypt
 Home-page: https://github.com/bdraco/kasa-crypt
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -57,14 +57,24 @@
 
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install kasa-crypt`
 
+## Example usage
+
+```python
+from kasa_crypt import encrypt, decrypt
+
+encrypted = encrypt('{"hello":"world"}')
+decrypted = decrypt(encrypted[4:])  # Always a 4 byte header
+print (decrypted)
+```
+
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- markdownlint-disable -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kasa-crypt Version: 0.0.0 Summary: Fast kasa crypt
+Metadata-Version: 2.1 Name: kasa-crypt Version: 0.1.0 Summary: Fast kasa crypt
 Home-page: https://github.com/bdraco/kasa-crypt License: Apache Software
 License 2.0 Author: J. Nick Koston Author-email: nick@koston.org Requires-
 Python: >=3.7,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: Other/Proprietary
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
@@ -13,14 +13,17 @@
 Changelog, https://github.com/bdraco/kasa-crypt/blob/main/CHANGELOG.md Project-
 URL: Repository, https://github.com/bdraco/kasa-crypt Description-Content-Type:
 text/markdown # kasa-crypt
                     [CI_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 Fast kasa crypt ## Installation Install this via pip (or your favourite package
-manager): `pip install kasa-crypt` ## Contributors â¨ Thanks goes to these
-wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-This project follows the [all-contributors](https://github.com/all-
-contributors/all-contributors) specification. Contributions of any kind
-welcome! ## Credits This package was created with [Copier](https://
-copier.readthedocs.io/) and the [browniebroke/pypackage-template](https://
-github.com/browniebroke/pypackage-template) project template.
+manager): `pip install kasa-crypt` ## Example usage ```python from kasa_crypt
+import encrypt, decrypt encrypted = encrypt('{"hello":"world"}') decrypted =
+decrypt(encrypted[4:]) # Always a 4 byte header print (decrypted) ``` ##
+Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
+allcontributors.org/docs/en/emoji-key)):       This project follows the [all-
+contributors](https://github.com/all-contributors/all-contributors)
+specification. Contributions of any kind welcome! ## Credits This package was
+created with [Copier](https://copier.readthedocs.io/) and the [browniebroke/
+pypackage-template](https://github.com/browniebroke/pypackage-template) project
+template.
```

