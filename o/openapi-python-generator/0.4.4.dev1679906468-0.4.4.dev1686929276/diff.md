# Comparing `tmp/openapi-python-generator-0.4.4.dev1679906468.tar.gz` & `tmp/openapi_python_generator-0.4.4.dev1686929276.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi-python-generator-0.4.4.dev1679906468.tar", last modified: Mon Mar 27 08:41:13 2023, max compression
+gzip compressed data, was "openapi_python_generator-0.4.4.dev1686929276.tar", max compression
```

## Comparing `openapi-python-generator-0.4.4.dev1679906468.tar` & `openapi_python_generator-0.4.4.dev1686929276.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-03-27 08:40:55.295009 openapi-python-generator-0.4.4.dev1679906468/LICENSE
--rw-r--r--   0        0        0     4118 2023-03-27 08:40:55.295009 openapi-python-generator-0.4.4.dev1679906468/README.md
--rw-r--r--   0        0        0     2171 2023-03-27 08:41:09.295254 openapi-python-generator-0.4.4.dev1679906468/pyproject.toml
--rw-r--r--   0        0        0      476 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/__init__.py
--rw-r--r--   0        0        0     1622 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/__main__.py
--rw-r--r--   0        0        0      959 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/common.py
--rw-r--r--   0        0        0     4970 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/generate_data.py
--rw-r--r--   0        0        0        0 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/__init__.py
--rw-r--r--   0        0        0      740 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/api_config_generator.py
--rw-r--r--   0        0        0      409 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/common.py
--rw-r--r--   0        0        0     1296 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/generator.py
--rw-r--r--   0        0        0      426 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/jinja_config.py
--rw-r--r--   0        0        0    11507 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/model_generator.py
--rw-r--r--   0        0        0    13016 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/service_generator.py
--rw-r--r--   0        0        0     1977 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/templates/aiohttp.jinja2
--rw-r--r--   0        0        0     1256 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/templates/apiconfig.jinja2
--rw-r--r--   0        0        0      242 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/templates/enum.jinja2
--rw-r--r--   0        0        0     2143 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/templates/httpx.jinja2
--rw-r--r--   0        0        0      671 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/templates/models.jinja2
--rw-r--r--   0        0        0     1874 2023-03-27 08:40:55.299009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/templates/requests.jinja2
--rw-r--r--   0        0        0      202 2023-03-27 08:40:55.303009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/templates/service.jinja2
--rw-r--r--   0        0        0     1726 2023-03-27 08:40:55.303009 openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/models.py
--rw-r--r--   0        0        0     5523 2023-03-27 08:41:13.861964 openapi-python-generator-0.4.4.dev1679906468/setup.py
--rw-r--r--   0        0        0     5304 2023-03-27 08:41:13.862526 openapi-python-generator-0.4.4.dev1679906468/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-16 15:27:35.450719 openapi_python_generator-0.4.4.dev1686929276/LICENSE
+-rw-r--r--   0        0        0     4118 2023-06-16 15:27:35.450719 openapi_python_generator-0.4.4.dev1686929276/README.md
+-rw-r--r--   0        0        0     2171 2023-06-16 15:27:56.878798 openapi_python_generator-0.4.4.dev1686929276/pyproject.toml
+-rw-r--r--   0        0        0      476 2023-06-16 15:27:35.454719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/__init__.py
+-rw-r--r--   0        0        0     1622 2023-06-16 15:27:35.454719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/__main__.py
+-rw-r--r--   0        0        0      959 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/common.py
+-rw-r--r--   0        0        0     4970 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/generate_data.py
+-rw-r--r--   0        0        0        0 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/__init__.py
+-rw-r--r--   0        0        0      740 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/api_config_generator.py
+-rw-r--r--   0        0        0      921 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/common.py
+-rw-r--r--   0        0        0     1296 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/generator.py
+-rw-r--r--   0        0        0      426 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/jinja_config.py
+-rw-r--r--   0        0        0    12001 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/model_generator.py
+-rw-r--r--   0        0        0    13109 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/service_generator.py
+-rw-r--r--   0        0        0     1977 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/templates/aiohttp.jinja2
+-rw-r--r--   0        0        0     1256 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/templates/apiconfig.jinja2
+-rw-r--r--   0        0        0      242 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/templates/enum.jinja2
+-rw-r--r--   0        0        0     2143 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/templates/httpx.jinja2
+-rw-r--r--   0        0        0      671 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/templates/models.jinja2
+-rw-r--r--   0        0        0     1874 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/templates/requests.jinja2
+-rw-r--r--   0        0        0      202 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/templates/service.jinja2
+-rw-r--r--   0        0        0     1726 2023-06-16 15:27:35.458719 openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/models.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 openapi_python_generator-0.4.4.dev1686929276/setup.py
+-rw-r--r--   0        0        0     5456 1970-01-01 00:00:00.000000 openapi_python_generator-0.4.4.dev1686929276/PKG-INFO
```

### Comparing `openapi-python-generator-0.4.4.dev1679906468/LICENSE` & `openapi_python_generator-0.4.4.dev1686929276/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi-python-generator-0.4.4.dev1679906468/README.md` & `openapi_python_generator-0.4.4.dev1686929276/README.md`

 * *Files identical despite different names*

### Comparing `openapi-python-generator-0.4.4.dev1679906468/pyproject.toml` & `openapi_python_generator-0.4.4.dev1686929276/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-python-generator"
-version = "0.4.4.dev.1679906468"
+version = "0.4.4.dev.1686929276"
 description = "Openapi Python Generator"
 authors = ["Marco Müllner <muellnermarco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/MarcoMuellner/openapi-python-generator"
 repository = "https://github.com/MarcoMuellner/openapi-python-generator"
 documentation = "https://openapi-python-generator.readthedocs.io"
```

### Comparing `openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/__main__.py` & `openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/__main__.py`

 * *Files identical despite different names*

### Comparing `openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/common.py` & `openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/common.py`

 * *Files identical despite different names*

### Comparing `openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/generate_data.py` & `openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/generate_data.py`

 * *Files identical despite different names*

### Comparing `openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/api_config_generator.py` & `openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/api_config_generator.py`

 * *Files identical despite different names*

### Comparing `openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/generator.py` & `openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/generator.py`

 * *Files identical despite different names*

### Comparing `openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/model_generator.py` & `openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/model_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,14 +115,22 @@
         )
     # We only want to auto convert to datetime if orjson is used throghout the code, otherwise we can not
     # serialize it to JSON.
     elif schema.type == "string" and (
         schema.schema_format is None or not common.get_use_orjson()
     ):
         converted_type = pre_type + "str" + post_type
+    elif schema.type == "string" and schema.schema_format.startswith("uuid") and common.get_use_orjson():
+        if len(schema.schema_format) > 4 and schema.schema_format[4].isnumeric():
+            uuid_type = schema.schema_format.upper()
+            converted_type = pre_type + uuid_type + post_type
+            import_types = ["from pydantic import " + uuid_type]
+        else:
+            converted_type = pre_type + "UUID" + post_type
+            import_types = ["from uuid import UUID"]
     elif schema.type == "string" and schema.schema_format == "date-time":
         converted_type = pre_type + "datetime" + post_type
         import_types = ["from datetime import datetime"]
     elif schema.type == "integer":
         converted_type = pre_type + "int" + post_type
     elif schema.type == "number":
         converted_type = pre_type + "float" + post_type
```

### Comparing `openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/service_generator.py` & `openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/service_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,24 +79,25 @@
     default_params = ""
     if operation.parameters is not None:
         for param in operation.parameters:
             if not isinstance(param, Parameter):
                 continue  # pragma: no cover
             converted_result = ""
             required = False
+            param_name_cleaned = common.normalize_symbol(param.name)
 
             if isinstance(param.param_schema, Schema):
                 converted_result = (
-                    f"{param.name} : {type_converter(param.param_schema, param.required).converted_type}"
+                    f"{param_name_cleaned} : {type_converter(param.param_schema, param.required).converted_type}"
                     + ("" if param.required else " = None")
                 )
                 required = param.required
             elif isinstance(param.param_schema, Reference):
                 converted_result = (
-                    f"{param.name} : {param.param_schema.ref.split('/')[-1] }"
+                    f"{param_name_cleaned} : {param.param_schema.ref.split('/')[-1] }"
                     + (
                         ""
                         if isinstance(param, Reference) or param.required
                         else " = None"
                     )
                 )
                 required = isinstance(param, Reference) or param.required
@@ -149,28 +150,27 @@
     default_params = default_params.replace("-", "_")
 
     return params + default_params
 
 
 def generate_operation_id(operation: Operation, http_op: str) -> str:
     if operation.operationId is not None:
-        return f"{operation.operationId.replace('-', '_')}"
+        return common.normalize_symbol(operation.operationId)
     else:
         raise Exception(f"OperationId is not defined for {http_op}")  # pragma: no cover
 
 
 def _generate_params(operation: Operation, param_in : Literal["query", "header"] = "query"):
     if operation.parameters is None:
         return []
 
     params = []
     for param in operation.parameters:
         if isinstance(param, Parameter) and param.param_in == param_in:
-            param_name_cleaned = param.name.replace("-", "_")
-
+            param_name_cleaned = common.normalize_symbol(param.name)
             params.append(f"'{param.name}' : {param_name_cleaned}")
 
     return params
 
 def generate_query_params(operation: Operation) -> List[str]:
     return _generate_params(operation, "query")
```

### Comparing `openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/templates/aiohttp.jinja2` & `openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/templates/aiohttp.jinja2`

 * *Files identical despite different names*

### Comparing `openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/templates/apiconfig.jinja2` & `openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/templates/apiconfig.jinja2`

 * *Files identical despite different names*

### Comparing `openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/templates/httpx.jinja2` & `openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/templates/httpx.jinja2`

 * *Files identical despite different names*

### Comparing `openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/templates/models.jinja2` & `openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/templates/models.jinja2`

 * *Files identical despite different names*

### Comparing `openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/language_converters/python/templates/requests.jinja2` & `openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/language_converters/python/templates/requests.jinja2`

 * *Files identical despite different names*

### Comparing `openapi-python-generator-0.4.4.dev1679906468/src/openapi_python_generator/models.py` & `openapi_python_generator-0.4.4.dev1686929276/src/openapi_python_generator/models.py`

 * *Files identical despite different names*

### Comparing `openapi-python-generator-0.4.4.dev1679906468/setup.py` & `openapi_python_generator-0.4.4.dev1686929276/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 
 entry_points = \
 {'console_scripts': ['openapi-python-generator = '
                      'openapi_python_generator.__main__:main']}
 
 setup_kwargs = {
     'name': 'openapi-python-generator',
-    'version': '0.4.4.dev1679906468',
+    'version': '0.4.4.dev1686929276',
     'description': 'Openapi Python Generator',
     'long_description': "# Openapi Python Generator\n\n[![PyPI](https://img.shields.io/pypi/v/openapi-python-generator.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/openapi-python-generator.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/openapi-python-generator)][python version]\n[![License](https://img.shields.io/pypi/l/openapi-python-generator)][license]\n\n[![](https://img.shields.io/static/v1?label=documentation&message=enabled&color=<COLOR>)][documentation]\n[![Tests](https://github.com/MarcoMuellner/openapi-python-generator/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/MarcoMuellner/openapi-python-generator/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/openapi-python-generator/\n[status]: https://pypi.org/project/openapi-python-generator/\n[python version]: https://pypi.org/project/openapi-python-generator\n[documentation]: https://marcomuellner.github.io/openapi-python-generator/\n[tests]: https://github.com/MarcoMuellner/openapi-python-generator/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/MarcoMuellner/openapi-python-generator\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n![](logo.png)\n\n---\n__Documentation:__ [here][documentation]\n\n---\n\n## Features\n\n- __Ease of use__. Provide input, output and the library, and the generator will do the rest.\n- __Type safety and type hinting.__ __OpenAPI python generator__ makes heavy use of pydantic models to provide type-safe data structures.\n- __Support for multiple rest frameworks.__ __OpenAPI python generator__ currently supports the following:\n    - [httpx](https://pypi.org/project/httpx/)\n    - [requests](https://pypi.org/project/requests/)\n    - [aiohttp](https://pypi.org/project/aiohttp/)\n- __Async and sync code generation support__, depending on the framework. It will automatically create both for frameworks that support both.\n- __Easily extendable using Jinja2 templates__. The code is designed to be easily extendable and should support even more languages and frameworks in the future.\n- __Fully tested__. Every generated code is automatically tested against the OpenAPI spec and we have 100% coverage.\n- __Usage as CLI or as library__.\n\n## Requirements\n\n- Python 3.7+\n\n## Installation\n\nYou can install _Openapi Python Generator_ via [pip] from [PyPI]:\n\n```console\n$ pip install openapi-python-generator\n```\n\n## Usage\n\nPlease see the [Quick start page] for details.\n\n## Roadmap\n\n- Support for all commonly used http libraries in the python ecosystem (~~requests~~, urllib, ...)\n- Support for multiple languages\n- Support for multiple authentication schemes\n- Support custom themes\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Openapi Python Generator_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nSpecial thanks to the peeps from [openapi-schema-pydantic](https://github.com/kuimono/openapi-schema-pydantic),\nwhich already did a lot of the legwork by providing a pydantic schema for the OpenAPI 3.0.0+ specification.\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/MarcoMuellner/openapi-python-generator/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/MarcoMuellner/openapi-python-generator/blob/main/LICENSE\n[contributor guide]: https://github.com/MarcoMuellner/openapi-python-generator/blob/main/CONTRIBUTING.md\n[Quick start page]: https://marcomuellner.github.io/openapi-python-generator/quick_start/\n",
     'author': 'Marco Müllner',
     'author_email': 'muellnermarco@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/MarcoMuellner/openapi-python-generator',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
```

### Comparing `openapi-python-generator-0.4.4.dev1679906468/PKG-INFO` & `openapi_python_generator-0.4.4.dev1686929276/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: openapi-python-generator
-Version: 0.4.4.dev1679906468
+Version: 0.4.4.dev1686929276
 Summary: Openapi Python Generator
 Home-page: https://github.com/MarcoMuellner/openapi-python-generator
 License: MIT
 Keywords: OpenAPI,Generator,Python,async
 Author: Marco Müllner
 Author-email: muellnermarco@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: black (>=21.10b0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: httpx[all] (>=0.23.0,<0.24.0)
 Requires-Dist: isort (>=5.10.1)
 Requires-Dist: openapi-schema-pydantic (>=1.2.3,<2.0.0)
 Requires-Dist: orjson (>=3.7.2,<4.0.0)
```

