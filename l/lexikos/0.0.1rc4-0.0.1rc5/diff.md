# Comparing `tmp/lexikos-0.0.1rc4.tar.gz` & `tmp/lexikos-0.0.1rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikos-0.0.1rc4.tar", last modified: Wed Jun 14 04:34:33 2023, max compression
+gzip compressed data, was "lexikos-0.0.1rc5.tar", last modified: Fri Jun 16 10:13:59 2023, max compression
```

## Comparing `lexikos-0.0.1rc4.tar` & `lexikos-0.0.1rc5.tar`

### file list

```diff
@@ -1,43 +1,49 @@
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.625024 lexikos-0.0.1rc4/
--rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1rc4/LICENSE
--rw-r--r--   0 mac        (502) staff       (20)       41 2023-06-14 04:34:25.000000 lexikos-0.0.1rc4/MANIFEST.in
--rw-r--r--   0 mac        (502) staff       (20)    29266 2023-06-14 04:34:33.625297 lexikos-0.0.1rc4/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)    15542 2023-06-14 04:29:02.000000 lexikos-0.0.1rc4/README.md
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.591140 lexikos-0.0.1rc4/lexikos/
--rw-r--r--   0 mac        (502) staff       (20)      105 2023-06-14 04:29:58.000000 lexikos-0.0.1rc4/lexikos/__init__.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.587243 lexikos-0.0.1rc4/lexikos/dict/
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.599592 lexikos-0.0.1rc4/lexikos/dict/cmudict-ipa/
--rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1rc4/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
--rw-r--r--   0 mac        (502) staff       (20)  5371871 2023-05-05 05:21:25.000000 lexikos-0.0.1rc4/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.607560 lexikos-0.0.1rc4/lexikos/dict/synthetic/
--rw-r--r--   0 mac        (502) staff       (20)      406 2023-05-19 10:04:44.000000 lexikos-0.0.1rc4/lexikos/dict/synthetic/austalk_en_au.tsv
--rw-r--r--   0 mac        (502) staff       (20)     2618 2023-05-19 10:05:54.000000 lexikos-0.0.1rc4/lexikos/dict/synthetic/sc_cw_en_au.tsv
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.624666 lexikos-0.0.1rc4/lexikos/dict/wikipron/
--rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_au_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1222027 2023-05-03 03:54:38.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_ca_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    25360 2023-05-03 03:54:42.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1198453 2023-05-03 03:54:46.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_in_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    22107 2023-05-03 03:54:51.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_in_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1204678 2023-05-03 03:54:56.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_nz_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    23973 2023-05-03 03:55:01.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1927167 2023-04-21 09:43:15.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1841113 2023-04-21 09:43:18.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_us_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)     5360 2023-06-14 04:29:02.000000 lexikos-0.0.1rc4/lexikos/g2p.py
--rw-r--r--   0 mac        (502) staff       (20)     2747 2023-06-14 04:27:47.000000 lexikos-0.0.1rc4/lexikos/lexicon.py
--rw-r--r--   0 mac        (502) staff       (20)     3360 2023-06-14 04:29:02.000000 lexikos-0.0.1rc4/lexikos/normalizer.py
--rw-r--r--   0 mac        (502) staff       (20)     1354 2023-06-14 04:29:02.000000 lexikos-0.0.1rc4/lexikos/t5.py
--rw-r--r--   0 mac        (502) staff       (20)      722 2023-06-14 04:29:02.000000 lexikos-0.0.1rc4/lexikos/utils.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.593092 lexikos-0.0.1rc4/lexikos.egg-info/
--rw-r--r--   0 mac        (502) staff       (20)    29266 2023-06-14 04:34:33.000000 lexikos-0.0.1rc4/lexikos.egg-info/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)     1118 2023-06-14 04:34:33.000000 lexikos-0.0.1rc4/lexikos.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (502) staff       (20)        1 2023-06-14 04:34:33.000000 lexikos-0.0.1rc4/lexikos.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (502) staff       (20)       33 2023-06-14 04:34:33.000000 lexikos-0.0.1rc4/lexikos.egg-info/requires.txt
--rw-r--r--   0 mac        (502) staff       (20)        8 2023-06-14 04:34:33.000000 lexikos-0.0.1rc4/lexikos.egg-info/top_level.txt
--rw-r--r--   0 mac        (502) staff       (20)      821 2023-06-14 04:30:01.000000 lexikos-0.0.1rc4/pyproject.toml
--rw-r--r--   0 mac        (502) staff       (20)       32 2023-06-14 04:29:02.000000 lexikos-0.0.1rc4/requirements.txt
--rw-r--r--   0 mac        (502) staff       (20)      113 2023-06-14 04:34:33.625814 lexikos-0.0.1rc4/setup.cfg
--rw-r--r--   0 mac        (502) staff       (20)     1187 2023-06-14 04:32:35.000000 lexikos-0.0.1rc4/setup.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.761545 lexikos-0.0.1rc5/
+-rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1rc5/LICENSE
+-rw-r--r--   0 mac        (502) staff       (20)       41 2023-06-14 04:34:25.000000 lexikos-0.0.1rc5/MANIFEST.in
+-rw-r--r--   0 mac        (502) staff       (20)    29774 2023-06-16 10:13:59.761819 lexikos-0.0.1rc5/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)    16050 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/README.md
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.724793 lexikos-0.0.1rc5/lexikos/
+-rw-r--r--   0 mac        (502) staff       (20)      105 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/__init__.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.720392 lexikos-0.0.1rc5/lexikos/dict/
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.727176 lexikos-0.0.1rc5/lexikos/dict/asr-data/
+-rw-r--r--   0 mac        (502) staff       (20)      406 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/asr-data/austalk_en_au.tsv
+-rw-r--r--   0 mac        (502) staff       (20)     2618 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/asr-data/sc_cw_en_au.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.731688 lexikos-0.0.1rc5/lexikos/dict/cmudict-ipa/
+-rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1rc5/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  5371871 2023-05-05 05:21:25.000000 lexikos-0.0.1rc5/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.741535 lexikos-0.0.1rc5/lexikos/dict/synthetic/
+-rw-r--r--   0 mac        (502) staff       (20)     2953 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/synthetic/bookbot_en_v1-v2_lexicon.tsv
+-rw-r--r--   0 mac        (502) staff       (20)   114117 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/synthetic/common-voice-accent-gb_lexicon.tsv
+-rw-r--r--   0 mac        (502) staff       (20)      231 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/synthetic/common-voice-accent-id_lexicon.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1690872 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/synthetic/librispeech-lexicon-en-id.tsv
+-rw-r--r--   0 mac        (502) staff       (20)   202316 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/dict/synthetic/wu_lexicon.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.761183 lexikos-0.0.1rc5/lexikos/dict/wikipron/
+-rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_au_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1222027 2023-05-03 03:54:38.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_ca_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    25360 2023-05-03 03:54:42.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1198453 2023-05-03 03:54:46.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_in_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    22107 2023-05-03 03:54:51.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_in_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1204678 2023-05-03 03:54:56.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_nz_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    23973 2023-05-03 03:55:01.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1927152 2023-06-14 09:36:53.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1841107 2023-06-14 08:45:02.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_us_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)     5360 2023-06-14 04:29:02.000000 lexikos-0.0.1rc5/lexikos/g2p.py
+-rw-r--r--   0 mac        (502) staff       (20)     2823 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/lexikos/lexicon.py
+-rw-r--r--   0 mac        (502) staff       (20)     3360 2023-06-14 04:29:02.000000 lexikos-0.0.1rc5/lexikos/normalizer.py
+-rw-r--r--   0 mac        (502) staff       (20)     1354 2023-06-14 04:29:02.000000 lexikos-0.0.1rc5/lexikos/t5.py
+-rw-r--r--   0 mac        (502) staff       (20)      722 2023-06-14 04:29:02.000000 lexikos-0.0.1rc5/lexikos/utils.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-16 10:13:59.726527 lexikos-0.0.1rc5/lexikos.egg-info/
+-rw-r--r--   0 mac        (502) staff       (20)    29774 2023-06-16 10:13:59.000000 lexikos-0.0.1rc5/lexikos.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)     1375 2023-06-16 10:13:59.000000 lexikos-0.0.1rc5/lexikos.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (502) staff       (20)        1 2023-06-16 10:13:59.000000 lexikos-0.0.1rc5/lexikos.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (502) staff       (20)       51 2023-06-16 10:13:59.000000 lexikos-0.0.1rc5/lexikos.egg-info/requires.txt
+-rw-r--r--   0 mac        (502) staff       (20)        8 2023-06-16 10:13:59.000000 lexikos-0.0.1rc5/lexikos.egg-info/top_level.txt
+-rw-r--r--   0 mac        (502) staff       (20)      821 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/pyproject.toml
+-rw-r--r--   0 mac        (502) staff       (20)       50 2023-06-16 10:13:39.000000 lexikos-0.0.1rc5/requirements.txt
+-rw-r--r--   0 mac        (502) staff       (20)      113 2023-06-16 10:13:59.762347 lexikos-0.0.1rc5/setup.cfg
+-rw-r--r--   0 mac        (502) staff       (20)     1187 2023-06-14 04:32:35.000000 lexikos-0.0.1rc5/setup.py
```

### Comparing `lexikos-0.0.1rc4/LICENSE` & `lexikos-0.0.1rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/PKG-INFO` & `lexikos-0.0.1rc5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1rc4
+Version: 0.0.1rc5
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -264,14 +264,23 @@
 {'æ ɾ ɪ d', 'a d ɪ d', 'a d ə d', 'æ ɾ ə d', 'æ d ə d', 'æ d ɪ d'}
 >>> print(lexicon["runner"])
 {'ɹ ʌ n ɚ', 'ɹ ʌ n ə', 'r ʌ n ɝ', 'ɹ ʌ n ɝ'}
 >>> print(lexicon["water"])
 {'w o ɾ ə', 'w ɔ t ə', 'ʋ ɔ ʈ ə r', 'w a ʈ ə r ɯ', 'w ɔ t ə ɹ', 'ʋ a ʈ ə r ɯ', 'w ɑ ɾ ɚ', 'w o t ə', 'w ɔ t ɝ', 'w ɔ ʈ ə r', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ'}
 ```
 
+To include synthetic (non-dictionary-based) pronunciations:
+
+```py
+>>> from lexikos import Lexicon
+>>> lexicon = Lexicon(include_synthetic=True)
+>>> print(lexicon["athletic"])
+{'æ t l ɛ t ɪ k', 'æ θ ˈl ɛ t ɪ k', 'æ θ l ɛ t ɪ k'}
+```
+
 ### Phonemization
 
 ```py
 >>> from lexikos import G2p
 >>> g2p = G2p(lang="en-us")
 >>> g2p("Hello there! $100 is not a lot of money in 2023.")
 ['h ɛ l o ʊ', 'ð ɛ ə ɹ', 'w ʌ n', 'h ʌ n d ɹ ɪ d', 'd ɑ l ɚ z', 'ɪ z', 'n ɒ t', 'ə', 'l ɑ t', 'ʌ v', 'm ʌ n i', 'ɪ n', 't w ɛ n t i', 't w ɛ n t i', 'θ ɹ iː']
@@ -280,17 +289,17 @@
 ['h a ɪ', 'θ ɛ ə ɹ', 'm e ɪ t', 'h e ɪ v', 'ə', 'ɡ ə ˈd æ ɪ']
 ```
 
 ## Dictionaries & Models
 
 ### English `(en)`
 
-| Language | Dictionary | Phone Set | Corpus                                       | G2P Model |
-| -------- | ---------- | --------- | -------------------------------------------- | --------- |
-| en       | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn.tsv) |           |
+| Language | Dictionary | Phone Set | Corpus                                       | G2P Model                                                                                           |
+| -------- | ---------- | --------- | -------------------------------------------- | --------------------------------------------------------------------------------------------------- |
+| en       | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn.tsv) | [bookbot/byt5-small-wikipron-eng-latn](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn) |
 
 ### English `(en-US)`
 
 | Language       | Dictionary   | Phone Set | Corpus                                                                                                                     | G2P Model                                                                                                             |
 | -------------- | ------------ | --------- | -------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
 | en-US          | CMU Dict     | ARPA      | [External Link](https://github.com/microsoft/CNTK/blob/master/Examples/SequenceToSequence/CMUDict/Data/cmudict-0.7b.train) | [bookbot/byt5-small-cmudict](https://huggingface.co/bookbot/byt5-small-cmudict)                                       |
 | en-US          | CMU Dict IPA | IPA       | [External Link](https://github.com/menelik3/cmudict-ipa/blob/master/cmudict-0.7b-ipa.txt)                                  |                                                                                                                       |
@@ -305,20 +314,20 @@
 | -------------- | ---------- | --------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
 | en-UK          | CharsiuG2P | IPA       | [External Link](https://github.com/lingjzhu/CharsiuG2P/blob/main/dicts/eng-uk.tsv)                      | [charsiu/g2p_multilingual_byT5_small_100](https://huggingface.co/charsiu/g2p_multilingual_byT5_small_100)             |
 | en-UK (Broad)  | Wikipron   | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_uk_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-uk-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-uk-broad) |
 | en-UK (Narrow) | Wikipron   | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_uk_narrow.tsv) |                                                                                                                       |
 
 ### English `(en-AU)`
 
-| Language       | Dictionary  | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
-| -------------- | ----------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
-| en-AU (Broad)  | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
-| en-AU (Narrow) | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
-| en-AU          | AusTalk (§) | IPA       | [Link](./lexikos/dict/synthetic/austalk_en_au.tsv)     |                                                                                                                       |
-| en-AU          | SC-CW (§)   | IPA       | [Link](./lexikos/dict/synthetic/sc_cw_en_au.tsv)       |                                                                                                                       |
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-AU (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
+| en-AU (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
+| en-AU          | AusTalk    | IPA       | [Link](./lexikos/dict/asr-data/austalk_en_au.tsv)      |                                                                                                                       |
+| en-AU          | SC-CW      | IPA       | [Link](./lexikos/dict/asr-data/sc_cw_en_au.tsv)        |                                                                                                                       |
 
 ### English `(en-CA)`
 
 | Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
 | -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
 | en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-ca-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-ca-broad) |
 | en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |                                                                                                                       |
```

### Comparing `lexikos-0.0.1rc4/README.md` & `lexikos-0.0.1rc5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,23 @@
 {'æ ɾ ɪ d', 'a d ɪ d', 'a d ə d', 'æ ɾ ə d', 'æ d ə d', 'æ d ɪ d'}
 >>> print(lexicon["runner"])
 {'ɹ ʌ n ɚ', 'ɹ ʌ n ə', 'r ʌ n ɝ', 'ɹ ʌ n ɝ'}
 >>> print(lexicon["water"])
 {'w o ɾ ə', 'w ɔ t ə', 'ʋ ɔ ʈ ə r', 'w a ʈ ə r ɯ', 'w ɔ t ə ɹ', 'ʋ a ʈ ə r ɯ', 'w ɑ ɾ ɚ', 'w o t ə', 'w ɔ t ɝ', 'w ɔ ʈ ə r', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ'}
 ```
 
+To include synthetic (non-dictionary-based) pronunciations:
+
+```py
+>>> from lexikos import Lexicon
+>>> lexicon = Lexicon(include_synthetic=True)
+>>> print(lexicon["athletic"])
+{'æ t l ɛ t ɪ k', 'æ θ ˈl ɛ t ɪ k', 'æ θ l ɛ t ɪ k'}
+```
+
 ### Phonemization
 
 ```py
 >>> from lexikos import G2p
 >>> g2p = G2p(lang="en-us")
 >>> g2p("Hello there! $100 is not a lot of money in 2023.")
 ['h ɛ l o ʊ', 'ð ɛ ə ɹ', 'w ʌ n', 'h ʌ n d ɹ ɪ d', 'd ɑ l ɚ z', 'ɪ z', 'n ɒ t', 'ə', 'l ɑ t', 'ʌ v', 'm ʌ n i', 'ɪ n', 't w ɛ n t i', 't w ɛ n t i', 'θ ɹ iː']
@@ -61,17 +70,17 @@
 ['h a ɪ', 'θ ɛ ə ɹ', 'm e ɪ t', 'h e ɪ v', 'ə', 'ɡ ə ˈd æ ɪ']
 ```
 
 ## Dictionaries & Models
 
 ### English `(en)`
 
-| Language | Dictionary | Phone Set | Corpus                                       | G2P Model |
-| -------- | ---------- | --------- | -------------------------------------------- | --------- |
-| en       | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn.tsv) |           |
+| Language | Dictionary | Phone Set | Corpus                                       | G2P Model                                                                                           |
+| -------- | ---------- | --------- | -------------------------------------------- | --------------------------------------------------------------------------------------------------- |
+| en       | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn.tsv) | [bookbot/byt5-small-wikipron-eng-latn](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn) |
 
 ### English `(en-US)`
 
 | Language       | Dictionary   | Phone Set | Corpus                                                                                                                     | G2P Model                                                                                                             |
 | -------------- | ------------ | --------- | -------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
 | en-US          | CMU Dict     | ARPA      | [External Link](https://github.com/microsoft/CNTK/blob/master/Examples/SequenceToSequence/CMUDict/Data/cmudict-0.7b.train) | [bookbot/byt5-small-cmudict](https://huggingface.co/bookbot/byt5-small-cmudict)                                       |
 | en-US          | CMU Dict IPA | IPA       | [External Link](https://github.com/menelik3/cmudict-ipa/blob/master/cmudict-0.7b-ipa.txt)                                  |                                                                                                                       |
@@ -86,20 +95,20 @@
 | -------------- | ---------- | --------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
 | en-UK          | CharsiuG2P | IPA       | [External Link](https://github.com/lingjzhu/CharsiuG2P/blob/main/dicts/eng-uk.tsv)                      | [charsiu/g2p_multilingual_byT5_small_100](https://huggingface.co/charsiu/g2p_multilingual_byT5_small_100)             |
 | en-UK (Broad)  | Wikipron   | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_uk_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-uk-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-uk-broad) |
 | en-UK (Narrow) | Wikipron   | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_uk_narrow.tsv) |                                                                                                                       |
 
 ### English `(en-AU)`
 
-| Language       | Dictionary  | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
-| -------------- | ----------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
-| en-AU (Broad)  | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
-| en-AU (Narrow) | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
-| en-AU          | AusTalk (§) | IPA       | [Link](./lexikos/dict/synthetic/austalk_en_au.tsv)     |                                                                                                                       |
-| en-AU          | SC-CW (§)   | IPA       | [Link](./lexikos/dict/synthetic/sc_cw_en_au.tsv)       |                                                                                                                       |
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-AU (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
+| en-AU (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
+| en-AU          | AusTalk    | IPA       | [Link](./lexikos/dict/asr-data/austalk_en_au.tsv)      |                                                                                                                       |
+| en-AU          | SC-CW      | IPA       | [Link](./lexikos/dict/asr-data/sc_cw_en_au.tsv)        |                                                                                                                       |
 
 ### English `(en-CA)`
 
 | Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
 | -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
 | en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-ca-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-ca-broad) |
 | en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |                                                                                                                       |
```

### Comparing `lexikos-0.0.1rc4/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv` & `lexikos-0.0.1rc5/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv` & `lexikos-0.0.1rc5/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/dict/synthetic/sc_cw_en_au.tsv` & `lexikos-0.0.1rc5/lexikos/dict/asr-data/sc_cw_en_au.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn.tsv` & `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_au_broad.tsv` & `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_au_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_au_narrow.tsv` & `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_au_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_ca_broad.tsv` & `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_ca_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv` & `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_in_broad.tsv` & `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_in_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_in_narrow.tsv` & `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_in_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_nz_broad.tsv` & `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_nz_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv` & `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_uk_broad.tsv` & `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_uk_broad.tsv`

 * *Files 0% similar despite different names*

```diff
@@ -4012,15 +4012,14 @@
 arduity	ɑː d j uː ɪ t i
 arduous	ɑː d j uː ə s
 arduous	ɑː d͡ʒ uː ə s
 arduousness	ɑː d j uː ə s n ə s
 are	ɑː ɹ
 are	ə ɹ
 are	ɛ ə
-are	ɛː
 area	ɛː r ɪ ə
 areek	ə ɹ iː k
 arefaction	æ ɹ ɪ f æ k ʃ ə n
 arefy	æ ɹ ɪ f a ɪ
 arefy	ɛ ə ɹ ɪ f a ɪ
 aren'chu	ɑː n t ʃ uː
 aren't	ɑː n t
@@ -45441,15 +45440,14 @@
 oestrone	iː s t ɹ ə ʊ n
 oestrone	ɛ s t ɹ ə ʊ n
 oestrus	iː s t ɹ ə s
 oeuf	ɜː f
 oeuvre	uː v ɹ ə
 oeuvre	ɜː v ɹ ə
 of	ɒ v
-of	ə
 of	ə v
 ofay	o ʊ f e ɪ
 ofer	o ʊ f ɚ
 off	ɒ f
 offal	ɒ f l̩
 offcut	ɒ f k ʌ t
 offend	ə f ɛ n d
```

### Comparing `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv` & `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_us_broad.tsv` & `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_us_broad.tsv`

 * *Files 0% similar despite different names*

```diff
@@ -44217,15 +44217,14 @@
 oenophile	iː n ə f a ɪ l
 oenophile	iː n ə ʊ f a ɪ l
 oesophagus	ɪ s ɑ f ə ɡ ə s
 oestrus	iː s t ɹ ə s
 oeuf	əː f
 oeuvre	uː v ɹ ə
 oeuvre	əː v ɹ ə
-of	ə
 of	ə v
 of	ʌ v
 ofay	o ʊ f e ɪ
 ofer	o ʊ f ɚ
 off	ɔ f
 offal	ɑ f l̩
 offal	ɔ f l̩
```

### Comparing `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_us_narrow.tsv` & `lexikos-0.0.1rc5/lexikos/dict/wikipron/eng_latn_us_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/g2p.py` & `lexikos-0.0.1rc5/lexikos/g2p.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/lexicon.py` & `lexikos-0.0.1rc5/lexikos/lexicon.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,27 +13,26 @@
 # limitations under the License.
 
 from collections import UserDict
 from pathlib import Path
 from typing import Any, Dict, List, Set, Union
 import os
 
-DICTIONARIES = os.path.join(os.path.dirname(__file__), "dict")
-
 
 class Lexicon(UserDict):
     def __init__(
         self,
         normalize_phonemes: bool = False,
-        dictionaries_dir: Union[Path, str] = DICTIONARIES,
+        include_synthetic: bool = False,
     ):
-        if isinstance(dictionaries_dir, str):
-            dictionaries_dir = Path(dictionaries_dir)
-
+        dictionaries_dir = Path(os.path.join(os.path.dirname(__file__), "dict"))
         files = list(dictionaries_dir.rglob("*/*.tsv"))
+        synthetic_files = list(dictionaries_dir.rglob("synthetic/*.tsv"))
+        if not include_synthetic:
+            files = filter(lambda x: x not in synthetic_files, files)
         dicts = [self._parse_tsv(file, normalize_phonemes) for file in files]
         mapping: Dict[str, Set[str]] = self._merge_dicts(dicts)
         super().__init__(mapping)
 
     def _parse_tsv(
         self, file: Union[Path, str], normalize_phonemes: bool
     ) -> Dict[str, Set[str]]:
```

### Comparing `lexikos-0.0.1rc4/lexikos/normalizer.py` & `lexikos-0.0.1rc5/lexikos/normalizer.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/t5.py` & `lexikos-0.0.1rc5/lexikos/t5.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos/utils.py` & `lexikos-0.0.1rc5/lexikos/utils.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc4/lexikos.egg-info/PKG-INFO` & `lexikos-0.0.1rc5/lexikos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1rc4
+Version: 0.0.1rc5
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -264,14 +264,23 @@
 {'æ ɾ ɪ d', 'a d ɪ d', 'a d ə d', 'æ ɾ ə d', 'æ d ə d', 'æ d ɪ d'}
 >>> print(lexicon["runner"])
 {'ɹ ʌ n ɚ', 'ɹ ʌ n ə', 'r ʌ n ɝ', 'ɹ ʌ n ɝ'}
 >>> print(lexicon["water"])
 {'w o ɾ ə', 'w ɔ t ə', 'ʋ ɔ ʈ ə r', 'w a ʈ ə r ɯ', 'w ɔ t ə ɹ', 'ʋ a ʈ ə r ɯ', 'w ɑ ɾ ɚ', 'w o t ə', 'w ɔ t ɝ', 'w ɔ ʈ ə r', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ'}
 ```
 
+To include synthetic (non-dictionary-based) pronunciations:
+
+```py
+>>> from lexikos import Lexicon
+>>> lexicon = Lexicon(include_synthetic=True)
+>>> print(lexicon["athletic"])
+{'æ t l ɛ t ɪ k', 'æ θ ˈl ɛ t ɪ k', 'æ θ l ɛ t ɪ k'}
+```
+
 ### Phonemization
 
 ```py
 >>> from lexikos import G2p
 >>> g2p = G2p(lang="en-us")
 >>> g2p("Hello there! $100 is not a lot of money in 2023.")
 ['h ɛ l o ʊ', 'ð ɛ ə ɹ', 'w ʌ n', 'h ʌ n d ɹ ɪ d', 'd ɑ l ɚ z', 'ɪ z', 'n ɒ t', 'ə', 'l ɑ t', 'ʌ v', 'm ʌ n i', 'ɪ n', 't w ɛ n t i', 't w ɛ n t i', 'θ ɹ iː']
@@ -280,17 +289,17 @@
 ['h a ɪ', 'θ ɛ ə ɹ', 'm e ɪ t', 'h e ɪ v', 'ə', 'ɡ ə ˈd æ ɪ']
 ```
 
 ## Dictionaries & Models
 
 ### English `(en)`
 
-| Language | Dictionary | Phone Set | Corpus                                       | G2P Model |
-| -------- | ---------- | --------- | -------------------------------------------- | --------- |
-| en       | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn.tsv) |           |
+| Language | Dictionary | Phone Set | Corpus                                       | G2P Model                                                                                           |
+| -------- | ---------- | --------- | -------------------------------------------- | --------------------------------------------------------------------------------------------------- |
+| en       | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn.tsv) | [bookbot/byt5-small-wikipron-eng-latn](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn) |
 
 ### English `(en-US)`
 
 | Language       | Dictionary   | Phone Set | Corpus                                                                                                                     | G2P Model                                                                                                             |
 | -------------- | ------------ | --------- | -------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
 | en-US          | CMU Dict     | ARPA      | [External Link](https://github.com/microsoft/CNTK/blob/master/Examples/SequenceToSequence/CMUDict/Data/cmudict-0.7b.train) | [bookbot/byt5-small-cmudict](https://huggingface.co/bookbot/byt5-small-cmudict)                                       |
 | en-US          | CMU Dict IPA | IPA       | [External Link](https://github.com/menelik3/cmudict-ipa/blob/master/cmudict-0.7b-ipa.txt)                                  |                                                                                                                       |
@@ -305,20 +314,20 @@
 | -------------- | ---------- | --------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
 | en-UK          | CharsiuG2P | IPA       | [External Link](https://github.com/lingjzhu/CharsiuG2P/blob/main/dicts/eng-uk.tsv)                      | [charsiu/g2p_multilingual_byT5_small_100](https://huggingface.co/charsiu/g2p_multilingual_byT5_small_100)             |
 | en-UK (Broad)  | Wikipron   | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_uk_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-uk-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-uk-broad) |
 | en-UK (Narrow) | Wikipron   | IPA       | [External Link](https://github.com/CUNY-CL/wikipron/blob/master/data/scrape/tsv/eng_latn_uk_narrow.tsv) |                                                                                                                       |
 
 ### English `(en-AU)`
 
-| Language       | Dictionary  | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
-| -------------- | ----------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
-| en-AU (Broad)  | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
-| en-AU (Narrow) | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
-| en-AU          | AusTalk (§) | IPA       | [Link](./lexikos/dict/synthetic/austalk_en_au.tsv)     |                                                                                                                       |
-| en-AU          | SC-CW (§)   | IPA       | [Link](./lexikos/dict/synthetic/sc_cw_en_au.tsv)       |                                                                                                                       |
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-AU (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
+| en-AU (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
+| en-AU          | AusTalk    | IPA       | [Link](./lexikos/dict/asr-data/austalk_en_au.tsv)      |                                                                                                                       |
+| en-AU          | SC-CW      | IPA       | [Link](./lexikos/dict/asr-data/sc_cw_en_au.tsv)        |                                                                                                                       |
 
 ### English `(en-CA)`
 
 | Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
 | -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
 | en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-ca-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-ca-broad) |
 | en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |                                                                                                                       |
```

### Comparing `lexikos-0.0.1rc4/lexikos.egg-info/SOURCES.txt` & `lexikos-0.0.1rc5/lexikos.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -12,18 +12,23 @@
 lexikos/t5.py
 lexikos/utils.py
 lexikos.egg-info/PKG-INFO
 lexikos.egg-info/SOURCES.txt
 lexikos.egg-info/dependency_links.txt
 lexikos.egg-info/requires.txt
 lexikos.egg-info/top_level.txt
+lexikos/dict/asr-data/austalk_en_au.tsv
+lexikos/dict/asr-data/sc_cw_en_au.tsv
 lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
 lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
-lexikos/dict/synthetic/austalk_en_au.tsv
-lexikos/dict/synthetic/sc_cw_en_au.tsv
+lexikos/dict/synthetic/bookbot_en_v1-v2_lexicon.tsv
+lexikos/dict/synthetic/common-voice-accent-gb_lexicon.tsv
+lexikos/dict/synthetic/common-voice-accent-id_lexicon.tsv
+lexikos/dict/synthetic/librispeech-lexicon-en-id.tsv
+lexikos/dict/synthetic/wu_lexicon.tsv
 lexikos/dict/wikipron/eng_latn.tsv
 lexikos/dict/wikipron/eng_latn_au_broad.tsv
 lexikos/dict/wikipron/eng_latn_au_narrow.tsv
 lexikos/dict/wikipron/eng_latn_ca_broad.tsv
 lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
 lexikos/dict/wikipron/eng_latn_in_broad.tsv
 lexikos/dict/wikipron/eng_latn_in_narrow.tsv
```

### Comparing `lexikos-0.0.1rc4/pyproject.toml` & `lexikos-0.0.1rc5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lexikos"
-version = "0.0.1rc4"
+version = "0.0.1rc5"
 description = "A collection of pronunciation dictionaries and neural grapheme-to-phoneme models."
 readme = "README.md"
 authors = [{ name="w11wo", email="wilson@bookbotkids.com" }, { name="anantoj", email="gg.ananto@gmail.com" }, { name="DavidSamuell", email="davidsamuel.7878@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
```

### Comparing `lexikos-0.0.1rc4/setup.py` & `lexikos-0.0.1rc5/setup.py`

 * *Files identical despite different names*

