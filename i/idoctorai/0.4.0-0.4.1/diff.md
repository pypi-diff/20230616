# Comparing `tmp/idoctorai-0.4.0.tar.gz` & `tmp/idoctorai-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.4.0.tar", max compression
+gzip compressed data, was "idoctorai-0.4.1.tar", max compression
```

## Comparing `idoctorai-0.4.0.tar` & `idoctorai-0.4.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.4.0/LICENSE
--rw-r--r--   0        0        0    19487 2023-06-16 10:05:01.910834 idoctorai-0.4.0/pandasai/__init__.py
--rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.4.0/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.4.0/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.4.0/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.4.0/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.4.0/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.4.0/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.4.0/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.4.0/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.4.0/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     2994 2023-06-16 09:50:05.591027 idoctorai-0.4.0/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.4.0/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.4.0/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.4.0/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.4.0/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.4.0/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.4.0/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3269 2023-06-14 13:05:20.642518 idoctorai-0.4.0/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.4.0/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.4.0/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.4.0/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.4.0/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.4.0/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1726 2023-06-16 10:02:42.064438 idoctorai-0.4.0/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.4.0/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1546 2023-06-16 10:03:30.167997 idoctorai-0.4.0/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1431 2023-06-16 10:17:27.224598 idoctorai-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.4.0/README.md
--rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 idoctorai-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.4.1/LICENSE
+-rw-r--r--   0        0        0    19487 2023-06-16 10:05:01.910834 idoctorai-0.4.1/pandasai/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.4.1/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.4.1/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.4.1/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.4.1/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.4.1/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.4.1/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.4.1/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.4.1/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.4.1/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     2994 2023-06-16 09:50:05.591027 idoctorai-0.4.1/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.4.1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.4.1/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.4.1/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.4.1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.4.1/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.4.1/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3269 2023-06-14 13:05:20.642518 idoctorai-0.4.1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.4.1/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.4.1/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.4.1/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.4.1/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.4.1/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1726 2023-06-16 10:02:42.064438 idoctorai-0.4.1/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.4.1/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1560 2023-06-16 10:57:49.811499 idoctorai-0.4.1/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1431 2023-06-16 10:58:22.260552 idoctorai-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.4.1/README.md
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 idoctorai-0.4.1/PKG-INFO
```

### Comparing `idoctorai-0.4.0/LICENSE` & `idoctorai-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/__init__.py` & `idoctorai-0.4.1/pandasai/__init__.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/constants.py` & `idoctorai-0.4.1/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/exceptions.py` & `idoctorai-0.4.1/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/helpers/_optional.py` & `idoctorai-0.4.1/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/helpers/anonymizer.py` & `idoctorai-0.4.1/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/helpers/cache.py` & `idoctorai-0.4.1/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/helpers/from_excel.py` & `idoctorai-0.4.1/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/helpers/notebook.py` & `idoctorai-0.4.1/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/helpers/save_chart.py` & `idoctorai-0.4.1/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/langchain/__init__.py` & `idoctorai-0.4.1/pandasai/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/llm/azure_openai.py` & `idoctorai-0.4.1/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/llm/base.py` & `idoctorai-0.4.1/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/llm/fake.py` & `idoctorai-0.4.1/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/llm/google_palm.py` & `idoctorai-0.4.1/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/llm/open_assistant.py` & `idoctorai-0.4.1/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/llm/openai.py` & `idoctorai-0.4.1/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/llm/starcoder.py` & `idoctorai-0.4.1/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/prompts/base.py` & `idoctorai-0.4.1/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.4.1/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.4.1/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/prompts/generate_python_code.py` & `idoctorai-0.4.1/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/prompts/generate_response.py` & `idoctorai-0.4.1/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.0/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.4.1/pandasai/prompts/multiple_dataframes.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     text: str = """
 Today is {today_date}.
 You are provided with the following pandas dataframes:"""
     instruction: str = """
 When asked about the data, your response should include a python code that describes the dataframes provided.
 Don't add too many code comments.
-Using the provided dataframes and no other dataframes, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
+Using the provided dataframes and no other dataframes, return the python code(no duplicate) and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """
 
     def __init__(self, dataframes: list[pd.DataFrame]): # pylint: disable=super-init-not-called
         for i, dataframe in enumerate(dataframes, start=1):
             row, col = dataframe.shape
 
             data_text = dataframe.head().to_string()
```

### Comparing `idoctorai-0.4.0/pyproject.toml` & `idoctorai-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.4.0"
+version = "0.4.1"
 description = "idoctorai"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
```

### Comparing `idoctorai-0.4.0/PKG-INFO` & `idoctorai-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.4.0
+Version: 0.4.1
 Summary: idoctorai
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

