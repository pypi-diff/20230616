# Comparing `tmp/eld-0.9.0.tar.gz` & `tmp/eld-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eld-0.9.0.tar", last modified: Sat May 27 00:07:48 2023, max compression
+gzip compressed data, was "eld-0.9.1.tar", last modified: Fri Jun 16 16:39:58 2023, max compression
```

## Comparing `eld-0.9.0.tar` & `eld-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 00:07:48.832382 eld-0.9.0/
--rw-rw-rw-   0        0        0    11582 2023-05-25 18:01:36.000000 eld-0.9.0/LICENSE
--rw-rw-rw-   0        0        0    11437 2023-05-27 00:07:48.832382 eld-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0    10816 2023-05-27 00:06:32.000000 eld-0.9.0/README.md
--rw-rw-rw-   0        0        0     3421 2023-05-26 23:27:41.000000 eld-0.9.0/demo.py
--rw-rw-rw-   0        0        0       42 2023-05-27 00:07:48.832382 eld-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-05-27 00:07:22.000000 eld-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:07:48.778991 eld-0.9.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 00:07:48.794615 eld-0.9.0/src/eld/
--rw-rw-rw-   0        0        0       46 2023-05-26 23:19:27.000000 eld-0.9.0/src/eld/__init__.py
--rw-rw-rw-   0        0        0     6718 2023-05-25 17:56:12.000000 eld-0.9.0/src/eld/languageDetector.py
--rw-rw-rw-   0        0        0     3931 2023-05-25 17:56:12.000000 eld-0.9.0/src/eld/languagesData.py
--rw-rw-rw-   0        0        0     4921 2023-05-25 17:56:12.000000 eld-0.9.0/src/eld/languagesSubset.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:07:48.832382 eld-0.9.0/src/eld/ngrams/
--rw-rw-rw-   0        0        0        0 2023-05-25 17:56:12.000000 eld-0.9.0/src/eld/ngrams/__init__.py
--rw-rw-rw-   0        0        0   301240 2023-05-25 17:56:12.000000 eld-0.9.0/src/eld/ngrams/ngrams_2f37045c74780aba1d36d6717f3244dc025fb935.py
--rw-rw-rw-   0        0        0  5853755 2023-05-25 17:56:12.000000 eld-0.9.0/src/eld/ngrams/ngrams_L.py
--rw-rw-rw-   0        0        0  2507406 2023-05-25 17:56:12.000000 eld-0.9.0/src/eld/ngrams/ngrams_m.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:07:48.810244 eld-0.9.0/src/eld.egg-info/
--rw-rw-rw-   0        0        0    11437 2023-05-27 00:07:48.000000 eld-0.9.0/src/eld.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2023-05-27 00:07:48.000000 eld-0.9.0/src/eld.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 00:07:48.000000 eld-0.9.0/src/eld.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-27 00:07:48.000000 eld-0.9.0/src/eld.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-27 00:07:48.000000 eld-0.9.0/src/eld.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 16:39:58.294348 eld-0.9.1/
+-rw-rw-rw-   0        0        0    11582 2023-05-25 18:01:36.000000 eld-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0    11482 2023-06-16 16:39:58.278727 eld-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10861 2023-06-09 11:52:56.000000 eld-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 16:39:58.231845 eld-0.9.1/benchmarks/
+-rw-rw-rw-   0        0        0     1179 2023-06-08 23:01:35.000000 eld-0.9.1/benchmarks/bench.py
+-rw-rw-rw-   0        0        0 10358240 2023-02-27 22:33:57.000000 eld-0.9.1/benchmarks/big-test.txt
+-rw-rw-rw-   0        0        0  8450164 2023-05-25 17:56:12.000000 eld-0.9.1/benchmarks/sentences.txt
+-rw-rw-rw-   0        0        0    21403 2023-06-08 17:38:17.000000 eld-0.9.1/benchmarks/sentences_avg_py.png
+-rw-rw-rw-   0        0        0   957542 2023-05-25 17:56:12.000000 eld-0.9.1/benchmarks/single-words.txt
+-rw-rw-rw-   0        0        0     5359 2023-05-25 17:56:12.000000 eld-0.9.1/benchmarks/table_accuracy_py.svg
+-rw-rw-rw-   0        0        0     5596 2023-05-25 17:56:12.000000 eld-0.9.1/benchmarks/table_time_py.svg
+-rw-rw-rw-   0        0        0   777348 2023-05-25 17:56:12.000000 eld-0.9.1/benchmarks/tweets.txt
+-rw-rw-rw-   0        0        0  1624811 2023-05-25 17:56:12.000000 eld-0.9.1/benchmarks/word-pairs.txt
+-rw-rw-rw-   0        0        0     3383 2023-06-08 22:58:29.000000 eld-0.9.1/demo.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 16:39:58.294348 eld-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1471 2023-06-16 16:30:12.000000 eld-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:39:58.162839 eld-0.9.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 16:39:58.247477 eld-0.9.1/src/eld/
+-rw-rw-rw-   0        0        0       46 2023-05-26 23:19:27.000000 eld-0.9.1/src/eld/__init__.py
+-rw-rw-rw-   0        0        0     3942 2023-06-09 11:51:28.000000 eld-0.9.1/src/eld/languageData.py
+-rw-rw-rw-   0        0        0     6703 2023-06-13 22:21:23.000000 eld-0.9.1/src/eld/languageDetector.py
+-rw-rw-rw-   0        0        0     4903 2023-06-09 11:51:34.000000 eld-0.9.1/src/eld/languageSubset.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:39:58.278727 eld-0.9.1/src/eld/ngrams/
+-rw-rw-rw-   0        0        0        0 2023-05-25 17:56:12.000000 eld-0.9.1/src/eld/ngrams/__init__.py
+-rw-rw-rw-   0        0        0    63137 2023-06-16 14:55:30.000000 eld-0.9.1/src/eld/ngrams/ngrams_17ba0791499db908433b80f37c5fbc89b870084b.py
+-rw-rw-rw-   0        0        0   301240 2023-05-25 17:56:12.000000 eld-0.9.1/src/eld/ngrams/ngrams_2f37045c74780aba1d36d6717f3244dc025fb935.py
+-rw-rw-rw-   0        0        0  5853755 2023-05-25 17:56:12.000000 eld-0.9.1/src/eld/ngrams/ngrams_L.py
+-rw-rw-rw-   0        0        0  2507406 2023-05-25 17:56:12.000000 eld-0.9.1/src/eld/ngrams/ngrams_m.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:39:58.247477 eld-0.9.1/src/eld.egg-info/
+-rw-rw-rw-   0        0        0    11482 2023-06-16 16:39:58.000000 eld-0.9.1/src/eld.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      782 2023-06-16 16:39:58.000000 eld-0.9.1/src/eld.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 16:39:58.000000 eld-0.9.1/src/eld.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 16:39:58.000000 eld-0.9.1/src/eld.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-16 16:39:58.000000 eld-0.9.1/src/eld.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 16:39:58.278727 eld-0.9.1/tests/
+-rw-rw-rw-   0        0        0     3019 2023-06-11 13:37:35.000000 eld-0.9.1/tests/test_detector.py
+-rw-rw-rw-   0        0        0     2687 2023-06-11 13:38:16.000000 eld-0.9.1/tests/test_subset.py
```

### Comparing `eld-0.9.0/LICENSE` & `eld-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eld-0.9.0/PKG-INFO` & `eld-0.9.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,21 @@
-Metadata-Version: 2.1
-Name: eld
-Version: 0.9.0
-Summary: Fast and accurate natural language detection. Detector written in Python. Nito-ELD, ELD.
-Home-page: https://github.com/nitotm/efficient-language-detector-py/
-Author: Nito T.M.
-Keywords: nlp language natural-language-processing natural-language language-detection language-detector language-identification
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Efficient Language Detector
 
 <div align="center">
 	
 ![supported Python versions](https://img.shields.io/badge/Python-%3E%3D%203.7-blue)
 [![license](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
-[![supported languages](https://img.shields.io/badge/supported%20languages-60-green.svg)](#languages)
+[![supported languages](https://img.shields.io/badge/supported%20languages-60-brightgreen.svg)](#languages)
 	
 </div>
 
-Efficient language detector (Nito-ELD or ELD) is a fast and accurate language detector, is one of the fastest non compiled detectors, while its accuracy is within the range of the heaviest and slowest detectors.
+Efficient language detector (*Nito-ELD* or *ELD*) is a fast and accurate language detector, is one of the fastest non compiled detectors, while its accuracy is within the range of the heaviest and slowest detectors.
 
 It's 100% Python, easy installation and no dependencies other than `regex`.  
-ELD is also avalible in [Javascript](https://github.com/nitotm/efficient-language-detector-js/) and [PHP](https://github.com/nitotm/efficient-language-detector/).
+ELD is also available in [Javascript](https://github.com/nitotm/efficient-language-detector-js) and [PHP](https://github.com/nitotm/efficient-language-detector).
 
 > This is the first version of a port made from the original version in PHP, the structure might not be definitive, the code can be optimized. My knowledge of Python is basic, feel free to suggest improvements.
 
 1. [Installation](#installation)
 2. [How to use](#how-to-use)
 3. [Benchmarks](#benchmarks)
 4. [Languages](#languages)
@@ -46,21 +32,21 @@
 ```python
 # from src.eld.languageDetector import LanguageDetector # To load ELD without install. Update path.
 from eld import LanguageDetector
 detector = LanguageDetector()
 
 print(detector.detect('Hola, cómo te llamas?'))
 ```
-`detect()` expects an UTF-8 string, and returns a list, with a value named 'language', which will be either an *ISO 639-1 code* or `False`
+`detect()` expects a UTF-8 string, and returns a list, with a value named 'language', which will be either an *ISO 639-1 code* or `False`
 ```
 {'language': 'es'}
 {'language': False, 'error': 'Some error', 'scores': {}}
 ```
 
-- To get the best guess, deactive minimum length & confidence threshold; used for benchmarking.
+- To get the best guess, turn off minimum length & confidence threshold; also used for benchmarking.
 ```python
 print(detector.detect('To', False, False, 0, 1))
 # To improve readability Named Parameters can be used
 detector.detect(text='To', clean_text=False, check_confidence=False, min_byte_length=0, min_ngrams=1)
 # clean_text=True, Removes Urls, domains, emails, alphanumerical & numbers
 ```
 
@@ -69,46 +55,46 @@
 detector.return_scores = True
 print(detector.detect('How are you? Bien, gracias'))
 # {'language': 'en', 'scores': {'en': 0.32, 'es': 0.31, ...}}
 ```
 
 - To reduce the languages to be detected, there are 3 different options, they only need to be executed once. (Check available [languages](#languages) below)
 ```python
-langs_subset = ['en', 'es', 'fr', 'it', 'nl', 'de']
+lang_subset = ['en', 'es', 'fr', 'it', 'nl', 'de']
 
-# with dynamic_langs_subset() the detector executes normally, and then filters excluded languages
-detector.dynamic_langs_subset(langs_subset)
+# with dynamic_lang_subset() the detector executes normally, and then filters excluded languages
+detector.dynamic_lang_subset(lang_subset)
 
-# langs_subset() Will first remove the excluded languages, from the n-grams database
-# For a single detection is slower than dynamic_langs_subset(), but for several will be faster
+# lang_subset() Will first remove the excluded languages, from the n-grams database
+# For a single detection is slower than dynamic_lang_subset(), but for several will be faster
 # If save option is true (default), the new Ngrams subset will be stored, and loaded next call
-detector.langs_subset(langs_subset) # langs_subset(langs, save=True) 
+detector.lang_subset(lang_subset) # lang_subset(langs, save=True) 
 
-# To remove either dynamic_langs_subset() or langs_subset(), call the methods with False as argument
-detector.langs_subset(False); 
+# To remove either dynamic_lang_subset() or lang_subset(), call the methods with False as argument
+detector.lang_subset(False)
 
 # Finally the fastest way to regularly use a languages subset: we create the instance with a file
-# The file in the argument can be a subset by langs_subset() or another database like ngrams_L.php
+# The file in the argument can be a subset by lang_subset() or another database like ngrams_L.php
 langSubsetDetect = LanguageDetector('ngrams_2f37045c74780aba1d36d6717f3244dc025fb935')
 ```
 
 ## Benchmarks
 
 I compared *ELD* with a different variety of detectors, since the interesting part is the algorithm.
 
-| URL                                                       | Version       | Language     |
-| :-                                                        | :-            | :-           |
-| https://github.com/nitotm/efficient-language-detector-py/ | 0.9.0         | Python       |
-| https://github.com/nitotm/efficient-language-detector/    | 1.0.0         | PHP          |
-| https://github.com/pemistahl/lingua-py                    | 1.3.2         | Python       |
-| https://github.com/CLD2Owners/cld2                        | Aug 21, 2015  | C++          |
-| https://github.com/google/cld3                            | Aug 28, 2020  | C++          |
-| https://github.com/wooorm/franc                           | 6.1.0         | Javasript    |
+| URL                                                       | Version      | Language   |
+|:----------------------------------------------------------|:-------------|:-----------|
+| https://github.com/nitotm/efficient-language-detector-py/ | 0.9.0        | Python     |
+| https://github.com/nitotm/efficient-language-detector/    | 1.0.0        | PHP        |
+| https://github.com/pemistahl/lingua-py                    | 1.3.2        | Python     |
+| https://github.com/CLD2Owners/cld2                        | Aug 21, 2015 | C++        |
+| https://github.com/google/cld3                            | Aug 28, 2020 | C++        |
+| https://github.com/wooorm/franc                           | 6.1.0        | Javascript |
 
-Tests: **Tweets**: *760KB*, short sentences of 140 chars max.; **Big test**: *10MB*, sentences in all 60 languages supported; **Sentences**: *8MB*, this is the *Lingua* sentences test, minus unsupported languages.  
+Benchmarks: **Tweets**: *760KB*, short sentences of 140 chars max.; **Big test**: *10MB*, sentences in all 60 languages supported; **Sentences**: *8MB*, this is the *Lingua* sentences test, minus unsupported languages.  
 Short sentences is what *ELD* and most detectors focus on, as very short text is unreliable, but I included the *Lingua* **Word pairs** *1.5MB*, and **Single words** *880KB* tests to see how they all compare beyond their reliable limits.
 
 These are the results, first, accuracy and then execution time.
 
 <!-- Accuracy table
 |                     | Tweets       | Big test     | Sentences    | Word pairs   | Single words |
 |:--------------------|:------------:|:------------:|:------------:|:------------:|:------------:|
@@ -116,42 +102,42 @@
 | **Nito-ELD-L**      | 99.4%        | 99.4%        | 98.7%        | 89.4%        | 76.1%        |
 | **Lingua**          | 98.8%        | 99.1%        | 98.6%        | 93.1%        | 80.0%        |
 | **CLD2**            | 93.8%        | 97.2%        | 97.2%        | 87.7%        | 69.6%        |
 | **Lingua low**      | 96.0%        | 97.2%        | 96.3%        | 83.7%        | 68.0%        |
 | **CLD3**            | 92.2%        | 95.8%        | 94.7%        | 69.0%        | 51.5%        |
 | **franc**           | 89.8%        | 92.0%        | 90.5%        | 65.9%        | 52.9%        |
 -->
-<img width="800" src="https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/table_accuracy_py.svg">
+<img alt="accuracy table" width="800" src="https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/table_accuracy_py.svg">
 
 <!--- Time table
 |                     | Tweets       | Big test     | Sentences    | Word pairs   | Single words |
 |:--------------------|:------------:|:------------:|:------------:|:------------:|:------------:|
 | **Nito-ELD-py**     |     0.96"    |      7.8"    |      6.7"    |     2.6"     |     2.1"     |
 | **Nito-ELD-L-py**   |     1"       |      8"      |      6.9"    |     2.7"     |     2.1"     |
 | **Lingua**          |  4790"       |  24000"      |  18700"      |  8450"       |  6700"       |
 | **CLD2**            |     0.35"    |      2"      |      1.7"    |     0.98"    |     0.8"     |
 | **Lingua low**      |    64"       |    370"      |    308"      |   108"       |    85"       |
 | **CLD3**            |     3.9"     |     29"      |     26"      |    12"       |    11"       |
 | **franc**           |     1.2"     |      8"      |      7.8"    |     2.8"     |     2"       |
 | **Nito-ELD-php**    |     0.31"    |      2.5"    |      2.2"    |     0.66"    |     0.48"    |
 -->
-<img width="800" src="https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/table_time_py.svg">
+<img alt="time table" width="800" src="https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/table_time_py.svg">
 
 <sup style="color:#08e">1.</sup> <sup style="color:#777">Lingua could have a small advantage as it participates with 54 languages, 6 less.</sup>  
 <sup style="color:#08e">2.</sup> <sup style="color:#777">CLD2 and CLD3, return a list of languages, the ones not included in this test where discarded, but usually they return one language, I believe they have a disadvantage. 
 Also, I confirm the results of CLD2 for short text are correct, contrary to the test on the *Lingua* page, they did not use the parameter "bestEffort = True", their benchmark for CLD2 is unfair.
 
 *Lingua* is the average accuracy winner, but at what cost, the same test that in *ELD* or *CLD2* is below 10 seconds, in Lingua takes more than 5 hours! It acts like a brute-force software. 
-Also its lead comes from single and pair words, which are unreliable regardless.
+Also, its lead comes from single and pair words, which are unreliable regardless.
 
 The Python version of *NITO-ELD* is not the fastest but is still considered fast, as it is faster than any other non compiled detector tested.
 
 I added *ELD-L* for comparison, which has a 2.3x bigger database, but only increases execution time marginally, a testament to the efficiency of the algorithm. *ELD-L* is not the main database as it does not improve language detection in sentences.
 
-Here is the average, per test, of Tweets, Big test & Sentences.
+Here is the average, per benchmark, of Tweets, Big test & Sentences.
 
 ![Sentences tests average](https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/sentences_avg_py.png)
 <!--- Sentences average
 |                     | Time         | Accuracy     |
 |:--------------------|:------------:|:------------:|
 | **Nito-ELD-py**     |      5.17"   | 99.16%       |
 | **Nito-ELD-php**    |      1.65"   | 99.16%       |
@@ -175,8 +161,9 @@
 
 
 ## Future improvements
 
 - Train from bigger datasets, and more languages.
 - The tokenizer could separate characters from languages that have their own alphabet, potentially improving accuracy and reducing the N-grams database. Retraining and testing is needed.
 
-If you wish to Donate for open source improvements, Hire me for private modifications / upgrades, or to Contact me, use the following link: https://linktr.ee/nitotm
+**Donate / Hire**   
+If you wish to Donate for open source improvements, Hire me for private modifications / upgrades, or to Contact me, use the following link: https://linktr.ee/nitotm
```

### Comparing `eld-0.9.0/README.md` & `eld-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,35 @@
+Metadata-Version: 2.1
+Name: eld
+Version: 0.9.1
+Summary: Fast and accurate natural language detection. Detector written in Python. Nito-ELD, ELD.
+Home-page: https://github.com/nitotm/efficient-language-detector-py/
+Author: Nito T.M.
+Keywords: nlp language natural-language-processing natural-language language-detection language-detector language-identification
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Efficient Language Detector
 
 <div align="center">
 	
 ![supported Python versions](https://img.shields.io/badge/Python-%3E%3D%203.7-blue)
 [![license](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
-[![supported languages](https://img.shields.io/badge/supported%20languages-60-green.svg)](#languages)
+[![supported languages](https://img.shields.io/badge/supported%20languages-60-brightgreen.svg)](#languages)
 	
 </div>
 
-Efficient language detector (Nito-ELD or ELD) is a fast and accurate language detector, is one of the fastest non compiled detectors, while its accuracy is within the range of the heaviest and slowest detectors.
+Efficient language detector (*Nito-ELD* or *ELD*) is a fast and accurate language detector, is one of the fastest non compiled detectors, while its accuracy is within the range of the heaviest and slowest detectors.
 
 It's 100% Python, easy installation and no dependencies other than `regex`.  
-ELD is also avalible in [Javascript](https://github.com/nitotm/efficient-language-detector-js/) and [PHP](https://github.com/nitotm/efficient-language-detector/).
+ELD is also available in [Javascript](https://github.com/nitotm/efficient-language-detector-js) and [PHP](https://github.com/nitotm/efficient-language-detector).
 
 > This is the first version of a port made from the original version in PHP, the structure might not be definitive, the code can be optimized. My knowledge of Python is basic, feel free to suggest improvements.
 
 1. [Installation](#installation)
 2. [How to use](#how-to-use)
 3. [Benchmarks](#benchmarks)
 4. [Languages](#languages)
@@ -32,21 +46,21 @@
 ```python
 # from src.eld.languageDetector import LanguageDetector # To load ELD without install. Update path.
 from eld import LanguageDetector
 detector = LanguageDetector()
 
 print(detector.detect('Hola, cómo te llamas?'))
 ```
-`detect()` expects an UTF-8 string, and returns a list, with a value named 'language', which will be either an *ISO 639-1 code* or `False`
+`detect()` expects a UTF-8 string, and returns a list, with a value named 'language', which will be either an *ISO 639-1 code* or `False`
 ```
 {'language': 'es'}
 {'language': False, 'error': 'Some error', 'scores': {}}
 ```
 
-- To get the best guess, deactive minimum length & confidence threshold; used for benchmarking.
+- To get the best guess, turn off minimum length & confidence threshold; also used for benchmarking.
 ```python
 print(detector.detect('To', False, False, 0, 1))
 # To improve readability Named Parameters can be used
 detector.detect(text='To', clean_text=False, check_confidence=False, min_byte_length=0, min_ngrams=1)
 # clean_text=True, Removes Urls, domains, emails, alphanumerical & numbers
 ```
 
@@ -55,46 +69,46 @@
 detector.return_scores = True
 print(detector.detect('How are you? Bien, gracias'))
 # {'language': 'en', 'scores': {'en': 0.32, 'es': 0.31, ...}}
 ```
 
 - To reduce the languages to be detected, there are 3 different options, they only need to be executed once. (Check available [languages](#languages) below)
 ```python
-langs_subset = ['en', 'es', 'fr', 'it', 'nl', 'de']
+lang_subset = ['en', 'es', 'fr', 'it', 'nl', 'de']
 
-# with dynamic_langs_subset() the detector executes normally, and then filters excluded languages
-detector.dynamic_langs_subset(langs_subset)
+# with dynamic_lang_subset() the detector executes normally, and then filters excluded languages
+detector.dynamic_lang_subset(lang_subset)
 
-# langs_subset() Will first remove the excluded languages, from the n-grams database
-# For a single detection is slower than dynamic_langs_subset(), but for several will be faster
+# lang_subset() Will first remove the excluded languages, from the n-grams database
+# For a single detection is slower than dynamic_lang_subset(), but for several will be faster
 # If save option is true (default), the new Ngrams subset will be stored, and loaded next call
-detector.langs_subset(langs_subset) # langs_subset(langs, save=True) 
+detector.lang_subset(lang_subset) # lang_subset(langs, save=True) 
 
-# To remove either dynamic_langs_subset() or langs_subset(), call the methods with False as argument
-detector.langs_subset(False); 
+# To remove either dynamic_lang_subset() or lang_subset(), call the methods with False as argument
+detector.lang_subset(False)
 
 # Finally the fastest way to regularly use a languages subset: we create the instance with a file
-# The file in the argument can be a subset by langs_subset() or another database like ngrams_L.php
+# The file in the argument can be a subset by lang_subset() or another database like ngrams_L.php
 langSubsetDetect = LanguageDetector('ngrams_2f37045c74780aba1d36d6717f3244dc025fb935')
 ```
 
 ## Benchmarks
 
 I compared *ELD* with a different variety of detectors, since the interesting part is the algorithm.
 
-| URL                                                       | Version       | Language     |
-| :-                                                        | :-            | :-           |
-| https://github.com/nitotm/efficient-language-detector-py/ | 0.9.0         | Python       |
-| https://github.com/nitotm/efficient-language-detector/    | 1.0.0         | PHP          |
-| https://github.com/pemistahl/lingua-py                    | 1.3.2         | Python       |
-| https://github.com/CLD2Owners/cld2                        | Aug 21, 2015  | C++          |
-| https://github.com/google/cld3                            | Aug 28, 2020  | C++          |
-| https://github.com/wooorm/franc                           | 6.1.0         | Javasript    |
+| URL                                                       | Version      | Language   |
+|:----------------------------------------------------------|:-------------|:-----------|
+| https://github.com/nitotm/efficient-language-detector-py/ | 0.9.0        | Python     |
+| https://github.com/nitotm/efficient-language-detector/    | 1.0.0        | PHP        |
+| https://github.com/pemistahl/lingua-py                    | 1.3.2        | Python     |
+| https://github.com/CLD2Owners/cld2                        | Aug 21, 2015 | C++        |
+| https://github.com/google/cld3                            | Aug 28, 2020 | C++        |
+| https://github.com/wooorm/franc                           | 6.1.0        | Javascript |
 
-Tests: **Tweets**: *760KB*, short sentences of 140 chars max.; **Big test**: *10MB*, sentences in all 60 languages supported; **Sentences**: *8MB*, this is the *Lingua* sentences test, minus unsupported languages.  
+Benchmarks: **Tweets**: *760KB*, short sentences of 140 chars max.; **Big test**: *10MB*, sentences in all 60 languages supported; **Sentences**: *8MB*, this is the *Lingua* sentences test, minus unsupported languages.  
 Short sentences is what *ELD* and most detectors focus on, as very short text is unreliable, but I included the *Lingua* **Word pairs** *1.5MB*, and **Single words** *880KB* tests to see how they all compare beyond their reliable limits.
 
 These are the results, first, accuracy and then execution time.
 
 <!-- Accuracy table
 |                     | Tweets       | Big test     | Sentences    | Word pairs   | Single words |
 |:--------------------|:------------:|:------------:|:------------:|:------------:|:------------:|
@@ -102,42 +116,42 @@
 | **Nito-ELD-L**      | 99.4%        | 99.4%        | 98.7%        | 89.4%        | 76.1%        |
 | **Lingua**          | 98.8%        | 99.1%        | 98.6%        | 93.1%        | 80.0%        |
 | **CLD2**            | 93.8%        | 97.2%        | 97.2%        | 87.7%        | 69.6%        |
 | **Lingua low**      | 96.0%        | 97.2%        | 96.3%        | 83.7%        | 68.0%        |
 | **CLD3**            | 92.2%        | 95.8%        | 94.7%        | 69.0%        | 51.5%        |
 | **franc**           | 89.8%        | 92.0%        | 90.5%        | 65.9%        | 52.9%        |
 -->
-<img width="800" src="https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/table_accuracy_py.svg">
+<img alt="accuracy table" width="800" src="https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/table_accuracy_py.svg">
 
 <!--- Time table
 |                     | Tweets       | Big test     | Sentences    | Word pairs   | Single words |
 |:--------------------|:------------:|:------------:|:------------:|:------------:|:------------:|
 | **Nito-ELD-py**     |     0.96"    |      7.8"    |      6.7"    |     2.6"     |     2.1"     |
 | **Nito-ELD-L-py**   |     1"       |      8"      |      6.9"    |     2.7"     |     2.1"     |
 | **Lingua**          |  4790"       |  24000"      |  18700"      |  8450"       |  6700"       |
 | **CLD2**            |     0.35"    |      2"      |      1.7"    |     0.98"    |     0.8"     |
 | **Lingua low**      |    64"       |    370"      |    308"      |   108"       |    85"       |
 | **CLD3**            |     3.9"     |     29"      |     26"      |    12"       |    11"       |
 | **franc**           |     1.2"     |      8"      |      7.8"    |     2.8"     |     2"       |
 | **Nito-ELD-php**    |     0.31"    |      2.5"    |      2.2"    |     0.66"    |     0.48"    |
 -->
-<img width="800" src="https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/table_time_py.svg">
+<img alt="time table" width="800" src="https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/table_time_py.svg">
 
 <sup style="color:#08e">1.</sup> <sup style="color:#777">Lingua could have a small advantage as it participates with 54 languages, 6 less.</sup>  
 <sup style="color:#08e">2.</sup> <sup style="color:#777">CLD2 and CLD3, return a list of languages, the ones not included in this test where discarded, but usually they return one language, I believe they have a disadvantage. 
 Also, I confirm the results of CLD2 for short text are correct, contrary to the test on the *Lingua* page, they did not use the parameter "bestEffort = True", their benchmark for CLD2 is unfair.
 
 *Lingua* is the average accuracy winner, but at what cost, the same test that in *ELD* or *CLD2* is below 10 seconds, in Lingua takes more than 5 hours! It acts like a brute-force software. 
-Also its lead comes from single and pair words, which are unreliable regardless.
+Also, its lead comes from single and pair words, which are unreliable regardless.
 
 The Python version of *NITO-ELD* is not the fastest but is still considered fast, as it is faster than any other non compiled detector tested.
 
 I added *ELD-L* for comparison, which has a 2.3x bigger database, but only increases execution time marginally, a testament to the efficiency of the algorithm. *ELD-L* is not the main database as it does not improve language detection in sentences.
 
-Here is the average, per test, of Tweets, Big test & Sentences.
+Here is the average, per benchmark, of Tweets, Big test & Sentences.
 
 ![Sentences tests average](https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/sentences_avg_py.png)
 <!--- Sentences average
 |                     | Time         | Accuracy     |
 |:--------------------|:------------:|:------------:|
 | **Nito-ELD-py**     |      5.17"   | 99.16%       |
 | **Nito-ELD-php**    |      1.65"   | 99.16%       |
@@ -161,8 +175,9 @@
 
 
 ## Future improvements
 
 - Train from bigger datasets, and more languages.
 - The tokenizer could separate characters from languages that have their own alphabet, potentially improving accuracy and reducing the N-grams database. Retraining and testing is needed.
 
-If you wish to Donate for open source improvements, Hire me for private modifications / upgrades, or to Contact me, use the following link: https://linktr.ee/nitotm
+**Donate / Hire**   
+If you wish to Donate for open source improvements, Hire me for private modifications / upgrades, or to Contact me, use the following link: https://linktr.ee/nitotm
```

### Comparing `eld-0.9.0/demo.py` & `eld-0.9.1/demo.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from src.eld.languageDetector import LanguageDetector
-#from eld import LanguageDetector
+# from eld import LanguageDetector
 
 detector = LanguageDetector()
 
-# detect() expects an UTF-8 string, and returns a dictionary, with a value named 'language', which will be either an ISO 639-1 code or false
+# detect() expects a UTF-8 string, and returns a dictionary, with key 'language', value: ISO 639-1 code or false
 print(detector.detect('Hola, cómo te llamas?'))
 # {'language': 'es'}
 # {'language': False, 'error': 'Some error', 'scores': {}}
 
-# To get the best guess, deactivating minimum length, confidence threshold and also for benchmarking.
+# To get the best guess, turn off minimum length and confidence threshold; also used for benchmarking.
 print(detector.detect('To', False, False, 0, 1))
 
 # To improve readability Named Parameters can be used
 detector.detect(text='To', clean_text=False, check_confidence=False, min_byte_length=0, min_ngrams=1)
 # clean_text=True, Removes Urls, domains, emails, alphanumerical & numbers
 
 # To retrieve the scores of all languages detected, we will set returnScores to True, just once
@@ -40,31 +40,30 @@
 # To reduce the languages to be detected, there are 3 different options, they only need to be executed once.
 # This is the complete list on languages for ELD v1, using ISO 639-1 codes:
 """ ['am', 'ar', 'az', 'be', 'bg', 'bn', 'ca', 'cs', 'da', 'de', 'el', 'en', 'es', 'et', 'eu', 'fa', 'fi', 'fr', 'gu',
  'he', 'hi', 'hr', 'hu', 'hy', 'is', 'it', 'ja', 'ka', 'kn', 'ko', 'ku', 'lo', 'lt', 'lv', 'ml', 'mr', 'ms', 'nl', 'no',
  'or', 'pa', 'pl', 'pt', 'ro', 'ru', 'sk', 'sl', 'sq', 'sr', 'sv', 'ta', 'te', 'th', 'tl', 'tr', 'uk', 'ur', 'vi', 'yo',
  'zh']
 """
-langs_subset = ['en', 'es', 'fr', 'it', 'nl', 'de']
+lang_subset = ['en', 'es', 'fr', 'it', 'nl', 'de']
 
-# dynamic_langs_subset() Will execute the detector normally, but at the end will filter the excluded languages.
-detector.dynamic_langs_subset(langs_subset)
+# dynamic_lang_subset() Will execute the detector normally, but at the end will filter the excluded languages.
+detector.dynamic_lang_subset(lang_subset)
 
 # to remove the subset
-detector.dynamic_langs_subset(False)
+detector.dynamic_lang_subset(False)
 
-""" langs_subset(langs,save=True) Will previously remove the excluded languages form the Ngrams database; for a single
- detection might be slower than dynamic_langs_subset(), but for several strings will be faster. If save option is true
+""" lang_subset(langs,save=True) Will previously remove the excluded languages form the Ngrams database; for a single
+ detection might be slower than dynamic_lang_subset(), but for several strings will be faster. If save option is true
 (default), the new ngrams subset will be stored, and loaded for the same languages subset, increasing startup speed
 """
-detector.langs_subset(langs_subset)
+detector.lang_subset(lang_subset)
 
 # to remove the subset
-detector.langs_subset(False)
+detector.lang_subset(False)
 
-""" Finally the fastest option to regularly use the same languages subset, will be to add as an argument the file 
-   stored by langs_subset(), when creating an instance of the class. In this case the subset Ngrams database will
+""" Finally the fastest option to regularly use the same language subset, will be to add as an argument the file 
+   stored by lang_subset(), when creating an instance of the class. In this case the subset Ngrams database will
    be loaded directly, and not the default database. Also, you can use this option to load different ngram databases
-	stored at src/ngrams/
+   stored at src/ngrams/
 """
 langSubsetDetect = LanguageDetector('ngrams_2f37045c74780aba1d36d6717f3244dc025fb935')
-
```

### Comparing `eld-0.9.0/src/eld/languageDetector.py` & `eld-0.9.1/src/eld/languageDetector.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import regex as re
 
-from .languagesData import languagesData
-from .languagesSubset import LanguagesSubset
+from .languageData import languageData
+from .languageSubset import LanguageSubset
 
 
-class LanguageDetector(LanguagesSubset):
+class LanguageDetector(LanguageSubset):
     def __init__(self, subset_file=''):
         self.return_scores = False
-        LanguagesSubset.subset = False
-        LanguagesSubset.loadedSubset = False
-        LanguagesSubset.defaultNgrams = False
-        languagesData.load_ngrams(subset_file)
+        LanguageSubset.subset = False
+        LanguageSubset.loadedSubset = False
+        LanguageSubset.defaultNgrams = False
+        languageData.load_ngrams(subset_file)
 
     """
       detect() returns a dictionary, with a value named 'language', which will be either a ISO 639-1 code or False
       {'language': 'en'}
       {'language': False, 'error': 'Some error', 'scores': {}}
 
       When return_scores = True;
@@ -60,86 +60,86 @@
         txt_ngrams = get_byte_ngrams(text)
         num_ngrams = len(txt_ngrams)
 
         if num_ngrams >= min_ngrams:
             results = calc_scores(txt_ngrams, num_ngrams)
 
             if self.subset:
-                results = LanguagesSubset.filter_langs_subset(self, results)
+                results = LanguageSubset.filter_lang_subset(self, results)
 
             results.sort(key=lambda x: -x[1])
 
             if results:
                 top_lang = results[0][0]
                 # Minimum confidence threshold. 
                 if check_confidence:
-                    # A minimum of a 17% per ngram score from average
+                    # A minimum of a 24% per ngram score from average
                     next_score = (results[1][0] if len(results) > 1 else 0)
-                    if (languagesData.avgScore[top_lang] * 0.17 > (results[0][1] / num_ngrams) or 0.01 > abs(
+                    if (languageData.avgScore[top_lang] * 0.24 > (results[0][1] / num_ngrams) or 0.01 > abs(
                             results[0][1] - next_score)):
                         return {'language': False,
                                 'error': "No language has been identified with sufficient confidence,"
                                          " set checkConfidence to false to avoid this error",
                                 'scores': []}
                 if not self.return_scores:
-                    return {'language': languagesData.langCodes[top_lang]}
+                    return {'language': languageData.langCodes[top_lang]}
                 else:
-                    return {'language': languagesData.langCodes[top_lang], 'scores': get_scores(results)}
+                    return {'language': languageData.langCodes[top_lang], 'scores': get_scores(results)}
             return {'language': False, 'error': 'Language not detected', 'scores': {}}
         return {'language': False, 'error': 'Not enough distinct ngrams', 'scores': {}}
 
 
 def tokenizer(txt):
     return filter(None, re.split(b'\x20', txt))
 
 
 def clean_txt(txt):
     # Remove URLS
     txt = re.sub(r'[hw]((ttps?://(www\.)?)|ww\.)([^\s/?\.#-]+\.?)+(\/\S*)?', ' ', txt, flags=re.IGNORECASE)
     # Remove emails
     txt = re.sub(r'[a-zA-Z0-9.!$%&?+_`-]+@[A-Za-z0-9.-]+\.[A-Za-z0-9-]{2,64}', ' ', txt)
-    # Remove domains
+    # Remove .com domains
     txt = re.sub(r'([A-Za-z0-9-]+\.)+com(\/\S*|[^\pL])', ' ', txt)
     # Remove alphanumerical/number codes
     txt = re.sub(r'[a-zA-Z]*[0-9]+[a-zA-Z0-9]*', ' ', txt)
     return txt
 
 
 def get_scores(array):
     scores = {}
     for value in array:
         if value[1] == 0:
             break
-        scores[languagesData.langCodes[value[0]]] = value[1]
+        scores[languageData.langCodes[value[0]]] = value[1]
     return scores
 
 
 def calc_scores(txt_ngrams, num_ngrams):
-    lang_score = languagesData.langScore[:]
+    lang_score = languageData.langScore[:]
     for nbytes, frequency in txt_ngrams.items():
-        if nbytes in languagesData.ngrams:
-            num_langs = len(languagesData.ngrams[nbytes])
+        if nbytes in languageData.ngrams:
+            num_langs = len(languageData.ngrams[nbytes])
             # Ngram score multiplier, the fewer languages found the more relevancy. Formula can be fine-tuned.
             if num_langs == 1:
                 relevancy = 27
             elif num_langs < 16:
                 relevancy = (16 - num_langs) / 2 + 1
             else:
                 relevancy = 1
 
             # Most time-consuming loop, do only the strictly necessary inside
-            for lang, ngramFrequency in languagesData.ngrams[nbytes].items():
+            for lang, ngramFrequency in languageData.ngrams[nbytes].items():
                 lang_score[lang] += (ngramFrequency / frequency if frequency > ngramFrequency
                                      else frequency / ngramFrequency) * relevancy + 2
     # This divisor will produce a final score between 0 - ~1, score could be >1. Can be improved.
     result_divisor = num_ngrams * 3.2
     results = []
     for lang in range(len(lang_score)):
         if lang_score[lang]:
-            results.append([lang, lang_score[lang] / result_divisor])  # * languagesData.scoreNormalizer[lang]
+            results.append([lang, lang_score[lang] / result_divisor])  # * languageData.scoreNormalizer[lang]
     return results
 
 
 def get_byte_ngrams(txt):
     tokens = {}
     count_ngrams = 0
```

### Comparing `eld-0.9.0/src/eld/languagesData.py` & `eld-0.9.1/src/eld/languageData.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import importlib
+import importlib.util
 import os
 
 
-class LanguagesData:
+class LanguageData:
     def __init__(self):
         self.ngrams = None
         # ISO 639-1 codes
         self.langCodes = ['am', 'ar', 'az', 'be', 'bg', 'bn', 'ca', 'cs', 'da', 'de', 'el', 'en', 'es', 'et', 'eu',
                           'fa', 'fi', 'fr', 'gu', 'he', 'hi', 'hr', 'hu', 'hy', 'is', 'it', 'ja', 'ka', 'kn', 'ko',
                           'ku', 'lo', 'lt', 'lv', 'ml', 'mr', 'ms', 'nl', 'no', 'or', 'pa', 'pl', 'pt', 'ro', 'ru',
                           'sk', 'sl', 'sq', 'sr', 'sv', 'ta', 'te', 'th', 'tl', 'tr', 'uk', 'ur', 'vi', 'yo', 'zh']
         """ 
-			['Amharic', 'Arabic', 'Azerbaijani (Latin)', 'Belarusian', 'Bulgarian', 'Bengali', 'Catalan', 'Czech',
+         ['Amharic', 'Arabic', 'Azerbaijani (Latin)', 'Belarusian', 'Bulgarian', 'Bengali', 'Catalan', 'Czech',
          'Danish', 'German', 'Greek', 'English', 'Spanish', 'Estonian', 'Basque', 'Persian', 'Finnish', 'French',
          'Gujarati', 'Hebrew', 'Hindi', 'Croatian', 'Hungarian', 'Armenian', 'Icelandic', 'Italian', 'Japanese',
          'Georgian', 'Kannada', 'Korean', 'Kurdish (Arabic)', 'Lao', 'Lithuanian', 'Latvian', 'Malayalam', 'Marathi',
          'Malay (Latin)', 'Dutch', 'Norwegian', 'Oriya', 'Punjabi', 'Polish', 'Portuguese', 'Romanian', 'Russian',
          'Slovak', 'Slovene', 'Albanian', 'Serbian (Cyrillic)', 'Swedish', 'Tamil', 'Telugu', 'Thai', 'Tagalog',
          'Turkish', 'Ukrainian', 'Urdu', 'Vietnamese', 'Yoruba', 'Chinese']
         """
@@ -53,16 +53,16 @@
                          0.0234, 0.033, 0.1513, 0.1547, 0.0882, 0.0368, 0.0258, 0.0206, 0.0282, 0.0467, 0.0329, 0.0152]
 
     def load_ngrams(self, subset_file=''):
         if subset_file == '':
             from .ngrams.ngrams_m import ngrams
             self.ngrams = ngrams
         else:
-            #module = importlib.import_module('.ngrams.' + subset_file)
-            file_path = os.path.dirname(__file__)+'/ngrams/' + subset_file + '.py'
+            # module = importlib.import_module('.ngrams.' + subset_file)
+            file_path = os.path.dirname(__file__) + '/ngrams/' + subset_file + '.py'
             spec = importlib.util.spec_from_file_location(subset_file, file_path)
             module = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(module)
             self.ngrams = module.ngrams
 
 
-languagesData = LanguagesData()
+languageData = LanguageData()
```

### Comparing `eld-0.9.0/src/eld/languagesSubset.py` & `eld-0.9.1/src/eld/languageSubset.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,95 +14,95 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import hashlib
 import os
 import copy
-import importlib
+import importlib.util
 
-from .languagesData import languagesData
+from .languageData import languageData
 
 """
 To reduce the languages to be detected, there are 3 different options, they only need to be execute once.
 
-The fastest option to regularly use the same languages subset, will be to add as an argument the file stored 
-(and returned) by langs_subset(), when creating an instance of the languageDetector class. 
+The fastest option to regularly use the same language subset, will be to add as an argument the file stored 
+(and returned) by lang_subset(), when creating an instance of the languageDetector class. 
   In this case the subset ngrams database will be loaded directly, and not the default database. 
   Also you can use this option to load different ngram databases.
 """
 
 
-class LanguagesSubset:
+class LanguageSubset:
 
-    # dynamic_langs_subset() Will execute the detector normally, but at the end it will filter the excluded languages.
-    def dynamic_langs_subset(self, langs):
+    # dynamic_lang_subset() Will execute the detector normally, but at the end it will filter the excluded languages.
+    def dynamic_lang_subset(self, langs):
         self.subset = []
         if not langs:
             langs = []
         for value in langs:
-            if value in languagesData.langCodes:
-                self.subset.append(languagesData.langCodes.index(value))
+            if value in languageData.langCodes:
+                self.subset.append(languageData.langCodes.index(value))
         self.subset.sort()
         return self.subset
 
-    """ langs_subset(langs,save=true) Will previously remove the excluded languages form the ngrams database; for a
-     single detection might be slower than dynamic_langs_subset(), but for multiple strings will be faster. if 'save' 
+    """ lang_subset(langs,save=true) Will previously remove the excluded languages form the ngrams database; for a
+     single detection might be slower than dynamic_lang_subset(), but for multiple strings will be faster. if 'save' 
      option is true (default), the new ngrams subset will be stored, and next loaded for the same languages subset,
      increasing startup speed.
     """
-    def langs_subset(self, langs, save=True):
+    def lang_subset(self, langs, save=True):
         if not langs:
             if self.loadedSubset:
-                languagesData.ngrams = copy.deepcopy(self.defaultNgrams)
+                languageData.ngrams = copy.deepcopy(self.defaultNgrams)
                 self.loadedSubset = False
             return True
         
-        langs_array = self.dynamic_langs_subset(langs)
+        langs_array = self.dynamic_lang_subset(langs)
         if not langs_array:
             return 'No languages found'
-        self.subset = False  # We use dynamic_langs_subset() to filter languages, but set dynamic subset to false
+        self.subset = False  # We use dynamic_lang_subset() to filter languages, but set dynamic subset to false
         if self.defaultNgrams is False:
-            self.defaultNgrams = copy.deepcopy(languagesData.ngrams)
+            self.defaultNgrams = copy.deepcopy(languageData.ngrams)
 
         langs_str = [str(lang) for lang in langs_array]
         new_subset = hashlib.sha1(','.join(langs_str).encode()).hexdigest()
         file_name = 'ngrams_' + new_subset
         file_path = os.path.dirname(__file__)+'/ngrams/' + file_name + '.py'
 
         if self.loadedSubset != new_subset:
             self.loadedSubset = new_subset
 
             if os.path.exists(file_path):
-                #module = importlib.import_module('.ngrams.' + file_name, package=file_name)
+                # module = importlib.import_module('.ngrams.' + file_name, package=file_name)
                 spec = importlib.util.spec_from_file_location(file_name, file_path)
                 module = importlib.util.module_from_spec(spec)
                 spec.loader.exec_module(module)
-                languagesData.ngrams = module.ngrams
+                languageData.ngrams = module.ngrams
                 return
 
-            if self.defaultNgrams != languagesData.ngrams:
-                languagesData.ngrams = copy.deepcopy(self.defaultNgrams)
+            if self.defaultNgrams != languageData.ngrams:
+                languageData.ngrams = copy.deepcopy(self.defaultNgrams)
 
             for ngram, langsID in self.defaultNgrams.items():
                 for lid, value in langsID.items():
                     if lid not in langs_array:
-                        del languagesData.ngrams[ngram][lid]
-                if not languagesData.ngrams[ngram]:
-                    del languagesData.ngrams[ngram]
+                        del languageData.ngrams[ngram][lid]
+                if not languageData.ngrams[ngram]:
+                    del languageData.ngrams[ngram]
 
         if save:
             if not os.path.exists(file_path):  # in case self.loadedSubset != new_subset, and was previously saved
                 with open(file_path, 'w') as f:
-                    f.write('ngrams = ' + self.ngram_export(languagesData.ngrams))
+                    f.write('ngrams = ' + self.ngram_export(languageData.ngrams))
             return file_path
 
         return True
 
-    def filter_langs_subset(self, results):
+    def filter_lang_subset(self, results):
         sub_results = []
         for value in results:
             if value[0] in self.subset:
                 sub_results.append(value)
         return sub_results
 
     def ngram_export(self, var, safe=False):
```

### Comparing `eld-0.9.0/src/eld/ngrams/ngrams_2f37045c74780aba1d36d6717f3244dc025fb935.py` & `eld-0.9.1/src/eld/ngrams/ngrams_2f37045c74780aba1d36d6717f3244dc025fb935.py`

 * *Files identical despite different names*

### Comparing `eld-0.9.0/src/eld/ngrams/ngrams_L.py` & `eld-0.9.1/src/eld/ngrams/ngrams_L.py`

 * *Files identical despite different names*

### Comparing `eld-0.9.0/src/eld/ngrams/ngrams_m.py` & `eld-0.9.1/src/eld/ngrams/ngrams_m.py`

 * *Files identical despite different names*

### Comparing `eld-0.9.0/src/eld.egg-info/PKG-INFO` & `eld-0.9.1/src/eld.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eld
-Version: 0.9.0
+Version: 0.9.1
 Summary: Fast and accurate natural language detection. Detector written in Python. Nito-ELD, ELD.
 Home-page: https://github.com/nitotm/efficient-language-detector-py/
 Author: Nito T.M.
 Keywords: nlp language natural-language-processing natural-language language-detection language-detector language-identification
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,22 +14,22 @@
 
 # Efficient Language Detector
 
 <div align="center">
 	
 ![supported Python versions](https://img.shields.io/badge/Python-%3E%3D%203.7-blue)
 [![license](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
-[![supported languages](https://img.shields.io/badge/supported%20languages-60-green.svg)](#languages)
+[![supported languages](https://img.shields.io/badge/supported%20languages-60-brightgreen.svg)](#languages)
 	
 </div>
 
-Efficient language detector (Nito-ELD or ELD) is a fast and accurate language detector, is one of the fastest non compiled detectors, while its accuracy is within the range of the heaviest and slowest detectors.
+Efficient language detector (*Nito-ELD* or *ELD*) is a fast and accurate language detector, is one of the fastest non compiled detectors, while its accuracy is within the range of the heaviest and slowest detectors.
 
 It's 100% Python, easy installation and no dependencies other than `regex`.  
-ELD is also avalible in [Javascript](https://github.com/nitotm/efficient-language-detector-js/) and [PHP](https://github.com/nitotm/efficient-language-detector/).
+ELD is also available in [Javascript](https://github.com/nitotm/efficient-language-detector-js) and [PHP](https://github.com/nitotm/efficient-language-detector).
 
 > This is the first version of a port made from the original version in PHP, the structure might not be definitive, the code can be optimized. My knowledge of Python is basic, feel free to suggest improvements.
 
 1. [Installation](#installation)
 2. [How to use](#how-to-use)
 3. [Benchmarks](#benchmarks)
 4. [Languages](#languages)
@@ -46,21 +46,21 @@
 ```python
 # from src.eld.languageDetector import LanguageDetector # To load ELD without install. Update path.
 from eld import LanguageDetector
 detector = LanguageDetector()
 
 print(detector.detect('Hola, cómo te llamas?'))
 ```
-`detect()` expects an UTF-8 string, and returns a list, with a value named 'language', which will be either an *ISO 639-1 code* or `False`
+`detect()` expects a UTF-8 string, and returns a list, with a value named 'language', which will be either an *ISO 639-1 code* or `False`
 ```
 {'language': 'es'}
 {'language': False, 'error': 'Some error', 'scores': {}}
 ```
 
-- To get the best guess, deactive minimum length & confidence threshold; used for benchmarking.
+- To get the best guess, turn off minimum length & confidence threshold; also used for benchmarking.
 ```python
 print(detector.detect('To', False, False, 0, 1))
 # To improve readability Named Parameters can be used
 detector.detect(text='To', clean_text=False, check_confidence=False, min_byte_length=0, min_ngrams=1)
 # clean_text=True, Removes Urls, domains, emails, alphanumerical & numbers
 ```
 
@@ -69,46 +69,46 @@
 detector.return_scores = True
 print(detector.detect('How are you? Bien, gracias'))
 # {'language': 'en', 'scores': {'en': 0.32, 'es': 0.31, ...}}
 ```
 
 - To reduce the languages to be detected, there are 3 different options, they only need to be executed once. (Check available [languages](#languages) below)
 ```python
-langs_subset = ['en', 'es', 'fr', 'it', 'nl', 'de']
+lang_subset = ['en', 'es', 'fr', 'it', 'nl', 'de']
 
-# with dynamic_langs_subset() the detector executes normally, and then filters excluded languages
-detector.dynamic_langs_subset(langs_subset)
+# with dynamic_lang_subset() the detector executes normally, and then filters excluded languages
+detector.dynamic_lang_subset(lang_subset)
 
-# langs_subset() Will first remove the excluded languages, from the n-grams database
-# For a single detection is slower than dynamic_langs_subset(), but for several will be faster
+# lang_subset() Will first remove the excluded languages, from the n-grams database
+# For a single detection is slower than dynamic_lang_subset(), but for several will be faster
 # If save option is true (default), the new Ngrams subset will be stored, and loaded next call
-detector.langs_subset(langs_subset) # langs_subset(langs, save=True) 
+detector.lang_subset(lang_subset) # lang_subset(langs, save=True) 
 
-# To remove either dynamic_langs_subset() or langs_subset(), call the methods with False as argument
-detector.langs_subset(False); 
+# To remove either dynamic_lang_subset() or lang_subset(), call the methods with False as argument
+detector.lang_subset(False)
 
 # Finally the fastest way to regularly use a languages subset: we create the instance with a file
-# The file in the argument can be a subset by langs_subset() or another database like ngrams_L.php
+# The file in the argument can be a subset by lang_subset() or another database like ngrams_L.php
 langSubsetDetect = LanguageDetector('ngrams_2f37045c74780aba1d36d6717f3244dc025fb935')
 ```
 
 ## Benchmarks
 
 I compared *ELD* with a different variety of detectors, since the interesting part is the algorithm.
 
-| URL                                                       | Version       | Language     |
-| :-                                                        | :-            | :-           |
-| https://github.com/nitotm/efficient-language-detector-py/ | 0.9.0         | Python       |
-| https://github.com/nitotm/efficient-language-detector/    | 1.0.0         | PHP          |
-| https://github.com/pemistahl/lingua-py                    | 1.3.2         | Python       |
-| https://github.com/CLD2Owners/cld2                        | Aug 21, 2015  | C++          |
-| https://github.com/google/cld3                            | Aug 28, 2020  | C++          |
-| https://github.com/wooorm/franc                           | 6.1.0         | Javasript    |
+| URL                                                       | Version      | Language   |
+|:----------------------------------------------------------|:-------------|:-----------|
+| https://github.com/nitotm/efficient-language-detector-py/ | 0.9.0        | Python     |
+| https://github.com/nitotm/efficient-language-detector/    | 1.0.0        | PHP        |
+| https://github.com/pemistahl/lingua-py                    | 1.3.2        | Python     |
+| https://github.com/CLD2Owners/cld2                        | Aug 21, 2015 | C++        |
+| https://github.com/google/cld3                            | Aug 28, 2020 | C++        |
+| https://github.com/wooorm/franc                           | 6.1.0        | Javascript |
 
-Tests: **Tweets**: *760KB*, short sentences of 140 chars max.; **Big test**: *10MB*, sentences in all 60 languages supported; **Sentences**: *8MB*, this is the *Lingua* sentences test, minus unsupported languages.  
+Benchmarks: **Tweets**: *760KB*, short sentences of 140 chars max.; **Big test**: *10MB*, sentences in all 60 languages supported; **Sentences**: *8MB*, this is the *Lingua* sentences test, minus unsupported languages.  
 Short sentences is what *ELD* and most detectors focus on, as very short text is unreliable, but I included the *Lingua* **Word pairs** *1.5MB*, and **Single words** *880KB* tests to see how they all compare beyond their reliable limits.
 
 These are the results, first, accuracy and then execution time.
 
 <!-- Accuracy table
 |                     | Tweets       | Big test     | Sentences    | Word pairs   | Single words |
 |:--------------------|:------------:|:------------:|:------------:|:------------:|:------------:|
@@ -116,42 +116,42 @@
 | **Nito-ELD-L**      | 99.4%        | 99.4%        | 98.7%        | 89.4%        | 76.1%        |
 | **Lingua**          | 98.8%        | 99.1%        | 98.6%        | 93.1%        | 80.0%        |
 | **CLD2**            | 93.8%        | 97.2%        | 97.2%        | 87.7%        | 69.6%        |
 | **Lingua low**      | 96.0%        | 97.2%        | 96.3%        | 83.7%        | 68.0%        |
 | **CLD3**            | 92.2%        | 95.8%        | 94.7%        | 69.0%        | 51.5%        |
 | **franc**           | 89.8%        | 92.0%        | 90.5%        | 65.9%        | 52.9%        |
 -->
-<img width="800" src="https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/table_accuracy_py.svg">
+<img alt="accuracy table" width="800" src="https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/table_accuracy_py.svg">
 
 <!--- Time table
 |                     | Tweets       | Big test     | Sentences    | Word pairs   | Single words |
 |:--------------------|:------------:|:------------:|:------------:|:------------:|:------------:|
 | **Nito-ELD-py**     |     0.96"    |      7.8"    |      6.7"    |     2.6"     |     2.1"     |
 | **Nito-ELD-L-py**   |     1"       |      8"      |      6.9"    |     2.7"     |     2.1"     |
 | **Lingua**          |  4790"       |  24000"      |  18700"      |  8450"       |  6700"       |
 | **CLD2**            |     0.35"    |      2"      |      1.7"    |     0.98"    |     0.8"     |
 | **Lingua low**      |    64"       |    370"      |    308"      |   108"       |    85"       |
 | **CLD3**            |     3.9"     |     29"      |     26"      |    12"       |    11"       |
 | **franc**           |     1.2"     |      8"      |      7.8"    |     2.8"     |     2"       |
 | **Nito-ELD-php**    |     0.31"    |      2.5"    |      2.2"    |     0.66"    |     0.48"    |
 -->
-<img width="800" src="https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/table_time_py.svg">
+<img alt="time table" width="800" src="https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/table_time_py.svg">
 
 <sup style="color:#08e">1.</sup> <sup style="color:#777">Lingua could have a small advantage as it participates with 54 languages, 6 less.</sup>  
 <sup style="color:#08e">2.</sup> <sup style="color:#777">CLD2 and CLD3, return a list of languages, the ones not included in this test where discarded, but usually they return one language, I believe they have a disadvantage. 
 Also, I confirm the results of CLD2 for short text are correct, contrary to the test on the *Lingua* page, they did not use the parameter "bestEffort = True", their benchmark for CLD2 is unfair.
 
 *Lingua* is the average accuracy winner, but at what cost, the same test that in *ELD* or *CLD2* is below 10 seconds, in Lingua takes more than 5 hours! It acts like a brute-force software. 
-Also its lead comes from single and pair words, which are unreliable regardless.
+Also, its lead comes from single and pair words, which are unreliable regardless.
 
 The Python version of *NITO-ELD* is not the fastest but is still considered fast, as it is faster than any other non compiled detector tested.
 
 I added *ELD-L* for comparison, which has a 2.3x bigger database, but only increases execution time marginally, a testament to the efficiency of the algorithm. *ELD-L* is not the main database as it does not improve language detection in sentences.
 
-Here is the average, per test, of Tweets, Big test & Sentences.
+Here is the average, per benchmark, of Tweets, Big test & Sentences.
 
 ![Sentences tests average](https://raw.githubusercontent.com/nitotm/efficient-language-detector-py/main/benchmarks/sentences_avg_py.png)
 <!--- Sentences average
 |                     | Time         | Accuracy     |
 |:--------------------|:------------:|:------------:|
 | **Nito-ELD-py**     |      5.17"   | 99.16%       |
 | **Nito-ELD-php**    |      1.65"   | 99.16%       |
@@ -175,8 +175,9 @@
 
 
 ## Future improvements
 
 - Train from bigger datasets, and more languages.
 - The tokenizer could separate characters from languages that have their own alphabet, potentially improving accuracy and reducing the N-grams database. Retraining and testing is needed.
 
+**Donate / Hire**   
 If you wish to Donate for open source improvements, Hire me for private modifications / upgrades, or to Contact me, use the following link: https://linktr.ee/nitotm
```

