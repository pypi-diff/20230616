# Comparing `tmp/bareunpy-1.6.1.tar.gz` & `tmp/bareunpy-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bareunpy-1.6.1.tar", max compression
+gzip compressed data, was "bareunpy-1.6.2.tar", max compression
```

## Comparing `bareunpy-1.6.1.tar` & `bareunpy-1.6.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1547 2023-01-30 00:41:12.108840 bareunpy-1.6.1/LICENSE
--rw-r--r--   0        0        0     4119 2023-03-24 00:58:50.777709 bareunpy-1.6.1/README.md
--rw-r--r--   0        0        0     1432 2023-06-05 09:40:00.081909 bareunpy-1.6.1/bareunpy/__init__.py
--rw-r--r--   0        0        0     7475 2023-06-05 09:39:16.952459 bareunpy-1.6.1/bareunpy/_custom_dict.py
--rw-r--r--   0        0        0     6006 2023-06-05 09:39:16.952459 bareunpy-1.6.1/bareunpy/_custom_dict_client.py
--rw-r--r--   0        0        0     3427 2023-03-24 00:58:50.781709 bareunpy-1.6.1/bareunpy/_lang_service_client.py
--rw-r--r--   0        0        0     8871 2023-03-24 00:58:50.781709 bareunpy-1.6.1/bareunpy/_tagger.py
--rw-r--r--   0        0        0     9633 2023-03-24 00:58:50.781709 bareunpy-1.6.1/bareunpy/_tokenizer.py
--rw-r--r--   0        0        0     1379 2023-06-05 09:39:47.193476 bareunpy-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     5903 1970-01-01 00:00:00.000000 bareunpy-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1547 2023-01-30 00:41:12.108840 bareunpy-1.6.2/LICENSE
+-rw-r--r--   0        0        0     4119 2023-03-24 00:58:50.777709 bareunpy-1.6.2/README.md
+-rw-r--r--   0        0        0     1432 2023-06-16 07:55:52.795277 bareunpy-1.6.2/bareunpy/__init__.py
+-rw-r--r--   0        0        0     7475 2023-06-05 09:39:16.952459 bareunpy-1.6.2/bareunpy/_custom_dict.py
+-rw-r--r--   0        0        0     6006 2023-06-05 09:39:16.952459 bareunpy-1.6.2/bareunpy/_custom_dict_client.py
+-rw-r--r--   0        0        0     3427 2023-03-24 00:58:50.781709 bareunpy-1.6.2/bareunpy/_lang_service_client.py
+-rw-r--r--   0        0        0     9452 2023-06-16 07:55:52.795277 bareunpy-1.6.2/bareunpy/_tagger.py
+-rw-r--r--   0        0        0     9633 2023-03-24 00:58:50.781709 bareunpy-1.6.2/bareunpy/_tokenizer.py
+-rw-r--r--   0        0        0     1379 2023-06-16 07:55:52.795277 bareunpy-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     5903 1970-01-01 00:00:00.000000 bareunpy-1.6.2/PKG-INFO
```

### Comparing `bareunpy-1.6.1/LICENSE` & `bareunpy-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.1/README.md` & `bareunpy-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.1/bareunpy/__init__.py` & `bareunpy-1.6.2/bareunpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,9 +51,9 @@
 
 from bareunpy._tagger import Tagger, Tagged
 from bareunpy._tokenizer import Tokenizer, Tokenized
 from bareunpy._custom_dict import CustomDict
 from bareunpy._custom_dict_client import CustomDictionaryServiceClient
 from bareunpy._lang_service_client import BareunLanguageServiceClient
 
-version = "1.6.1"
+version = "1.6.2"
 bareun_version = "1.8.0"
```

### Comparing `bareunpy-1.6.1/bareunpy/_custom_dict.py` & `bareunpy-1.6.2/bareunpy/_custom_dict.py`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.1/bareunpy/_custom_dict_client.py` & `bareunpy-1.6.2/bareunpy/_custom_dict_client.py`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.1/bareunpy/_lang_service_client.py` & `bareunpy-1.6.2/bareunpy/_lang_service_client.py`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.1/bareunpy/_tagger.py` & `bareunpy-1.6.2/bareunpy/_tagger.py`

 * *Files 16% similar despite different names*

```diff
@@ -198,36 +198,39 @@
 
         if domain in self.custom_dicts:
             return self.custom_dicts[domain]
         else:
             self.custom_dicts[domain] = CustomDict(self.apikey, domain,  self.channel)
             return self.custom_dicts[domain]
 
-    def tag(self, phrase: str, auto_split: bool = False) -> Tagged:
+    def tag(self, phrase: str, auto_split: bool = False, auto_spacing: bool = True, auto_jointing: bool = True) -> Tagged:
         if len(phrase) == 0:
             print("OOPS, no sentences.")
             return Tagged('', AnalyzeSyntaxResponse())
         try:
-            res = self.client.analyze_syntax(phrase, self.domain, auto_split)
+            res = self.client.analyze_syntax(phrase, self.domain, auto_split=auto_split, auto_spacing=auto_spacing, auto_jointing=auto_jointing)
             return Tagged(phrase, res)
         except Exception as e:
             raise e
 
-    def tags(self, phrase: List[str]) -> Tagged:
+    def tags(self, phrase: List[str], auto_split: bool = False, auto_spacing: bool = True, auto_jointing: bool = True) -> Tagged:
         """
         tag string array.
         :param phrase: array of string
+        :param auto_split(bool, optional): Whether to automatically perform sentence split
+        :param auto_spacing(bool, optional): Whether to automatically perform space insertion for typo correction
+        :param auto_jointing(bool, optional): Whether to automatically perform word joining for typo correction
         :return: Tagged result instance
         """
         if len(phrase) == 0:
             print("OOPS, no sentences.")
             return Tagged('', AnalyzeSyntaxResponse())
         p = '\n'.join(phrase)
         try:
-            res = self.client.analyze_syntax(p, self.domain, auto_split=False)
+            res = self.client.analyze_syntax(p, self.domain, auto_split=auto_split, auto_spacing=auto_spacing, auto_jointing=auto_jointing)
             return Tagged(p, res)
         except Exception as e:
             raise e
 
     def pos(self, phrase: str, flatten: bool = True, join: bool = False, detail: bool = False) -> List:
         """
         POS tagger.
```

### Comparing `bareunpy-1.6.1/bareunpy/_tokenizer.py` & `bareunpy-1.6.2/bareunpy/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.1/pyproject.toml` & `bareunpy-1.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bareunpy"
-version = "1.6.1"
+version = "1.6.2"
 description = "The bareun python library using grpc"
 authors = ["Gihyun YUN <gih2yun@baikal.ai>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://bareun.ai/"
 repository = "https://github.com/bareun-nlp/bareunpy"
 keywords = [ "NLP", "Korean", "Deep Learning", "POS tagger", "bareun"]
```

### Comparing `bareunpy-1.6.1/PKG-INFO` & `bareunpy-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bareunpy
-Version: 1.6.1
+Version: 1.6.2
 Summary: The bareun python library using grpc
 Home-page: https://bareun.ai/
 License: BSD-3-Clause
 Keywords: NLP,Korean,Deep Learning,POS tagger,bareun
 Author: Gihyun YUN
 Author-email: gih2yun@baikal.ai
 Requires-Python: >=3.6,<4.0
```

