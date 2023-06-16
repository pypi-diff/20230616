# Comparing `tmp/openapi_spec_validator-0.6.0a1.tar.gz` & `tmp/openapi_spec_validator-0.6.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_spec_validator-0.6.0a1.tar", max compression
+gzip compressed data, was "openapi_spec_validator-0.6.0a2.tar", max compression
```

## Comparing `openapi_spec_validator-0.6.0a1.tar` & `openapi_spec_validator-0.6.0a2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/LICENSE
--rw-r--r--   0        0        0     3936 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/README.rst
--rw-r--r--   0        0        0      847 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/__init__.py
--rw-r--r--   0        0        0     3041 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/__main__.py
--rw-r--r--   0        0        0       53 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/py.typed
--rw-r--r--   0        0        0      670 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/readers.py
--rw-r--r--   0        0        0    40203 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v2.0/schema.json
--rw-r--r--   0        0        0    35816 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v3.0/schema.json
--rw-r--r--   0        0        0    37211 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v3.0.0/schema.json
--rw-r--r--   0        0        0    34260 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v3.1/schema.json
--rw-r--r--   0        0        0      612 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/schemas/__init__.py
--rw-r--r--   0        0        0      924 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/schemas/utils.py
--rw-r--r--   0        0        0      756 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/shortcuts.py
--rw-r--r--   0        0        0     2523 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/__init__.py
--rw-r--r--   0        0        0      922 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/decorators.py
--rw-r--r--   0        0        0      529 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/exceptions.py
--rw-r--r--   0        0        0      644 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/protocols.py
--rw-r--r--   0        0        0     1537 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/proxies.py
--rw-r--r--   0        0        0    11887 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/validators.py
--rw-r--r--   0        0        0     2533 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/pyproject.toml
--rw-r--r--   0        0        0     1401 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/conftest.py
--rw-r--r--   0        0        0        2 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/empty.yaml
--rw-r--r--   0        0        0       14 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v2.0/empty.yaml
--rw-r--r--   0        0        0     2137 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v2.0/missing-reference.yaml
--rw-r--r--   0        0        0     2145 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v2.0/petstore.yaml
--rw-r--r--   0        0        0       16 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/empty.yaml
--rw-r--r--   0        0        0      267 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/missing-description.yaml
--rw-r--r--   0        0        0      306 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/parent-reference/common.yaml
--rw-r--r--   0        0        0      938 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/parent-reference/openapi.yaml
--rw-r--r--   0        0        0       94 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/parent-reference/recursive.yaml
--rw-r--r--   0        0        0      159 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/parent-reference/recursive2.yaml
--rw-r--r--   0        0        0      198 2023-06-15 11:39:35.580022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/parent-reference/spec/components.yaml
--rw-r--r--   0        0        0      127 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore-separate/common/schemas/Error.yaml
--rw-r--r--   0        0        0     2037 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore-separate/spec/openapi.yaml
--rw-r--r--   0        0        0      128 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore-separate/spec/schemas/Pet.yaml
--rw-r--r--   0        0        0       37 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore-separate/spec/schemas/Pets.yaml
--rw-r--r--   0        0        0     2571 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore.yaml
--rw-r--r--   0        0        0      279 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/property-missing-reference.yaml
--rw-r--r--   0        0        0      295 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/property-recursive.yaml
--rw-r--r--   0        0        0     2718 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/data/v3.1/petstore.yaml
--rw-r--r--   0        0        0     3576 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/test_main.py
--rw-r--r--   0        0        0     4643 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/test_shortcuts.py
--rw-r--r--   0        0        0    16360 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/validation/test_exceptions.py
--rw-r--r--   0        0        0     5846 2023-06-15 11:39:35.584022 openapi_spec_validator-0.6.0a1/tests/integration/validation/test_validators.py
--rw-r--r--   0        0        0     5276 1970-01-01 00:00:00.000000 openapi_spec_validator-0.6.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/LICENSE
+-rw-r--r--   0        0        0     3936 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/README.rst
+-rw-r--r--   0        0        0      847 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/__init__.py
+-rw-r--r--   0        0        0     3041 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/__main__.py
+-rw-r--r--   0        0        0       53 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/py.typed
+-rw-r--r--   0        0        0      670 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/readers.py
+-rw-r--r--   0        0        0    40203 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/resources/schemas/v2.0/schema.json
+-rw-r--r--   0        0        0    35816 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/resources/schemas/v3.0/schema.json
+-rw-r--r--   0        0        0    37211 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/resources/schemas/v3.0.0/schema.json
+-rw-r--r--   0        0        0    34260 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/resources/schemas/v3.1/schema.json
+-rw-r--r--   0        0        0      612 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/schemas/utils.py
+-rw-r--r--   0        0        0      839 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/shortcuts.py
+-rw-r--r--   0        0        0     2523 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/validation/__init__.py
+-rw-r--r--   0        0        0      922 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/validation/decorators.py
+-rw-r--r--   0        0        0      529 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/validation/exceptions.py
+-rw-r--r--   0        0        0      786 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/validation/protocols.py
+-rw-r--r--   0        0        0     1761 2023-06-16 08:23:25.307186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/validation/proxies.py
+-rw-r--r--   0        0        0    11887 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/openapi_spec_validator/validation/validators.py
+-rw-r--r--   0        0        0     2533 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1401 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/conftest.py
+-rw-r--r--   0        0        0        2 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/empty.yaml
+-rw-r--r--   0        0        0       14 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v2.0/empty.yaml
+-rw-r--r--   0        0        0     2137 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v2.0/missing-reference.yaml
+-rw-r--r--   0        0        0     2145 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v2.0/petstore.yaml
+-rw-r--r--   0        0        0       16 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/empty.yaml
+-rw-r--r--   0        0        0      267 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/missing-description.yaml
+-rw-r--r--   0        0        0      306 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/parent-reference/common.yaml
+-rw-r--r--   0        0        0      938 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/parent-reference/openapi.yaml
+-rw-r--r--   0        0        0       94 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/parent-reference/recursive.yaml
+-rw-r--r--   0        0        0      159 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/parent-reference/recursive2.yaml
+-rw-r--r--   0        0        0      198 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/parent-reference/spec/components.yaml
+-rw-r--r--   0        0        0      127 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/petstore-separate/common/schemas/Error.yaml
+-rw-r--r--   0        0        0     2037 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/petstore-separate/spec/openapi.yaml
+-rw-r--r--   0        0        0      128 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/petstore-separate/spec/schemas/Pet.yaml
+-rw-r--r--   0        0        0       37 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/petstore-separate/spec/schemas/Pets.yaml
+-rw-r--r--   0        0        0     2571 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/petstore.yaml
+-rw-r--r--   0        0        0      279 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/property-missing-reference.yaml
+-rw-r--r--   0        0        0      295 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/property-recursive.yaml
+-rw-r--r--   0        0        0     2718 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/data/v3.1/petstore.yaml
+-rw-r--r--   0        0        0     3576 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/test_main.py
+-rw-r--r--   0        0        0     4643 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/test_shortcuts.py
+-rw-r--r--   0        0        0    16360 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/validation/test_exceptions.py
+-rw-r--r--   0        0        0     5846 2023-06-16 08:23:25.311186 openapi_spec_validator-0.6.0a2/tests/integration/validation/test_validators.py
+-rw-r--r--   0        0        0     5276 1970-01-01 00:00:00.000000 openapi_spec_validator-0.6.0a2/PKG-INFO
```

### Comparing `openapi_spec_validator-0.6.0a1/LICENSE` & `openapi_spec_validator-0.6.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/README.rst` & `openapi_spec_validator-0.6.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/__init__.py` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from openapi_spec_validator.validation import openapi_v2_spec_validator
 from openapi_spec_validator.validation import openapi_v3_spec_validator
 from openapi_spec_validator.validation import openapi_v30_spec_validator
 from openapi_spec_validator.validation import openapi_v31_spec_validator
 
 __author__ = "Artur Maciag"
 __email__ = "maciag.artur@gmail.com"
-__version__ = "0.6.0a1"
+__version__ = "0.6.0a2"
 __url__ = "https://github.com/python-openapi/openapi-spec-validator"
 __license__ = "Apache License, Version 2.0"
 
 __all__ = [
     "openapi_v2_spec_validator",
     "openapi_v3_spec_validator",
     "openapi_v30_spec_validator",
```

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/__main__.py` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/readers.py` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/readers.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v2.0/schema.json` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/resources/schemas/v2.0/schema.json`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v3.0/schema.json` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/resources/schemas/v3.0/schema.json`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v3.0.0/schema.json` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/resources/schemas/v3.0.0/schema.json`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/resources/schemas/v3.1/schema.json` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/resources/schemas/v3.1/schema.json`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/schemas/__init__.py` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/schemas/utils.py` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/shortcuts.py` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/shortcuts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """OpenAPI spec validator shortcuts module."""
 from typing import Any
 from typing import Hashable
 from typing import Mapping
+from typing import Optional
 
 from jsonschema_spec.handlers import all_urls_handler
 
 from openapi_spec_validator.validation import openapi_spec_validator_proxy
 from openapi_spec_validator.validation.protocols import SupportsValidation
 
 
 def validate_spec(
     spec: Mapping[Hashable, Any],
-    spec_url: str = "",
+    base_uri: str = "",
     validator: SupportsValidation = openapi_spec_validator_proxy,
+    spec_url: Optional[str] = None,
 ) -> None:
-    return validator.validate(spec, spec_url=spec_url)
+    return validator.validate(spec, base_uri=base_uri, spec_url=spec_url)
 
 
 def validate_spec_url(
     spec_url: str,
     validator: SupportsValidation = openapi_spec_validator_proxy,
 ) -> None:
     spec = all_urls_handler(spec_url)
-    return validator.validate(spec, spec_url=spec_url)
+    return validator.validate(spec, base_uri=spec_url)
```

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/__init__.py` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/decorators.py` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/validation/decorators.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/exceptions.py` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/protocols.py` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/validation/protocols.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from typing import Any
 from typing import Hashable
 from typing import Iterator
 from typing import Mapping
+from typing import Optional
 from typing import Protocol
 from typing import runtime_checkable
 
 from openapi_spec_validator.validation.exceptions import OpenAPIValidationError
 
 
 @runtime_checkable
 class SupportsValidation(Protocol):
     def is_valid(self, instance: Mapping[Hashable, Any]) -> bool:
         ...
 
     def iter_errors(
-        self, instance: Mapping[Hashable, Any], spec_url: str = ""
+        self,
+        instance: Mapping[Hashable, Any],
+        base_uri: str = "",
+        spec_url: Optional[str] = None,
     ) -> Iterator[OpenAPIValidationError]:
         ...
 
     def validate(
-        self, instance: Mapping[Hashable, Any], spec_url: str = ""
+        self,
+        instance: Mapping[Hashable, Any],
+        base_uri: str = "",
+        spec_url: Optional[str] = None,
     ) -> None:
         ...
```

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/proxies.py` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/validation/proxies.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """OpenAPI spec validator validation proxies module."""
 from typing import Any
 from typing import Hashable
 from typing import Iterator
 from typing import Mapping
+from typing import Optional
 from typing import Tuple
 
 from openapi_spec_validator.validation.exceptions import OpenAPIValidationError
 from openapi_spec_validator.validation.exceptions import ValidatorDetectError
 from openapi_spec_validator.validation.validators import SpecValidator
 
 
@@ -17,23 +18,33 @@
     def detect(self, instance: Mapping[Hashable, Any]) -> SpecValidator:
         for (key, value), validator in self.choices.items():
             if key in instance and instance[key].startswith(value):
                 return validator
         raise ValidatorDetectError("Spec schema version not detected")
 
     def validate(
-        self, instance: Mapping[Hashable, Any], spec_url: str = ""
+        self,
+        instance: Mapping[Hashable, Any],
+        base_uri: str = "",
+        spec_url: Optional[str] = None,
     ) -> None:
         validator = self.detect(instance)
-        for err in validator.iter_errors(instance, spec_url=spec_url):
+        for err in validator.iter_errors(
+            instance, base_uri=base_uri, spec_url=spec_url
+        ):
             raise err
 
     def is_valid(self, instance: Mapping[Hashable, Any]) -> bool:
         validator = self.detect(instance)
         error = next(validator.iter_errors(instance), None)
         return error is None
 
     def iter_errors(
-        self, instance: Mapping[Hashable, Any], spec_url: str = ""
+        self,
+        instance: Mapping[Hashable, Any],
+        base_uri: str = "",
+        spec_url: Optional[str] = None,
     ) -> Iterator[OpenAPIValidationError]:
         validator = self.detect(instance)
-        yield from validator.iter_errors(instance, spec_url=spec_url)
+        yield from validator.iter_errors(
+            instance, base_uri=base_uri, spec_url=spec_url
+        )
```

### Comparing `openapi_spec_validator-0.6.0a1/openapi_spec_validator/validation/validators.py` & `openapi_spec_validator-0.6.0a2/openapi_spec_validator/validation/validators.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/pyproject.toml` & `openapi_spec_validator-0.6.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [[tool.mypy.overrides]]
 module = "lazy_object_proxy.*"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "openapi-spec-validator"
-version = "0.6.0a1"
+version = "0.6.0a2"
 description = "OpenAPI 2.0 (aka Swagger) and OpenAPI 3 spec validator"
 authors = ["Artur Maciag <maciag.artur@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/python-openapi/openapi-spec-validator"
 keywords = ["openapi", "swagger", "schema"]
 classifiers = [
```

### Comparing `openapi_spec_validator-0.6.0a1/tests/integration/conftest.py` & `openapi_spec_validator-0.6.0a2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/tests/integration/data/v2.0/missing-reference.yaml` & `openapi_spec_validator-0.6.0a2/tests/integration/data/v2.0/missing-reference.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/tests/integration/data/v2.0/petstore.yaml` & `openapi_spec_validator-0.6.0a2/tests/integration/data/v2.0/petstore.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/parent-reference/openapi.yaml` & `openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/parent-reference/openapi.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore-separate/spec/openapi.yaml` & `openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/petstore-separate/spec/openapi.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/tests/integration/data/v3.0/petstore.yaml` & `openapi_spec_validator-0.6.0a2/tests/integration/data/v3.0/petstore.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/tests/integration/data/v3.1/petstore.yaml` & `openapi_spec_validator-0.6.0a2/tests/integration/data/v3.1/petstore.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/tests/integration/test_main.py` & `openapi_spec_validator-0.6.0a2/tests/integration/test_main.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/tests/integration/test_shortcuts.py` & `openapi_spec_validator-0.6.0a2/tests/integration/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/tests/integration/validation/test_exceptions.py` & `openapi_spec_validator-0.6.0a2/tests/integration/validation/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/tests/integration/validation/test_validators.py` & `openapi_spec_validator-0.6.0a2/tests/integration/validation/test_validators.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.6.0a1/PKG-INFO` & `openapi_spec_validator-0.6.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-spec-validator
-Version: 0.6.0a1
+Version: 0.6.0a2
 Summary: OpenAPI 2.0 (aka Swagger) and OpenAPI 3 spec validator
 Home-page: https://github.com/python-openapi/openapi-spec-validator
 License: Apache-2.0
 Keywords: openapi,swagger,schema
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
```

