# Comparing `tmp/openai_copilot-0.2.1.tar.gz` & `tmp/openai_copilot-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_copilot-0.2.1.tar", max compression
+gzip compressed data, was "openai_copilot-0.2.2.tar", max compression
```

## Comparing `openai_copilot-0.2.1.tar` & `openai_copilot-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-03-25 14:19:56.857428 openai_copilot-0.2.1/LICENSE
--rw-r--r--   0        0        0     2968 2023-04-10 14:40:42.139625 openai_copilot-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-03-25 14:19:56.868078 openai_copilot-0.2.1/openai_copilot/__init__.py
--rw-r--r--   0        0        0     2857 2023-04-10 14:19:03.562584 openai_copilot-0.2.1/openai_copilot/agent.py
--rw-r--r--   0        0        0     1059 2023-04-10 14:39:24.193477 openai_copilot-0.2.1/openai_copilot/cli.py
--rw-r--r--   0        0        0      671 2023-03-25 15:08:13.458787 openai_copilot-0.2.1/openai_copilot/llm.py
--rw-r--r--   0        0        0      674 2023-04-21 04:52:05.236119 openai_copilot-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3661 1970-01-01 00:00:00.000000 openai_copilot-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-25 14:19:56.857428 openai_copilot-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2968 2023-04-10 14:40:42.139625 openai_copilot-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-25 14:19:56.868078 openai_copilot-0.2.2/openai_copilot/__init__.py
+-rw-r--r--   0        0        0     2882 2023-06-16 04:26:19.677452 openai_copilot-0.2.2/openai_copilot/agent.py
+-rw-r--r--   0        0        0     1059 2023-04-10 14:39:24.193477 openai_copilot-0.2.2/openai_copilot/cli.py
+-rw-r--r--   0        0        0      671 2023-03-25 15:08:13.458787 openai_copilot-0.2.2/openai_copilot/llm.py
+-rw-r--r--   0        0        0      674 2023-06-16 04:27:49.757663 openai_copilot-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3661 1970-01-01 00:00:00.000000 openai_copilot-0.2.2/PKG-INFO
```

### Comparing `openai_copilot-0.2.1/LICENSE` & `openai_copilot-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_copilot-0.2.1/README.md` & `openai_copilot-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `openai_copilot-0.2.1/openai_copilot/agent.py` & `openai_copilot-0.2.2/openai_copilot/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 
 def get_chat_chain(verbose=True, model="gpt-3.5-turbo", additional_tools=None,
                    agent="chat-conversational-react-description",
                    enable_terminal=False, max_iterations=30,
                    max_tokens=1024):
     '''Initialize the LLM chain with useful tools.'''
     if os.getenv("OPENAI_API_TYPE") == "azure":
-        if model == "gpt-3.5-turbo":
-            model = "gpt-35-turbo"
-        llm = ChatOpenAI(engine=model, max_tokens=max_tokens)
+        engine = model.replace(".", "")
+        llm = ChatOpenAI(model=model, max_tokens=max_tokens,
+                         model_kwargs={"engine": engine})
     else:
         llm = ChatOpenAI(model=model, max_tokens=max_tokens)
 
     default_tools = ["human"]
     if enable_terminal:
         default_tools += ["terminal"]
     tools = load_tools(default_tools, llm)
```

### Comparing `openai_copilot-0.2.1/openai_copilot/cli.py` & `openai_copilot-0.2.2/openai_copilot/cli.py`

 * *Files identical despite different names*

### Comparing `openai_copilot-0.2.1/openai_copilot/llm.py` & `openai_copilot-0.2.2/openai_copilot/llm.py`

 * *Files identical despite different names*

### Comparing `openai_copilot-0.2.1/pyproject.toml` & `openai_copilot-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "openai-copilot"
-version = "0.2.1"
+version = "0.2.2"
 description = "OpenAI Copilot"
 authors = ["Pengfei Ni <feiskyer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_copilot"}]
 homepage = "https://github.com/feiskyer/openai-copilot"
 repository = "https://github.com/feiskyer/openai-copilot"
 keywords = ["copilot", "openai", "chatgpt"]
 
 [tool.poetry.scripts]
 openai-copilot = 'openai_copilot.cli:main'
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
-langchain = ">=0.0.141"
+langchain = ">=0.0.171"
 requests = ">=2.28"
 openai = ">=0.27.4"
 google-api-python-client = ">=2.85.0"
 click = ">=8.1.3"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `openai_copilot-0.2.1/PKG-INFO` & `openai_copilot-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openai-copilot
-Version: 0.2.1
+Version: 0.2.2
 Summary: OpenAI Copilot
 Home-page: https://github.com/feiskyer/openai-copilot
 Keywords: copilot,openai,chatgpt
 Author: Pengfei Ni
 Author-email: feiskyer@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3)
 Requires-Dist: google-api-python-client (>=2.85.0)
-Requires-Dist: langchain (>=0.0.141)
+Requires-Dist: langchain (>=0.0.171)
 Requires-Dist: openai (>=0.27.4)
 Requires-Dist: requests (>=2.28)
 Project-URL: Repository, https://github.com/feiskyer/openai-copilot
 Description-Content-Type: text/markdown
 
 # OpenAI Copilot
```

