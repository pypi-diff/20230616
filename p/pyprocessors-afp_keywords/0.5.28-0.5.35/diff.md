# Comparing `tmp/pyprocessors-afp_keywords-0.5.28.tar.gz` & `tmp/pyprocessors_afp_keywords-0.5.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors-afp_keywords-0.5.28.tar", last modified: Thu Dec 15 21:59:22 2022, max compression
+gzip compressed data, was "pyprocessors_afp_keywords-0.5.35.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyprocessors-afp_keywords-0.5.28.tar` & `pyprocessors_afp_keywords-0.5.35.tar`

### file list

```diff
@@ -1,32 +1,29 @@
--rw-r--r--   0        0        0      501 2022-10-04 08:09:48.718779 pyprocessors-afp_keywords-0.5.28/.bumpversion.cfg
--rw-r--r--   0        0        0     1760 2022-10-04 08:09:48.718779 pyprocessors-afp_keywords-0.5.28/.gitignore
--rw-r--r--   0        0        0      419 2022-10-04 08:09:48.719780 pyprocessors-afp_keywords-0.5.28/.pre-commit-config.yaml
--rw-r--r--   0        0        0      202 2022-10-04 08:09:48.719780 pyprocessors-afp_keywords-0.5.28/.readthedocs.yml
--rw-r--r--   0        0        0      121 2022-10-04 08:09:48.720780 pyprocessors-afp_keywords-0.5.28/AUTHORS.md
--rw-r--r--   0        0        0      268 2022-10-04 08:09:48.720780 pyprocessors-afp_keywords-0.5.28/CHANGELOG.md
--rw-r--r--   0        0        0      476 2022-10-04 08:09:48.720780 pyprocessors-afp_keywords-0.5.28/Dockerfile
--rw-r--r--   0        0        0     8602 2022-12-15 21:49:05.819962 pyprocessors-afp_keywords-0.5.28/Jenkinsfile
--rw-r--r--   0        0        0     1082 2022-10-04 08:09:48.721779 pyprocessors-afp_keywords-0.5.28/LICENSE
--rw-r--r--   0        0        0     1613 2022-10-04 08:09:48.721779 pyprocessors-afp_keywords-0.5.28/README.md
--rw-r--r--   0        0        0      949 2022-10-04 08:09:48.721779 pyprocessors-afp_keywords-0.5.28/RELEASE.md
--rw-r--r--   0        0        0     1559 2022-10-04 08:09:48.722780 pyprocessors-afp_keywords-0.5.28/bumpversion.py
--rw-r--r--   0        0        0       62 2022-10-04 08:09:48.722780 pyprocessors-afp_keywords-0.5.28/docs/.gitignore
--rw-r--r--   0        0        0      268 2022-10-04 08:09:48.723780 pyprocessors-afp_keywords-0.5.28/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2022-10-04 08:09:48.723780 pyprocessors-afp_keywords-0.5.28/docs/LICENSE
--rw-r--r--   0        0        0        0 2022-10-04 08:09:48.723780 pyprocessors-afp_keywords-0.5.28/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2022-10-04 08:09:48.724780 pyprocessors-afp_keywords-0.5.28/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     2899 2022-10-04 08:09:48.725780 pyprocessors-afp_keywords-0.5.28/docs/conf.py
--rw-r--r--   0        0        0      146 2022-10-04 08:09:48.726780 pyprocessors-afp_keywords-0.5.28/docs/index.rst
--rw-r--r--   0        0        0       98 2022-10-04 08:09:48.726780 pyprocessors-afp_keywords-0.5.28/mypy.ini
--rw-r--r--   0        0        0     2265 2022-10-04 08:09:48.727780 pyprocessors-afp_keywords-0.5.28/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-04 08:09:48.728780 pyprocessors-afp_keywords-0.5.28/src/__init__.py
--rw-r--r--   0        0        0      107 2022-12-15 21:59:10.067853 pyprocessors-afp_keywords-0.5.28/src/pyprocessors_afp_keywords/__init__.py
--rw-r--r--   0        0        0     3286 2022-10-04 08:09:48.730780 pyprocessors-afp_keywords-0.5.28/src/pyprocessors_afp_keywords/afp_keywords.py
--rw-r--r--   0        0        0     5949 2022-10-04 08:09:48.731780 pyprocessors-afp_keywords-0.5.28/tests/data/afp_doc_en.json
--rw-r--r--   0        0        0     6500 2022-10-04 08:09:48.732780 pyprocessors-afp_keywords-0.5.28/tests/data/afp_doc_en_slug.json
--rw-r--r--   0        0        0    26875 2022-10-04 08:09:48.733780 pyprocessors-afp_keywords-0.5.28/tests/data/afp_doc_fr.json
--rw-r--r--   0        0        0  2375990 2022-10-04 08:09:48.749780 pyprocessors-afp_keywords-0.5.28/tests/data/afp_doc_fr_slug.json
--rw-r--r--   0        0        0     1825 2022-10-04 08:09:48.749780 pyprocessors-afp_keywords-0.5.28/tests/test_afp_keywords.py
--rw-r--r--   0        0        0      428 2022-10-04 08:09:48.750780 pyprocessors-afp_keywords-0.5.28/tox.ini
--rw-r--r--   0        0        0     1396 1970-01-01 00:00:00.000000 pyprocessors-afp_keywords-0.5.28/setup.py
--rw-r--r--   0        0        0     3412 1970-01-01 00:00:00.000000 pyprocessors-afp_keywords-0.5.28/PKG-INFO
+-rw-r--r--   0        0        0      501 2023-06-16 14:12:55.547285 pyprocessors_afp_keywords-0.5.35/.bumpversion.cfg
+-rw-r--r--   0        0        0     1760 2023-06-16 14:12:55.547285 pyprocessors_afp_keywords-0.5.35/.gitignore
+-rw-r--r--   0        0        0      419 2023-06-16 14:12:55.548285 pyprocessors_afp_keywords-0.5.35/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      202 2023-06-16 14:12:55.548285 pyprocessors_afp_keywords-0.5.35/.readthedocs.yml
+-rw-r--r--   0        0        0      121 2023-06-16 14:12:55.549285 pyprocessors_afp_keywords-0.5.35/AUTHORS.md
+-rw-r--r--   0        0        0      268 2023-06-16 14:12:55.549285 pyprocessors_afp_keywords-0.5.35/CHANGELOG.md
+-rw-r--r--   0        0        0      476 2023-06-16 14:12:55.550285 pyprocessors_afp_keywords-0.5.35/Dockerfile
+-rw-r--r--   0        0        0     8602 2023-06-16 14:12:55.550285 pyprocessors_afp_keywords-0.5.35/Jenkinsfile
+-rw-r--r--   0        0        0     1082 2023-06-16 14:12:55.551285 pyprocessors_afp_keywords-0.5.35/LICENSE
+-rw-r--r--   0        0        0     1613 2023-06-16 14:12:55.551285 pyprocessors_afp_keywords-0.5.35/README.md
+-rw-r--r--   0        0        0      949 2023-06-16 14:12:55.551285 pyprocessors_afp_keywords-0.5.35/RELEASE.md
+-rw-r--r--   0        0        0     1559 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.35/bumpversion.py
+-rw-r--r--   0        0        0       62 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.35/docs/.gitignore
+-rw-r--r--   0        0        0      268 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.35/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.35/docs/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.35/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-16 14:12:55.553285 pyprocessors_afp_keywords-0.5.35/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     2899 2023-06-16 14:12:55.553285 pyprocessors_afp_keywords-0.5.35/docs/conf.py
+-rw-r--r--   0        0        0      146 2023-06-16 14:12:55.553285 pyprocessors_afp_keywords-0.5.35/docs/index.rst
+-rw-r--r--   0        0        0       98 2023-06-16 14:12:55.554285 pyprocessors_afp_keywords-0.5.35/mypy.ini
+-rw-r--r--   0        0        0     2191 2023-06-16 14:12:55.554285 pyprocessors_afp_keywords-0.5.35/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 14:12:55.554285 pyprocessors_afp_keywords-0.5.35/src/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-16 14:16:11.251565 pyprocessors_afp_keywords-0.5.35/src/pyprocessors_afp_keywords/__init__.py
+-rw-r--r--   0        0        0     1885 2023-06-16 14:12:55.555285 pyprocessors_afp_keywords-0.5.35/src/pyprocessors_afp_keywords/afp_keywords.py
+-rw-r--r--   0        0        0     4662 2023-06-16 14:12:55.555285 pyprocessors_afp_keywords-0.5.35/tests/data/afp_doc_fr.json
+-rw-r--r--   0        0        0     1026 2023-06-16 14:12:55.556285 pyprocessors_afp_keywords-0.5.35/tests/test_afp_keywords.py
+-rw-r--r--   0        0        0      428 2023-06-16 14:12:55.556285 pyprocessors_afp_keywords-0.5.35/tox.ini
+-rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 pyprocessors_afp_keywords-0.5.35/setup.py
+-rw-r--r--   0        0        0     3306 1970-01-01 00:00:00.000000 pyprocessors_afp_keywords-0.5.35/PKG-INFO
```

### Comparing `pyprocessors-afp_keywords-0.5.28/.gitignore` & `pyprocessors_afp_keywords-0.5.35/.gitignore`

 * *Files identical despite different names*

### Comparing `pyprocessors-afp_keywords-0.5.28/Jenkinsfile` & `pyprocessors_afp_keywords-0.5.35/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyprocessors-afp_keywords-0.5.28/LICENSE` & `pyprocessors_afp_keywords-0.5.35/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors-afp_keywords-0.5.28/README.md` & `pyprocessors_afp_keywords-0.5.35/README.md`

 * *Files identical despite different names*

### Comparing `pyprocessors-afp_keywords-0.5.28/RELEASE.md` & `pyprocessors_afp_keywords-0.5.35/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyprocessors-afp_keywords-0.5.28/bumpversion.py` & `pyprocessors_afp_keywords-0.5.35/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-afp_keywords-0.5.28/docs/LICENSE` & `pyprocessors_afp_keywords-0.5.35/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors-afp_keywords-0.5.28/docs/conf.py` & `pyprocessors_afp_keywords-0.5.35/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-afp_keywords-0.5.28/pyproject.toml` & `pyprocessors_afp_keywords-0.5.35/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -20,19 +20,15 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development",
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3.8",
 ]
 requires = [
-    "pymultirole-plugins>=0.5.158,<0.6.0",
-    "spacy==2.3.7",
-    "textacy==0.10.1",
-    "cytoolz",
-    "fasttext"
+    "pymultirole-plugins>=0.5.158,<0.6.0"
 ]
 dist-name = "pyprocessors-afp_keywords"
 
 [tool.flit.entrypoints."pyprocessors.plugins"]
 afp_keywords = "pyprocessors_afp_keywords.afp_keywords:AFPKeywordsProcessor"
 
 [tool.flit.metadata.requires-extra]
```

### Comparing `pyprocessors-afp_keywords-0.5.28/setup.py` & `pyprocessors_afp_keywords-0.5.35/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,15 @@
 package_data = \
 {'': ['*']}
 
 package_dir = \
 {'': 'src'}
 
 install_requires = \
-['pymultirole-plugins>=0.5.158,<0.6.0',
- 'spacy==2.3.7',
- 'textacy==0.10.1',
- 'cytoolz',
- 'fasttext']
+['pymultirole-plugins>=0.5.158,<0.6.0']
 
 extras_require = \
 {'dev': ['flit', 'pre-commit', 'bump2version'],
  'docs': ['sphinx',
           'sphinx-rtd-theme',
           'm2r2',
           'sphinxcontrib.apidoc',
@@ -34,15 +30,15 @@
           'tox']}
 
 entry_points = \
 {'pyprocessors.plugins': ['afp_keywords = '
                           'pyprocessors_afp_keywords.afp_keywords:AFPKeywordsProcessor']}
 
 setup(name='pyprocessors-afp_keywords',
-      version='0.5.28',
+      version='0.5.35',
       description='Processor based on Huggingface transformers zero-shot classification pipeline',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://github.com/oterrier/pyprocessors_afp_keywords/',
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `pyprocessors-afp_keywords-0.5.28/PKG-INFO` & `pyprocessors_afp_keywords-0.5.35/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-afp_keywords
-Version: 0.5.28
+Version: 0.5.35
 Summary: Processor based on Huggingface transformers zero-shot classification pipeline
 Home-page: https://github.com/oterrier/pyprocessors_afp_keywords/
 Keywords: 
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -16,18 +16,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: pymultirole-plugins>=0.5.158,<0.6.0
-Requires-Dist: spacy==2.3.7
-Requires-Dist: textacy==0.10.1
-Requires-Dist: cytoolz
-Requires-Dist: fasttext
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: bump2version ; extra == "dev"
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Requires-Dist: m2r2 ; extra == "docs"
 Requires-Dist: sphinxcontrib.apidoc ; extra == "docs"
```

