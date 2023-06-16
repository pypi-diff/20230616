# Comparing `tmp/jupyter_ai_magics-0.7.3.tar.gz` & `tmp/jupyter_ai_magics-0.8.0.tar.gz`

## Comparing `jupyter_ai_magics-0.7.3.tar` & `jupyter_ai_magics-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/setup.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/_version.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/aliases.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/embedding_providers.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/exception.py
--rw-r--r--   0        0        0    14995 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/magics.py
--rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/providers.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/jupyter_ai_magics/tests/__init__.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/LICENSE
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/README.md
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/setup.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/_version.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/aliases.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/embedding_providers.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/exception.py
+-rw-r--r--   0        0        0    21622 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/magics.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/parsers.py
+-rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/providers.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/jupyter_ai_magics/tests/__init__.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/LICENSE
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/README.md
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.8.0/PKG-INFO
```

### Comparing `jupyter_ai_magics-0.7.3/package.json` & `jupyter_ai_magics-0.8.0/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.8.0'"}*

```diff
@@ -16,9 +16,9 @@
         "type": "git",
         "url": "https://github.com/jupyterlab/jupyter-ai.git"
     },
     "scripts": {
         "dev-install": "pip install -e \".[all]\"",
         "dev-uninstall": "pip uninstall jupyter_ai_magics -y"
     },
-    "version": "0.7.3"
+    "version": "0.8.0"
 }
```

### Comparing `jupyter_ai_magics-0.7.3/jupyter_ai_magics/__init__.py` & `jupyter_ai_magics-0.8.0/jupyter_ai_magics/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.3/jupyter_ai_magics/embedding_providers.py` & `jupyter_ai_magics-0.8.0/jupyter_ai_magics/embedding_providers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import ClassVar, List, Type
-from jupyter_ai_magics.providers import AuthStrategy, EnvAuthStrategy
+from jupyter_ai_magics.providers import AuthStrategy, EnvAuthStrategy, Field
 from pydantic import BaseModel, Extra
 from langchain.embeddings import OpenAIEmbeddings, CohereEmbeddings, HuggingFaceHubEmbeddings
 from langchain.embeddings.base import Embeddings
 
 
 class BaseEmbeddingsProvider(BaseModel):
     """Base class for embedding providers"""
@@ -31,15 +31,22 @@
     """Authentication/authorization strategy. Declares what credentials are
     required to use this model provider. Generally should not be `None`."""
 
     model_id: str
 
     provider_klass: ClassVar[Type[Embeddings]]    
 
+    registry: ClassVar[bool] = False
+    """Whether this provider is a registry provider."""
+
+    fields: ClassVar[List[Field]] = []
+    """Fields expected by this provider in its constructor. Each `Field` `f`
+    should be passed as a keyword argument, keyed by `f.key`."""
     
+
 class OpenAIEmbeddingsProvider(BaseEmbeddingsProvider):
     id = "openai"
     name = "OpenAI"
     models = [
         "text-embedding-ada-002"
     ]
     model_id_key = "model"
@@ -69,7 +76,8 @@
     model_id_key = "repo_id"
     # ipywidgets needed to suppress tqdm warning
     # https://stackoverflow.com/questions/67998191
     # tqdm is a dependency of huggingface_hub
     pypi_package_deps = ["huggingface_hub", "ipywidgets"]
     auth_strategy = EnvAuthStrategy(name="HUGGINGFACEHUB_API_TOKEN")
     provider_klass = HuggingFaceHubEmbeddings
+    registry = True
```

### Comparing `jupyter_ai_magics-0.7.3/jupyter_ai_magics/exception.py` & `jupyter_ai_magics-0.8.0/jupyter_ai_magics/exception.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.3/jupyter_ai_magics/providers.py` & `jupyter_ai_magics-0.8.0/jupyter_ai_magics/providers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-from typing import ClassVar, Dict, List, Union, Literal, Optional
-
+from typing import Any, ClassVar, Dict, List, Union, Literal, Optional
 import base64
-
 import io
+import json
+import copy
 
+from jsonpath_ng import jsonpath, parse
 from langchain.schema import BaseModel as BaseLangchainProvider
 from langchain.llms import (
     AI21,
     Anthropic,
     Cohere,
     HuggingFaceHub,
     OpenAI,
     OpenAIChat,
     SagemakerEndpoint
 )
+from langchain.llms.sagemaker_endpoint import LLMContentHandler
 from langchain.utils import get_from_dict_or_env
 from langchain.llms.utils import enforce_stop_tokens
 
 from pydantic import BaseModel, Extra, root_validator
 from langchain.chat_models import ChatOpenAI
 
 class EnvAuthStrategy(BaseModel):
@@ -41,14 +43,26 @@
     Union[
         EnvAuthStrategy,
         MultiEnvAuthStrategy,
         AwsAuthStrategy,
     ]
 ]
 
+class TextField(BaseModel):
+    type: Literal["text"] = "text"
+    key: str
+    label: str
+
+class MultilineTextField(BaseModel):
+    type: Literal["text-multiline"] = "text-multiline"
+    key: str
+    label: str
+
+Field = Union[TextField, MultilineTextField]
+
 class BaseProvider(BaseLangchainProvider):
     #
     # pydantic config
     #
     class Config:
         extra = Extra.allow
 
@@ -71,14 +85,21 @@
     pypi_package_deps: ClassVar[List[str]] = []
     """List of PyPi package dependencies."""
 
     auth_strategy: ClassVar[AuthStrategy] = None
     """Authentication/authorization strategy. Declares what credentials are
     required to use this model provider. Generally should not be `None`."""
 
+    registry: ClassVar[bool] = False
+    """Whether this provider is a registry provider."""
+
+    fields: ClassVar[List[Field]] = []
+    """User inputs expected by this provider when initializing it. Each `Field` `f` 
+    should be passed in the constructor as a keyword argument, keyed by `f.key`."""
+
     #
     # instance attrs
     #
     model_id: str
 
     def __init__(self, *args, **kwargs):
         try:
@@ -140,14 +161,15 @@
     models = ["*"]
     model_id_key = "repo_id"
     # ipywidgets needed to suppress tqdm warning
     # https://stackoverflow.com/questions/67998191
     # tqdm is a dependency of huggingface_hub
     pypi_package_deps = ["huggingface_hub", "ipywidgets"]
     auth_strategy = EnvAuthStrategy(name="HUGGINGFACEHUB_API_TOKEN")
+    registry = True
 
     # Override the parent's validate_environment with a custom list of valid tasks
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         huggingfacehub_api_token = get_from_dict_or_env(
             values, "huggingfacehub_api_token", "HUGGINGFACEHUB_API_TOKEN"
@@ -288,16 +310,66 @@
         "gpt-3.5-turbo",
         "gpt-3.5-turbo-0301",
     ]
     model_id_key = "model_name"
     pypi_package_deps = ["openai"]
     auth_strategy = EnvAuthStrategy(name="OPENAI_API_KEY")
 
+class JsonContentHandler(LLMContentHandler):
+    content_type = "application/json"
+    accepts = "application/json"
+
+    def __init__(self, request_schema, response_path):
+        self.request_schema = json.loads(request_schema)
+        self.response_path = response_path
+        self.response_parser = parse(response_path)
+
+    def replace_values(self, old_val, new_val, d: Dict[str, Any]):
+        """Replaces values of a dictionary recursively."""
+        for key, val in d.items():
+            if val == old_val:
+                d[key] = new_val
+            if isinstance(val, dict):
+                self.replace_values(old_val, new_val, val)
+        
+        return d
+
+    def transform_input(self, prompt: str, model_kwargs: Dict) -> bytes:
+        request_obj = copy.deepcopy(self.request_schema)
+        self.replace_values("<prompt>", prompt, request_obj)
+        request = json.dumps(request_obj).encode('utf-8')
+        return request
+    
+    def transform_output(self, output: bytes) -> str:
+        response_json = json.loads(output.read().decode("utf-8"))
+        matches = self.response_parser.find(response_json)
+        return matches[0].value
+
 class SmEndpointProvider(BaseProvider, SagemakerEndpoint):
     id = "sagemaker-endpoint"
     name = "Sagemaker Endpoint"
     models = ["*"]
     model_id_key = "endpoint_name"
     pypi_package_deps = ["boto3"]
     auth_strategy = AwsAuthStrategy()
-
+    registry = True
+    fields = [
+        TextField(
+            key="region_name",
+            label="Region name",
+        ),
+        MultilineTextField(
+            key="request_schema",
+            label="Request schema",
+        ),
+        TextField(
+            key="response_path",
+            label="Response path",
+        )
+    ]
     
+    def __init__(self, *args, **kwargs):
+        request_schema = kwargs.pop('request_schema')
+        response_path = kwargs.pop('response_path')
+        content_handler = JsonContentHandler(request_schema=request_schema, response_path=response_path)
+        super().__init__(*args, **kwargs, content_handler=content_handler)
+
```

### Comparing `jupyter_ai_magics-0.7.3/jupyter_ai_magics/utils.py` & `jupyter_ai_magics-0.8.0/jupyter_ai_magics/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.3/.gitignore` & `jupyter_ai_magics-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.3/LICENSE` & `jupyter_ai_magics-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.7.3/pyproject.toml` & `jupyter_ai_magics-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 dependencies = [
     "ipython",
     "pydantic",
     "importlib_metadata~=5.2.0",
     "langchain==0.0.159",
-    "typing_extensions==4.5.0"
+    "typing_extensions==4.5.0",
+    "click~=8.0",
+    "jsonpath-ng~=1.5.3",
 ]
 
 [project.optional-dependencies]
 test = [
     "coverage",
     "pytest",
     "pytest-asyncio",
```

### Comparing `jupyter_ai_magics-0.7.3/PKG-INFO` & `jupyter_ai_magics-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai_magics
-Version: 0.7.3
+Version: 0.8.0
 Summary: Jupyter AI magics Python package. Not published on NPM.
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -41,16 +41,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Requires-Dist: click~=8.0
 Requires-Dist: importlib-metadata~=5.2.0
 Requires-Dist: ipython
+Requires-Dist: jsonpath-ng~=1.5.3
 Requires-Dist: langchain==0.0.159
 Requires-Dist: pydantic
 Requires-Dist: typing-extensions==4.5.0
 Provides-Extra: all
 Requires-Dist: ai21; extra == 'all'
 Requires-Dist: anthropic; extra == 'all'
 Requires-Dist: boto3; extra == 'all'
```

