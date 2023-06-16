# Comparing `tmp/gpt_fn-0.0.5.tar.gz` & `tmp/gpt_fn-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_fn-0.0.5.tar", max compression
+gzip compressed data, was "gpt_fn-0.0.6.tar", max compression
```

## Comparing `gpt_fn-0.0.5.tar` & `gpt_fn-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0     1066 2023-06-12 11:29:13.874951 gpt_fn-0.0.5/LICENSE
--rw-r--r--   0        0        0     3023 2023-06-12 11:29:13.874951 gpt_fn-0.0.5/README.md
--rw-r--r--   0        0        0      758 2023-06-12 11:29:41.779048 gpt_fn-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/__init__.py
--rw-r--r--   0        0        0      767 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/ai_function.py
--rw-r--r--   0        0        0     1212 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/completion.py
--rw-r--r--   0        0        0      537 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/conftest.py
--rw-r--r--   0        0        0      342 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/exceptions.py
--rw-r--r--   0        0        0      655 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/prompt.py
--rw-r--r--   0        0        0        0 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/py.typed
--rw-r--r--   0        0        0        0 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/__init__.py
--rw-r--r--   0        0        0      284 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
--rw-r--r--   0        0        0     1462 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/__snapshots__/test_completion.ambr
--rw-r--r--   0        0        0      330 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
--rw-r--r--   0        0        0     3423 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml
--rw-r--r--   0        0        0     4360 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml
--rw-r--r--   0        0        0     2794 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0     2656 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml
--rw-r--r--   0        0        0      872 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/test_ai_function.py
--rw-r--r--   0        0        0     1077 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/test_completion.py
--rw-r--r--   0        0        0      522 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/test_prompt.py
--rw-r--r--   0        0        0        0 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/__init__.py
--rw-r--r--   0        0        0     1945 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/pydantic_parser.py
--rw-r--r--   0        0        0     2411 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/signature.py
--rw-r--r--   0        0        0        0 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/tests/__init__.py
--rw-r--r--   0        0        0      960 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
--rw-r--r--   0        0        0     5591 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
--rw-r--r--   0        0        0      892 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/tests/test_pydantic_parser.py
--rw-r--r--   0        0        0     1733 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/tests/test_signature.py
--rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 gpt_fn-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-16 03:39:37.942535 gpt_fn-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4119 2023-06-16 03:39:37.942535 gpt_fn-0.0.6/README.md
+-rw-r--r--   0        0        0      810 2023-06-16 03:40:00.870205 gpt_fn-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/__init__.py
+-rw-r--r--   0        0        0      767 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/ai_function.py
+-rw-r--r--   0        0        0     4135 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/completion.py
+-rw-r--r--   0        0        0      537 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/conftest.py
+-rw-r--r--   0        0        0      342 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/exceptions.py
+-rw-r--r--   0        0        0      878 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/prompt.py
+-rw-r--r--   0        0        0        0 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/py.typed
+-rw-r--r--   0        0        0        0 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/__init__.py
+-rw-r--r--   0        0        0      284 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
+-rw-r--r--   0        0        0     4623 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/__snapshots__/test_completion.ambr
+-rw-r--r--   0        0        0      330 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
+-rw-r--r--   0        0        0    13049 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml
+-rw-r--r--   0        0        0    15305 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml
+-rw-r--r--   0        0        0    13478 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0    12997 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml
+-rw-r--r--   0        0        0     5955 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_function_completion.yaml
+-rw-r--r--   0        0        0     3239 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml
+-rw-r--r--   0        0        0     3892 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_structural_completion.yaml
+-rw-r--r--   0        0        0      872 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/test_ai_function.py
+-rw-r--r--   0        0        0     2927 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/test_completion.py
+-rw-r--r--   0        0        0      522 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/__init__.py
+-rw-r--r--   0        0        0     1945 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/pydantic_parser.py
+-rw-r--r--   0        0        0     3560 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/signature.py
+-rw-r--r--   0        0        0        0 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/tests/__init__.py
+-rw-r--r--   0        0        0      960 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
+-rw-r--r--   0        0        0    14006 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
+-rw-r--r--   0        0        0      892 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/tests/test_pydantic_parser.py
+-rw-r--r--   0        0        0     2647 2023-06-16 03:39:37.946535 gpt_fn-0.0.6/src/gpt_fn/utils/tests/test_signature.py
+-rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 gpt_fn-0.0.6/PKG-INFO
```

### Comparing `gpt_fn-0.0.5/LICENSE` & `gpt_fn-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.5/pyproject.toml` & `gpt_fn-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [tool.poetry]
 name = "gpt-fn"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gpt_fn", from = "src" }]
 include = ["fn/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-openai = "^0.27"
+openai = "^0.27.8"
 pydantic = "^1.0"
 jinja2 = "^3.0"
+docstring-parser = "^0.15"
 
 [tool.poetry.group.test.dependencies]
 syrupy = "^4.0.2"
 pytest-vcr = "^1.0.2"
 pytest-cov = "^4.1.0"
+coveralls = "^3.3.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.2"
 mkdocs-material = "^9.1.15"
-mkdocstrings = {extras = ["python"], version = "^0.22.0"}
+mkdocstrings = { extras = ["python"], version = "^0.22.0" }
 
 [tool.poetry-dynamic-versioning]
 enable = false
 pattern = "default-unprefixed"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
```

### Comparing `gpt_fn-0.0.5/src/gpt_fn/ai_function.py` & `gpt_fn-0.0.6/src/gpt_fn/ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.5/src/gpt_fn/conftest.py` & `gpt_fn-0.0.6/src/gpt_fn/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.5/src/gpt_fn/prompt.py` & `gpt_fn-0.0.6/src/gpt_fn/prompt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from typing import Literal
 
 import jinja2
 from pydantic import BaseModel
 
-from .completion import Message
+from .completion import FunctionMessage, Message
 
 
 class MessageTemplate(BaseModel):
-    role: Literal["system", "user", "assistant"]
+    role: Literal["system", "user", "assistant", "function"]
     content: str
+    name: str = ""
 
     def render(self, **kwargs: str) -> Message:
-        return {
-            "role": self.role,
-            "content": jinja2.Template(self.content).render(**kwargs),
-        }
+        content = jinja2.Template(self.content).render(**kwargs)
+        if self.role == "function":
+            return FunctionMessage(
+                role=self.role,
+                content=content,
+                name=self.name,
+            )
+        return Message(role=self.role, content=content)
 
     class Config:
         # remove whitespace
         anystr_strip_whitespace = True
 
 
 class ChatTemplate(BaseModel):
```

### Comparing `gpt_fn-0.0.5/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml` & `gpt_fn-0.0.6/src/gpt_fn/tests/cassettes/test_function_completion_without_neccess_function.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,93 +1,90 @@
 interactions:
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are now the following
-      python function:\n```\n# return fabnocci number\ndef fabnocci(n: int):\n```\nOnly
-      respond with your `return` value.\nThe output should be formatted as a JSON
-      instance that conforms to the JSON schema below.\n\nAs an example, for the schema
-      {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a list of
-      strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}}, \"required\":
-      [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted instance
-      of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}} is
-      not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\": {\"ret\":
-      {\"title\": \"Ret\", \"type\": \"integer\"}}, \"required\": [\"ret\"]}\n```"},
-      {"role": "user", "content": "fabnocci(10)"}], "model": "gpt-3.5-turbo", "temperature":
-      0.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty": 0.0, "user":
-      "", "stop": null}'
+    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
+      {"role": "user", "content": "I want to book a restaurant in London."}], "model":
+      "gpt-3.5-turbo-0613", "temperature": 1.0, "top_p": 1.0, "frequency_penalty":
+      0.0, "presence_penalty": 0.0, "user": "", "stop": null, "functions": [{"name":
+      "book_a_flight", "description": "", "parameters": {"type": "object", "required":
+      ["date", "destination"], "properties": {"date": {"title": "Date", "type": "string"},
+      "destination": {"title": "Destination", "type": "string"}, "origin": {"title":
+      "Origin", "default": "London", "type": "string"}}, "definitions": {}}}], "function_call":
+      "auto"}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
-      - gzip, deflate
+      - gzip, deflate, br
       Connection:
       - keep-alive
       Content-Length:
-      - '975'
+      - '656'
       Content-Type:
       - application/json
       User-Agent:
-      - OpenAI/v1 PythonBindings/0.27.7
+      - OpenAI/v1 PythonBindings/0.27.8
       X-OpenAI-Client-User-Agent:
-      - '{"bindings_version": "0.27.7", "httplib": "requests", "lang": "python", "lang_version":
-        "3.10.8", "platform": "Linux-5.15.0-72-generic-x86_64-with-glibc2.35", "publisher":
-        "openai", "uname": "Linux 5.15.0-72-generic #79-Ubuntu SMP Wed Apr 19 08:22:18
-        UTC 2023 x86_64"}'
+      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
+        "3.10.11", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
+        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
+        PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: "{\n  \"id\": \"chatcmpl-7QZLqAOMdygD2B0nE7xwIlZbI5dYJ\",\n  \"object\":
-        \"chat.completion\",\n  \"created\": 1686566774,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
-        \ \"usage\": {\n    \"prompt_tokens\": 199,\n    \"completion_tokens\": 6,\n
-        \   \"total_tokens\": 205\n  },\n  \"choices\": [\n    {\n      \"message\":
-        {\n        \"role\": \"assistant\",\n        \"content\": \"{\\\"ret\\\":
-        55}\"\n      },\n      \"finish_reason\": \"stop\",\n      \"index\": 0\n
-        \   }\n  ]\n}\n"
+      string: "{\n  \"id\": \"chatcmpl-7RcqnDDJFsuH6uxGHQnThegIztTIu\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1686818553,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+        \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
+        \"assistant\",\n        \"content\": \"I'm sorry, but I am currently unable
+        to book a restaurant for you. However, I can help you find some popular restaurants
+        in London.\"\n      },\n      \"finish_reason\": \"stop\"\n    }\n  ],\n  \"usage\":
+        {\n    \"prompt_tokens\": 67,\n    \"completion_tokens\": 30,\n    \"total_tokens\":
+        97\n  }\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d618241afc24a1e-TPE
+      - 7d7985333a61a9a7-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
-      - gzip
+      - br
       Content-Type:
       - application/json
       Date:
-      - Mon, 12 Jun 2023 10:46:14 GMT
+      - Thu, 15 Jun 2023 08:42:34 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
-      - gpt-3.5-turbo-0301
+      - gpt-3.5-turbo-0613
       openai-processing-ms:
-      - '394'
+      - '1199'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
-      - '3500'
+      - '3000'
       x-ratelimit-limit-tokens:
-      - '90000'
+      - '250000'
       x-ratelimit-remaining-requests:
-      - '3499'
+      - '2999'
       x-ratelimit-remaining-tokens:
-      - '89809'
+      - '249965'
       x-ratelimit-reset-requests:
-      - 17ms
+      - 20ms
       x-ratelimit-reset-tokens:
-      - 126ms
+      - 8ms
       x-request-id:
-      - 493e1bf4e826813b9d18a2843a8f3b9b
+      - 03348d5940aa708d149dff8ce7452a28
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `gpt_fn-0.0.5/src/gpt_fn/tests/test_ai_function.py` & `gpt_fn-0.0.6/src/gpt_fn/tests/test_ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.5/src/gpt_fn/tests/test_prompt.py` & `gpt_fn-0.0.6/src/gpt_fn/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.5/src/gpt_fn/utils/pydantic_parser.py` & `gpt_fn-0.0.6/src/gpt_fn/utils/pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.5/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr` & `gpt_fn-0.0.6/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.5/src/gpt_fn/utils/tests/test_pydantic_parser.py` & `gpt_fn-0.0.6/src/gpt_fn/utils/tests/test_pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.5/PKG-INFO` & `gpt_fn-0.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-Metadata-Version: 2.1
-Name: gpt-fn
-Version: 0.0.5
-Summary: 
-Author: lucemia
-Author-email: lucemia@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: jinja2 (>=3.0,<4.0)
-Requires-Dist: openai (>=0.27,<0.28)
-Requires-Dist: pydantic (>=1.0,<2.0)
-Description-Content-Type: text/markdown
-
 # GPT-Fn
 
+[![CI](https://github.com/livingbio/gpt-fn/workflows/python-unittest/badge.svg?branch=main)](https://github.com/livingbio/gpt-fn/actions?query=workflow%3Apython-unittest++branch%3Amain++)
+[![Coverage Status](https://coveralls.io/repos/github/livingbio/gpt-fn/badge.svg?branch=main)](https://coveralls.io/github/livingbio/gpt-fn?branch=main)
+[![pypi](https://img.shields.io/pypi/v/gpt-fn.svg)](https://pypi.python.org/pypi/gpt-fn)
+[![downloads](https://pepy.tech/badge/gpt-fn/month)](https://pepy.tech/project/gpt-fn)
+[![versions](https://img.shields.io/pypi/pyversions/gpt-fn.svg)](https://github.com/livingbio/gpt-fn)
+[![license](https://img.shields.io/github/license/livingbio/gpt-fn.svg)](https://github.com/livingbio/gpt-fn/blob/main/LICENSE)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
+
 GPT-Fn is a lightweight utility library designed to seamlessly integrate AI capabilities into your software applications. Our focus is on providing essential utilities that make it easy to incorporate artificial intelligence into your codebase without unnecessary complexities.
 
 ## Features
 
 - **Function-like API**: With GPT-Fn, you can utilize AI capabilities in your code just like any other function. No need to learn complex AI frameworks or APIs; simply call our functions and harness the power of AI effortlessly.
 
 - **AI Integration**: GPT-Fn seamlessly integrates state-of-the-art AI models, allowing you to perform tasks such as natural language processing, image recognition, sentiment analysis, and much more.
@@ -72,8 +68,7 @@
 ## Acknowledgements
 
 We would like to thank the open-source community for their valuable contributions and the creators of the underlying AI models that power GPT-Fn.
 
 ## Contact
 
 If you have any questions, suggestions, or feedback, please don't hesitate to contact us at [email protected]
-
```

