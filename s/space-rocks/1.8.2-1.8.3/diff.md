# Comparing `tmp/space_rocks-1.8.2.tar.gz` & `tmp/space_rocks-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_rocks-1.8.2.tar", max compression
+gzip compressed data, was "space_rocks-1.8.3.tar", max compression
```

## Comparing `space_rocks-1.8.2.tar` & `space_rocks-1.8.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2023-04-21 07:53:47.207007 space_rocks-1.8.2/LICENSE
--rw-r--r--   0        0        0     1731 2023-04-21 07:53:47.207007 space_rocks-1.8.2/README.md
--rw-r--r--   0        0        0     1519 2023-06-02 15:35:49.717529 space_rocks-1.8.2/pyproject.toml
--rw-r--r--   0        0        0      450 2023-06-02 15:35:49.717529 space_rocks-1.8.2/rocks/__init__.py
--rw-r--r--   0        0        0     4886 2023-04-21 07:53:47.215006 space_rocks-1.8.2/rocks/cache.py
--rw-r--r--   0        0        0    11457 2023-06-02 15:35:49.717529 space_rocks-1.8.2/rocks/cli.py
--rw-r--r--   0        0        0     7078 2023-04-21 07:53:47.215006 space_rocks-1.8.2/rocks/config.py
--rw-r--r--   0        0        0    39666 2023-05-26 20:42:35.837290 space_rocks-1.8.2/rocks/core.py
--rw-r--r--   0        0        0    32930 2023-04-21 07:53:47.215006 space_rocks-1.8.2/rocks/datacloud.py
--rw-r--r--   0        0        0    14953 2023-06-02 15:35:49.717529 space_rocks-1.8.2/rocks/index.py
--rw-r--r--   0        0        0      982 2023-04-21 07:53:47.215006 space_rocks-1.8.2/rocks/logging.py
--rw-r--r--   0        0        0     3765 2023-04-21 07:53:47.215006 space_rocks-1.8.2/rocks/metadata.py
--rw-r--r--   0        0        0     6300 2023-02-19 15:02:48.465877 space_rocks-1.8.2/rocks/plots.py
--rw-r--r--   0        0        0    13145 2023-06-02 15:35:49.717529 space_rocks-1.8.2/rocks/resolve.py
--rw-r--r--   0        0        0    12222 2023-05-04 09:06:04.136860 space_rocks-1.8.2/rocks/ssodnet.py
--rw-r--r--   0        0        0     3198 1970-01-01 00:00:00.000000 space_rocks-1.8.2/setup.py
--rw-r--r--   0        0        0     3317 1970-01-01 00:00:00.000000 space_rocks-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-21 07:53:47.207007 space_rocks-1.8.3/LICENSE
+-rw-r--r--   0        0        0     1731 2023-04-21 07:53:47.207007 space_rocks-1.8.3/README.md
+-rw-r--r--   0        0        0     1571 2023-06-16 10:39:48.752584 space_rocks-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0      450 2023-06-16 10:40:07.040585 space_rocks-1.8.3/rocks/__init__.py
+-rw-r--r--   0        0        0     4886 2023-04-21 07:53:47.215006 space_rocks-1.8.3/rocks/cache.py
+-rw-r--r--   0        0        0    11457 2023-06-02 15:35:49.717529 space_rocks-1.8.3/rocks/cli.py
+-rw-r--r--   0        0        0     7078 2023-04-21 07:53:47.215006 space_rocks-1.8.3/rocks/config.py
+-rw-r--r--   0        0        0    40000 2023-06-16 10:09:00.440549 space_rocks-1.8.3/rocks/core.py
+-rw-r--r--   0        0        0    32930 2023-04-21 07:53:47.215006 space_rocks-1.8.3/rocks/datacloud.py
+-rw-r--r--   0        0        0    14953 2023-06-02 15:35:49.717529 space_rocks-1.8.3/rocks/index.py
+-rw-r--r--   0        0        0      982 2023-04-21 07:53:47.215006 space_rocks-1.8.3/rocks/logging.py
+-rw-r--r--   0        0        0     3765 2023-04-21 07:53:47.215006 space_rocks-1.8.3/rocks/metadata.py
+-rw-r--r--   0        0        0     6300 2023-02-19 15:02:48.465877 space_rocks-1.8.3/rocks/plots.py
+-rw-r--r--   0        0        0    13145 2023-06-02 15:35:49.717529 space_rocks-1.8.3/rocks/resolve.py
+-rw-r--r--   0        0        0    12222 2023-05-04 09:06:04.136860 space_rocks-1.8.3/rocks/ssodnet.py
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 space_rocks-1.8.3/setup.py
+-rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 space_rocks-1.8.3/PKG-INFO
```

### Comparing `space_rocks-1.8.2/LICENSE` & `space_rocks-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.2/README.md` & `space_rocks-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.2/pyproject.toml` & `space_rocks-1.8.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "space-rocks"
-version = "1.8.2"
+version = "1.8.3"
 description = "Python client for SsODNet data access."
 authors = ["Max Mahlke <max.mahlke@oca.eu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://rocks.readthedocs.io/en/latest/"
 documentation = "https://rocks.readthedocs.io/en/latest/"
 repository = "https://github.com/maxmahlke/rocks.git"
@@ -29,14 +29,15 @@
 Levenshtein = ">=0.16.0"
 furo = "^2022.9.15"
 sphinx-copybutton = "^0.5.0"
 sphinx_design = "^0.3.0"
 beautifulsoup4 = "^4.11.1"
 platformdirs = "^2.6.2"
 rapidfuzz = "^3"
+sphinx-hoverxref = {version = "*", optional = true}
 
 [tool.poetry.extras]
 docs = ["sphinx", "sphinx-redactor-theme", "sphinx-hoverxref"]
 
 [tool.poetry.scripts]
 rocks = "rocks.cli:cli_rocks"
```

### Comparing `space_rocks-1.8.2/rocks/cache.py` & `space_rocks-1.8.3/rocks/cache.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.2/rocks/cli.py` & `space_rocks-1.8.3/rocks/cli.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.2/rocks/config.py` & `space_rocks-1.8.3/rocks/config.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.2/rocks/core.py` & `space_rocks-1.8.3/rocks/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,30 @@
             else:
                 value.path = f"{parent}.{name}"
     return values
 
 
 # The lowest level in the ssoCard tree is the are the differnt Values and the Error
 class Error(pydantic.BaseModel):
-    min_: float = pydantic.Field(np.nan, alias="min")
-    max_: float = pydantic.Field(np.nan, alias="max")
+    min: float = np.nan
+    max: float = np.nan
+
+    @property
+    def min_(self):
+        logger.warning(
+            "Use 'max' and 'min' to access the errors. The 'max_' and 'min_' attributes will soon be removed."
+        )
+        return self.min
+
+    @property
+    def max_(self):
+        logger.warning(
+            "Use 'max' and 'min' to access the errors. The 'max_' and 'min_' attributes will soon be removed."
+        )
+        return self.max
 
 
 # The second lowest level is the Parameter. Values inherit from Parameter.
 class Parameter(pydantic.BaseModel):
     _label: str = pydantic.Field("", exclude=True)
     _format: str = pydantic.Field("", exclude=True)
     _symbol: str = pydantic.Field("", exclude=True)
@@ -91,27 +105,27 @@
         if "description" in metadata.load_mappings()[self.path]:
             return metadata.load_mappings()[self.path]["description"]
         return ""
 
 
 class FloatValue(Parameter):
     _unit: str = ""
-    error: Error = Error(**{})  # min_ and max_ values
+    error: Error = Error(**{})  # min and max values
     value: float = np.nan
-    error_: float = np.nan  # average of min_ and max_
+    error_: float = np.nan  # average of min and max
 
     def __str__(self):
         """Print value of numerical parameter including errors and unit if available."""
 
         format = self.format.strip("%")
 
-        if abs(self.error.min_) == abs(self.error.max_):
-            return f"{self.value:{format}} +- {self.error.max_:{format}} {self.unit}"
+        if abs(self.error.min) == abs(self.error.max):
+            return f"{self.value:{format}} +- {self.error.max:{format}} {self.unit}"
         else:
-            return f"{self.value:{format}} +- ({self.error.max_:{format}}, {self.error.min_:{format}}) {self.unit}"
+            return f"{self.value:{format}} +- ({self.error.max:{format}}, {self.error.min:{format}}) {self.unit}"
 
     def __bool__(self):
         if np.isnan(self.value):
             return False
         return True
 
     @property
@@ -429,17 +443,17 @@
     id_filter_2: StringValue = StringValue(**{})
 
     def __bool__(self):
         return bool(np.isfinite(self.color.value))
 
     def __str__(self):
         if not np.isnan(self.color.value):
-            if self.color.error.max_ == self.color.error.min_:
-                return rf"{self.color.value:.2f} +- {self.color.error.max_:.2f}  {self.bibref.shortbib}"
-            return rf"{self.color.value:.2f} + {self.color.error.max_:.2f} - {self.color.error.min_:.2f}  {self.bibref.shortbib}"
+            if self.color.error.max == self.color.error.min:
+                return rf"{self.color.value:.2f} +- {self.color.error.max:.2f}  {self.bibref.shortbib}"
+            return rf"{self.color.value:.2f} + {self.color.error.max:.2f} - {self.color.error.min:.2f}  {self.bibref.shortbib}"
         return "No color on record in this filter."
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
         return add_paths(cls, values, "parameters.physical.colors.<id>.color")
 
     _convert_list_to_parameterlist: classmethod = pydantic.validator(
```

### Comparing `space_rocks-1.8.2/rocks/datacloud.py` & `space_rocks-1.8.3/rocks/datacloud.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.2/rocks/index.py` & `space_rocks-1.8.3/rocks/index.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.2/rocks/logging.py` & `space_rocks-1.8.3/rocks/logging.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.2/rocks/metadata.py` & `space_rocks-1.8.3/rocks/metadata.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.2/rocks/plots.py` & `space_rocks-1.8.3/rocks/plots.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.2/rocks/resolve.py` & `space_rocks-1.8.3/rocks/resolve.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.2/rocks/ssodnet.py` & `space_rocks-1.8.3/rocks/ssodnet.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.2/setup.py` & `space_rocks-1.8.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,22 +24,23 @@
  'requests>=2.26.0,<3.0.0',
  'rich>=12.2.0',
  'sphinx-copybutton>=0.5.0,<0.6.0',
  'sphinx_design>=0.3.0,<0.4.0']
 
 extras_require = \
 {':python_version >= "3.11" and python_version < "4.0"': ['numpy>=1.24'],
- ':python_version >= "3.7" and python_version < "3.11"': ['numpy>=1.21']}
+ ':python_version >= "3.7" and python_version < "3.11"': ['numpy>=1.21'],
+ 'docs': ['sphinx-hoverxref']}
 
 entry_points = \
 {'console_scripts': ['rocks = rocks.cli:cli_rocks']}
 
 setup_kwargs = {
     'name': 'space-rocks',
-    'version': '1.8.2',
+    'version': '1.8.3',
     'description': 'Python client for SsODNet data access.',
     'long_description': '<p align="center">\n  <img width="260" src="https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/logo_rocks.svg">\n</p>\n\n<p align="center">\n  <a href="https://github.com/maxmahlke/rocks#features"> Features </a> - <a href="https://github.com/maxmahlke/rocks#install"> Install </a> - <a href="https://github.com/maxmahlke/rocks#documentation"> Documentation </a>\n</p>\n\n<br>\n\n<div align="center">\n  <a href="https://img.shields.io/pypi/pyversions/space-rocks">\n    <img src="https://img.shields.io/pypi/pyversions/space-rocks"/>\n  </a>\n  <a href="https://img.shields.io/pypi/v/space-rocks">\n    <img src="https://img.shields.io/pypi/v/space-rocks"/>\n  </a>\n  <a href="https://readthedocs.org/projects/rocks/badge/?version=latest">\n    <img src="https://readthedocs.org/projects/rocks/badge/?version=latest"/>\n  </a>\n  <a href="https://arxiv.org/abs/2209.10697">\n    <img src="https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg"/>\n  </a>\n</div>\n\n<br>\n\n## Features\n\nExplore asteroid data on the command-line...\n\n``` sh\n$ rocks id 221\n(221) Eos\n\n$ rocks class Eos\nMB>Outer\n\n$ rocks albedo Eos\n0.136 +- 0.004\n\n$ rocks taxonomy Eos\nK\n\n$ rocks density Eos\n4.559e+03 +- 1.139e+03 kg/m$^3$\n```\n\n... and in a `python` script.\n\n``` python\n>>> import rocks\n>>> rocks.identify("1902ug")\n(\'Fortuna\', 19)\n>>> ceres = rocks.Rock("ceres")\n>>> ceres.diameter.value\n848.4\n>>> ceres.diameter.unit\n\'km\'\n>>> ceres.mass.value\n9.384e+20\n>>> ceres.mass.error\n6.711e+17\n```\n\n## Install\n\nInstall from PyPi using `pip`:\n\n     $ pip install space-rocks\n\nThe minimum required `python` version is 3.7.\n\n\n## Documentation\n\nCheck out the documentation at [rocks.readthedocs.io](https://rocks.readthedocs.io/en/latest/) or run\n\n     $ rocks docs\n',
     'author': 'Max Mahlke',
     'author_email': 'max.mahlke@oca.eu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://rocks.readthedocs.io/en/latest/',
```

#### html2text {}

```diff
@@ -3,18 +3,18 @@
 'aiodns>=3.0.0,<4.0.0', 'aiohttp>=3.8.2', 'beautifulsoup4>=4.11.1,<5.0.0',
 'click>=8.1.2', 'faust-cchardet>=2.1.7', 'furo>=2022.9.15,<2023.0.0',
 'matplotlib>=3.4.3', 'nest-asyncio>=1.5.1,<2.0.0', 'pandas>=1.3.5',
 'platformdirs>=2.6.2,<3.0.0', 'pydantic>=1.8.2,<2.0.0', 'rapidfuzz>=3,<4',
 'requests>=2.26.0,<3.0.0', 'rich>=12.2.0', 'sphinx-copybutton>=0.5.0,<0.6.0',
 'sphinx_design>=0.3.0,<0.4.0'] extras_require = \ {':python_version >= "3.11"
 and python_version < "4.0"': ['numpy>=1.24'], ':python_version >= "3.7" and
-python_version < "3.11"': ['numpy>=1.21']} entry_points = \ {'console_scripts':
-['rocks = rocks.cli:cli_rocks']} setup_kwargs = { 'name': 'space-rocks',
-'version': '1.8.2', 'description': 'Python client for SsODNet data access.',
-'long_description': '
+python_version < "3.11"': ['numpy>=1.21'], 'docs': ['sphinx-hoverxref']}
+entry_points = \ {'console_scripts': ['rocks = rocks.cli:cli_rocks']}
+setup_kwargs = { 'name': 'space-rocks', 'version': '1.8.3', 'description':
+'Python client for SsODNet data access.', 'long_description': '
   \n [https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/
                                logo_rocks.svg]\n
 \n\n
                     \n Features - Install - Documentation\n
 \n\n
 \n\n
   \n \n_[https://img.shields.io/pypi/pyversions/space-rocks]\n\n \n_[https://
```

### Comparing `space_rocks-1.8.2/PKG-INFO` & `space_rocks-1.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-rocks
-Version: 1.8.2
+Version: 1.8.3
 Summary: Python client for SsODNet data access.
 Home-page: https://rocks.readthedocs.io/en/latest/
 License: MIT
 Author: Max Mahlke
 Author-email: max.mahlke@oca.eu
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -28,14 +28,15 @@
 Requires-Dist: pandas (>=1.3.5)
 Requires-Dist: platformdirs (>=2.6.2,<3.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: rapidfuzz (>=3,<4)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: rich (>=12.2.0)
 Requires-Dist: sphinx-copybutton (>=0.5.0,<0.6.0)
+Requires-Dist: sphinx-hoverxref; extra == "docs"
 Requires-Dist: sphinx_design (>=0.3.0,<0.4.0)
 Project-URL: Documentation, https://rocks.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/maxmahlke/rocks.git
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img width="260" src="https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/logo_rocks.svg">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: space-rocks Version: 1.8.2 Summary: Python client
+Metadata-Version: 2.1 Name: space-rocks Version: 1.8.3 Summary: Python client
 for SsODNet data access. Home-page: https://rocks.readthedocs.io/en/latest/
 License: MIT Author: Max Mahlke Author-email: max.mahlke@oca.eu Requires-
 Python: >=3.7.1,<3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: docs Requires-Dist: Levenshtein
@@ -12,17 +12,18 @@
 (>=2022.9.15,<2023.0.0) Requires-Dist: matplotlib (>=3.4.3) Requires-Dist:
 nest-asyncio (>=1.5.1,<2.0.0) Requires-Dist: numpy (>=1.21); python_version >=
 "3.7" and python_version < "3.11" Requires-Dist: numpy (>=1.24); python_version
 >= "3.11" and python_version < "4.0" Requires-Dist: pandas (>=1.3.5) Requires-
 Dist: platformdirs (>=2.6.2,<3.0.0) Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: rapidfuzz (>=3,<4) Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: rich (>=12.2.0) Requires-Dist: sphinx-copybutton
-(>=0.5.0,<0.6.0) Requires-Dist: sphinx_design (>=0.3.0,<0.4.0) Project-URL:
-Documentation, https://rocks.readthedocs.io/en/latest/ Project-URL: Repository,
-https://github.com/maxmahlke/rocks.git Description-Content-Type: text/markdown
+(>=0.5.0,<0.6.0) Requires-Dist: sphinx-hoverxref; extra == "docs" Requires-
+Dist: sphinx_design (>=0.3.0,<0.4.0) Project-URL: Documentation, https://
+rocks.readthedocs.io/en/latest/ Project-URL: Repository, https://github.com/
+maxmahlke/rocks.git Description-Content-Type: text/markdown
     [https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/
                                 logo_rocks.svg]
                       Features - Install - Documentation
 
  [https://img.shields.io/pypi/pyversions/space-rocks] [https://img.shields.io/
       pypi/v/space-rocks] [https://readthedocs.org/projects/rocks/badge/
   ?version=latest] [https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg]
```

