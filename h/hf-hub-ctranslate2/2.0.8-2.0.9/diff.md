# Comparing `tmp/hf_hub_ctranslate2-2.0.8.tar.gz` & `tmp/hf_hub_ctranslate2-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf_hub_ctranslate2-2.0.8.tar", last modified: Sat May 20 00:36:46 2023, max compression
+gzip compressed data, was "hf_hub_ctranslate2-2.0.9.tar", last modified: Fri Jun  2 15:54:11 2023, max compression
```

## Comparing `hf_hub_ctranslate2-2.0.8.tar` & `hf_hub_ctranslate2-2.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15568 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/util/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-20 00:36:46.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-20 00:36:46.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:36:46.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-20 00:36:46.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 00:36:46.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:54:11.639657 hf_hub_ctranslate2-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-02 15:54:11.639657 hf_hub_ctranslate2-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:54:11.635657 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:54:11.639657 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:54:11.639657 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-02 15:54:11.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-02 15:54:11.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:54:11.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 15:54:11.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 15:54:11.000000 hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:54:11.639657 hf_hub_ctranslate2-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:54:11.639657 hf_hub_ctranslate2-2.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 15:54:00.000000 hf_hub_ctranslate2-2.0.9/tests/test_version.py
```

### Comparing `hf_hub_ctranslate2-2.0.8/LICENSE` & `hf_hub_ctranslate2-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.8/PKG-INFO` & `hf_hub_ctranslate2-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf_hub_ctranslate2
-Version: 2.0.8
+Version: 2.0.9
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-2.0.8/README.md` & `hf_hub_ctranslate2-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/translate.py` & `hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         self,
         model_name_or_path: str,
         device: Literal["cpu", "cuda"] = "cuda",
         device_index=0,
         compute_type: Literal["int8_float16", "int8"] = "int8_float16",
         tokenizer: Union[AutoTokenizer, None] = None,
         hub_kwargs: dict = {},
+        **kwargs: Any
     ):
         # adaptions from https://github.com/guillaumekln/faster-whisper
         if os.path.isdir(model_name_or_path):
             model_path = model_name_or_path
         else:
             try:
                 model_path = _utils._download_model(model_name_or_path, hub_kwargs=hub_kwargs)
@@ -39,14 +40,15 @@
                 hub_kwargs["local_files_only"] = True
                 model_path = _utils._download_model(model_name_or_path, hub_kwargs=hub_kwargs)
         self.model = self.ctranslate_class(
             model_path,
             device=device,
             device_index=device_index,
             compute_type=compute_type,
+            **kwargs
         )
 
         if tokenizer is not None:
             self.tokenizer = tokenizer
         else:
             if "tokenizer.json" in os.listdir(model_path):
                 if not autotokenizer_ok:
@@ -86,33 +88,36 @@
         self,
         model_name_or_path: str,
         device: Literal["cpu", "cuda"] = "cuda",
         device_index=0,
         compute_type: Literal["int8_float16", "int8"] = "int8_float16",
         tokenizer: Union[AutoTokenizer, None] = None,
         hub_kwargs={},
+        **kwargs: Any
     ):
         """for ctranslate2.Translator models, in particular m2m-100
 
         Args:
             model_name_or_path (str): _description_
             device (Literal[&quot;cpu&quot;, &quot;cuda&quot;], optional): _description_. Defaults to "cuda".
             device_index (int, optional): _description_. Defaults to 0.
             compute_type (Literal[&quot;int8_float16&quot;, &quot;int8&quot;], optional): _description_. Defaults to "int8_float16".
             tokenizer (Union[AutoTokenizer, None], optional): _description_. Defaults to None.
             hub_kwargs (dict, optional): _description_. Defaults to {}.
+            **kwargs (Any, optional): Any additional arguments
         """
         self.ctranslate_class = ctranslate2.Translator
         super().__init__(
             model_name_or_path,
             device,
             device_index,
             compute_type,
             tokenizer,
             hub_kwargs,
+            **kwargs
         )
 
     def _forward(self, *args, **kwds):
         return self.model.translate_batch(*args, **kwds)
     
     def tokenize_decode(self, tokens_out, *args, **kwargs):
         return [
@@ -170,33 +175,36 @@
         self,
         model_name_or_path: str,
         device: Literal["cpu", "cuda"] = "cuda",
         device_index=0,
         compute_type: Literal["int8_float16", "int8"] = "int8_float16",
         tokenizer: Union[AutoTokenizer, None] = None,
         hub_kwargs={},
+        **kwargs: Any
     ):
         """for ctranslate2.Translator models
 
         Args:
             model_name_or_path (str): _description_
             device (Literal[&quot;cpu&quot;, &quot;cuda&quot;], optional): _description_. Defaults to "cuda".
             device_index (int, optional): _description_. Defaults to 0.
             compute_type (Literal[&quot;int8_float16&quot;, &quot;int8&quot;], optional): _description_. Defaults to "int8_float16".
             tokenizer (Union[AutoTokenizer, None], optional): _description_. Defaults to None.
             hub_kwargs (dict, optional): _description_. Defaults to {}.
+            **kwargs (Any, optional): Any additional arguments
         """
         self.ctranslate_class = ctranslate2.Translator
         super().__init__(
             model_name_or_path,
             device,
             device_index,
             compute_type,
             tokenizer,
             hub_kwargs,
+            **kwargs
         )
         
     def _forward(self, *args, **kwds):
         target_prefix = [[self.tokenizer.lang_code_to_token[l]] for l in kwds.pop("tgt_lang")]
         # target_prefix=[['__de__'], ['__fr__']]
         return self.model.translate_batch(*args, **kwds, target_prefix=target_prefix)
     
@@ -267,33 +275,36 @@
         self,
         model_name_or_path: str,
         device: Literal["cpu", "cuda"] = "cuda",
         device_index=0,
         compute_type: Literal["int8_float16", "int8"] = "int8_float16",
         tokenizer: Union[AutoTokenizer, None] = None,
         hub_kwargs={},
+        **kwargs: Any
     ):
         """for ctranslate2.Generator models
 
         Args:
             model_name_or_path (str): _description_
             device (Literal[&quot;cpu&quot;, &quot;cuda&quot;], optional): _description_. Defaults to "cuda".
             device_index (int, optional): _description_. Defaults to 0.
             compute_type (Literal[&quot;int8_float16&quot;, &quot;int8&quot;], optional): _description_. Defaults to "int8_float16".
             tokenizer (Union[AutoTokenizer, None], optional): _description_. Defaults to None.
             hub_kwargs (dict, optional): _description_. Defaults to {}.
+            **kwargs (Any, optional): Any additional arguments
         """
         self.ctranslate_class = ctranslate2.Generator
         super().__init__(
             model_name_or_path,
             device,
             device_index,
             compute_type,
             tokenizer,
             hub_kwargs,
+            **kwargs
         )
 
     def _forward(self, *args, **kwds):
         return self.model.generate_batch(*args, **kwds)
         
     def tokenize_decode(self, tokens_out, *args, **kwargs):
         return [
```

### Comparing `hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/util/utils.py` & `hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2/util/utils.py`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/PKG-INFO` & `hf_hub_ctranslate2-2.0.9/hf_hub_ctranslate2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-hub-ctranslate2
-Version: 2.0.8
+Version: 2.0.9
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-2.0.8/setup.py` & `hf_hub_ctranslate2-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.8/tests/test_translate.py` & `hf_hub_ctranslate2-2.0.9/tests/test_translate.py`

 * *Files identical despite different names*

