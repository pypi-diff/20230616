# Comparing `tmp/uedition-0.2.0.tar.gz` & `tmp/uedition-0.2.1.tar.gz`

## Comparing `uedition-0.2.0.tar` & `uedition-0.2.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 uedition-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uedition-0.2.0/tox.ini
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 uedition-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 uedition-0.2.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 uedition-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 uedition-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/test_about.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/test_build.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/test_check.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/test_settings.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/basic/uEdition.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/empty/.gitkeep
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/invalid_core_files/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/invalid_core_files/en/_config.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/invalid_core_files/en/_toc.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_core_files/uEdition.yaml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_files/.gitignore
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_files/references.bib
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_files/uEdition.yaml
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_files/en/_config.yml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_files/en/_toc.yml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_files/en/intro.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_toc_root/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_toc_root/en/_config.yml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_toc_root/en/_toc.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_toc_root_file/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_toc_root_file/en/_config.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/missing_toc_root_file/en/_toc.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/.gitignore
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/references.bib
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/uEdition.yaml
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/_config.yml
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/_toc.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/a-1-page.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/a-2-page.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/a-page.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/b-page.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/de/intro.md
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/_config.yml
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/_toc.yml
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/a-1-page.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/a-2-page.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/a-page.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/b-page.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/multilang/en/intro.md
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.2.0/tests/fixtures/yaml/uEdition.yaml
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/__about__.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/__main__.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/settings.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/cli/__init__.py
--rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/cli/check.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/cli/serve.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/ext/__init__.py
--rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/ext/config.py
--rw-r--r--   0        0        0    10626 2020-02-02 00:00:00.000000 uedition-0.2.0/uedition/ext/tei.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 uedition-0.2.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uedition-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 uedition-0.2.0/README.md
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 uedition-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 uedition-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 uedition-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uedition-0.2.1/tox.ini
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 uedition-0.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 uedition-0.2.1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 uedition-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 uedition-0.2.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/test_about.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/test_build.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/test_check.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/test_settings.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/basic/uEdition.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/empty/.gitkeep
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/invalid_core_files/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/invalid_core_files/en/_config.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/invalid_core_files/en/_toc.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/missing_core_files/uEdition.yaml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/missing_files/.gitignore
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/missing_files/references.bib
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/missing_files/uEdition.yaml
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/missing_files/en/_config.yml
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/missing_files/en/_toc.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/missing_files/en/intro.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/missing_toc_root/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/missing_toc_root/en/_config.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/missing_toc_root/en/_toc.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/missing_toc_root_file/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/missing_toc_root_file/en/_config.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/missing_toc_root_file/en/_toc.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/.gitignore
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/references.bib
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/uEdition.yaml
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/de/_config.yml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/de/_toc.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/de/a-1-page.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/de/a-2-page.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/de/a-page.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/de/b-page.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/de/intro.md
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/en/_config.yml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/en/_toc.yml
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/en/a-1-page.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/en/a-2-page.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/en/a-page.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/en/b-page.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/multilang/en/intro.md
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.2.1/tests/fixtures/yaml/uEdition.yaml
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 uedition-0.2.1/uedition/__about__.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 uedition-0.2.1/uedition/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 uedition-0.2.1/uedition/__main__.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 uedition-0.2.1/uedition/settings.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 uedition-0.2.1/uedition/cli/__init__.py
+-rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 uedition-0.2.1/uedition/cli/check.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 uedition-0.2.1/uedition/cli/serve.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 uedition-0.2.1/uedition/ext/__init__.py
+-rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 uedition-0.2.1/uedition/ext/config.py
+-rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 uedition-0.2.1/uedition/ext/tei.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 uedition-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uedition-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 uedition-0.2.1/README.md
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 uedition-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 uedition-0.2.1/PKG-INFO
```

### Comparing `uedition-0.2.0/.github/workflows/coverage.yml` & `uedition-0.2.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/.github/workflows/release.yml` & `uedition-0.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/.github/workflows/tests.yml` & `uedition-0.2.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/tests/conftest.py` & `uedition-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/tests/test_build.py` & `uedition-0.2.1/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/tests/test_check.py` & `uedition-0.2.1/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/tests/test_settings.py` & `uedition-0.2.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/tests/fixtures/missing_files/references.bib` & `uedition-0.2.1/tests/fixtures/missing_files/references.bib`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/tests/fixtures/missing_files/en/_config.yml` & `uedition-0.2.1/tests/fixtures/missing_files/en/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/tests/fixtures/multilang/references.bib` & `uedition-0.2.1/tests/fixtures/multilang/references.bib`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/tests/fixtures/multilang/de/_config.yml` & `uedition-0.2.1/tests/fixtures/multilang/de/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/tests/fixtures/multilang/en/_config.yml` & `uedition-0.2.1/tests/fixtures/multilang/en/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/uedition/settings.py` & `uedition-0.2.1/uedition/settings.py`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/uedition/cli/__init__.py` & `uedition-0.2.1/uedition/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/uedition/cli/check.py` & `uedition-0.2.1/uedition/cli/check.py`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/uedition/cli/serve.py` & `uedition-0.2.1/uedition/cli/serve.py`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/uedition/ext/config.py` & `uedition-0.2.1/uedition/ext/config.py`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/uedition/ext/tei.py` & `uedition-0.2.1/uedition/ext/tei.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         # If there is text after this XML node and we are adding all text, then add text content to the parent
         if node.tail and not text_only_in_leaf_nodes:
             parent.append(nodes.Text(node.tail))
 
     def _wrap_sections(self: 'TEIParser', section: nodes.Element, tmp: nodes.Element) -> None:
         """Ensure that sections are correctly wrapped."""
         section_stack = [(0, section)]
-        for node in tmp.findall():
+        for node in tmp.children:
             if isinstance(node, TeiElement) and node.attributes['html_tag'] in ['h1', 'h2', 'h3', 'h4', 'h5', 'h6']:
                 section_level = int(node.attributes['html_tag'][1])
                 while section_level <= section_stack[-1][0]:
                     section_stack.pop()
                 new_section = nodes.section(ids=[nodes.make_id(node.astext())])
                 title = nodes.title()
                 title.children = node.children
```

### Comparing `uedition-0.2.0/LICENSE.txt` & `uedition-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/README.md` & `uedition-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/pyproject.toml` & `uedition-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uedition-0.2.0/PKG-INFO` & `uedition-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uEdition
-Version: 0.2.0
+Version: 0.2.1
 Project-URL: Documentation, https://github.com/unknown/uedition#readme
 Project-URL: Issues, https://github.com/unknown/uedition/issues
 Project-URL: Source, https://github.com/unknown/uedition
 Author-email: Mark Hall <mark.hall@work.room3b.eu>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

