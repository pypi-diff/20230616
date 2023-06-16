# Comparing `tmp/uedition-0.1.0.tar.gz` & `tmp/uedition-0.2.0.tar.gz`

## Comparing `uedition-0.1.0.tar` & `uedition-0.2.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 uedition-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uedition-0.1.0/tox.ini
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 uedition-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 uedition-0.1.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 uedition-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 uedition-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/test_about.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/test_build.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/test_check.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/test_settings.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/basic/uEdition.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/empty/.gitkeep
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/invalid_core_files/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/invalid_core_files/en/_config.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/invalid_core_files/en/_toc.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_core_files/uEdition.yaml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_files/.gitignore
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_files/references.bib
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_files/uEdition.yaml
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_files/en/_config.yml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_files/en/_toc.yml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_files/en/intro.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_toc_root/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_toc_root/en/_config.yml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_toc_root/en/_toc.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_toc_root_file/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_toc_root_file/en/_config.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_toc_root_file/en/_toc.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/.gitignore
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/references.bib
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/uEdition.yaml
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/_config.yml
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/_toc.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/a-1-page.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/a-2-page.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/a-page.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/b-page.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/intro.md
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/_config.yml
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/_toc.yml
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/a-1-page.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/a-2-page.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/a-page.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/b-page.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/intro.md
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/yaml/uEdition.yaml
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/__about__.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/__main__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/settings.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/cli/__init__.py
--rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/cli/check.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/ext/__init__.py
--rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/ext/config.py
--rw-r--r--   0        0        0     9716 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/ext/tei.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 uedition-0.1.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uedition-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 uedition-0.1.0/README.md
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 uedition-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 uedition-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 uedition-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uedition-0.2.0/tox.ini
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 uedition-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 uedition-0.2.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 uedition-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 uedition-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/test_about.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/test_build.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/test_check.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/test_settings.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/basic/uEdition.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/empty/.gitkeep
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/invalid_core_files/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/invalid_core_files/en/_config.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/invalid_core_files/en/_toc.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_core_files/uEdition.yaml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_files/.gitignore
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_files/references.bib
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_files/uEdition.yaml
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_files/en/_config.yml
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_files/en/_toc.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_files/en/intro.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_toc_root/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_toc_root/en/_config.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_toc_root/en/_toc.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_toc_root_file/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_toc_root_file/en/_config.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_toc_root_file/en/_toc.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/.gitignore
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/references.bib
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/uEdition.yaml
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/_config.yml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/_toc.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/a-1-page.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/a-2-page.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/a-page.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/b-page.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/intro.md
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/_config.yml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/_toc.yml
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/a-1-page.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/a-2-page.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/a-page.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/b-page.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/intro.md
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/yaml/uEdition.yaml
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/__about__.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/__main__.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/settings.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/cli/__init__.py
+-rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/cli/check.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/cli/serve.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/ext/__init__.py
+-rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/ext/config.py
+-rw-r--r--   0        0        0    10626 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/ext/tei.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 uedition-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uedition-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 uedition-0.2.0/README.md
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 uedition-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 uedition-0.2.0/PKG-INFO
```

### Comparing `uedition-0.1.0/.github/workflows/coverage.yml` & `uedition-0.2.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/.github/workflows/release.yml` & `uedition-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/.github/workflows/tests.yml` & `uedition-0.2.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/tests/conftest.py` & `uedition-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/tests/test_build.py` & `uedition-0.2.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/tests/test_check.py` & `uedition-0.2.0/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/tests/test_settings.py` & `uedition-0.2.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/tests/fixtures/missing_files/references.bib` & `uedition-0.2.0/tests/fixtures/missing_files/references.bib`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/tests/fixtures/missing_files/en/_config.yml` & `uedition-0.2.0/tests/fixtures/missing_files/en/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/tests/fixtures/multilang/references.bib` & `uedition-0.2.0/tests/fixtures/multilang/references.bib`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/tests/fixtures/multilang/de/_config.yml` & `uedition-0.2.0/tests/fixtures/multilang/de/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/tests/fixtures/multilang/en/_config.yml` & `uedition-0.2.0/tests/fixtures/multilang/en/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/uedition/settings.py` & `uedition-0.2.0/uedition/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     """Application settings."""
 
     version: str = '1'
     """The configuration file version."""
     languages: list[LanguageSetting] = []
     """The configured languages."""
     output: str = 'docs'
-    """The output directory"""
+    """The output directory."""
 
     class Config:
         """Configuration overrides."""
 
         @classmethod
         def customise_sources(
             cls,  # noqa: ANN102
```

### Comparing `uedition-0.1.0/uedition/cli/__init__.py` & `uedition-0.2.0/uedition/cli/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import typer
 
 from rich import print as print_cli
 from shutil import rmtree, copytree
 from subprocess import run
 
-from . import check as check_module
+from . import check as check_module, serve as serve_module
 from ..__about__ import __version__
 from ..settings import settings
 
 
 app = typer.Typer()
 
 
@@ -30,14 +30,20 @@
         copytree(
             os.path.join(language['path'], '_build', 'html'),
             os.path.join(settings['output'], language['path'])
         )
 
 
 @app.command()
+def serve() -> None:
+    """Serve the μEdition for writing."""
+    serve_module.run()
+
+
+@app.command()
 def check() -> None:
     """Check that the μEdition is set up correctly."""
     check_module.run()
 
 
 @app.command()
 def version() -> None:
```

### Comparing `uedition-0.1.0/uedition/cli/check.py` & `uedition-0.2.0/uedition/cli/check.py`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/uedition/ext/config.py` & `uedition-0.2.0/uedition/ext/config.py`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/uedition/ext/tei.py` & `uedition-0.2.0/uedition/ext/tei.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,24 +10,26 @@
 namespaces = {'tei': 'http://www.tei-c.org/ns/1.0'}
 
 
 class TeiElement(nodes.Element): pass
 
 
 def tei_element_html_enter(self, node: TeiElement) -> None:
-    buffer = [f'<{node.get("html_tag")} data-tei-tag="{node.get("tei_tag")[29:]}"']
-    if node.get('ids'):
-        buffer.append(f' id="{node.get("ids")[0]}"')
-    for key, value in node.get('tei_attributes').items():
-        buffer.append(f' {key}="{value}"')
-    self.body.append(f'{"".join(buffer)}>')
+    if node.get('html_tag') is not None:
+        buffer = [f'<{node.get("html_tag")} data-tei-tag="{node.get("tei_tag")[29:]}"']
+        if node.get('ids'):
+            buffer.append(f' id="{node.get("ids")[0]}"')
+        for key, value in node.get('tei_attributes').items():
+            buffer.append(f' {key}="{value}"')
+        self.body.append(f'{"".join(buffer)}>')
 
 
 def tei_element_html_exit(self, node: TeiElement) -> None:
-    self.body.append(f'</{node.get("html_tag")}>')
+    if node.get('html_tag') is not None:
+        self.body.append(f'</{node.get("html_tag")}>')
 
 
 class TEIParser(SphinxParser):
     """Sphinx parser for Text Encoding Initiative XML."""
 
     supported: tuple[str, ...] = ('tei',)
     """Specify that only .tei files are parsed"""
@@ -45,43 +47,37 @@
         """
         root = etree.fromstring(inputstring.encode('UTF-8'))
         title = root.xpath('string(/tei:TEI/tei:teiHeader/tei:fileDesc/tei:titleStmt/tei:title)', namespaces=namespaces)
         doc_section = nodes.section(ids=['document'])
         doc_title = nodes.title()
         doc_title.append(nodes.Text(title if title else '[Untitled]'))
         doc_section.append(doc_title)
-        tab_set = create_component('tab-set', classes=['sd-tab-set'])
         if 'tei' in self.config.uEdition and 'sections' in self.config.uEdition['tei']:
-            for section in self.config.uEdition['tei']['sections']:
-                if section['type'] == 'text':
-                    source = root.xpath(section['content'], namespaces=namespaces)
+            for conf_section in self.config.uEdition['tei']['sections']:
+                section = nodes.section(ids=[nodes.make_id(conf_section['title'])])
+                section_title = nodes.title()
+                section_title.append(nodes.Text(conf_section['title']))
+                section.append(section_title)
+                if conf_section['type'] == 'text':
+                    source = root.xpath(conf_section['content'], namespaces=namespaces)
                     if len(source) > 0:
-                        tab_item = create_component('tab-item', classes=['sd-tab-item'])
-                        tab_label = nodes.rubric(section['title'], nodes.Text(section['title']), classes=['sd-tab-label'])
-                        tab_item.append(tab_label)
-                        tab_content = create_component('tab-content', classes=['sd-tab-content', 'tei', nodes.make_id(section['title'])])
-                        tab_item.append(tab_content)
+                        doc_section.append(section)
+                        tmp = nodes.section()
                         for child in source:
-                            self._walk_tree(child, tab_content, section['mappings'])
-                        tab_set.append(tab_item)
-                elif section['type'] == 'fields':
-                    tab_item = create_component('tab-item', classes=['sd-tab-item'])
-                    tab_label = nodes.rubric(section['title'], nodes.Text(section['title']), classes=['sd-tab-label'])
-                    tab_item.append(tab_label)
-                    tab_content = create_component('tab-content', classes=['sd-tab-content', 'tei', nodes.make_id(section['title'])])
-                    tab_item.append(tab_content)
+                            self._walk_tree(child, tmp, conf_section['mappings'])
+                        self._wrap_sections(section, tmp)
+                elif conf_section['type'] == 'fields':
+                    doc_section.append(section)
                     fields = nodes.definition_list()
-                    tab_content.append(fields)
-                    for field in section['fields']:
+                    section.append(fields)
+                    for field in conf_section['fields']:
                         if field['type'] == 'single':
                             self._parse_single_field(fields, field, root)
                         elif field['type'] == 'list':
                             self._parse_list_field(fields, field, root)
-                    tab_set.append(tab_item)
-        doc_section.append(tab_set)
         document.append(doc_section)
 
     def _walk_tree(self: 'TEIParser', node: etree.Element, parent: nodes.Element, rules) -> None:
         """Walk the XML tree and create the appropriate AST nodes.
 
         Uses the mapping rules defined in :mod:`~uEdition.extensions.config` to determine what to
         map the XML to.
@@ -141,14 +137,42 @@
         # Process any children
         for child in node:
             self._walk_tree(child, new_element, rules)
         # If there is text after this XML node and we are adding all text, then add text content to the parent
         if node.tail and not text_only_in_leaf_nodes:
             parent.append(nodes.Text(node.tail))
 
+    def _wrap_sections(self: 'TEIParser', section: nodes.Element, tmp: nodes.Element) -> None:
+        """Ensure that sections are correctly wrapped."""
+        section_stack = [(0, section)]
+        for node in tmp.findall():
+            if isinstance(node, TeiElement) and node.attributes['html_tag'] in ['h1', 'h2', 'h3', 'h4', 'h5', 'h6']:
+                section_level = int(node.attributes['html_tag'][1])
+                while section_level <= section_stack[-1][0]:
+                    section_stack.pop()
+                new_section = nodes.section(ids=[nodes.make_id(node.astext())])
+                title = nodes.title()
+                title.children = node.children
+                new_section.append(title)
+                section_stack[-1][1].append(new_section)
+                section_stack.append((section_level, new_section))
+            elif isinstance(node, nodes.section):
+                pass
+            else:
+                # Need to check that the
+                in_heading = False
+                tmp = node
+                while tmp.parent is not None and isinstance(tmp.parent, TeiElement):
+                    if tmp.parent.attributes['html_tag'] in ['h1', 'h2', 'h3', 'h4', 'h5', 'h6']:
+                        in_heading = True
+                        break
+                    tmp = tmp.parent
+                if not in_heading:
+                    section_stack[-1][1].append(node)
+
     def _rule_for_node(self: 'TEIParser', node: etree.Element, rules: list[dict]) -> dict:
         """Determine the first matching mapping rule for the node from the configured rules."""
         tei_tag = node.tag
         for rule in rules:
             if rule['selector']['tag'] == tei_tag:
                 if 'attributes' in rule['selector']:
                     attr_match = True
```

### Comparing `uedition-0.1.0/LICENSE.txt` & `uedition-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/README.md` & `uedition-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `uedition-0.1.0/pyproject.toml` & `uedition-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 ]
 dependencies = [
   "jupyter-book>=0.15.1,<1.0.0",
   "pydantic[dotenv]>=1.0.0,<2.0.0",
   "PyYAML>=6.0.0,<7.0.0",
   "typer[all]<1.0.0",
   "lxml>=4.9.2,<5.0.0",
+  "livereload",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 uEdition = "uedition.cli:app"
 
 [project.urls]
```

### Comparing `uedition-0.1.0/PKG-INFO` & `uedition-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: uEdition
-Version: 0.1.0
+Version: 0.2.0
 Project-URL: Documentation, https://github.com/unknown/uedition#readme
 Project-URL: Issues, https://github.com/unknown/uedition/issues
 Project-URL: Source, https://github.com/unknown/uedition
 Author-email: Mark Hall <mark.hall@work.room3b.eu>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: jupyter-book<1.0.0,>=0.15.1
+Requires-Dist: livereload
 Requires-Dist: lxml<5.0.0,>=4.9.2
 Requires-Dist: pydantic[dotenv]<2.0.0,>=1.0.0
 Requires-Dist: pyyaml<7.0.0,>=6.0.0
 Requires-Dist: typer[all]<1.0.0
 Description-Content-Type: text/markdown
 
 # μEdition
```

