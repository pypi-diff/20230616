# Comparing `tmp/pydantic-distiller-0.2.4.tar.gz` & `tmp/pydantic_distiller-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-distiller-0.2.4.tar", last modified: Mon Jul 18 14:23:06 2022, max compression
+gzip compressed data, was "pydantic_distiller-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pydantic-distiller-0.2.4.tar` & `pydantic_distiller-0.2.5.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0      150 2020-12-08 16:24:32.984283 pydantic-distiller-0.2.4/.coveragerc
--rw-r--r--   0        0        0      499 2020-12-08 16:24:32.984501 pydantic-distiller-0.2.4/.editorconfig
--rw-r--r--   0        0        0      277 2020-12-08 16:24:32.984673 pydantic-distiller-0.2.4/.flake8
--rw-r--r--   0        0        0      463 2022-07-18 12:57:42.525669 pydantic-distiller-0.2.4/.gitignore
--rw-r--r--   0        0        0     1083 2020-12-08 16:24:32.985252 pydantic-distiller-0.2.4/LICENSE
--rw-r--r--   0        0        0      346 2020-12-08 16:24:32.985469 pydantic-distiller-0.2.4/Makefile
--rw-r--r--   0        0        0      186 2020-12-08 16:24:32.985791 pydantic-distiller-0.2.4/README.md
--rw-r--r--   0        0        0      559 2022-07-18 13:01:41.775107 pydantic-distiller-0.2.4/distiller/__init__.py
--rw-r--r--   0        0        0     5023 2022-07-18 14:16:53.673284 pydantic-distiller-0.2.4/distiller/base.py
--rw-r--r--   0        0        0     2219 2020-12-08 16:24:32.986900 pydantic-distiller-0.2.4/distiller/helpers.py
--rw-r--r--   0        0        0      334 2020-12-08 16:24:32.987234 pydantic-distiller-0.2.4/distiller/json/__init__.py
--rw-r--r--   0        0        0     3470 2020-12-08 16:24:32.987702 pydantic-distiller-0.2.4/distiller/markup/__init__.py
--rw-r--r--   0        0        0     1987 2020-12-08 16:24:32.987978 pydantic-distiller-0.2.4/distiller/markup/mapper.py
--rw-r--r--   0        0        0     7793 2021-09-16 12:24:43.604420 pydantic-distiller-0.2.4/distiller/markup/parser.py
--rw-r--r--   0        0        0     2348 2020-12-08 16:24:32.988616 pydantic-distiller-0.2.4/distiller/markup/preprocessor.py
--rw-r--r--   0        0        0    11437 2022-07-18 14:16:53.673937 pydantic-distiller-0.2.4/distiller/nodes.py
--rw-r--r--   0        0        0      455 2020-12-08 16:24:32.989148 pydantic-distiller-0.2.4/mypy.ini
--rw-r--r--   0        0        0     1596 2022-07-18 14:17:36.082001 pydantic-distiller-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       76 2020-12-08 16:24:32.989504 pydantic-distiller-0.2.4/pytest.ini
--rw-r--r--   0        0        0        0 2020-12-08 16:24:32.989705 pydantic-distiller-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0      106 2020-12-08 16:24:32.989968 pydantic-distiller-0.2.4/tests/conftest.py
--rw-r--r--   0        0        0      420 2020-12-08 16:24:32.990215 pydantic-distiller-0.2.4/tests/helpers.py
--rw-r--r--   0        0        0      513 2020-12-08 16:24:32.990413 pydantic-distiller-0.2.4/tests/playground.py
--rw-r--r--   0        0        0     1776 2020-12-08 16:24:32.990589 pydantic-distiller-0.2.4/tests/test_base_distiller_setup.py
--rw-r--r--   0        0        0     3199 2020-12-08 16:24:32.990795 pydantic-distiller-0.2.4/tests/test_base_nodes.py
--rw-r--r--   0        0        0      962 2020-12-08 16:24:32.990974 pydantic-distiller-0.2.4/tests/test_distilled_finalization.py
--rw-r--r--   0        0        0     1127 2020-12-08 16:24:32.991454 pydantic-distiller-0.2.4/tests/test_helpers.py
--rw-r--r--   0        0        0     3178 2020-12-08 16:24:32.991764 pydantic-distiller-0.2.4/tests/test_htmlfication.py
--rw-r--r--   0        0        0     4124 2022-07-18 13:03:35.224612 pydantic-distiller-0.2.4/tests/test_markup_parsing.py
--rw-r--r--   0        0        0      954 2020-12-08 16:24:32.992211 pydantic-distiller-0.2.4/tests/test_plaintextification.py
--rw-r--r--   0        0        0     1799 2020-12-08 16:24:32.992383 pydantic-distiller-0.2.4/tests/test_tagification.py
--rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 pydantic-distiller-0.2.4/setup.py
--rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 pydantic-distiller-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      150 2022-07-18 10:50:09.689716 pydantic_distiller-0.2.5/.coveragerc
+-rw-r--r--   0        0        0      499 2022-07-18 10:50:09.690023 pydantic_distiller-0.2.5/.editorconfig
+-rw-r--r--   0        0        0      277 2022-07-18 10:50:09.690299 pydantic_distiller-0.2.5/.flake8
+-rw-r--r--   0        0        0      504 2023-06-16 12:58:18.333506 pydantic_distiller-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1083 2022-07-18 10:50:09.690888 pydantic_distiller-0.2.5/LICENSE
+-rw-r--r--   0        0        0      346 2022-07-18 10:50:09.691182 pydantic_distiller-0.2.5/Makefile
+-rw-r--r--   0        0        0      186 2022-07-18 10:50:09.691441 pydantic_distiller-0.2.5/README.md
+-rw-r--r--   0        0        0      559 2023-06-16 12:58:18.334427 pydantic_distiller-0.2.5/distiller/__init__.py
+-rw-r--r--   0        0        0     5023 2023-06-16 12:58:18.335259 pydantic_distiller-0.2.5/distiller/base.py
+-rw-r--r--   0        0        0     2219 2022-07-18 13:45:06.706000 pydantic_distiller-0.2.5/distiller/helpers.py
+-rw-r--r--   0        0        0      334 2022-07-18 13:45:06.708000 pydantic_distiller-0.2.5/distiller/json/__init__.py
+-rw-r--r--   0        0        0     3470 2022-07-18 13:45:06.709000 pydantic_distiller-0.2.5/distiller/markup/__init__.py
+-rw-r--r--   0        0        0     1987 2022-07-18 13:45:06.710000 pydantic_distiller-0.2.5/distiller/markup/mapper.py
+-rw-r--r--   0        0        0     7793 2022-07-18 13:45:06.710000 pydantic_distiller-0.2.5/distiller/markup/parser.py
+-rw-r--r--   0        0        0     2348 2022-07-18 13:45:06.711000 pydantic_distiller-0.2.5/distiller/markup/preprocessor.py
+-rw-r--r--   0        0        0    11530 2023-06-16 12:58:18.335995 pydantic_distiller-0.2.5/distiller/nodes.py
+-rw-r--r--   0        0        0      455 2022-07-18 10:50:09.694573 pydantic_distiller-0.2.5/mypy.ini
+-rw-r--r--   0        0        0     1633 2023-06-16 13:14:06.079899 pydantic_distiller-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       76 2022-07-18 10:50:09.695030 pydantic_distiller-0.2.5/pytest.ini
+-rw-r--r--   0        0        0        0 2022-07-18 10:50:09.695367 pydantic_distiller-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0      106 2022-07-18 10:50:09.695646 pydantic_distiller-0.2.5/tests/conftest.py
+-rw-r--r--   0        0        0      420 2022-07-18 10:50:09.696049 pydantic_distiller-0.2.5/tests/helpers.py
+-rw-r--r--   0        0        0      513 2022-07-18 10:50:09.696388 pydantic_distiller-0.2.5/tests/playground.py
+-rw-r--r--   0        0        0     1776 2022-07-18 10:50:09.696645 pydantic_distiller-0.2.5/tests/test_base_distiller_setup.py
+-rw-r--r--   0        0        0     3587 2023-06-16 12:58:18.338466 pydantic_distiller-0.2.5/tests/test_base_nodes.py
+-rw-r--r--   0        0        0      962 2022-07-18 10:50:09.697191 pydantic_distiller-0.2.5/tests/test_distilled_finalization.py
+-rw-r--r--   0        0        0     1127 2022-07-18 10:50:09.697519 pydantic_distiller-0.2.5/tests/test_helpers.py
+-rw-r--r--   0        0        0     3178 2022-07-18 10:50:09.697905 pydantic_distiller-0.2.5/tests/test_htmlfication.py
+-rw-r--r--   0        0        0     4124 2022-07-18 10:50:09.698201 pydantic_distiller-0.2.5/tests/test_markup_parsing.py
+-rw-r--r--   0        0        0      954 2022-07-18 10:50:09.698528 pydantic_distiller-0.2.5/tests/test_plaintextification.py
+-rw-r--r--   0        0        0     1799 2022-07-18 10:50:09.698900 pydantic_distiller-0.2.5/tests/test_tagification.py
+-rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 pydantic_distiller-0.2.5/PKG-INFO
```

### Comparing `pydantic-distiller-0.2.4/LICENSE` & `pydantic_distiller-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/distiller/__init__.py` & `pydantic_distiller-0.2.5/distiller/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/distiller/base.py` & `pydantic_distiller-0.2.5/distiller/base.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/distiller/helpers.py` & `pydantic_distiller-0.2.5/distiller/helpers.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/distiller/markup/__init__.py` & `pydantic_distiller-0.2.5/distiller/markup/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/distiller/markup/mapper.py` & `pydantic_distiller-0.2.5/distiller/markup/mapper.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/distiller/markup/parser.py` & `pydantic_distiller-0.2.5/distiller/markup/parser.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/distiller/markup/preprocessor.py` & `pydantic_distiller-0.2.5/distiller/markup/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/distiller/nodes.py` & `pydantic_distiller-0.2.5/distiller/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,29 +13,33 @@
     NamedTuple,
     Optional,
     Set,
     Type,
     Union,
 )
 
-from pydantic import BaseModel, Extra, Field, NoneStr, validator
+from pydantic import BaseModel, Extra, Field, NoneStr, PrivateAttr, validator
 
 from .helpers import KNOWN_CONTAINER_KINDS, NodeKind, jsonify_node_value, normalize_whitespace
 
 RESERVED_NODE_ATTRS_NAMES = {'kind', 'children'}
 DEFAULT_NODE_SCHEMA_TITLE = 'Distilled node'
 TEXT_NODE_KIND = NodeKind('text')
 INVALID_NODE_KIND = NodeKind('invalid-node')
 
 
 class NodeContext(NamedTuple):
     parent: Optional['Node'] = None
     data: Dict[str, Any] = {}
 
 
+class State(BaseModel):
+    context: NodeContext = Field(default_factory=NodeContext)
+
+
 class BaseNode(BaseModel):
     kind: NodeKind
 
     def serialize(self, **kwargs: Any) -> Any:
         return self.dict(**kwargs)
 
     def to_html(self, **kwargs: Any) -> str:
@@ -45,14 +49,16 @@
         raise NotImplementedError  # pragma: no cover
 
 
 class Node(BaseNode):
     kind: NodeKind = Field(default=None, title='Distilled node kind')
     children: 'NodeChildren' = Field(default=[], title='Distilled subnodes')
 
+    _state: State = PrivateAttr(default_factory=State)
+
     # Custom kind value may be set only for base nodes without specific schema,
     # otherwise class name is used
     @validator('kind', pre=True, always=True)
     def set_node_kind(cls, value: NoneStr) -> NodeKind:
         if value is not None and cls is Node:  # type: ignore
             return NodeKind(value)
         return cls.get_node_kind_value()
@@ -159,27 +165,24 @@
     @property
     def post_init_method(self) -> Optional[Callable]:
         method = getattr(self, 'post_init', None)
         return method if callable(method) else None
 
     @property
     def context(self) -> NodeContext:
-        return self._State.context
+        return self._state.context
 
     def update_context(self, parent: 'Node' = None, **kwargs: Any) -> NodeContext:
         ctx = NodeContext(
-            parent=parent or self._State.context.parent,
-            data={**self._State.context.data, **kwargs},
+            parent=parent or self._state.context.parent,
+            data={**self._state.context.data, **kwargs},
         )
-        self._State.context = ctx
+        self._state.context = ctx
         return ctx
 
-    class _State:
-        context: NodeContext = NodeContext()
-
     class Config:
         @staticmethod
         def _modify_node_schema(schema: Dict[str, Any], model: 'NodeType') -> None:
             title = schema.get('title', None)
             if title in {DEFAULT_NODE_SCHEMA_TITLE, None}:
                 title = model.__name__
             properties = schema.get('properties', {})
```

### Comparing `pydantic-distiller-0.2.4/pyproject.toml` & `pydantic_distiller-0.2.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "pydantic-distiller"
-version = "0.2.4"
-description = "HTML/JSON documents parser into Pydantic models"
+version = "0.2.5"
 authors = [
-  {name = "Arseny Gabdullin", email = "a.gabdullin@tinkoff.ru"}
+    {name = "Arseny Gabdullin", email = "a.gabdullin@tinkoff.ru"},
+    {name = "Vladimir Troflyanin", email = "v.troflyanin@tinkoff.ru"}
 ]
+readme = "README.md"
 classifiers = [
   "Intended Audience :: Information Technology",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
@@ -23,21 +24,24 @@
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development",
   "Topic :: Text Processing :: Markup :: HTML",
   "License :: OSI Approved :: MIT License",
 ]
 requires-python = ">=3.6"
 dependencies = [
-  "pydantic >=1.0.0",
+    "pydantic >=1.0.0",
 ]
-readme = "README.md"
+dynamic = ["description"]
 
 [project.urls]
 Source = "https://github.com/tinkoffjournal/distiller"
 
+[tool.flit.module]
+name = "distiller"
+
 [project.optional-dependencies]
 html = [
   "beautifulsoup4 >=4.8.1",
   "lxml",
 ]
 test = [
   "pytest >=4.0.0",
@@ -48,17 +52,14 @@
   "faker",
   "flake8",
 ]
 dev = [
   "devtools"
 ]
 
-[tool.flit.module]
-name = "distiller"
-
 [tool.black]
 target-version = ["py37"]
 skip-string-normalization = true
 line_length = 100
 
 [tool.isort]
 multi_line_output = 3
```

### Comparing `pydantic-distiller-0.2.4/tests/playground.py` & `pydantic_distiller-0.2.5/tests/playground.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/tests/test_base_distiller_setup.py` & `pydantic_distiller-0.2.5/tests/test_base_distiller_setup.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/tests/test_base_nodes.py` & `pydantic_distiller-0.2.5/tests/test_base_nodes.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,14 +52,27 @@
     parent_node = Node(kind='parent')
     lead = Lead()
     lead.update_context(parent=parent_node, foo='bar')
     assert lead.context.parent == parent_node
     assert lead.context.data['foo'] == 'bar'
 
 
+def test_node_switch_context():
+    first_lead = Lead()
+    second_lead = Lead()
+
+    first_lead.update_context(foo='foo')
+    second_lead.update_context(bar='bar')
+
+    assert first_lead.context.data.get('foo') == 'foo'
+    assert first_lead.context.data.get('bar') is None
+    assert second_lead.context.data.get('foo') is None
+    assert second_lead.context.data.get('bar') == 'bar'
+
+
 def test_node_schema():
     schema = Lead.schema()
     assert schema['title'] == Lead.__name__
     assert schema['properties']['allOf'] == {'$ref': f'#/definitions/{Node.__name__}'}
 
 
 @mark.parametrize(
```

### Comparing `pydantic-distiller-0.2.4/tests/test_distilled_finalization.py` & `pydantic_distiller-0.2.5/tests/test_distilled_finalization.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/tests/test_helpers.py` & `pydantic_distiller-0.2.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/tests/test_htmlfication.py` & `pydantic_distiller-0.2.5/tests/test_htmlfication.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/tests/test_markup_parsing.py` & `pydantic_distiller-0.2.5/tests/test_markup_parsing.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/tests/test_plaintextification.py` & `pydantic_distiller-0.2.5/tests/test_plaintextification.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/tests/test_tagification.py` & `pydantic_distiller-0.2.5/tests/test_tagification.py`

 * *Files identical despite different names*

### Comparing `pydantic-distiller-0.2.4/PKG-INFO` & `pydantic_distiller-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pydantic-distiller
-Version: 0.2.4
+Version: 0.2.5
 Summary: HTML/JSON documents parser into Pydantic models
-Author-email: Arseny Gabdullin <a.gabdullin@tinkoff.ru>
+Author-email: Arseny Gabdullin <a.gabdullin@tinkoff.ru>, Vladimir Troflyanin <v.troflyanin@tinkoff.ru>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

