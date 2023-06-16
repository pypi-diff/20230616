# Comparing `tmp/idoctorai-0.3.4.tar.gz` & `tmp/idoctorai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.3.4.tar", max compression
+gzip compressed data, was "idoctorai-0.4.0.tar", max compression
```

## Comparing `idoctorai-0.3.4.tar` & `idoctorai-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.3.4/LICENSE
--rw-r--r--   0        0        0    19255 2023-06-12 12:05:15.993358 idoctorai-0.3.4/pandasai/__init__.py
--rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.3.4/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.3.4/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.3.4/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.3.4/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.3.4/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.3.4/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.3.4/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.3.4/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.3.4/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     2982 2023-06-14 13:10:20.872222 idoctorai-0.3.4/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.3.4/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.3.4/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.3.4/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.3.4/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.3.4/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.3.4/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3269 2023-06-14 13:05:20.642518 idoctorai-0.3.4/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.3.4/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.3.4/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.3.4/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.3.4/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.3.4/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.3.4/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.3.4/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1511 2023-06-08 05:58:42.812889 idoctorai-0.3.4/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1474 2023-06-14 13:12:56.242390 idoctorai-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.3.4/README.md
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 idoctorai-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.4.0/LICENSE
+-rw-r--r--   0        0        0    19487 2023-06-16 10:05:01.910834 idoctorai-0.4.0/pandasai/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.4.0/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.4.0/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.4.0/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.4.0/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.4.0/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.4.0/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.4.0/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.4.0/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.4.0/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     2994 2023-06-16 09:50:05.591027 idoctorai-0.4.0/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.4.0/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.4.0/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.4.0/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.4.0/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.4.0/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.4.0/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3269 2023-06-14 13:05:20.642518 idoctorai-0.4.0/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.4.0/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.4.0/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.4.0/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.4.0/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.4.0/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1726 2023-06-16 10:02:42.064438 idoctorai-0.4.0/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.4.0/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1546 2023-06-16 10:03:30.167997 idoctorai-0.4.0/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1431 2023-06-16 10:17:27.224598 idoctorai-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.4.0/README.md
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 idoctorai-0.4.0/PKG-INFO
```

### Comparing `idoctorai-0.3.4/LICENSE` & `idoctorai-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/__init__.py` & `idoctorai-0.4.0/pandasai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     """
 
     _llm: LLM
     _verbose: bool = False
     _is_conversational_answer: bool = False
     _enforce_privacy: bool = False
-    _max_retries: int = 1
+    _max_retries: int = 3
     _is_notebook: bool = False
     _original_instructions: dict = {
         "question": None,
         "df_head": None,
         "num_rows": None,
         "num_columns": None,
         "rows_to_display": None,
@@ -248,14 +248,15 @@
                     if anonymize_df:
                         df_head = anonymize_dataframe_head(df_head)
 
                     code = self._llm.generate_code(
                         GeneratePythonCodePrompt(
                             prompt=prompt,
                             df_head=df_head,
+                            df_columns=data_frame.columns.tolist(),
                             num_rows=data_frame.shape[0],
                             num_columns=data_frame.shape[1],
                             rows_to_display=rows_to_display,
                         ),
                         prompt,
                         history,
                     )
@@ -366,32 +367,32 @@
                     import_optional_dependency(alias.name)
                     continue
                 if alias.name.split(".")[0] not in WHITELISTED_LIBRARIES:
                     raise BadImportError(alias.name)
 
         return False
 
-    def _is_df_overwrite(self, node: ast.stmt) -> bool:
+    def _is_df_overwrite(self, node: ast.stmt, multiple: bool) -> bool:
         """
         Remove df declarations from the code to prevent malicious code execution. A helper method.
 
         Args:
             node (object): ast.stmt
 
         Returns (bool):
 
         """
 
         return (
             isinstance(node, ast.Assign)
             and isinstance(node.targets[0], ast.Name)
-            and re.match(r"df\d{0,2}$", node.targets[0].id)
+            and re.match(r"df\d{1,2}$", node.targets[0].id)
         )
 
-    def _clean_code(self, code: str) -> str:
+    def _clean_code(self, code: str, multiple: bool) -> str:
         """
         A method to clean the code to prevent malicious code execution
 
         Args:
             code(str): A python code
 
         Returns (str): Returns a Clean Code String
@@ -399,15 +400,15 @@
         """
 
         tree = ast.parse(code)
 
         new_body = [
             node
             for node in tree.body
-            if not (self._is_unsafe_import(node) or self._is_df_overwrite(node))
+            if not (self._is_unsafe_import(node) or self._is_df_overwrite(node, multiple))
         ]
 
         new_tree = ast.Module(body=new_body)
         return astor.to_source(new_tree).strip()
 
     def run_code(
         self,
@@ -434,15 +435,15 @@
         multiple: bool = isinstance(data_frame, list)
 
         # Add save chart code
         if self._save_charts:
             code = add_save_chart(code, self._prompt_id)
 
         # Get the code to run removing unsafe imports and df overwrites
-        code_to_run = self._clean_code(code)
+        code_to_run = self._clean_code(code, multiple)
         self.last_run_code = code_to_run
         self.log(
             f"""
 Code running:
 ```
 {code_to_run}
 ```"""
@@ -493,14 +494,15 @@
 
                     else:
                         error_correcting_instruction = CorrectErrorPrompt(
                             code=code,
                             error_returned=e,
                             question=self._original_instructions["question"],
                             df_head=self._original_instructions["df_head"],
+                            df_columns=self._original_instructions["df_columns"],
                             num_rows=self._original_instructions["num_rows"],
                             num_columns=self._original_instructions["num_columns"],
                             rows_to_display=self._original_instructions[
                                 "rows_to_display"
                             ],
                         )
 
@@ -517,16 +519,17 @@
 
         match = re.match(r"^print\((.*)\)$", last_line)
         if match:
             last_line = match.group(1)
 
         try:
             return eval(last_line, environment)
-        except Exception:  # pylint: disable=W0718
+        except Exception as e:  # pylint: disable=W0718
             return captured_output
+            # raise e
 
     def log(self, message: str):
         """Log a message"""
         if self._verbose:
             print(message)
 
     def process_id(self) -> str:
```

### Comparing `idoctorai-0.3.4/pandasai/constants.py` & `idoctorai-0.4.0/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/exceptions.py` & `idoctorai-0.4.0/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/helpers/_optional.py` & `idoctorai-0.4.0/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/helpers/anonymizer.py` & `idoctorai-0.4.0/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/helpers/cache.py` & `idoctorai-0.4.0/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/helpers/from_excel.py` & `idoctorai-0.4.0/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/helpers/notebook.py` & `idoctorai-0.4.0/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/helpers/save_chart.py` & `idoctorai-0.4.0/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/langchain/__init__.py` & `idoctorai-0.4.0/pandasai/langchain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 class LangChain:
 
     api_token: str
     conversation: ConversationChain
     llm: OpenAI
     model_name: str = "gpt-3.5-turbo"
     k: int = 2
+    max_tokens: int = 4097
 
     template = """Assistant is a large language model trained by OpenAI.
 
 Assistant is designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, Assistant is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
 
 Assistant is constantly learning and improving, and its capabilities are constantly evolving. It is able to process and understand large amounts of text, and can use this knowledge to provide accurate and informative responses to a wide range of questions. Additionally, Assistant is able to generate its own text based on the input it receives, allowing it to engage in discussions and provide explanations and descriptions on a wide range of topics.
 
@@ -34,15 +35,15 @@
     template= """
 {history}
 Human: {human_input}
 Assistant:"""
 
     def __init__(self, api_token: Optional[str] = None, **kwargs,):
         self.api_token = api_token or None
-        self.llm = OpenAI(model_name=self.model_name, openai_api_key=self.api_token, temperature=0, max_tokens=512)
+        self.llm = OpenAI(model_name=self.model_name, openai_api_key=self.api_token, temperature=0)
         prompt = PromptTemplate(
             input_variables=["history","human_input"], 
             template=self.template
         )
 
         memory = ConversationBufferWindowMemory(k=self.k)
         # memory = ConversationBufferMemory(memory_key="history", memory_size=3)
```

### Comparing `idoctorai-0.3.4/pandasai/llm/azure_openai.py` & `idoctorai-0.4.0/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/llm/base.py` & `idoctorai-0.4.0/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/llm/fake.py` & `idoctorai-0.4.0/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/llm/google_palm.py` & `idoctorai-0.4.0/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/llm/open_assistant.py` & `idoctorai-0.4.0/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/llm/openai.py` & `idoctorai-0.4.0/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/llm/starcoder.py` & `idoctorai-0.4.0/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/prompts/base.py` & `idoctorai-0.4.0/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.4.0/pandasai/prompts/correct_error_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     # pylint: disable=too-few-public-methods
 
     text: str = """
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the result of `print(df.head({rows_to_display}))`:
 {df_head}.
+the columns are {df_columns}.
 
 The user asked the following question:
 {question}
 
 You generated this python code:
 {code}
```

### Comparing `idoctorai-0.3.4/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.4.0/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/prompts/generate_python_code.py` & `idoctorai-0.4.0/pandasai/prompts/generate_python_code.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,16 +25,18 @@
     # pylint: disable=too-few-public-methods
 
     text: str = """
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the result of `print(df.head({rows_to_display}))`:
 {df_head}.
+the columns are {df_columns}.
 
-When asked about the data, your response should include a python code that describes the dataframe `df`.
+When asked about the data, your response should include a python code(no duplicate) that describes the dataframe `df`.
+Don't add too many code comments.
 Using the provided dataframe, df, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """
 
     def __init__(self, **kwargs):
         super().__init__(
             **kwargs,
             START_CODE_TAG=START_CODE_TAG,
```

### Comparing `idoctorai-0.3.4/pandasai/prompts/generate_response.py` & `idoctorai-0.4.0/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.4/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.4.0/pandasai/prompts/multiple_dataframes.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     # pylint: disable=too-few-public-methods
 
     text: str = """
 Today is {today_date}.
 You are provided with the following pandas dataframes:"""
     instruction: str = """
 When asked about the data, your response should include a python code that describes the dataframes provided.
+Don't add too many code comments.
 Using the provided dataframes and no other dataframes, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """
 
     def __init__(self, dataframes: list[pd.DataFrame]): # pylint: disable=super-init-not-called
         for i, dataframe in enumerate(dataframes, start=1):
             row, col = dataframe.shape
```

### Comparing `idoctorai-0.3.4/pyproject.toml` & `idoctorai-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.3.4"
-description = "this is idoctorai, Generate code with natural speech"
+version = "0.4.0"
+description = "idoctorai"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 
 [tool.poetry.dependencies]
```

### Comparing `idoctorai-0.3.4/PKG-INFO` & `idoctorai-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.3.4
-Summary: this is idoctorai, Generate code with natural speech
+Version: 0.4.0
+Summary: idoctorai
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

