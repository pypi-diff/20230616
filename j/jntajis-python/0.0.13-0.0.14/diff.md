# Comparing `tmp/jntajis-python-0.0.13.tar.gz` & `tmp/jntajis-python-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jntajis-python-0.0.13.tar", last modified: Mon Sep  6 04:52:38 2021, max compression
+gzip compressed data, was "jntajis-python-0.0.14.tar", last modified: Fri Jun 16 13:55:22 2023, max compression
```

## Comparing `jntajis-python-0.0.13.tar` & `jntajis-python-0.0.14.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 moriyoshi   (501) staff       (20)        0 2021-09-06 04:52:38.868540 jntajis-python-0.0.13/
--rw-r--r--   0 moriyoshi   (501) staff       (20)       25 2021-08-22 09:00:40.000000 jntajis-python-0.0.13/.black.ini
--rw-r--r--   0 moriyoshi   (501) staff       (20)       35 2021-08-22 09:02:01.000000 jntajis-python-0.0.13/.flake8
-drwxr-xr-x   0 moriyoshi   (501) staff       (20)        0 2021-09-06 04:52:38.771911 jntajis-python-0.0.13/.github/
-drwxr-xr-x   0 moriyoshi   (501) staff       (20)        0 2021-09-06 04:52:38.779479 jntajis-python-0.0.13/.github/workflows/
--rw-r--r--   0 moriyoshi   (501) staff       (20)      645 2021-09-05 18:31:23.000000 jntajis-python-0.0.13/.github/workflows/wheels.yml
--rw-r--r--   0 moriyoshi   (501) staff       (20)     2194 2021-08-22 09:01:45.000000 jntajis-python-0.0.13/.gitignore
--rw-r--r--   0 moriyoshi   (501) staff       (20)      165 2021-08-23 14:40:53.000000 jntajis-python-0.0.13/.readthedocs.yaml
--rw-r--r--   0 moriyoshi   (501) staff       (20)     1494 2021-08-29 12:09:20.000000 jntajis-python-0.0.13/LICENSE
--rw-r--r--   0 moriyoshi   (501) staff       (20)      231 2021-08-23 14:30:34.000000 jntajis-python-0.0.13/MANIFEST.in
--rw-r--r--   0 moriyoshi   (501) staff       (20)      897 2021-08-23 03:12:30.000000 jntajis-python-0.0.13/Makefile
--rw-r--r--   0 moriyoshi   (501) staff       (20)     6282 2021-09-06 04:52:38.868788 jntajis-python-0.0.13/PKG-INFO
--rw-r--r--   0 moriyoshi   (501) staff       (20)     4766 2021-09-05 19:50:20.000000 jntajis-python-0.0.13/README.md
-drwxr-xr-x   0 moriyoshi   (501) staff       (20)        0 2021-09-06 04:52:38.790578 jntajis-python-0.0.13/docs/
--rw-r--r--   0 moriyoshi   (501) staff       (20)       11 2021-08-23 14:31:01.000000 jntajis-python-0.0.13/docs/.gitignore
--rw-r--r--   0 moriyoshi   (501) staff       (20)      638 2021-08-23 11:49:18.000000 jntajis-python-0.0.13/docs/Makefile
--rw-r--r--   0 moriyoshi   (501) staff       (20)      799 2021-08-23 11:49:18.000000 jntajis-python-0.0.13/docs/make.bat
-drwxr-xr-x   0 moriyoshi   (501) staff       (20)        0 2021-09-06 04:52:38.793464 jntajis-python-0.0.13/docs/source/
-drwxr-xr-x   0 moriyoshi   (501) staff       (20)        0 2021-09-06 04:52:38.772491 jntajis-python-0.0.13/docs/source/_static/
-drwxr-xr-x   0 moriyoshi   (501) staff       (20)        0 2021-09-06 04:52:38.795019 jntajis-python-0.0.13/docs/source/_static/images/
--rw-r--r--   0 moriyoshi   (501) staff       (20)    17147 2021-08-29 11:08:03.000000 jntajis-python-0.0.13/docs/source/_static/images/mj-jnta.svg
--rw-r--r--   0 moriyoshi   (501) staff       (20)    15907 2021-08-29 04:27:28.000000 jntajis-python-0.0.13/docs/source/_static/images/relationships-character-mappings.svg
--rw-r--r--   0 moriyoshi   (501) staff       (20)     5554 2021-09-05 20:13:14.000000 jntajis-python-0.0.13/docs/source/api.rst
--rw-r--r--   0 moriyoshi   (501) staff       (20)     1979 2021-08-23 14:28:43.000000 jntajis-python-0.0.13/docs/source/conf.py
--rw-r--r--   0 moriyoshi   (501) staff       (20)     4678 2021-09-05 18:30:10.000000 jntajis-python-0.0.13/docs/source/index.rst
--rw-r--r--   0 moriyoshi   (501) staff       (20)     2589 2021-08-29 22:56:44.000000 jntajis-python-0.0.13/docs/source/license.rst
--rw-r--r--   0 moriyoshi   (501) staff       (20)     1229 2021-09-06 04:52:38.869559 jntajis-python-0.0.13/setup.cfg
--rw-r--r--   0 moriyoshi   (501) staff       (20)      250 2021-08-23 11:46:24.000000 jntajis-python-0.0.13/setup.py
-drwxr-xr-x   0 moriyoshi   (501) staff       (20)        0 2021-09-06 04:52:38.773226 jntajis-python-0.0.13/src/
-drwxr-xr-x   0 moriyoshi   (501) staff       (20)        0 2021-09-06 04:52:38.861486 jntajis-python-0.0.13/src/jntajis/
--rw-r--r--   0 moriyoshi   (501) staff       (20)     3503 2021-08-25 10:52:21.000000 jntajis-python-0.0.13/src/jntajis/__init__.py
--rw-r--r--   0 moriyoshi   (501) staff       (20)   559569 2021-09-06 04:39:19.000000 jntajis-python-0.0.13/src/jntajis/_jntajis.c
--rw-r--r--   0 moriyoshi   (501) staff       (20) 13715812 2021-09-05 18:40:33.000000 jntajis-python-0.0.13/src/jntajis/_jntajis.h
--rw-r--r--   0 moriyoshi   (501) staff       (20)      652 2021-09-05 20:14:35.000000 jntajis-python-0.0.13/src/jntajis/_jntajis.pyi
--rw-r--r--   0 moriyoshi   (501) staff       (20)    34661 2021-09-06 04:36:27.000000 jntajis-python-0.0.13/src/jntajis/_jntajis.pyx
--rw-r--r--   0 moriyoshi   (501) staff       (20)    24449 2021-09-05 18:39:59.000000 jntajis-python-0.0.13/src/jntajis/gen.py
--rw-r--r--   0 moriyoshi   (501) staff       (20)        0 2021-08-20 05:17:02.000000 jntajis-python-0.0.13/src/jntajis/py.typed
-drwxr-xr-x   0 moriyoshi   (501) staff       (20)        0 2021-09-06 04:52:38.862490 jntajis-python-0.0.13/src/jntajis/tests/
--rw-r--r--   0 moriyoshi   (501) staff       (20)     6721 2021-09-05 18:24:03.000000 jntajis-python-0.0.13/src/jntajis/tests/test_encoder.py
--rw-r--r--   0 moriyoshi   (501) staff       (20)     4745 2021-09-06 04:28:48.000000 jntajis-python-0.0.13/src/jntajis/tests/test_mj_translit.py
-drwxr-xr-x   0 moriyoshi   (501) staff       (20)        0 2021-09-06 04:52:38.865013 jntajis-python-0.0.13/src/jntajis/xlsx_parser/
--rw-r--r--   0 moriyoshi   (501) staff       (20)       44 2021-08-22 09:04:06.000000 jntajis-python-0.0.13/src/jntajis/xlsx_parser/__init__.py
--rw-r--r--   0 moriyoshi   (501) staff       (20)    16627 2021-08-22 09:18:48.000000 jntajis-python-0.0.13/src/jntajis/xlsx_parser/parser.py
--rw-r--r--   0 moriyoshi   (501) staff       (20)    11629 2021-08-23 05:42:34.000000 jntajis-python-0.0.13/src/jntajis/xlsx_parser/xmlutils.py
-drwxr-xr-x   0 moriyoshi   (501) staff       (20)        0 2021-09-06 04:52:38.868104 jntajis-python-0.0.13/src/jntajis_python.egg-info/
--rw-r--r--   0 moriyoshi   (501) staff       (20)     6282 2021-09-06 04:52:38.000000 jntajis-python-0.0.13/src/jntajis_python.egg-info/PKG-INFO
--rw-r--r--   0 moriyoshi   (501) staff       (20)      955 2021-09-06 04:52:38.000000 jntajis-python-0.0.13/src/jntajis_python.egg-info/SOURCES.txt
--rw-r--r--   0 moriyoshi   (501) staff       (20)        1 2021-09-06 04:52:38.000000 jntajis-python-0.0.13/src/jntajis_python.egg-info/dependency_links.txt
--rw-r--r--   0 moriyoshi   (501) staff       (20)        1 2021-08-18 12:40:45.000000 jntajis-python-0.0.13/src/jntajis_python.egg-info/not-zip-safe
--rw-r--r--   0 moriyoshi   (501) staff       (20)      109 2021-09-06 04:52:38.000000 jntajis-python-0.0.13/src/jntajis_python.egg-info/requires.txt
--rw-r--r--   0 moriyoshi   (501) staff       (20)        8 2021-09-06 04:52:38.000000 jntajis-python-0.0.13/src/jntajis_python.egg-info/top_level.txt
+drwxr-xr-x   0 moriyoshi  (1000) moriyoshi  (1000)        0 2023-06-16 13:55:22.723109 jntajis-python-0.0.14/
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)       25 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/.black.ini
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)       35 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/.flake8
+drwxr-xr-x   0 moriyoshi  (1000) moriyoshi  (1000)        0 2023-06-16 13:55:22.703109 jntajis-python-0.0.14/.github/
+drwxr-xr-x   0 moriyoshi  (1000) moriyoshi  (1000)        0 2023-06-16 13:55:22.713109 jntajis-python-0.0.14/.github/workflows/
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)      312 2023-06-16 13:43:50.000000 jntajis-python-0.0.14/.github/workflows/main.yml
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)      529 2023-06-16 13:40:38.000000 jntajis-python-0.0.14/.github/workflows/tests.yml
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)      709 2023-06-16 13:40:38.000000 jntajis-python-0.0.14/.github/workflows/wheels.yml
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     2194 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/.gitignore
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)      165 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/.readthedocs.yaml
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     1494 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/LICENSE
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)      231 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/MANIFEST.in
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)      897 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/Makefile
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     5667 2023-06-16 13:55:22.723109 jntajis-python-0.0.14/PKG-INFO
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     4766 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/README.md
+drwxr-xr-x   0 moriyoshi  (1000) moriyoshi  (1000)        0 2023-06-16 13:55:22.713109 jntajis-python-0.0.14/docs/
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)       11 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/docs/.gitignore
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)      638 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/docs/Makefile
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)      799 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/docs/make.bat
+drwxr-xr-x   0 moriyoshi  (1000) moriyoshi  (1000)        0 2023-06-16 13:55:22.713109 jntajis-python-0.0.14/docs/source/
+drwxr-xr-x   0 moriyoshi  (1000) moriyoshi  (1000)        0 2023-06-16 13:55:22.703109 jntajis-python-0.0.14/docs/source/_static/
+drwxr-xr-x   0 moriyoshi  (1000) moriyoshi  (1000)        0 2023-06-16 13:55:22.713109 jntajis-python-0.0.14/docs/source/_static/images/
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)    17147 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/docs/source/_static/images/mj-jnta.svg
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)    15907 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/docs/source/_static/images/relationships-character-mappings.svg
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     5554 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/docs/source/api.rst
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     1979 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/docs/source/conf.py
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     4678 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/docs/source/index.rst
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     2589 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/docs/source/license.rst
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     1295 2023-06-16 13:55:22.723109 jntajis-python-0.0.14/setup.cfg
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)      250 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/setup.py
+drwxr-xr-x   0 moriyoshi  (1000) moriyoshi  (1000)        0 2023-06-16 13:55:22.713109 jntajis-python-0.0.14/src/
+drwxr-xr-x   0 moriyoshi  (1000) moriyoshi  (1000)        0 2023-06-16 13:55:22.723109 jntajis-python-0.0.14/src/jntajis/
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     3503 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/src/jntajis/__init__.py
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)   568829 2023-06-16 05:33:18.000000 jntajis-python-0.0.14/src/jntajis/_jntajis.c
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000) 13715812 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/src/jntajis/_jntajis.h
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)      658 2023-06-16 05:34:34.000000 jntajis-python-0.0.14/src/jntajis/_jntajis.pyi
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)    34661 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/src/jntajis/_jntajis.pyx
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)    24448 2023-06-16 05:34:34.000000 jntajis-python-0.0.14/src/jntajis/gen.py
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)        0 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/src/jntajis/py.typed
+drwxr-xr-x   0 moriyoshi  (1000) moriyoshi  (1000)        0 2023-06-16 13:55:22.723109 jntajis-python-0.0.14/src/jntajis/tests/
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     6721 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/src/jntajis/tests/test_encoder.py
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     4773 2023-06-16 05:34:34.000000 jntajis-python-0.0.14/src/jntajis/tests/test_mj_translit.py
+drwxr-xr-x   0 moriyoshi  (1000) moriyoshi  (1000)        0 2023-06-16 13:55:22.723109 jntajis-python-0.0.14/src/jntajis/xlsx_parser/
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)       44 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/src/jntajis/xlsx_parser/__init__.py
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)    16570 2023-06-16 05:45:54.000000 jntajis-python-0.0.14/src/jntajis/xlsx_parser/parser.py
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)    11629 2023-06-15 23:50:57.000000 jntajis-python-0.0.14/src/jntajis/xlsx_parser/xmlutils.py
+drwxr-xr-x   0 moriyoshi  (1000) moriyoshi  (1000)        0 2023-06-16 13:55:22.723109 jntajis-python-0.0.14/src/jntajis_python.egg-info/
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     5667 2023-06-16 13:55:22.000000 jntajis-python-0.0.14/src/jntajis_python.egg-info/PKG-INFO
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)     1010 2023-06-16 13:55:22.000000 jntajis-python-0.0.14/src/jntajis_python.egg-info/SOURCES.txt
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)        1 2023-06-16 13:55:22.000000 jntajis-python-0.0.14/src/jntajis_python.egg-info/dependency_links.txt
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)        1 2023-06-16 05:19:41.000000 jntajis-python-0.0.14/src/jntajis_python.egg-info/not-zip-safe
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)       97 2023-06-16 13:55:22.000000 jntajis-python-0.0.14/src/jntajis_python.egg-info/requires.txt
+-rw-r--r--   0 moriyoshi  (1000) moriyoshi  (1000)        8 2023-06-16 13:55:22.000000 jntajis-python-0.0.14/src/jntajis_python.egg-info/top_level.txt
```

### Comparing `jntajis-python-0.0.13/.gitignore` & `jntajis-python-0.0.14/.gitignore`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/LICENSE` & `jntajis-python-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/Makefile` & `jntajis-python-0.0.14/Makefile`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/PKG-INFO` & `jntajis-python-0.0.14/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,115 @@
 Metadata-Version: 2.1
 Name: jntajis-python
-Version: 0.0.13
+Version: 0.0.14
 Summary: A fast character conversion and transliteration library based on the scheme defined for Japan National Tax Agency's corporate number system.
 Home-page: https://github.com/opencollector/jntajis-python
 Author: Open Collector, inc.
 Author-email: <info@opencollector.co.jp>
 License: BSD License
-Description: # jntajis-python
-        
-        Documentation: https://jntajis-python.readthedocs.io/
-        
-        ## What's JNTAJIS-python?
-        
-        JNTAJIS-python is a transliteration library, specifically designed for dealing with three different character sets; JIS X 0208, JIS X 0213, and Unicode.
-        
-        ```python
-        import jntajis
-        
-        print(jntajis.mj_shrink_candidates("髙島屋", jntajis.MJShrinkSchemeCombo.JIS_INCORPORATION_UCS_UNIFICATION_RULE))  # outputs ["高島屋", "髙島屋"]
-        print(jntajis.jnta_shrink_translit("麴町"))  # outputs "麹町"
-        ```
-        
-        To that end, this library refers to three different character tables; MJ character table, MJ shrink conversion map, and NTA shrink conversion map.
-        
-        The MJ character table (*MJ文字一覧表*) defines a vast set of kanji (*漢字*) characters used in information processing of Japanese texts initially developed by Information-technology Promotion Agency.
-        
-        The MJ shrink conversion map (*MJ縮退マップ*) was also developed alongside for the sake of interoperability between MJ-aware systems and systems based on Unicode, which is used to transliterate complex, less-frequently-used character variants to commonly-used, more-used ones.
-        
-        The NTA shrink conversion map (*国税庁JIS縮退マップ*) was developed by Japan National Tax Agency to canonicalize user inputs for its corporation number search service provided as a public web API.  This maps JIS level 3 and 4 characters to JIS level 1 and 2 characters (i.e. characters defined in JIS X 0208.)  Note that not all level 3 and level 4 characters have level 1 and 2 counterparts.  Also note that some of level 3 and 4 characters don't map to a single character one by each.  Instead, they map to sequences of two or more characters.
-        
-        The table below shows some examples of transliteration by the MJ character table suite and NTA shrink conversion map.
-        
-        | Glyph | MJ code | Unicode | JIS X 0213 | Glyph\* | MJ code\* | JIS X 0208\* | Transliterator |
-        | ----- | ------- | ------- | ---------- | ------ | ------- | ---------- | -------------- | 
-        | ![棃](https://moji.or.jp/mojikibansearch/img/MJ/MJ014031.png) | MJ014031 | U+68C3 | 2-14-90 | ![梨](https://moji.or.jp/mojikibansearch/img/MJ/MJ014007.png) | MJ014007 | 1-45-92 | MJ / JNTA |
-        | ![﨑](https://moji.or.jp/mojikibansearch/img/MJ/MJ030196.png) | MJ030196 | U+FA11 | 1-47-82 | ![崎](https://moji.or.jp/mojikibansearch/img/MJ/MJ010541.png) | MJ010541 | 1-26-74 | MJ / JNTA |
-        | ![髙](https://moji.or.jp/mojikibansearch/img/MJ/MJ028902.png) | MJ028902 | U+9AD9 | N/A | ![高](https://moji.or.jp/mojikibansearch/img/MJ/MJ028901.png) | MJ028901 | 1-25-66 | MJ |
-        
-        The conversion schematics is shown below:
-        
-        ![](https://github.com/opencollector/jntajis-python/raw/main/docs/source/_static/images/mj-jnta.svg)
-        
-        * JNTA transliteration
-        
-            As every JIS X 0213 characters maps to its Unicode counterpart, the conversion is done only with the single JNTA character mappings table.
-        
-        * MJ transliteration
-        
-            Transliteration is done in two phases:
-        
-            1. Conversion from Unicode to MJ character mappings.
-        
-                While not all characters in the MJ characters table map to Unicode, each MJ code has different shrink mappings. Because of this, the transliterator tries to convert Unicode codepoints to MJ codes first.
-        
-            2. Transliteration by MJ shrink mappings.
-        
-                The transliteration result as a string isn't necessarily single as some MJ codes have more than one transliteration candidate. This happens because a) a Unicode codepoint may map to multiple MJ codes and b) multiple transliteration schemes are designated to a single MJ code.
-        
-        
-        Relationship between Unicode, MJ character mappings, JIS X 0213, and JIS X 0208 can be depicted as follows:
-        
-        ![](https://github.com/opencollector/jntajis-python/raw/main/docs/source/_static/images/relationships-character-mappings.svg)
-        
-        ## License
-        
-        The source code except `src/jntajis/_jntajis.h` is published under the BSD 3-clause license.
-        
-        `src/jntajis/_jntajis.h` contains the data from the following entities:
-        
-        * JIS shrink conversion mappings (国税庁: JIS縮退マップ)
-        
-          Publisher: National Tax Agency
-        
-          Author: National Tax Agency
-        
-          Source: https://www.houjin-bangou.nta.go.jp/download/
-        
-          License: CC BY 4.0
-        
-        * MJ character table (文字情報技術促進協議会: MJ文字一覧表)
-        
-          Publisher: Character Information Technology Promotion Council (CITPC)
-        
-          Author: Information-technology Promotion Agency (IPA)
-        
-          Source: https://moji.or.jp/mojikiban/mjlist/
-        
-          License: CC BY-SA 2.1 JP
-        
-        * MJ shrink conversion mappings (文字情報技術促進協議会: MJ縮退マップ)
-        
-          Publisher: Character Information Technology Promotion Council (CITPC)
-        
-          Author: Information-technology Promotion Agency (IPA)
-        
-          Source: https://moji.or.jp/mojikiban/map/ 
-        
-          License: CC BY-SA 2.1 JP
-        
 Keywords: Unicode,JIS,encoding,conversion,transliteration,Japanese
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: Filters
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# jntajis-python
+
+Documentation: https://jntajis-python.readthedocs.io/
+
+## What's JNTAJIS-python?
+
+JNTAJIS-python is a transliteration library, specifically designed for dealing with three different character sets; JIS X 0208, JIS X 0213, and Unicode.
+
+```python
+import jntajis
+
+print(jntajis.mj_shrink_candidates("髙島屋", jntajis.MJShrinkSchemeCombo.JIS_INCORPORATION_UCS_UNIFICATION_RULE))  # outputs ["高島屋", "髙島屋"]
+print(jntajis.jnta_shrink_translit("麴町"))  # outputs "麹町"
+```
+
+To that end, this library refers to three different character tables; MJ character table, MJ shrink conversion map, and NTA shrink conversion map.
+
+The MJ character table (*MJ文字一覧表*) defines a vast set of kanji (*漢字*) characters used in information processing of Japanese texts initially developed by Information-technology Promotion Agency.
+
+The MJ shrink conversion map (*MJ縮退マップ*) was also developed alongside for the sake of interoperability between MJ-aware systems and systems based on Unicode, which is used to transliterate complex, less-frequently-used character variants to commonly-used, more-used ones.
+
+The NTA shrink conversion map (*国税庁JIS縮退マップ*) was developed by Japan National Tax Agency to canonicalize user inputs for its corporation number search service provided as a public web API.  This maps JIS level 3 and 4 characters to JIS level 1 and 2 characters (i.e. characters defined in JIS X 0208.)  Note that not all level 3 and level 4 characters have level 1 and 2 counterparts.  Also note that some of level 3 and 4 characters don't map to a single character one by each.  Instead, they map to sequences of two or more characters.
+
+The table below shows some examples of transliteration by the MJ character table suite and NTA shrink conversion map.
+
+| Glyph | MJ code | Unicode | JIS X 0213 | Glyph\* | MJ code\* | JIS X 0208\* | Transliterator |
+| ----- | ------- | ------- | ---------- | ------ | ------- | ---------- | -------------- | 
+| ![棃](https://moji.or.jp/mojikibansearch/img/MJ/MJ014031.png) | MJ014031 | U+68C3 | 2-14-90 | ![梨](https://moji.or.jp/mojikibansearch/img/MJ/MJ014007.png) | MJ014007 | 1-45-92 | MJ / JNTA |
+| ![﨑](https://moji.or.jp/mojikibansearch/img/MJ/MJ030196.png) | MJ030196 | U+FA11 | 1-47-82 | ![崎](https://moji.or.jp/mojikibansearch/img/MJ/MJ010541.png) | MJ010541 | 1-26-74 | MJ / JNTA |
+| ![髙](https://moji.or.jp/mojikibansearch/img/MJ/MJ028902.png) | MJ028902 | U+9AD9 | N/A | ![高](https://moji.or.jp/mojikibansearch/img/MJ/MJ028901.png) | MJ028901 | 1-25-66 | MJ |
+
+The conversion schematics is shown below:
+
+![](https://github.com/opencollector/jntajis-python/raw/main/docs/source/_static/images/mj-jnta.svg)
+
+* JNTA transliteration
+
+    As every JIS X 0213 characters maps to its Unicode counterpart, the conversion is done only with the single JNTA character mappings table.
+
+* MJ transliteration
+
+    Transliteration is done in two phases:
+
+    1. Conversion from Unicode to MJ character mappings.
+
+        While not all characters in the MJ characters table map to Unicode, each MJ code has different shrink mappings. Because of this, the transliterator tries to convert Unicode codepoints to MJ codes first.
+
+    2. Transliteration by MJ shrink mappings.
+
+        The transliteration result as a string isn't necessarily single as some MJ codes have more than one transliteration candidate. This happens because a) a Unicode codepoint may map to multiple MJ codes and b) multiple transliteration schemes are designated to a single MJ code.
+
+
+Relationship between Unicode, MJ character mappings, JIS X 0213, and JIS X 0208 can be depicted as follows:
+
+![](https://github.com/opencollector/jntajis-python/raw/main/docs/source/_static/images/relationships-character-mappings.svg)
+
+## License
+
+The source code except `src/jntajis/_jntajis.h` is published under the BSD 3-clause license.
+
+`src/jntajis/_jntajis.h` contains the data from the following entities:
+
+* JIS shrink conversion mappings (国税庁: JIS縮退マップ)
+
+  Publisher: National Tax Agency
+
+  Author: National Tax Agency
+
+  Source: https://www.houjin-bangou.nta.go.jp/download/
+
+  License: CC BY 4.0
+
+* MJ character table (文字情報技術促進協議会: MJ文字一覧表)
+
+  Publisher: Character Information Technology Promotion Council (CITPC)
+
+  Author: Information-technology Promotion Agency (IPA)
+
+  Source: https://moji.or.jp/mojikiban/mjlist/
+
+  License: CC BY-SA 2.1 JP
+
+* MJ shrink conversion mappings (文字情報技術促進協議会: MJ縮退マップ)
+
+  Publisher: Character Information Technology Promotion Council (CITPC)
+
+  Author: Information-technology Promotion Agency (IPA)
+
+  Source: https://moji.or.jp/mojikiban/map/ 
+
+  License: CC BY-SA 2.1 JP
+
+
```

### Comparing `jntajis-python-0.0.13/README.md` & `jntajis-python-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/docs/Makefile` & `jntajis-python-0.0.14/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/docs/make.bat` & `jntajis-python-0.0.14/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/docs/source/_static/images/mj-jnta.svg` & `jntajis-python-0.0.14/docs/source/_static/images/mj-jnta.svg`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/docs/source/_static/images/relationships-character-mappings.svg` & `jntajis-python-0.0.14/docs/source/_static/images/relationships-character-mappings.svg`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/docs/source/api.rst` & `jntajis-python-0.0.14/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/docs/source/conf.py` & `jntajis-python-0.0.14/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/docs/source/index.rst` & `jntajis-python-0.0.14/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/docs/source/license.rst` & `jntajis-python-0.0.14/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/setup.cfg` & `jntajis-python-0.0.14/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -9,41 +9,43 @@
 keywords = Unicode, JIS, encoding, conversion, transliteration, Japanese
 license = BSD License
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Text Processing :: Filters
 
 [options]
 zip_safe = False
 include_package_data = True
 python_requires = >= 3.8
 setup_requires = 
 	setuptools>=38.6.0
 	wheel>=0.31.0
 	cython>=0.29.0
-	setuptools-scm>=6.*
+	setuptools-scm>=6
 install_requires = 
 tests_require = 
 	pytest
 packages = find:
 package_dir = 
 	= src
 
 [options.extras_require]
 dev = 
-	black==21.7b0
-	flake8>=3.9.*
-	jinja2>=3.*
+	black>=23.3
+	flake8>=3.9
+	jinja2>=3
 	mypy>=0.910
-	pytest>=6.2.*
-	sphinx>=4.*
-	sphinx-rtd-theme>=0.5.*
+	pytest>=6.2
+	sphinx>=4
+	sphinx-rtd-theme>=0.5
 
 [options.package_data]
 * = 
 	py.typed
 
 [options.packages.find]
 where = src
```

### Comparing `jntajis-python-0.0.13/src/jntajis/__init__.py` & `jntajis-python-0.0.14/src/jntajis/__init__.py`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/src/jntajis/_jntajis.c` & `jntajis-python-0.0.14/src/jntajis/_jntajis.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.24 */
+/* Generated by Cython 0.29.35 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_24"
-#define CYTHON_HEX_VERSION 0x001D18F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -73,26 +74,34 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -122,18 +131,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -145,61 +203,72 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -308,17 +377,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -424,35 +552,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -548,18 +676,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -576,16 +704,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -711,14 +841,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -825,15 +956,15 @@
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
   "src/jntajis/_jntajis.pyx",
   "stringsource",
-  ".eggs/Cython-0.29.24-py3.9-macosx-10.15-x86_64.egg/Cython/Includes/cpython/type.pxd",
+  ".eggs/Cython-0.29.35-py3.7-linux-x86_64.egg/Cython/Includes/cpython/type.pxd",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_7jntajis_8_jntajis_IncrementalEncoder;
 struct __pyx_t_7jntajis_8_jntajis_JNTAJISIncrementalEncoder;
 typedef struct __pyx_t_7jntajis_8_jntajis_JNTAJISIncrementalEncoder __pyx_t_7jntajis_8_jntajis_JNTAJISIncrementalEncoder;
 struct __pyx_t_7jntajis_8_jntajis_JNTAJISIncrementalEncoderContext;
@@ -1066,21 +1197,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -1196,14 +1335,17 @@
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* BuildPyUnicode.proto */
 static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
                                                 int prepend_sign, char padding_char);
 
+/* IncludeStringH.proto */
+#include <string.h>
+
 /* CIntToPyUnicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char);
 
 /* PyCFunctionFastCall.proto */
 #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
 #else
@@ -1279,26 +1421,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1350,22 +1492,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
@@ -4556,15 +4706,15 @@
  * 
  *     def encode(self, in_, final):
  *         return JNTAJISIncrementalEncoder_encode(&self._impl, in_, final)             # <<<<<<<<<<<<<<
  * 
  *     def reset(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_in_))||((__pyx_v_in_) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_in_)->tp_name), 0))) __PYX_ERR(0, 436, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_in_))||((__pyx_v_in_) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_in_)->tp_name), 0))) __PYX_ERR(0, 436, __pyx_L1_error)
   __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_final); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 436, __pyx_L1_error)
   __pyx_t_2 = __pyx_f_7jntajis_8_jntajis_JNTAJISIncrementalEncoder_encode((&__pyx_v_self->_impl), ((PyObject*)__pyx_v_in_), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 436, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
@@ -6704,15 +6854,15 @@
     /* "jntajis/_jntajis.pyx":655
  *         if len(<object>t.replacement) == 0:
  *             raise TransliterationError(f"transliteration failed at position {t.pos}")
  *         _PyUnicodeWriter_WriteStr(&t.writer, <object>t.replacement)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    if (!(likely(PyUnicode_CheckExact(((PyObject *)__pyx_v_t->replacement)))||((((PyObject *)__pyx_v_t->replacement)) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(((PyObject *)__pyx_v_t->replacement))->tp_name), 0))) __PYX_ERR(0, 655, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(((PyObject *)__pyx_v_t->replacement)))||((((PyObject *)__pyx_v_t->replacement)) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(((PyObject *)__pyx_v_t->replacement))->tp_name), 0))) __PYX_ERR(0, 655, __pyx_L1_error)
     __pyx_t_2 = ((PyObject *)__pyx_v_t->replacement);
     __Pyx_INCREF(__pyx_t_2);
     _PyUnicodeWriter_WriteStr((&__pyx_v_t->writer), ((PyObject*)__pyx_t_2));
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L3:;
 
@@ -7426,15 +7576,15 @@
  *     return _PyUnicodeWriter_Finish(&t.writer)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = _PyUnicodeWriter_Finish((&__pyx_v_t->writer)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 730, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 730, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 730, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "jntajis/_jntajis.pyx":726
  *     return True
  * 
@@ -11566,20 +11716,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
@@ -11774,15 +11927,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -11847,22 +12000,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -12049,15 +12201,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_jntajis___jntajis) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -12417,15 +12569,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -12592,28 +12744,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -12840,15 +12992,15 @@
         uval = NULL;
         if (uoffset > 0) {
             prepend_sign = !!prepend_sign;
             if (uoffset > prepend_sign) {
                 padding = PyUnicode_FromOrdinal(padding_char);
                 if (likely(padding) && uoffset > prepend_sign + 1) {
                     PyObject *tmp;
-                    PyObject *repeat = PyInt_FromSize_t(uoffset - prepend_sign);
+                    PyObject *repeat = PyInt_FromSsize_t(uoffset - prepend_sign);
                     if (unlikely(!repeat)) goto done_or_error;
                     tmp = PyNumber_Multiply(padding, repeat);
                     Py_DECREF(repeat);
                     Py_DECREF(padding);
                     padding = tmp;
                 }
                 if (unlikely(!padding)) goto done_or_error;
@@ -12874,25 +13026,14 @@
         Py_XDECREF(sign);
     }
 #endif
     return uval;
 }
 
 /* CIntToPyUnicode */
-#ifdef _MSC_VER
-    #ifndef _MSC_STDINT_H_
-        #if _MSC_VER < 1300
-           typedef unsigned short    uint16_t;
-        #else
-           typedef unsigned __int16  uint16_t;
-        #endif
-    #endif
-#else
-   #include <stdint.h>
-#endif
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char) {
     char digits[sizeof(int)*3+2];
     char *dpos, *end = digits + sizeof(int)*3+2;
     const char *hex_digits = DIGITS_HEX;
     Py_ssize_t length, ulength;
     int prepend_sign, last_one_off;
     int remaining;
@@ -12915,22 +13056,22 @@
     do {
         int digit_pos;
         switch (format_char) {
         case 'o':
             digit_pos = abs((int)(remaining % (8*8)));
             remaining = (int) (remaining / (8*8));
             dpos -= 2;
-            *(uint16_t*)dpos = ((const uint16_t*)DIGIT_PAIRS_8)[digit_pos];
+            memcpy(dpos, DIGIT_PAIRS_8 + digit_pos * 2, 2);
             last_one_off = (digit_pos < 8);
             break;
         case 'd':
             digit_pos = abs((int)(remaining % (10*10)));
             remaining = (int) (remaining / (10*10));
             dpos -= 2;
-            *(uint16_t*)dpos = ((const uint16_t*)DIGIT_PAIRS_10)[digit_pos];
+            memcpy(dpos, DIGIT_PAIRS_10 + digit_pos * 2, 2);
             last_one_off = (digit_pos < 10);
             break;
         case 'x':
             *(--dpos) = hex_digits[abs((int)(remaining % 16))];
             remaining = (int) (remaining / 16);
             break;
         default:
@@ -13549,25 +13690,14 @@
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
 /* CIntToPyUnicode */
-#ifdef _MSC_VER
-    #ifndef _MSC_STDINT_H_
-        #if _MSC_VER < 1300
-           typedef unsigned short    uint16_t;
-        #else
-           typedef unsigned __int16  uint16_t;
-        #endif
-    #endif
-#else
-   #include <stdint.h>
-#endif
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_Py_ssize_t(Py_ssize_t value, Py_ssize_t width, char padding_char, char format_char) {
     char digits[sizeof(Py_ssize_t)*3+2];
     char *dpos, *end = digits + sizeof(Py_ssize_t)*3+2;
     const char *hex_digits = DIGITS_HEX;
     Py_ssize_t length, ulength;
     int prepend_sign, last_one_off;
     Py_ssize_t remaining;
@@ -13590,22 +13720,22 @@
     do {
         int digit_pos;
         switch (format_char) {
         case 'o':
             digit_pos = abs((int)(remaining % (8*8)));
             remaining = (Py_ssize_t) (remaining / (8*8));
             dpos -= 2;
-            *(uint16_t*)dpos = ((const uint16_t*)DIGIT_PAIRS_8)[digit_pos];
+            memcpy(dpos, DIGIT_PAIRS_8 + digit_pos * 2, 2);
             last_one_off = (digit_pos < 8);
             break;
         case 'd':
             digit_pos = abs((int)(remaining % (10*10)));
             remaining = (Py_ssize_t) (remaining / (10*10));
             dpos -= 2;
-            *(uint16_t*)dpos = ((const uint16_t*)DIGIT_PAIRS_10)[digit_pos];
+            memcpy(dpos, DIGIT_PAIRS_10 + digit_pos * 2, 2);
             last_one_off = (digit_pos < 10);
             break;
         case 'x':
             *(--dpos) = hex_digits[abs((int)(remaining % 16))];
             remaining = (Py_ssize_t) (remaining / 16);
             break;
         default:
@@ -13780,25 +13910,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -13835,71 +13983,91 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -14078,15 +14246,15 @@
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -14108,15 +14276,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -14202,41 +14370,48 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -14247,34 +14422,49 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -14365,15 +14555,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -14561,15 +14751,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -14833,15 +15023,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15071,19 +15261,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -15333,14 +15545,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `jntajis-python-0.0.13/src/jntajis/_jntajis.h` & `jntajis-python-0.0.14/src/jntajis/_jntajis.h`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/src/jntajis/_jntajis.pyi` & `jntajis-python-0.0.14/src/jntajis/_jntajis.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,10 @@
 class TransliterationError(Exception): ...
 
 def jnta_encode(encoding: str, in_: str, conv_mode: int) -> bytes: ...
 def jnta_decode(encoding: str, in_: bytes) -> str: ...
 def jnta_shrink_translit(
     in_: str, replacement: str = "\ufffe", passthrough: bool = False
 ) -> str: ...
-def mj_shrink_candidates(in_: str, combo: int, limit: int = 100) -> typing.List[str]: ...
+def mj_shrink_candidates(
+    in_: str, combo: int, limit: int = 100
+) -> typing.List[str]: ...
```

### Comparing `jntajis-python-0.0.13/src/jntajis/_jntajis.pyx` & `jntajis-python-0.0.14/src/jntajis/_jntajis.pyx`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/src/jntajis/gen.py` & `jntajis-python-0.0.14/src/jntajis/gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,15 +427,14 @@
 
         if _row[16]:
             m = memo_regexp.match(_row[16])
             if m is not None:
                 try:
                     sus = (parse_uni_repr(m.group(1)),)
                 except ValueError as e:
-
                     raise InvalidFormatError(
                         f"failed to parse rune in memo ({_row[16]}) at row {ro + 2}"
                     ) from e
 
         mappings.append(
             ShrinkingTransliterationMapping(
                 jis=jis,
```

### Comparing `jntajis-python-0.0.13/src/jntajis/tests/test_encoder.py` & `jntajis-python-0.0.14/src/jntajis/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/src/jntajis/tests/test_mj_translit.py` & `jntajis-python-0.0.14/src/jntajis/tests/test_mj_translit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 import jntajis
 
 
-@pytest.mark.parametrize( ("input", "combo", "expected"),
+@pytest.mark.parametrize(
+    ("input", "combo", "expected"),
     [
         # 斎
         (
             "\u658e",
             jntajis.MJShrinkSchemeCombo.JIS_INCORPORATION_UCS_UNIFICATION_RULE,
             ["\u658e"],
         ),
@@ -69,15 +70,16 @@
         (
             "\u9089",
             jntajis.MJShrinkSchemeCombo.MOJ_FAMILY_REGISTER_ACT_RELATED_NOTICE,
             ["\u8fba", "\u908a", "\u9089"],
         ),
         (
             "\u9089",
-            jntajis.MJShrinkSchemeCombo.JIS_INCORPORATION_UCS_UNIFICATION_RULE | jntajis.MJShrinkSchemeCombo.MOJ_FAMILY_REGISTER_ACT_RELATED_NOTICE,
+            jntajis.MJShrinkSchemeCombo.JIS_INCORPORATION_UCS_UNIFICATION_RULE
+            | jntajis.MJShrinkSchemeCombo.MOJ_FAMILY_REGISTER_ACT_RELATED_NOTICE,
             ["\u8fba", "\u908a", "\u9089"],
         ),
         # 邊󠄏
         (
             "\u908a",
             jntajis.MJShrinkSchemeCombo.JIS_INCORPORATION_UCS_UNIFICATION_RULE,
             ["\u908a"],
@@ -120,15 +122,16 @@
         (
             "\u908a",
             jntajis.MJShrinkSchemeCombo.MOJ_FAMILY_REGISTER_ACT_RELATED_NOTICE,
             ["\u8fba", "\u908a"],
         ),
         (
             "\u908a",
-            jntajis.MJShrinkSchemeCombo.JIS_INCORPORATION_UCS_UNIFICATION_RULE | jntajis.MJShrinkSchemeCombo.MOJ_FAMILY_REGISTER_ACT_RELATED_NOTICE,
+            jntajis.MJShrinkSchemeCombo.JIS_INCORPORATION_UCS_UNIFICATION_RULE
+            | jntajis.MJShrinkSchemeCombo.MOJ_FAMILY_REGISTER_ACT_RELATED_NOTICE,
             ["\u8fba", "\u908a"],
         ),
         # 㑐
         (
             "\u3450",
             jntajis.MJShrinkSchemeCombo.JIS_INCORPORATION_UCS_UNIFICATION_RULE,
             ["\u3450"],
```

### Comparing `jntajis-python-0.0.13/src/jntajis/xlsx_parser/parser.py` & `jntajis-python-0.0.14/src/jntajis/xlsx_parser/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,14 @@
         self.c += 1
         return None
 
     def end_element(self, name: str) -> typing.Optional[Handlers]:
         self.c -= 1
         if self.c < 0:
             if self._attlist is not None:
-                value: typing.Union[str, OpenXMLFormula]
                 self.outer.set_value(
                     OpenXMLFormula(value=self._value, **self._attlist)
                     if self._elem_type == "f"
                     else self._value
                 )
             return self.outer
         else:
```

### Comparing `jntajis-python-0.0.13/src/jntajis/xlsx_parser/xmlutils.py` & `jntajis-python-0.0.14/src/jntajis/xlsx_parser/xmlutils.py`

 * *Files identical despite different names*

### Comparing `jntajis-python-0.0.13/src/jntajis_python.egg-info/PKG-INFO` & `jntajis-python-0.0.14/src/jntajis_python.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,115 @@
 Metadata-Version: 2.1
 Name: jntajis-python
-Version: 0.0.13
+Version: 0.0.14
 Summary: A fast character conversion and transliteration library based on the scheme defined for Japan National Tax Agency's corporate number system.
 Home-page: https://github.com/opencollector/jntajis-python
 Author: Open Collector, inc.
 Author-email: <info@opencollector.co.jp>
 License: BSD License
-Description: # jntajis-python
-        
-        Documentation: https://jntajis-python.readthedocs.io/
-        
-        ## What's JNTAJIS-python?
-        
-        JNTAJIS-python is a transliteration library, specifically designed for dealing with three different character sets; JIS X 0208, JIS X 0213, and Unicode.
-        
-        ```python
-        import jntajis
-        
-        print(jntajis.mj_shrink_candidates("髙島屋", jntajis.MJShrinkSchemeCombo.JIS_INCORPORATION_UCS_UNIFICATION_RULE))  # outputs ["高島屋", "髙島屋"]
-        print(jntajis.jnta_shrink_translit("麴町"))  # outputs "麹町"
-        ```
-        
-        To that end, this library refers to three different character tables; MJ character table, MJ shrink conversion map, and NTA shrink conversion map.
-        
-        The MJ character table (*MJ文字一覧表*) defines a vast set of kanji (*漢字*) characters used in information processing of Japanese texts initially developed by Information-technology Promotion Agency.
-        
-        The MJ shrink conversion map (*MJ縮退マップ*) was also developed alongside for the sake of interoperability between MJ-aware systems and systems based on Unicode, which is used to transliterate complex, less-frequently-used character variants to commonly-used, more-used ones.
-        
-        The NTA shrink conversion map (*国税庁JIS縮退マップ*) was developed by Japan National Tax Agency to canonicalize user inputs for its corporation number search service provided as a public web API.  This maps JIS level 3 and 4 characters to JIS level 1 and 2 characters (i.e. characters defined in JIS X 0208.)  Note that not all level 3 and level 4 characters have level 1 and 2 counterparts.  Also note that some of level 3 and 4 characters don't map to a single character one by each.  Instead, they map to sequences of two or more characters.
-        
-        The table below shows some examples of transliteration by the MJ character table suite and NTA shrink conversion map.
-        
-        | Glyph | MJ code | Unicode | JIS X 0213 | Glyph\* | MJ code\* | JIS X 0208\* | Transliterator |
-        | ----- | ------- | ------- | ---------- | ------ | ------- | ---------- | -------------- | 
-        | ![棃](https://moji.or.jp/mojikibansearch/img/MJ/MJ014031.png) | MJ014031 | U+68C3 | 2-14-90 | ![梨](https://moji.or.jp/mojikibansearch/img/MJ/MJ014007.png) | MJ014007 | 1-45-92 | MJ / JNTA |
-        | ![﨑](https://moji.or.jp/mojikibansearch/img/MJ/MJ030196.png) | MJ030196 | U+FA11 | 1-47-82 | ![崎](https://moji.or.jp/mojikibansearch/img/MJ/MJ010541.png) | MJ010541 | 1-26-74 | MJ / JNTA |
-        | ![髙](https://moji.or.jp/mojikibansearch/img/MJ/MJ028902.png) | MJ028902 | U+9AD9 | N/A | ![高](https://moji.or.jp/mojikibansearch/img/MJ/MJ028901.png) | MJ028901 | 1-25-66 | MJ |
-        
-        The conversion schematics is shown below:
-        
-        ![](https://github.com/opencollector/jntajis-python/raw/main/docs/source/_static/images/mj-jnta.svg)
-        
-        * JNTA transliteration
-        
-            As every JIS X 0213 characters maps to its Unicode counterpart, the conversion is done only with the single JNTA character mappings table.
-        
-        * MJ transliteration
-        
-            Transliteration is done in two phases:
-        
-            1. Conversion from Unicode to MJ character mappings.
-        
-                While not all characters in the MJ characters table map to Unicode, each MJ code has different shrink mappings. Because of this, the transliterator tries to convert Unicode codepoints to MJ codes first.
-        
-            2. Transliteration by MJ shrink mappings.
-        
-                The transliteration result as a string isn't necessarily single as some MJ codes have more than one transliteration candidate. This happens because a) a Unicode codepoint may map to multiple MJ codes and b) multiple transliteration schemes are designated to a single MJ code.
-        
-        
-        Relationship between Unicode, MJ character mappings, JIS X 0213, and JIS X 0208 can be depicted as follows:
-        
-        ![](https://github.com/opencollector/jntajis-python/raw/main/docs/source/_static/images/relationships-character-mappings.svg)
-        
-        ## License
-        
-        The source code except `src/jntajis/_jntajis.h` is published under the BSD 3-clause license.
-        
-        `src/jntajis/_jntajis.h` contains the data from the following entities:
-        
-        * JIS shrink conversion mappings (国税庁: JIS縮退マップ)
-        
-          Publisher: National Tax Agency
-        
-          Author: National Tax Agency
-        
-          Source: https://www.houjin-bangou.nta.go.jp/download/
-        
-          License: CC BY 4.0
-        
-        * MJ character table (文字情報技術促進協議会: MJ文字一覧表)
-        
-          Publisher: Character Information Technology Promotion Council (CITPC)
-        
-          Author: Information-technology Promotion Agency (IPA)
-        
-          Source: https://moji.or.jp/mojikiban/mjlist/
-        
-          License: CC BY-SA 2.1 JP
-        
-        * MJ shrink conversion mappings (文字情報技術促進協議会: MJ縮退マップ)
-        
-          Publisher: Character Information Technology Promotion Council (CITPC)
-        
-          Author: Information-technology Promotion Agency (IPA)
-        
-          Source: https://moji.or.jp/mojikiban/map/ 
-        
-          License: CC BY-SA 2.1 JP
-        
 Keywords: Unicode,JIS,encoding,conversion,transliteration,Japanese
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: Filters
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# jntajis-python
+
+Documentation: https://jntajis-python.readthedocs.io/
+
+## What's JNTAJIS-python?
+
+JNTAJIS-python is a transliteration library, specifically designed for dealing with three different character sets; JIS X 0208, JIS X 0213, and Unicode.
+
+```python
+import jntajis
+
+print(jntajis.mj_shrink_candidates("髙島屋", jntajis.MJShrinkSchemeCombo.JIS_INCORPORATION_UCS_UNIFICATION_RULE))  # outputs ["高島屋", "髙島屋"]
+print(jntajis.jnta_shrink_translit("麴町"))  # outputs "麹町"
+```
+
+To that end, this library refers to three different character tables; MJ character table, MJ shrink conversion map, and NTA shrink conversion map.
+
+The MJ character table (*MJ文字一覧表*) defines a vast set of kanji (*漢字*) characters used in information processing of Japanese texts initially developed by Information-technology Promotion Agency.
+
+The MJ shrink conversion map (*MJ縮退マップ*) was also developed alongside for the sake of interoperability between MJ-aware systems and systems based on Unicode, which is used to transliterate complex, less-frequently-used character variants to commonly-used, more-used ones.
+
+The NTA shrink conversion map (*国税庁JIS縮退マップ*) was developed by Japan National Tax Agency to canonicalize user inputs for its corporation number search service provided as a public web API.  This maps JIS level 3 and 4 characters to JIS level 1 and 2 characters (i.e. characters defined in JIS X 0208.)  Note that not all level 3 and level 4 characters have level 1 and 2 counterparts.  Also note that some of level 3 and 4 characters don't map to a single character one by each.  Instead, they map to sequences of two or more characters.
+
+The table below shows some examples of transliteration by the MJ character table suite and NTA shrink conversion map.
+
+| Glyph | MJ code | Unicode | JIS X 0213 | Glyph\* | MJ code\* | JIS X 0208\* | Transliterator |
+| ----- | ------- | ------- | ---------- | ------ | ------- | ---------- | -------------- | 
+| ![棃](https://moji.or.jp/mojikibansearch/img/MJ/MJ014031.png) | MJ014031 | U+68C3 | 2-14-90 | ![梨](https://moji.or.jp/mojikibansearch/img/MJ/MJ014007.png) | MJ014007 | 1-45-92 | MJ / JNTA |
+| ![﨑](https://moji.or.jp/mojikibansearch/img/MJ/MJ030196.png) | MJ030196 | U+FA11 | 1-47-82 | ![崎](https://moji.or.jp/mojikibansearch/img/MJ/MJ010541.png) | MJ010541 | 1-26-74 | MJ / JNTA |
+| ![髙](https://moji.or.jp/mojikibansearch/img/MJ/MJ028902.png) | MJ028902 | U+9AD9 | N/A | ![高](https://moji.or.jp/mojikibansearch/img/MJ/MJ028901.png) | MJ028901 | 1-25-66 | MJ |
+
+The conversion schematics is shown below:
+
+![](https://github.com/opencollector/jntajis-python/raw/main/docs/source/_static/images/mj-jnta.svg)
+
+* JNTA transliteration
+
+    As every JIS X 0213 characters maps to its Unicode counterpart, the conversion is done only with the single JNTA character mappings table.
+
+* MJ transliteration
+
+    Transliteration is done in two phases:
+
+    1. Conversion from Unicode to MJ character mappings.
+
+        While not all characters in the MJ characters table map to Unicode, each MJ code has different shrink mappings. Because of this, the transliterator tries to convert Unicode codepoints to MJ codes first.
+
+    2. Transliteration by MJ shrink mappings.
+
+        The transliteration result as a string isn't necessarily single as some MJ codes have more than one transliteration candidate. This happens because a) a Unicode codepoint may map to multiple MJ codes and b) multiple transliteration schemes are designated to a single MJ code.
+
+
+Relationship between Unicode, MJ character mappings, JIS X 0213, and JIS X 0208 can be depicted as follows:
+
+![](https://github.com/opencollector/jntajis-python/raw/main/docs/source/_static/images/relationships-character-mappings.svg)
+
+## License
+
+The source code except `src/jntajis/_jntajis.h` is published under the BSD 3-clause license.
+
+`src/jntajis/_jntajis.h` contains the data from the following entities:
+
+* JIS shrink conversion mappings (国税庁: JIS縮退マップ)
+
+  Publisher: National Tax Agency
+
+  Author: National Tax Agency
+
+  Source: https://www.houjin-bangou.nta.go.jp/download/
+
+  License: CC BY 4.0
+
+* MJ character table (文字情報技術促進協議会: MJ文字一覧表)
+
+  Publisher: Character Information Technology Promotion Council (CITPC)
+
+  Author: Information-technology Promotion Agency (IPA)
+
+  Source: https://moji.or.jp/mojikiban/mjlist/
+
+  License: CC BY-SA 2.1 JP
+
+* MJ shrink conversion mappings (文字情報技術促進協議会: MJ縮退マップ)
+
+  Publisher: Character Information Technology Promotion Council (CITPC)
+
+  Author: Information-technology Promotion Agency (IPA)
+
+  Source: https://moji.or.jp/mojikiban/map/ 
+
+  License: CC BY-SA 2.1 JP
+
+
```

### Comparing `jntajis-python-0.0.13/src/jntajis_python.egg-info/SOURCES.txt` & `jntajis-python-0.0.14/src/jntajis_python.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 .readthedocs.yaml
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 setup.cfg
 setup.py
+.github/workflows/main.yml
+.github/workflows/tests.yml
 .github/workflows/wheels.yml
 docs/.gitignore
 docs/Makefile
 docs/make.bat
 docs/source/api.rst
 docs/source/conf.py
 docs/source/index.rst
```

