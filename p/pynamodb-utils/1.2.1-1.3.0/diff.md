# Comparing `tmp/pynamodb_utils-1.2.1.tar.gz` & `tmp/pynamodb_utils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamodb_utils-1.2.1.tar", last modified: Thu Apr 20 10:58:11 2023, max compression
+gzip compressed data, was "pynamodb_utils-1.3.0.tar", last modified: Fri Jun 16 19:02:07 2023, max compression
```

## Comparing `pynamodb_utils-1.2.1.tar` & `pynamodb_utils-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:58:11.085047 pynamodb_utils-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-20 10:58:05.000000 pynamodb_utils-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-20 10:58:11.085047 pynamodb_utils-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-20 10:58:05.000000 pynamodb_utils-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 10:58:11.089047 pynamodb_utils-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-20 10:58:05.000000 pynamodb_utils-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:58:11.081046 pynamodb_utils-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:58:11.085047 pynamodb_utils-1.2.1/src/pynamodb_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-20 10:58:05.000000 pynamodb_utils-1.2.1/src/pynamodb_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-20 10:58:05.000000 pynamodb_utils-1.2.1/src/pynamodb_utils/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-20 10:58:05.000000 pynamodb_utils-1.2.1/src/pynamodb_utils/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-20 10:58:05.000000 pynamodb_utils-1.2.1/src/pynamodb_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-20 10:58:05.000000 pynamodb_utils-1.2.1/src/pynamodb_utils/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-04-20 10:58:05.000000 pynamodb_utils-1.2.1/src/pynamodb_utils/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-04-20 10:58:05.000000 pynamodb_utils-1.2.1/src/pynamodb_utils/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-20 10:58:05.000000 pynamodb_utils-1.2.1/src/pynamodb_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:58:11.085047 pynamodb_utils-1.2.1/src/pynamodb_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-20 10:58:11.000000 pynamodb_utils-1.2.1/src/pynamodb_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-20 10:58:11.000000 pynamodb_utils-1.2.1/src/pynamodb_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:58:11.000000 pynamodb_utils-1.2.1/src/pynamodb_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 10:58:11.000000 pynamodb_utils-1.2.1/src/pynamodb_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 10:58:11.000000 pynamodb_utils-1.2.1/src/pynamodb_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:07.288944 pynamodb_utils-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-16 19:02:07.288944 pynamodb_utils-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-16 19:02:07.288944 pynamodb_utils-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:07.284944 pynamodb_utils-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:07.288944 pynamodb_utils-1.3.0/src/pynamodb_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-16 19:02:01.000000 pynamodb_utils-1.3.0/src/pynamodb_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:02:07.288944 pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-16 19:02:07.000000 pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-16 19:02:07.000000 pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:02:07.000000 pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 19:02:07.000000 pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 19:02:07.000000 pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/top_level.txt
```

### Comparing `pynamodb_utils-1.2.1/LICENSE` & `pynamodb_utils-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.2.1/PKG-INFO` & `pynamodb_utils-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb_utils
-Version: 1.2.1
+Version: 1.3.0
 Summary: Utilities package for pynamodb.
 Home-page: https://github.com/micmurawski/pynamodb-utils/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pynamodb_utils-1.2.1/README.md` & `pynamodb_utils-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.2.1/setup.py` & `pynamodb_utils-1.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def read(*parts):
     return codecs.open(os.path.join(HERE, *parts), "r").read()
 
 
 setup(
     name="pynamodb_utils",
-    version="1.2.1",
+    version="1.3.0",
     author="Michal Murawski",
     author_email="mmurawski777@gmail.com",
     description="Utilities package for pynamodb.",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/micmurawski/pynamodb-utils/",
     package_dir={"": "src"},
```

### Comparing `pynamodb_utils-1.2.1/src/pynamodb_utils/attributes.py` & `pynamodb_utils-1.3.0/src/pynamodb_utils/attributes.py`

 * *Files identical despite different names*

### Comparing `pynamodb_utils-1.2.1/src/pynamodb_utils/conditions.py` & `pynamodb_utils-1.3.0/src/pynamodb_utils/conditions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,74 @@
 import operator
 from functools import reduce
-from typing import Any, Callable, Dict
+from typing import Any, Callable, Dict, List, Set
 
 from pynamodb.attributes import Attribute
 from pynamodb.expressions.condition import Condition
 from pynamodb.expressions.operand import Path
 from pynamodb.models import Model
 
 from pynamodb_utils.exceptions import FilterError
 from pynamodb_utils.parsers import OPERATORS_MAPPING
-from pynamodb_utils.utils import get_nested_attribute
+from pynamodb_utils.utils import get_attribute, get_available_attributes_list
 
 
 def create_model_condition(
     model: Model,
     args: Dict[str, Any],
     _operator: Callable = operator.and_,
-    raise_exception: bool = True
+    raise_exception: bool = True,
+    unavailable_attributes: List[str] = []
 ) -> Condition:
     """
         Function creates pynamodb conditions based on input dictionary (args)
         Parameters:
                 model (pynamodb.model.Model): Corresponing pynamodb model
                 args (dict): The input dictionary with query
                 _operator (Callable): operator used to consolidate conditions
                 raise_exception (bool): boolean value enabling expceptions on missing nested attrs
+                unavailable_attributes (list): list of attribiutes that should be unavailable
         Returns:
                 condtion (Condition): computed pynamodb condition
     """
-    conditions_list = []
+    conditions_list: List[Condition] = []
 
+    available_attributes: Set[str] = get_available_attributes_list(
+        model=model,
+        unavaiable_attrs=unavailable_attributes
+    )
+
+    key: str
+    value: Any
     for key, value in args.items():
-        array = key.rsplit('__', 1)
-        field_name = array[0]
-        operator_name = array[1] if len(array) > 1 and array[1] != 'not' else ''
+        array: List[str] = key.rsplit('__', 1)
+        field_path: str = array[0]
+        operator_name: str = array[1] if len(array) > 1 and array[1] != 'not' else ''
         if operator_name.replace('not_', '') not in OPERATORS_MAPPING:
             raise FilterError(
                 message={key: [f'Operator {operator_name} does not exist.'
                                f' Choose some of available: {", ".join(OPERATORS_MAPPING.keys())}']}
             )
-        nested_attr = get_nested_attribute(model, field_name, raise_exception)
+        if field_path not in available_attributes and raise_exception:
+            raise FilterError(
+                message={
+                    field_path: [
+                        f"Parameter {field_path} does not exist."
+                        f' Choose some of available: {", ".join(available_attributes)}'
+                    ]
+                }
+            )
+
+        attr: Attribute = get_attribute(model, field_path)
 
-        if isinstance(nested_attr, (Attribute, Path)):
+        if isinstance(attr, (Attribute, Path)):
             if 'not_' in operator_name:
                 operator_name = operator_name.replace('not_', '')
                 operator_handler = OPERATORS_MAPPING[operator_name]
-                conditions_list.append(~operator_handler(model, field_name, nested_attr, value))
+                conditions_list.append(~operator_handler(model, field_path, attr, value))
             else:
                 operator_handler = OPERATORS_MAPPING[operator_name]
-                conditions_list.append(operator_handler(model, field_name, nested_attr, value))
+                conditions_list.append(operator_handler(model, field_path, attr, value))
     if not conditions_list:
         return None
     else:
         return reduce(_operator, conditions_list)
```

### Comparing `pynamodb_utils-1.2.1/src/pynamodb_utils/parsers.py` & `pynamodb_utils-1.3.0/src/pynamodb_utils/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from datetime import datetime
+from functools import reduce
+from operator import and_
 from typing import Any, Dict, List, Union
 
 from pynamodb import attributes
 from pynamodb.attributes import Attribute
 from pynamodb.expressions.condition import Condition
 from pynamodb.expressions.operand import Path
 from pynamodb.models import Model
@@ -104,14 +106,15 @@
         }
     )
 
 
 TYPE_MAPPING = {
     attributes.UTCDateTimeAttribute: parse_string_to_datetime,
     attributes.UnicodeAttribute: default_str_parser,
+    attributes.UnicodeSetAttribute: default_str_parser,
     Path: default_parser,
     attributes.ListAttribute: default_list_parser,
     attributes.JSONAttribute: default_dict_parser,
     attributes.MapAttribute: default_parser,
     attributes.BooleanAttribute: default_bool_parser,
     attributes.NumberAttribute: default_number_parser,
     EnumNumberAttribute: default_enum_parser,
@@ -167,15 +170,15 @@
         return attr.contains(*parsed_value)
     return attr.contains(parsed_value)
 
 
 def get_is_in_condition(model: Model, field_name: str, attr: Attribute, value: Any) -> Condition:
     parsed_value = parse_value(model, field_name, value)
     if isinstance(parsed_value, list):
-        return attr.is_in(*parsed_value)
+        return reduce(and_, [attr.is_in(item) for item in parsed_value])
     return attr.is_in(parsed_value)
 
 
 OPERATORS_MAPPING = {
     "": get_equals_condition,
     "equals": get_equals_condition,
     "contains": get_contains_condition,
```

### Comparing `pynamodb_utils-1.2.1/src/pynamodb_utils/serializers.py` & `pynamodb_utils-1.3.0/src/pynamodb_utils/serializers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 import operator
 import os
 from abc import abstractmethod
 from functools import reduce
-from typing import Any, Dict, Tuple, Union
+from typing import Any, Dict, List, Tuple, Union
 
 from pynamodb.indexes import GlobalSecondaryIndex, LocalSecondaryIndex
 from pynamodb.models import Model
 
 from pynamodb_utils.conditions import Condition, FilterError, create_model_condition
 
 from .exceptions import SerializerError
 from .parsers import parse_value
 from .utils import create_index_map, pick_index_keys
 
 MAX_QUERY_DEPTH = int(os.environ.get("PYNAMODB_UTILS_MAX_QUERY_DEPTH", 10))
 
 
 class Serializer:
-    def __init__(self, model) -> None:
-        self.model = model
+    def __init__(self, model: Model) -> None:
+        self.model: Model = model
         super().__init__()
 
     @abstractmethod
     def load(data: dict) -> Any:
         pass
 
 
 class ConditionsSerializer(Serializer):
     STATEMENT_OPERATOR_MAP = {"AND": operator.and_, "OR": operator.or_}
 
+    def __init__(self, model: Model, unavailable_attributes: List[str] = []) -> None:
+        self.unavailable_attributes: List[str] = unavailable_attributes
+        super().__init__(model)
+
     def _get_conditions(
         self,
         data: dict,
         raise_exception: bool = False,
         depth: int = 0,
         _operator=operator.and_,
     ):
@@ -54,28 +58,33 @@
         if data:
             conditions.append(
                 create_model_condition(
                     self.model,
                     args=data,
                     _operator=_operator,
                     raise_exception=raise_exception,
+                    unavailable_attributes=self.unavailable_attributes
                 )
             )
         return reduce(operator.and_, conditions) if conditions else None
 
     def load(self, data: dict, raise_exception: bool = False) -> Condition:
         try:
             return self._get_conditions(data, raise_exception)
         except ValueError as e:
             raise SerializerError(message={"Query": str(e)})
         except FilterError as e:
             raise SerializerError(message={"Query": e.message}) from e
 
 
 class QuerySerializer(Serializer):
+    def __init__(self, model: Model, unavailable_attributes: List[str] = []) -> None:
+        self.unavailable_attributes: List[str] = unavailable_attributes
+        super().__init__(model)
+
     def _create_query(self, data: dict, raise_exception: bool = False):
         idx_map = create_index_map(self.model)
         _equals = {}
         _rest = {}
         for k in data:
             if k not in ("AND", "OR"):
                 _name, *_operator = k.rsplit("__", 1)
@@ -94,15 +103,15 @@
         hash_keys = [_k for _k in data if _k.rsplit("__", 1)[0].startswith(prefered_index_key[0])]
         for _k in range_keys:
             range_key_query[_k] = data[_k]
             del data[_k]
 
         for _k in hash_keys:
             del data[_k]
-        condtions_serializer = ConditionsSerializer(self.model)
+        condtions_serializer = ConditionsSerializer(self.model, self.unavailable_attributes)
         range_key_condition = condtions_serializer.load(
             range_key_query, raise_exception
         )
         condition = condtions_serializer.load(data, raise_exception)
         hash_key = parse_value(self.model, prefered_index_key[0], _equals[prefered_index_key[0]])
 
         result = idx_map[prefered_index_key], {
```

### Comparing `pynamodb_utils-1.2.1/src/pynamodb_utils/utils.py` & `pynamodb_utils-1.3.0/src/pynamodb_utils/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from datetime import datetime, timezone
-from typing import Any, Dict, Tuple, Union
+from typing import Any, Dict, List, Set, Tuple, Union
 
 from pynamodb.attributes import Attribute, MapAttribute
 from pynamodb.indexes import GlobalSecondaryIndex, LocalSecondaryIndex
 from pynamodb.models import Model
 
 from pynamodb_utils.attributes import DynamicMapAttribute
-from pynamodb_utils.exceptions import FilterError
+
+NoneType = type(None)
 
 
 def create_index_map(
         model: Model
 ) -> Dict[Tuple[str, str], Union[Model, GlobalSecondaryIndex, LocalSecondaryIndex]]:
     """
     Function creates dictionary which maps hash_key and range_key to specific index.
@@ -35,15 +36,15 @@
     return idx_map
 
 
 def pick_index_keys(
     idx_map: Dict[Tuple[str, str], Union[Model, GlobalSecondaryIndex, LocalSecondaryIndex]],
     _equals: Dict[str, str],
     _rest: Dict[str, str]
-) -> Tuple[str, str]:
+) -> Tuple[str, str] | NoneType:
     common_keys = 0
     keys = None
     for k in idx_map:
         val_1 = len(set(_equals.keys()) & set(k))
         val_2 = int(k[0] in set(_equals.keys())) + int(k[1] in set(_rest.keys()))
         val = max(val_1, val_2)
         if val > common_keys:
@@ -68,35 +69,40 @@
 def parse_attrs_to_dict(obj: Any) -> Dict[str, Any]:
     """
     Function parses model/attribute to dictionary
     """
     return {k: parse_attr(getattr(obj, k, None)) for k in obj.get_attributes().keys()}
 
 
-def get_nested_attribute(model: Model, attr_string: str, raise_exception: bool = True) -> Attribute:
+def get_attributes_list(model: Model, depth: int = 0) -> List[str]:
+    attrs = []
+    for attr_str in model.get_attributes().keys():
+        attr = getattr(model, attr_str)
+        if isinstance(attr, MapAttribute):
+            attrs += [f"{attr_str}.{a}" for a in get_attributes_list(attr, depth=depth+1)]
+        attrs.append(attr_str)
+    return attrs
+
+
+def get_available_attributes_list(model: Model, unavaiable_attrs: List[str] = []) -> Set[str]:
+    atts: set = set(get_attributes_list(model))
+    return atts.difference(unavaiable_attrs)
+
+
+def get_attribute(model: Model, attr_string: str) -> Attribute:
     """
     Function gets nested attribute based on path (attr_string)
     """
     attrs = attr_string.split(".")
     result = model
     for attr in attrs:
         if isinstance(result, DynamicMapAttribute):
             result = result[attr]
         elif hasattr(result, attr):
             result = getattr(result, attr)
-        elif raise_exception:
-            raise FilterError(
-                message={
-                    attr_string: [
-                        f"Parameter {attr} does not exist."
-                        f' Choose some of available: {", ".join(result.get_attributes())}'
-                    ]
-                },
-                status_code=400,
-            )
         else:
             return None
     return result
 
 
 def get_timestamp(tzinfo: timezone = None) -> datetime:
     return datetime.now(tzinfo or timezone.utc)
```

### Comparing `pynamodb_utils-1.2.1/src/pynamodb_utils.egg-info/PKG-INFO` & `pynamodb_utils-1.3.0/src/pynamodb_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb-utils
-Version: 1.2.1
+Version: 1.3.0
 Summary: Utilities package for pynamodb.
 Home-page: https://github.com/micmurawski/pynamodb-utils/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

