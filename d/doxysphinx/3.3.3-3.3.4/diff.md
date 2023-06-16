# Comparing `tmp/doxysphinx-3.3.3.tar.gz` & `tmp/doxysphinx-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doxysphinx-3.3.3.tar", max compression
+gzip compressed data, was "doxysphinx-3.3.4.tar", max compression
```

## Comparing `doxysphinx-3.3.3.tar` & `doxysphinx-3.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1068 2023-04-27 15:36:40.127392 doxysphinx-3.3.3/LICENSE
--rw-r--r--   0        0        0     1078 2023-04-27 15:36:40.127392 doxysphinx-3.3.3/LICENSE.md
--rw-r--r--   0        0        0     2602 2023-04-27 15:36:40.127392 doxysphinx-3.3.3/README.md
--rw-r--r--   0        0        0      926 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/__init__.py
--rw-r--r--   0        0        0      608 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/__main__.py
--rw-r--r--   0        0        0     8173 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/cli.py
--rw-r--r--   0        0        0    12644 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/doxygen.py
--rw-r--r--   0        0        0    21980 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/html_parser.py
--rw-r--r--   0        0        0     9102 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/process.py
--rw-r--r--   0        0        0     5925 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/resources/custom.scss
--rw-r--r--   0        0        0        0 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/resources/toc_template.html.j2
--rw-r--r--   0        0        0    11645 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/resources.py
--rw-r--r--   0        0        0     2943 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/sphinx.py
--rw-r--r--   0        0        0    11504 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/toc.py
--rw-r--r--   0        0        0      527 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/utils/__init__.py
--rw-r--r--   0        0        0     2282 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/utils/contexts.py
--rw-r--r--   0        0        0     1156 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/utils/exceptions.py
--rw-r--r--   0        0        0     6235 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/utils/files.py
--rw-r--r--   0        0        0     1757 2023-04-27 15:36:40.143393 doxysphinx-3.3.3/doxysphinx/utils/iterators.py
--rw-r--r--   0        0        0     1431 2023-04-27 15:36:40.147393 doxysphinx-3.3.3/doxysphinx/utils/pathlib_fix.py
--rw-r--r--   0        0        0      924 2023-04-27 15:36:40.147393 doxysphinx-3.3.3/doxysphinx/utils/rst.py
--rw-r--r--   0        0        0    12187 2023-04-27 15:36:40.147393 doxysphinx-3.3.3/doxysphinx/writer.py
--rw-r--r--   0        0        0     4193 2023-04-27 15:36:40.147393 doxysphinx-3.3.3/pyproject.toml
--rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 doxysphinx-3.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-16 08:57:34.224739 doxysphinx-3.3.4/LICENSE
+-rw-r--r--   0        0        0     1078 2023-06-16 08:57:34.224739 doxysphinx-3.3.4/LICENSE.md
+-rw-r--r--   0        0        0     2602 2023-06-16 08:57:34.224739 doxysphinx-3.3.4/README.md
+-rw-r--r--   0        0        0      926 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/__init__.py
+-rw-r--r--   0        0        0      608 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/__main__.py
+-rw-r--r--   0        0        0     8173 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/cli.py
+-rw-r--r--   0        0        0    12644 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/doxygen.py
+-rw-r--r--   0        0        0    21980 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/html_parser.py
+-rw-r--r--   0        0        0     9102 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/process.py
+-rw-r--r--   0        0        0     5925 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/resources/custom.scss
+-rw-r--r--   0        0        0        0 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/resources/toc_template.html.j2
+-rw-r--r--   0        0        0    11663 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/resources.py
+-rw-r--r--   0        0        0     2943 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/sphinx.py
+-rw-r--r--   0        0        0    11504 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/toc.py
+-rw-r--r--   0        0        0      527 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/utils/__init__.py
+-rw-r--r--   0        0        0     2282 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/utils/contexts.py
+-rw-r--r--   0        0        0     1156 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/utils/exceptions.py
+-rw-r--r--   0        0        0     6235 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/utils/files.py
+-rw-r--r--   0        0        0     1757 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/utils/iterators.py
+-rw-r--r--   0        0        0     1431 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/utils/pathlib_fix.py
+-rw-r--r--   0        0        0      924 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/utils/rst.py
+-rw-r--r--   0        0        0    12187 2023-06-16 08:57:34.240739 doxysphinx-3.3.4/doxysphinx/writer.py
+-rw-r--r--   0        0        0     4193 2023-06-16 08:57:34.244739 doxysphinx-3.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 doxysphinx-3.3.4/PKG-INFO
```

### Comparing `doxysphinx-3.3.3/LICENSE` & `doxysphinx-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/LICENSE.md` & `doxysphinx-3.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/README.md` & `doxysphinx-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/__init__.py` & `doxysphinx-3.3.4/doxysphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/__main__.py` & `doxysphinx-3.3.4/doxysphinx/__main__.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/cli.py` & `doxysphinx-3.3.4/doxysphinx/cli.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/doxygen.py` & `doxysphinx-3.3.4/doxysphinx/doxygen.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/html_parser.py` & `doxysphinx-3.3.4/doxysphinx/html_parser.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/process.py` & `doxysphinx-3.3.4/doxysphinx/process.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/resources/custom.scss` & `doxysphinx-3.3.4/doxysphinx/resources/custom.scss`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/resources.py` & `doxysphinx-3.3.4/doxysphinx/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
         )
 
         # the sass compiler does also scope the html element (where typically css variables are
         # stored). We need to remove that scoping again because it will only work if it's in global scope.
         compiled_css = compiled_css.replace(f"{self._selector} html {{", "html {")
 
         # write stylesheet
-        target.write_text(compiled_css)
+        target.write_text(compiled_css, encoding="UTF-8")
 
         self._logger.debug(
             f"scoped original stylesheet '{stylesheet}' to selector '{self._selector}' in target '{target}'."
         )
         return target
 
     @staticmethod
```

### Comparing `doxysphinx-3.3.3/doxysphinx/sphinx.py` & `doxysphinx-3.3.4/doxysphinx/sphinx.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/toc.py` & `doxysphinx-3.3.4/doxysphinx/toc.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/utils/__init__.py` & `doxysphinx-3.3.4/doxysphinx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/utils/contexts.py` & `doxysphinx-3.3.4/doxysphinx/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/utils/exceptions.py` & `doxysphinx-3.3.4/doxysphinx/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/utils/files.py` & `doxysphinx-3.3.4/doxysphinx/utils/files.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/utils/iterators.py` & `doxysphinx-3.3.4/doxysphinx/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/utils/pathlib_fix.py` & `doxysphinx-3.3.4/doxysphinx/utils/pathlib_fix.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/utils/rst.py` & `doxysphinx-3.3.4/doxysphinx/utils/rst.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/doxysphinx/writer.py` & `doxysphinx-3.3.4/doxysphinx/writer.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.3/pyproject.toml` & `doxysphinx-3.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ##
 ##  Author(s):
 ##  - Markus Braun, :em engineering methods AG (contracted by Robert Bosch GmbH)
 ## =====================================================================================
 
 [tool.poetry]
 name = "doxysphinx"
-version = "3.3.3"
+version = "3.3.4"
 description = "Integrates doxygen html documentation with sphinx."
 authors = [
     "Nirmal Sasidharan <nirmal.sasidharan@de.bosch.com>",
     "Markus Braun <markus.braun@em.ag>",
     "Aniket Salve <aniketdilip.salve@bosch.com>",
 ]
 maintainers = ["Nirmal Sasidharan <nirmal.sasidharan@de.bosch.com>"]
@@ -80,15 +80,15 @@
 commitizen = "^2.42.1"
 
 [tool.poetry.scripts]
 doxysphinx = "doxysphinx.cli:cli"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "3.3.3"
+version = "3.3.4"
 tag_format = "v$version"
 version_files = ["pyproject.toml:^version"]
 bump_message = """chore(release): release $current_version → $new_version by commitizen [skip-ci]
 
 Signed-off-by: github-actions <actions@github.com>
 """
```

### Comparing `doxysphinx-3.3.3/PKG-INFO` & `doxysphinx-3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doxysphinx
-Version: 3.3.3
+Version: 3.3.4
 Summary: Integrates doxygen html documentation with sphinx.
 Home-page: https://github.com/boschglobal/doxysphinx
 License: MIT
 Keywords: DaC,docs-as-code,doxygen,sphinx
 Author: Nirmal Sasidharan
 Author-email: nirmal.sasidharan@de.bosch.com
 Maintainer: Nirmal Sasidharan
```

