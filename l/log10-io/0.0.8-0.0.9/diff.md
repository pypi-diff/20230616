# Comparing `tmp/log10_io-0.0.8.tar.gz` & `tmp/log10_io-0.0.9.tar.gz`

## Comparing `log10_io-0.0.8.tar` & `log10_io-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,42 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 log10_io-0.0.8/requirements.txt
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 log10_io-0.0.8/setup.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.0.8/.github/workflows/release.yml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/chatcompletion.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/chatcompletion_async_vs_sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/completion.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/completion_ada.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/get_url.py
--rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/langchain_babyagi.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/langchain_multiple_tools.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/langchain_qa.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/langchain_simple_sequential.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/langchain_sqlagent.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/multiple_sessions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.8/log10/        __init__.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.0.8/log10/bigquery.py
--rw-r--r--   0        0        0    11138 2020-02-02 00:00:00.000000 log10_io-0.0.8/log10/load.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.0.8/log10/schemas/bigquery.json
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 log10_io-0.0.8/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.8/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 log10_io-0.0.8/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 log10_io-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 log10_io-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 log10_io-0.0.9/setup.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.0.9/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/README.md
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/agents/biochemist.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/agents/code_optimizer.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/agents/coder.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/agents/cybersecurity_expert.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/agents/email_generator.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/agents/translator.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/evals/basic_eval.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/evals/compile.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/evals/fuzzy.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/evals/fuzzy_data.csv
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/evals/match_data.csv
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/logging/anthropic_completion.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/logging/chatcompletion.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/logging/chatcompletion_async_vs_sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/logging/completion.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/logging/completion_ada.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/logging/get_url.py
+-rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/logging/langchain_babyagi.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/logging/langchain_multiple_tools.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/logging/langchain_qa.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/logging/langchain_simple_sequential.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/logging/langchain_sqlagent.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.0.9/examples/logging/multiple_sessions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.9/log10/        __init__.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.0.9/log10/bigquery.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 log10_io-0.0.9/log10/evals.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 log10_io-0.0.9/log10/load.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 log10_io-0.0.9/log10/tools.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 log10_io-0.0.9/log10/utils.py
+-rw-r--r--   0        0        0    10057 2020-02-02 00:00:00.000000 log10_io-0.0.9/log10/agents/camel.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 log10_io-0.0.9/log10/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.0.9/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 log10_io-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 log10_io-0.0.9/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 log10_io-0.0.9/PKG-INFO
```

### Comparing `log10_io-0.0.8/.github/workflows/release.yml` & `log10_io-0.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.8/examples/chatcompletion_async_vs_sync.py` & `log10_io-0.0.9/examples/logging/chatcompletion_async_vs_sync.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.8/examples/get_url.py` & `log10_io-0.0.9/examples/logging/get_url.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.8/examples/langchain_babyagi.py` & `log10_io-0.0.9/examples/logging/langchain_babyagi.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.8/examples/langchain_multiple_tools.py` & `log10_io-0.0.9/examples/logging/langchain_multiple_tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.8/examples/langchain_qa.py` & `log10_io-0.0.9/examples/logging/langchain_qa.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.8/examples/langchain_simple_sequential.py` & `log10_io-0.0.9/examples/logging/langchain_simple_sequential.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.8/examples/langchain_sqlagent.py` & `log10_io-0.0.9/examples/logging/langchain_sqlagent.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.8/examples/multiple_sessions.py` & `log10_io-0.0.9/examples/logging/multiple_sessions.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.8/log10/bigquery.py` & `log10_io-0.0.9/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.8/log10/load.py` & `log10_io-0.0.9/log10/load.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import asyncio
 import threading
 import queue
 from contextlib import contextmanager
 import logging
 from dotenv import load_dotenv
 import backoff  # for exponential backoff
-from openai.error import RateLimitError
+from openai.error import RateLimitError, APIConnectionError
 
 load_dotenv()
 
 url = os.environ.get("LOG10_URL")
 token = os.environ.get("LOG10_TOKEN")
 org_id = os.environ.get("LOG10_ORG_ID")
 
@@ -30,15 +30,15 @@
     bigquery_client, bigquery_table = initialize_bigquery()
     import uuid
     from datetime import datetime, timezone
 elif target_service is None:
     target_service = "log10"  # default to log10
 
 
-@backoff.on_exception(backoff.expo, RateLimitError)
+@backoff.on_exception(backoff.expo, (RateLimitError, APIConnectionError))
 def func_with_backoff(func, *args, **kwargs):
     return func(*args, **kwargs)
 
 
 def get_session_id():
     if target_service == "bigquery":
         return str(uuid.uuid4())
@@ -56,28 +56,28 @@
                         "\nSee https://github.com/log10-io/log10#%EF%B8%8F-setup for details")
 
 
 # Global variable to store the current sessionID.
 sessionID = get_session_id()
 last_completion_response = None
 
+
 class log10_session:
     def __enter__(self):
         global sessionID
         global last_completion_response
         sessionID = get_session_id()
         last_completion_response = None
         return self
 
     def last_completion_url(self):
         if last_completion_response is None:
             return None
 
-        return url + '/app/' +  last_completion_response['organizationSlug'] + '/completions/' + last_completion_response['completionID']
-
+        return url + '/app/' + last_completion_response['organizationSlug'] + '/completions/' + last_completion_response['completionID']
 
     def __exit__(self, exc_type, exc_value, traceback):
         return
 
 
 @contextmanager
 def timed_block(block_name):
@@ -191,29 +191,43 @@
                            "lineno": frame.lineno,
                             "name": frame.name} for frame in current_stack_frame])
 
             start_time = time.perf_counter()
             output = func_with_backoff(func, *args, **kwargs)
             duration = time.perf_counter() - start_time
             logging.debug(
-                f"LOG10: TIMED BLOCK - OpenAI call duration: {duration}")
+                f"LOG10: TIMED BLOCK - LLM call duration: {duration}")
 
             if USE_ASYNC:
                 with timed_block("extra time spent waiting for log10 call"):
                     while result_queue.empty():
                         pass
                     completionID = result_queue.get()
 
             with timed_block("result call duration (sync)"):
-                log_row = {
-                    "response": json.dumps(output),
-                    "status": "finished",
-                    "duration": int(duration*1000),
-                    "stacktrace": json.dumps(stacktrace)
-                }
+                # Adjust the Anthropic output to match OAI completion output
+                if func.__qualname__ == "Client.completion":
+                    output['choices'] = [{
+                        'text': output['completion'],
+                        'index': 0,
+                    }]
+                    log_row = {
+                        "response": json.dumps(output),
+                        "status": "finished",
+                        "duration": int(duration*1000),
+                        "stacktrace": json.dumps(stacktrace),
+                        "kind": "completion"
+                    }
+                else:
+                    log_row = {
+                        "response": json.dumps(output),
+                        "status": "finished",
+                        "duration": int(duration*1000),
+                        "stacktrace": json.dumps(stacktrace)
+                    }
 
                 if target_service == "log10":
                     res = requests.request("POST",
                                            completion_url + "/" + completionID,
                                            headers={
                                                "x-log10-token": token, "Content-Type": "application/json"},
                                            json=log_row)
@@ -262,32 +276,53 @@
     global DEBUG, USE_ASYNC, sync_log_text
     DEBUG = DEBUG_
     USE_ASYNC = USE_ASYNC_
     sync_log_text = set_sync_log_text(USE_ASYNC=USE_ASYNC)
     logging.basicConfig(level=logging.DEBUG if DEBUG else logging.INFO,
                         format='%(asctime)s - %(levelname)s - LOG10 - %(message)s')
 
-    def intercept_nested_functions(obj):
-        for name, attr in vars(obj).items():
-            if callable(attr) and isinstance(attr, types.FunctionType):
-                setattr(obj, name, intercepting_decorator(attr))
-            elif inspect.isclass(attr):
-                intercept_class_methods(attr)
-
-    def intercept_class_methods(cls):
-        for method_name, method in vars(cls).items():
-            if isinstance(method, classmethod):
-                original_method = method.__func__
-                decorated_method = intercepting_decorator(original_method)
-                setattr(cls, method_name, classmethod(decorated_method))
-            elif isinstance(method, (types.FunctionType, types.MethodType)):
-                setattr(cls, method_name, intercepting_decorator(method))
-            elif inspect.isclass(method):  # Handle nested classes
-                intercept_class_methods(method)
+    # def intercept_nested_functions(obj):
+    #     for name, attr in vars(obj).items():
+    #         if callable(attr) and isinstance(attr, types.FunctionType):
+    #             setattr(obj, name, intercepting_decorator(attr))
+    #         elif inspect.isclass(attr):
+    #             intercept_class_methods(attr)
+
+    # def intercept_class_methods(cls):
+    #     for method_name, method in vars(cls).items():
+    #         if isinstance(method, classmethod):
+    #             original_method = method.__func__
+    #             decorated_method = intercepting_decorator(original_method)
+    #             setattr(cls, method_name, classmethod(decorated_method))
+    #         elif isinstance(method, (types.FunctionType, types.MethodType)):
+    #             print(f"method:{method}")
+    #             setattr(cls, method_name, intercepting_decorator(method))
+    #         elif inspect.isclass(method):  # Handle nested classes
+    #             intercept_class_methods(method)
 
     for name, attr in vars(module).items():
-        if callable(attr) and isinstance(attr, types.FunctionType):
-            setattr(module, name, intercepting_decorator(attr))
-        elif inspect.isclass(attr):  # Check if attribute is a class
-            intercept_class_methods(attr)
-        # else: # uncomment if we want to include nested function support
-        #     intercept_nested_functions(attr)
+        if inspect.isclass(attr):
+            # OpenAI
+            if module.__name__ == "openai" and name in ["ChatCompletion", "Completion"]:
+                for method_name, method in vars(attr).items():
+                    if isinstance(method, classmethod):
+                        original_method = method.__func__
+                        if original_method.__qualname__ in ["ChatCompletion.create", "Completion.create"]:
+                            decorated_method = intercepting_decorator(
+                                original_method)
+                            setattr(attr, method_name,
+                                    classmethod(decorated_method))
+            # Anthropic
+            elif module.__name__ == "anthropic" and name == "Client":
+                for method_name, method in vars(attr).items():
+                    if isinstance(method, (types.FunctionType, types.MethodType)) and method_name == "completion":
+                        setattr(attr, method_name,
+                                intercepting_decorator(method))
+
+            # For future reference:
+            # if callable(attr) and isinstance(attr, types.FunctionType):
+            #     print(f"attr:{attr}")
+            #     setattr(module, name, intercepting_decorator(attr))
+            # elif inspect.isclass(attr):  # Check if attribute is a class
+            #     intercept_class_methods(attr)
+            # # else: # uncomment if we want to include nested function support
+            # #     intercept_nested_functions(attr)
```

### Comparing `log10_io-0.0.8/log10/schemas/bigquery.json` & `log10_io-0.0.9/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.8/LICENSE` & `log10_io-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.8/README.md` & `log10_io-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.8/pyproject.toml` & `log10_io-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "log10-io"
-version = "0.0.8"
+version = "0.0.9"
 authors = []
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `log10_io-0.0.8/PKG-INFO` & `log10_io-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.0.8
+Version: 0.0.9
 Summary: Unified LLM data management
 Project-URL: Homepage, https://github.com/log10-io/log10
 Project-URL: Bug Tracker, https://github.com/log10-io/log10/issues
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

