# Comparing `tmp/SoMaJo-2.2.3.tar.gz` & `tmp/SoMaJo-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SoMaJo-2.2.3.tar", last modified: Thu Feb  2 10:38:09 2023, max compression
+gzip compressed data, was "SoMaJo-2.2.4.tar", last modified: Fri Jun 16 08:43:27 2023, max compression
```

## Comparing `SoMaJo-2.2.3.tar` & `SoMaJo-2.2.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-02 10:38:09.044050 SoMaJo-2.2.3/
--rw-r--r--   0 thomas    (1000) thomas    (1000)    10561 2023-02-02 10:36:54.000000 SoMaJo-2.2.3/CHANGES.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)    35147 2017-07-18 05:45:01.000000 SoMaJo-2.2.3/LICENSE.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       66 2017-07-18 05:45:01.000000 SoMaJo-2.2.3/MANIFEST.in
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1488 2023-02-02 10:38:09.044050 SoMaJo-2.2.3/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)      576 2018-08-27 16:50:42.000000 SoMaJo-2.2.3/README.rst
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-02 10:38:09.044050 SoMaJo-2.2.3/SoMaJo.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1488 2023-02-02 10:38:09.000000 SoMaJo-2.2.3/SoMaJo.egg-info/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)      772 2023-02-02 10:38:09.000000 SoMaJo-2.2.3/SoMaJo.egg-info/SOURCES.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-02-02 10:38:09.000000 SoMaJo-2.2.3/SoMaJo.egg-info/dependency_links.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       18 2023-02-02 10:38:09.000000 SoMaJo-2.2.3/SoMaJo.egg-info/requires.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        7 2023-02-02 10:38:09.000000 SoMaJo-2.2.3/SoMaJo.egg-info/top_level.txt
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-02 10:38:09.044050 SoMaJo-2.2.3/bin/
--rwxr-xr-x   0 thomas    (1000) thomas    (1000)      188 2017-11-15 19:39:47.000000 SoMaJo-2.2.3/bin/somajo-tokenizer
--rw-r--r--   0 thomas    (1000) thomas    (1000)       38 2023-02-02 10:38:09.044050 SoMaJo-2.2.3/setup.cfg
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2311 2023-01-27 11:14:07.000000 SoMaJo-2.2.3/setup.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-02 10:38:09.044050 SoMaJo-2.2.3/somajo/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      236 2019-12-19 14:00:00.000000 SoMaJo-2.2.3/somajo/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     8415 2021-08-24 11:27:48.000000 SoMaJo-2.2.3/somajo/abbreviations_de.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7465 2019-02-15 10:13:21.000000 SoMaJo-2.2.3/somajo/abbreviations_en.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)    77873 2018-03-22 21:04:28.000000 SoMaJo-2.2.3/somajo/camel_case_tokens.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5144 2022-09-12 17:47:07.000000 SoMaJo-2.2.3/somajo/cli.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4089 2021-12-13 15:17:37.000000 SoMaJo-2.2.3/somajo/doubly_linked_list.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      321 2017-11-15 19:39:47.000000 SoMaJo-2.2.3/somajo/eos_abbreviations.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)      130 2018-06-16 07:34:43.000000 SoMaJo-2.2.3/somajo/non-breaking_hyphenated_words_en.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)      727 2018-06-16 07:36:40.000000 SoMaJo-2.2.3/somajo/non-breaking_prefixes_en.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)      335 2018-06-16 07:38:17.000000 SoMaJo-2.2.3/somajo/non-breaking_suffixes_en.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)    13521 2021-07-09 08:10:19.000000 SoMaJo-2.2.3/somajo/sentence_splitter.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      607 2022-12-17 20:49:42.000000 SoMaJo-2.2.3/somajo/single_token_abbreviations_de.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)      248 2020-04-09 18:19:23.000000 SoMaJo-2.2.3/somajo/single_token_abbreviations_en.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)    17844 2022-01-18 09:45:25.000000 SoMaJo-2.2.3/somajo/somajo.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2895 2019-12-19 14:00:00.000000 SoMaJo-2.2.3/somajo/token.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    55610 2023-01-27 10:24:03.000000 SoMaJo-2.2.3/somajo/tokenizer.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4696 2020-03-04 19:09:04.000000 SoMaJo-2.2.3/somajo/tokens_with_plus_or_ampersand.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)      367 2023-01-27 09:51:47.000000 SoMaJo-2.2.3/somajo/units.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)    16636 2022-01-18 09:45:25.000000 SoMaJo-2.2.3/somajo/utils.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)       22 2023-02-02 10:37:12.000000 SoMaJo-2.2.3/somajo/version.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-16 08:43:27.717815 SoMaJo-2.2.4/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    10694 2023-06-16 08:42:20.000000 SoMaJo-2.2.4/CHANGES.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    35147 2017-07-18 05:45:01.000000 SoMaJo-2.2.4/LICENSE.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       66 2017-07-18 05:45:01.000000 SoMaJo-2.2.4/MANIFEST.in
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1488 2023-06-16 08:43:27.717815 SoMaJo-2.2.4/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      576 2018-08-27 16:50:42.000000 SoMaJo-2.2.4/README.rst
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-16 08:43:27.717815 SoMaJo-2.2.4/SoMaJo.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1488 2023-06-16 08:43:27.000000 SoMaJo-2.2.4/SoMaJo.egg-info/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      772 2023-06-16 08:43:27.000000 SoMaJo-2.2.4/SoMaJo.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-06-16 08:43:27.000000 SoMaJo-2.2.4/SoMaJo.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       18 2023-06-16 08:43:27.000000 SoMaJo-2.2.4/SoMaJo.egg-info/requires.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        7 2023-06-16 08:43:27.000000 SoMaJo-2.2.4/SoMaJo.egg-info/top_level.txt
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-16 08:43:27.717815 SoMaJo-2.2.4/bin/
+-rwxr-xr-x   0 thomas    (1000) thomas    (1000)      188 2017-11-15 19:39:47.000000 SoMaJo-2.2.4/bin/somajo-tokenizer
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       38 2023-06-16 08:43:27.717815 SoMaJo-2.2.4/setup.cfg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2311 2023-01-27 11:14:07.000000 SoMaJo-2.2.4/setup.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-16 08:43:27.717815 SoMaJo-2.2.4/somajo/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      236 2019-12-19 14:00:00.000000 SoMaJo-2.2.4/somajo/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     8415 2021-08-24 11:27:48.000000 SoMaJo-2.2.4/somajo/abbreviations_de.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7465 2019-02-15 10:13:21.000000 SoMaJo-2.2.4/somajo/abbreviations_en.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    77873 2018-03-22 21:04:28.000000 SoMaJo-2.2.4/somajo/camel_case_tokens.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5144 2022-09-12 17:47:07.000000 SoMaJo-2.2.4/somajo/cli.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4089 2021-12-13 15:17:37.000000 SoMaJo-2.2.4/somajo/doubly_linked_list.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      321 2017-11-15 19:39:47.000000 SoMaJo-2.2.4/somajo/eos_abbreviations.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      130 2018-06-16 07:34:43.000000 SoMaJo-2.2.4/somajo/non-breaking_hyphenated_words_en.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      727 2018-06-16 07:36:40.000000 SoMaJo-2.2.4/somajo/non-breaking_prefixes_en.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      335 2018-06-16 07:38:17.000000 SoMaJo-2.2.4/somajo/non-breaking_suffixes_en.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    13521 2021-07-09 08:10:19.000000 SoMaJo-2.2.4/somajo/sentence_splitter.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      607 2023-06-16 08:00:22.000000 SoMaJo-2.2.4/somajo/single_token_abbreviations_de.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      248 2020-04-09 18:19:23.000000 SoMaJo-2.2.4/somajo/single_token_abbreviations_en.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    17844 2022-01-18 09:45:25.000000 SoMaJo-2.2.4/somajo/somajo.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2895 2019-12-19 14:00:00.000000 SoMaJo-2.2.4/somajo/token.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    55988 2023-06-16 08:38:05.000000 SoMaJo-2.2.4/somajo/tokenizer.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4696 2020-03-04 19:09:04.000000 SoMaJo-2.2.4/somajo/tokens_with_plus_or_ampersand.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      367 2023-01-27 09:51:47.000000 SoMaJo-2.2.4/somajo/units.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    16636 2022-01-18 09:45:25.000000 SoMaJo-2.2.4/somajo/utils.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       22 2023-06-16 08:00:44.000000 SoMaJo-2.2.4/somajo/version.py
```

### Comparing `SoMaJo-2.2.3/CHANGES.txt` & `SoMaJo-2.2.4/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # CHANGELOG #
 
+## Version 2.2.4, 2023-06-23 ##
+
+- Improvements to tokenization of words containing numbers (e.g.
+  COVID-19-Pandemie, FFP2-Maske).
+
 ## Version 2.2.3, 2023-02-02 ##
 
 - Improvements to tokenization: Roman ordinals, abbreviation “Art.”
   preceding a number, certain units of measurement at the end of a
   sentence (e.g. km/h).
 
 ## Version 2.2.2, 2022-09-12 ##
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_yn703ie9_/tmps7x55ze8_TarContainer/0/1.txt", line 309, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_yn703ie9_/tmps7x55ze8_TarContainer/0/1.txt", line 309, column 0: CDATA terminal not found*

```diff
@@ -1,11 +1,12 @@
-# CHANGELOG # ## Version 2.2.3, 2023-02-02 ## - Improvements to tokenization:
-Roman ordinals, abbreviation âArt.â preceding a number, certain units of
-measurement at the end of a sentence (e.g. km/h). ## Version 2.2.2, 2022-09-12
-## - Bugfix: Command-line option --sentence_tag implies option --
-split_sentences. ## Version 2.2.1, 2022-03-08 ## - Bugfix: Command-line option
---strip-tags implies option --xml. ## Version 2.2.0, 2022-01-18 ## - New
-feature: Prune XML tags and their contents from the input before tokenization
-(via the command line option --prune TAGNAME1 --prune TAGNAME2 â¦ or by
-passing prune_tags=["TAGNAME1", "TAGNAME2", â¦] to tokenize_xml or
-tokenize_xml_file). This can be useful when processing HTML files, e.g. for
-removing any
+# CHANGELOG # ## Version 2.2.4, 2023-06-23 ## - Improvements to tokenization of
+words containing numbers (e.g. COVID-19-Pandemie, FFP2-Maske). ## Version
+2.2.3, 2023-02-02 ## - Improvements to tokenization: Roman ordinals,
+abbreviation âArt.â preceding a number, certain units of measurement at the
+end of a sentence (e.g. km/h). ## Version 2.2.2, 2022-09-12 ## - Bugfix:
+Command-line option --sentence_tag implies option --split_sentences. ## Version
+2.2.1, 2022-03-08 ## - Bugfix: Command-line option --strip-tags implies option
+--xml. ## Version 2.2.0, 2022-01-18 ## - New feature: Prune XML tags and their
+contents from the input before tokenization (via the command line option --
+prune TAGNAME1 --prune TAGNAME2 â¦ or by passing prune_tags=["TAGNAME1",
+"TAGNAME2", â¦] to tokenize_xml or tokenize_xml_file). This can be useful when
+processing HTML files, e.g. for removing any
```

### Comparing `SoMaJo-2.2.3/LICENSE.txt` & `SoMaJo-2.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/PKG-INFO` & `SoMaJo-2.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: SoMaJo
-Version: 2.2.3
+Version: 2.2.4
 Summary: A tokenizer and sentence splitter for German and English web and social media texts.
 Home-page: https://github.com/tsproisl/SoMaJo
-Download-URL: https://github.com/tsproisl/SoMaJo/archive/v2.2.3.tar.gz
+Download-URL: https://github.com/tsproisl/SoMaJo/archive/v2.2.4.tar.gz
 Author: Thomas Proisl, Peter Uhrig
 Author-email: thomas.proisl@fau.de
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `SoMaJo-2.2.3/README.rst` & `SoMaJo-2.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/SoMaJo.egg-info/PKG-INFO` & `SoMaJo-2.2.4/SoMaJo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: SoMaJo
-Version: 2.2.3
+Version: 2.2.4
 Summary: A tokenizer and sentence splitter for German and English web and social media texts.
 Home-page: https://github.com/tsproisl/SoMaJo
-Download-URL: https://github.com/tsproisl/SoMaJo/archive/v2.2.3.tar.gz
+Download-URL: https://github.com/tsproisl/SoMaJo/archive/v2.2.4.tar.gz
 Author: Thomas Proisl, Peter Uhrig
 Author-email: thomas.proisl@fau.de
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `SoMaJo-2.2.3/SoMaJo.egg-info/SOURCES.txt` & `SoMaJo-2.2.4/SoMaJo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/setup.py` & `SoMaJo-2.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/somajo/abbreviations_de.txt` & `SoMaJo-2.2.4/somajo/abbreviations_de.txt`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/somajo/abbreviations_en.txt` & `SoMaJo-2.2.4/somajo/abbreviations_en.txt`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/somajo/camel_case_tokens.txt` & `SoMaJo-2.2.4/somajo/camel_case_tokens.txt`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/somajo/cli.py` & `SoMaJo-2.2.4/somajo/cli.py`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/somajo/doubly_linked_list.py` & `SoMaJo-2.2.4/somajo/doubly_linked_list.py`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/somajo/non-breaking_prefixes_en.txt` & `SoMaJo-2.2.4/somajo/non-breaking_prefixes_en.txt`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/somajo/sentence_splitter.py` & `SoMaJo-2.2.4/somajo/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/somajo/single_token_abbreviations_de.txt` & `SoMaJo-2.2.4/somajo/single_token_abbreviations_de.txt`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/somajo/somajo.py` & `SoMaJo-2.2.4/somajo/somajo.py`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/somajo/token.py` & `SoMaJo-2.2.4/somajo/token.py`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/somajo/tokenizer.py` & `SoMaJo-2.2.4/somajo/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,16 +156,29 @@
                                '[̲̅$̲̅(̲̅ ͡° ͜ʖ ͡°̲̅)̲̅$̲̅]', '/╲/\\╭( ͡° ͡° ͜ʖ ͡° ͡°)╮/\\╱\\',
                                '( ͡°( ͡° ͜ʖ( ͡° ͜ʖ ͡°)ʖ ͡°) ͡°)', '(._.) ( l: ) ( .-. ) ( :l ) (._.)',
                                "̿ ̿ ̿'̿'\\̵͇̿̿\\з=(•_•)=ε/̵͇̿̿/'̿'̿ ̿", '༼ ºل͟º ༼ ºل͟º ༼ ºل͟º ༽ ºل͟º ༽ ºل͟º ༽',
                                "̿'̿'\\̵͇̿̿\\з=( ͠° ͟ʖ ͡°)=ε/̵͇̿̿/'̿̿ ̿ ̿ ̿ ̿ ̿",
                                "̿̿ ̿̿ ̿̿ ̿'̿'\\̵͇̿̿\\з= ( ▀ ͜͞ʖ▀) =ε/̵͇̿̿/’̿’̿ ̿ ̿̿ ̿̿ ̿̿",
                                # From Signal:
                                "ヽ(°◇° )ノ", "■-■¬ <(•_•)"])
-        textfaces_emoji = set(['♥‿♥', '☼.☼', '≧☉_☉≦', '(°ロ°)☝', '(☞ﾟ∀ﾟ)☞', '☜(˚▽˚)☞', '☜(⌒▽⌒)☞', '(☞ຈل͜ຈ)☞', 'ヾ(⌐■_■)ノ♪', '(☞ﾟヮﾟ)☞', '☜(ﾟヮﾟ☜)'])
-        textfaces_wo_emoji = set(['=U', 'ಠ_ಠ', '◉_◉', 'ಥ_ಥ', ":')", 'ಠ⌣ಠ', 'ಠ~ಠ', 'ಠ_ಥ', 'ಠ‿↼', 'ʘ‿ʘ', 'ಠoಠ', 'ರ_ರ', '◔̯◔', '¬_¬', 'ب_ب', '°Д°', '^̮^', '^̮^', '^̮^', '>_>', '^̮^', '^̮^', 'ಠ╭╮ಠ', '(>ლ)', 'ʕ•ᴥ•ʔ', '(ಥ﹏ಥ)', '(ᵔᴥᵔ)', '(¬‿¬)', '⌐╦╦═─', '(•ω•)', '(¬_¬)', '｡◕‿◕｡', '(ʘ‿ʘ)', '٩◔̯◔۶', '(>人<)', '(~_^)', '(^̮^)', '(･.◤)', '(◕‿◕✿)', '｡◕‿‿◕｡', '(─‿‿─)', '(；一_一)', "(ʘᗩʘ')", '(✿´‿`)', 'ლ(ಠ益ಠლ)', '~(˘▾˘~)', '(~˘▾˘)~', '(｡◕‿◕｡)', '(っ˘ڡ˘ς)', 'ლ(´ڡ`ლ)', 'ƪ(˘⌣˘)ʃ', '(´・ω・`)', '(ღ˘⌣˘ღ)', '(▰˘◡˘▰)', '〆(・∀・＠)', '༼ʘ̚ل͜ʘ̚༽', 'ᕙ(⇀‸↼‶)ᕗ', 'ᕦ(ò_óˇ)ᕤ', '(｡◕‿‿◕｡)', 'ヽ༼ຈل͜ຈ༽ﾉ', '(ง°ل͜°)ง', '╚(ಠ_ಠ)=┐', '(´・ω・)っ由', 'Ƹ̵̡Ӝ̵̨̄Ʒ', '¯\\_(ツ)_/¯', '▄︻̷̿┻̿═━一', "(ง'̀-'́)ง", '¯\\(°_o)/¯', '｡゜(｀Д´)゜｡', '(づ｡◕‿‿◕｡)づ', '(;´༎ຶД༎ຶ`)', '(ノಠ益ಠ)ノ彡┻━┻', 'ლ,ᔑ•ﺪ͟͠•ᔐ.ლ', '(ﾉ◕ヮ◕)ﾉ*:･ﾟ✧', '┬┴┬┴┤(･_├┬┴┬┴', '[̲̅$̲̅(̲̅5̲̅)̲̅$̲̅]'])
+        textfaces_emoji = set(['♥‿♥', '☼.☼', '≧☉_☉≦', '(°ロ°)☝', '(☞ﾟ∀ﾟ)☞', '☜(˚▽˚)☞', '☜(⌒▽⌒)☞',
+                               '(☞ຈل͜ຈ)☞', 'ヾ(⌐■_■)ノ♪', '(☞ﾟヮﾟ)☞', '☜(ﾟヮﾟ☜)'])
+        textfaces_wo_emoji = set(['=U', 'ಠ_ಠ', '◉_◉', 'ಥ_ಥ', ":')", 'ಠ⌣ಠ', 'ಠ~ಠ', 'ಠ_ಥ', 'ಠ‿↼',
+                                  'ʘ‿ʘ', 'ಠoಠ', 'ರ_ರ', '◔̯◔', '¬_¬', 'ب_ب', '°Д°', '^̮^', '^̮^', '^̮^',
+                                  '>_>', '^̮^', '^̮^', 'ಠ╭╮ಠ', '(>ლ)', 'ʕ•ᴥ•ʔ', '(ಥ﹏ಥ)', '(ᵔᴥᵔ)',
+                                  '(¬‿¬)', '⌐╦╦═─', '(•ω•)', '(¬_¬)', '｡◕‿◕｡', '(ʘ‿ʘ)', '٩◔̯◔۶',
+                                  '(>人<)', '(~_^)', '(^̮^)', '(･.◤)', '(◕‿◕✿)', '｡◕‿‿◕｡', '(─‿‿─)',
+                                  '(；一_一)', "(ʘᗩʘ')", '(✿´‿`)', 'ლ(ಠ益ಠლ)', '~(˘▾˘~)', '(~˘▾˘)~',
+                                  '(｡◕‿◕｡)', '(っ˘ڡ˘ς)', 'ლ(´ڡ`ლ)', 'ƪ(˘⌣˘)ʃ', '(´・ω・`)',
+                                  '(ღ˘⌣˘ღ)', '(▰˘◡˘▰)', '〆(・∀・＠)', '༼ʘ̚ل͜ʘ̚༽', 'ᕙ(⇀‸↼‶)ᕗ',
+                                  'ᕦ(ò_óˇ)ᕤ', '(｡◕‿‿◕｡)', 'ヽ༼ຈل͜ຈ༽ﾉ', '(ง°ل͜°)ง', '╚(ಠ_ಠ)=┐',
+                                  '(´・ω・)っ由', 'Ƹ̵̡Ӝ̵̨̄Ʒ', '¯\\_(ツ)_/¯', '▄︻̷̿┻̿═━一', "(ง'̀-'́)ง",
+                                  '¯\\(°_o)/¯', '｡゜(｀Д´)゜｡', '(づ｡◕‿‿◕｡)づ', '(;´༎ຶД༎ຶ`)',
+                                  '(ノಠ益ಠ)ノ彡┻━┻', 'ლ,ᔑ•ﺪ͟͠•ᔐ.ლ', '(ﾉ◕ヮ◕)ﾉ*:･ﾟ✧', '┬┴┬┴┤(･_├┬┴┬┴',
+                                  '[̲̅$̲̅(̲̅5̲̅)̲̅$̲̅]'])
         self.textfaces_space = re.compile(r"|".join([re.escape(_) for _ in sorted(textfaces_space, key=len, reverse=True)]))
         self.textfaces_emoji = re.compile(r"|".join([re.escape(_) for _ in sorted(textfaces_emoji, key=len, reverse=True)]))
         textfaces_signal = set(["\\(ˆ˚ˆ)/", "(╥﹏╥)", "(╯°□°)╯︵", "┻━┻", "┬─┬", "ノ(°–°ノ)", "(^._.^)ﾉ", "ฅ^•ﻌ•^ฅ", "(•_•)", "(■_■¬)", "ƪ(ړײ)ƪ"])
         emoticon_list = sorted(emoticon_set | textfaces_wo_emoji | textfaces_signal, key=len, reverse=True)
         self.emoticon = re.compile(r"""(?:(?:[:;]|(?<!\d)8)           # a variety of eyes, alt.: [:;8]
                                         [-'oO]?                       # optional nose or tear
                                         (?: \)+ | \(+ | [*] | ([DPp])\1*(?!\w)))   # a variety of mouths
@@ -311,17 +324,16 @@
                            )"""
         self.number_range = re.compile(r"(?<!\w|\d[.,]?)" + number_range + r"(?![.,]?\d)", re.VERBOSE)
         self.calculation = re.compile(r"(?P<arg1>\d+(?:[,.]\d+)?)(?P<op>[+*x×÷−])(?P<arg2>\d+(?:[,.]\d+)?)")
         self.amount = re.compile(r'(?<!\w)(?:\d+[\d,.]*[,.]-)(?!\w)')
         self.semester = re.compile(r'(?<!\w)(?P<a_semester>[WS]S|SoSe|WiSe)(?P<b_jahr>\d\d(?:/\d\d)?)(?!\w)', re.IGNORECASE)
         units = utils.read_abbreviation_file("units.txt")
         self.measurement = re.compile(r"(?<!\w|\d[.,]?)" + f"(?:{number}|{number_range})[ ]?" + r"(?P<unit>" + r"|".join([re.escape(_) for _ in units]) + ")" + r"(?!\w)", re.IGNORECASE | re.VERBOSE)
-        # auch Web2.0
-        self.number_compound = re.compile(r'(?<!\w) (?:\d+-?[\p{L}@][\p{L}@-]* | [\p{L}@][\p{L}@-]*-?\d+(?:\.\d)?) (?!\w)', re.VERBOSE)
-        self.number = re.compile(r"(?<!\w|\d[.,]?)" + number + r"(?![.,]?\d)", re.VERBOSE)
+        self.number_compound = re.compile(r'(?<!\w-?) (?:\d+-?[\p{L}@][\p{L}@-]*) (?!\w)', re.VERBOSE)
+        self.number = re.compile(r"(?<!\w-?|\d[.,]?)" + number + r"(?![.,]?\d)", re.VERBOSE)
         self.ipv4 = re.compile(r"(?<!\w|\d[.,]?)(?:\d{1,3}[.]){3}\d{1,3}(?![.,]?\d)")
         self.section_number = re.compile(r"(?<!\w|\d[.,]?)(?:\d+[.])+\d+[.]?(?![.,]?\d)")
 
         # PUNCTUATION
         self.quest_exclam = re.compile(r"([!?]+)")
         # arrows
         self.arrow = re.compile(r'(-+[ ]?>|<[ ]?-+|[\u2190-\u21ff])')
@@ -752,15 +764,15 @@
         # amounts (1.000,-)
         self._split_all_matches(self.amount, token_dll, "amount")
         # semesters
         self._split_all_matches(self.semester, token_dll, "semester")
         # measurements
         # self._split_all_matches(self.measurement, token_dll, "measurement")
         # number compounds
-        self._split_all_matches(self.number_compound, token_dll, "number_compound")
+        self._split_all_matches(self.number_compound, token_dll, "regular")
         # numbers
         self._split_all_matches(self.number, token_dll, "number")
         self._split_all_matches(self.ipv4, token_dll, "number")
         self._split_all_matches(self.section_number, token_dll, "number")
 
         # (clusters of) question marks and exclamation marks
         self._split_all_matches(self.quest_exclam, token_dll, "symbol")
```

### Comparing `SoMaJo-2.2.3/somajo/tokens_with_plus_or_ampersand.txt` & `SoMaJo-2.2.4/somajo/tokens_with_plus_or_ampersand.txt`

 * *Files identical despite different names*

### Comparing `SoMaJo-2.2.3/somajo/utils.py` & `SoMaJo-2.2.4/somajo/utils.py`

 * *Files identical despite different names*

