# Comparing `tmp/magicfunc-1.0.0.tar.gz` & `tmp/magicfunc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicfunc-1.0.0.tar", max compression
+gzip compressed data, was "magicfunc-1.0.1.tar", max compression
```

## Comparing `magicfunc-1.0.0.tar` & `magicfunc-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1079 2023-05-17 00:25:19.698337 magicfunc-1.0.0/LICENSE
--rw-r--r--   0        0        0      976 2023-05-18 09:22:57.198960 magicfunc-1.0.0/magicfunc/__core.py
--rw-r--r--   0        0        0      140 2023-05-17 02:00:16.275073 magicfunc-1.0.0/magicfunc/__init__.py
--rw-r--r--   0        0        0      147 2023-05-16 09:23:59.776790 magicfunc-1.0.0/magicfunc/__log.py
--rw-r--r--   0        0        0     1481 2023-05-18 05:47:26.325059 magicfunc-1.0.0/magicfunc/__type.py
--rw-r--r--   0        0        0     1067 2023-05-17 00:09:08.138622 magicfunc-1.0.0/magicfunc/chatgpt3.py
--rw-r--r--   0        0        0      492 2023-05-18 09:46:01.335450 magicfunc-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1312 2023-05-17 00:25:42.439674 magicfunc-1.0.0/README.md
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 magicfunc-1.0.0/setup.py
--rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 magicfunc-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-05-17 00:25:19.698337 magicfunc-1.0.1/LICENSE
+-rw-r--r--   0        0        0      976 2023-05-18 09:22:57.198960 magicfunc-1.0.1/magicfunc/__core.py
+-rw-r--r--   0        0        0      140 2023-05-17 02:00:16.275073 magicfunc-1.0.1/magicfunc/__init__.py
+-rw-r--r--   0        0        0      147 2023-05-16 09:23:59.776790 magicfunc-1.0.1/magicfunc/__log.py
+-rw-r--r--   0        0        0     1481 2023-05-18 05:47:26.325059 magicfunc-1.0.1/magicfunc/__type.py
+-rw-r--r--   0        0        0     1067 2023-06-16 02:43:00.751318 magicfunc-1.0.1/magicfunc/chatgpt3.py
+-rw-r--r--   0        0        0      492 2023-06-16 02:47:15.789534 magicfunc-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1312 2023-05-17 00:25:42.439674 magicfunc-1.0.1/README.md
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 magicfunc-1.0.1/setup.py
+-rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 magicfunc-1.0.1/PKG-INFO
```

### Comparing `magicfunc-1.0.0/LICENSE` & `magicfunc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magicfunc-1.0.0/magicfunc/__core.py` & `magicfunc-1.0.1/magicfunc/__core.py`

 * *Files identical despite different names*

### Comparing `magicfunc-1.0.0/magicfunc/__type.py` & `magicfunc-1.0.1/magicfunc/__type.py`

 * *Files identical despite different names*

### Comparing `magicfunc-1.0.0/magicfunc/chatgpt3.py` & `magicfunc-1.0.1/magicfunc/chatgpt3.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import openai
 
 from .__log import log
 from .__type import GenerateProvider
 
 openai.api_base = 'https://api.chatanywhere.com.cn/v1'
-openai.api_key = 'sk-0PfcSdT723UR44igwVxvEWvLoZJgi0FJyZWy0WCCATp5ka2a'
+openai.api_key = 'sk-9Jkmx4ZrJmw3WuHxMjiVCo0bZLGOqvjC0y2J08K51KLNMwpC'
 
 
 class ChatGPT3Provider(GenerateProvider):
     def __init__(self):
         self.prompt = textwrap.dedent('''
             You are a Python programmer, and I will give you some Python function signatures. You need to return the specific implementation of the function for me, and your return results should not contain any explanatory text.
         ''')[1:]
```

### Comparing `magicfunc-1.0.0/README.md` & `magicfunc-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `magicfunc-1.0.0/setup.py` & `magicfunc-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['openai>=0.27.6,<0.28.0']
 
 setup_kwargs = {
     'name': 'magicfunc',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'magicfunc is a Python library that uses LLM to generate function bodies for function signatures and dynamically proxies them at runtime.',
     'long_description': '# magicfunc\n\nmagicfunc is a Python library that uses LLM to generate function bodies for function signatures and dynamically proxies them at runtime.\n\n[中文文档](README_zh.md)\n\n## Installation\n\nYou can install magicfunc using pip:\n\n```bash\npip install magicfunc\n```\n\n## Usage\n\nTo use magicfunc, you need to define a function signature and pass it to the `magicfunc.magic` decorator. magicfunc will then generate a function body using LLM and dynamically proxy it at runtime.\n\n```python\nimport magicfunc\n\n@magicfunc.magic\ndef add(x: int, y: int) -> int:\n    """\n    Add two integers together.\n    """\n```\n\nYou can then call the function as you would any other function:\n\n```python\nresult = add(2, 3)\nprint(result) # Output: 5\n```\n\nmagicfunc will generate a function body that adds the two integers together and returns the result.\n\n## Configuration\n\nmagicfunc can be configured using these variables:\n\n- `DEFAULT_PROVIDER`: The default provider for generate function body.\n\n## Contributing\n\nIf you find a bug or have a feature request, please open an issue on GitHub. If you would like to contribute code, please fork the repository and submit a pull request.\n\n## License\n\nmagicfunc is licensed under the MIT License. See the LICENSE file for more information.',
     'author': 'jawide',
     'author_email': '596929059@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `magicfunc-1.0.0/PKG-INFO` & `magicfunc-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicfunc
-Version: 1.0.0
+Version: 1.0.1
 Summary: magicfunc is a Python library that uses LLM to generate function bodies for function signatures and dynamically proxies them at runtime.
 License: MIT
 Author: jawide
 Author-email: 596929059@qq.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

