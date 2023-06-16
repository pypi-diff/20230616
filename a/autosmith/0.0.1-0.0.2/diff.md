# Comparing `tmp/autosmith-0.0.1.tar.gz` & `tmp/autosmith-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosmith-0.0.1.tar", last modified: Thu Jun 15 05:10:17 2023, max compression
+gzip compressed data, was "autosmith-0.0.2.tar", last modified: Fri Jun 16 05:32:29 2023, max compression
```

## Comparing `autosmith-0.0.1.tar` & `autosmith-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:10:17.424484 autosmith-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 05:09:55.000000 autosmith-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-15 05:10:17.424484 autosmith-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 05:09:55.000000 autosmith-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:10:17.424484 autosmith-0.0.1/autosmith/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 05:09:55.000000 autosmith-0.0.1/autosmith/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-15 05:09:55.000000 autosmith-0.0.1/autosmith/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-15 05:09:55.000000 autosmith-0.0.1/autosmith/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:10:17.424484 autosmith-0.0.1/autosmith/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-15 05:09:55.000000 autosmith-0.0.1/autosmith/templates/Dockerfile.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-15 05:09:55.000000 autosmith-0.0.1/autosmith/templates/main.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-15 05:09:55.000000 autosmith-0.0.1/autosmith/types.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 05:09:55.000000 autosmith-0.0.1/autosmith/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:10:17.424484 autosmith-0.0.1/autosmith.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-15 05:10:17.000000 autosmith-0.0.1/autosmith.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-15 05:10:17.000000 autosmith-0.0.1/autosmith.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 05:10:17.000000 autosmith-0.0.1/autosmith.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 05:10:17.000000 autosmith-0.0.1/autosmith.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 05:10:17.000000 autosmith-0.0.1/autosmith.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 05:10:17.428484 autosmith-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-15 05:09:55.000000 autosmith-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:10:17.424484 autosmith-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-15 05:09:55.000000 autosmith-0.0.1/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-15 05:09:55.000000 autosmith-0.0.1/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:29.181148 autosmith-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 05:32:02.000000 autosmith-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-16 05:32:29.181148 autosmith-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-16 05:32:02.000000 autosmith-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:29.177147 autosmith-0.0.2/autosmith/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:02.000000 autosmith-0.0.2/autosmith/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-16 05:32:02.000000 autosmith-0.0.2/autosmith/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-16 05:32:02.000000 autosmith-0.0.2/autosmith/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-16 05:32:02.000000 autosmith-0.0.2/autosmith/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-16 05:32:02.000000 autosmith-0.0.2/autosmith/smith.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-16 05:32:02.000000 autosmith-0.0.2/autosmith/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-16 05:32:02.000000 autosmith-0.0.2/autosmith/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:29.181148 autosmith-0.0.2/autosmith/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-16 05:32:02.000000 autosmith-0.0.2/autosmith/templates/Dockerfile.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-16 05:32:02.000000 autosmith-0.0.2/autosmith/templates/main.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 05:32:02.000000 autosmith-0.0.2/autosmith/templates/requirements.txt.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 05:32:02.000000 autosmith-0.0.2/autosmith/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:29.181148 autosmith-0.0.2/autosmith.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-16 05:32:29.000000 autosmith-0.0.2/autosmith.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-16 05:32:29.000000 autosmith-0.0.2/autosmith.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 05:32:29.000000 autosmith-0.0.2/autosmith.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 05:32:29.000000 autosmith-0.0.2/autosmith.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 05:32:29.000000 autosmith-0.0.2/autosmith.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 05:32:29.181148 autosmith-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-16 05:32:02.000000 autosmith-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:29.181148 autosmith-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-16 05:32:02.000000 autosmith-0.0.2/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-16 05:32:02.000000 autosmith-0.0.2/tests/test_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-16 05:32:02.000000 autosmith-0.0.2/tests/test_template.py
```

### Comparing `autosmith-0.0.1/LICENSE` & `autosmith-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autosmith-0.0.1/autosmith/template.py` & `autosmith-0.0.2/autosmith/template.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import ast
 import inspect
 import json
 import textwrap
+import warnings
 from typing import Callable, Optional, Union, cast
 
+from datamodel_code_generator.parser.jsonschema import JsonSchemaParser
 from jinja2 import Environment, PackageLoader
 from pydantic import BaseModel, create_model
 
-from .env import consistent_requirements, get_requirements
-from .types import EncodedTool, ToolEnv
+from .env import EncodedTool, ToolEnv
+from .func import consistent_requirements, get_requirements
 
 
 def make_schema(func: Callable) -> BaseModel:
     """Make a schema from a function"""
     name = func.__name__
     desc = func.__doc__
+    if desc is None:
+        raise ValueError("Function must have a docstring if inferring schema")
     properties = {}
-    for arg in func.__code__.co_varnames:
-        # use type hints
-        if arg in func.__annotations__:
-            properties[arg] = (func.__annotations__[arg], ...)
+    for arg in func.__code__.co_varnames[: func.__code__.co_argcount]:
         # use default values
-        elif func.__defaults__ and arg in func.__defaults__:
-            properties[arg] = (
-                type(
-                    func.__defaults__[
-                        func.__code__.co_varnames.index(arg) - len(func.__defaults__)
-                    ]
-                ),
-                ...,
-            )
-        # use str as default
+        if func.__defaults__ and arg in func.__defaults__:
+            properties[arg] = func.__defaults__[func.__code__.co_varnames.index(arg)]
+        # use type hints (no elif - intentional
+        if arg in func.__annotations__:
+            if arg in properties:
+                properties[arg] = (func.__annotations__[arg], properties[arg])
+            else:
+                properties[arg] = (func.__annotations__[arg], ...)
+        # use str as default (or rely on type inference from default)
         else:
             properties[arg] = (str, ...)
-    return create_model(name, **properties, description=desc)
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+        return create_model(name.capitalize(), **properties, __doc__=desc)
 
 
 def get_func_name(func: Union[Callable, str]) -> str:
     """Get the name of a function"""
     if callable(func):
         return func.__name__
 
@@ -65,41 +67,46 @@
     raise ValueError("Could not find function description")
 
 
 def func_to_url(name: str) -> str:
     return name.replace("_", "-")
 
 
-def template_server(
+def render_server(
     func: Union[Callable, str],
     schema: Optional[Union[BaseModel, str]] = None,
     tool_env: Optional[ToolEnv] = None,
 ) -> str:
     """Stamp a function with a schema and tool environment"""
     if isinstance(func, str) and schema is None:
         raise ValueError("Must provide schema if func is a string")
     raw_schema: Optional[str] = None
     schema_title: str = ""
     if schema is None:
         schema = make_schema(cast(Callable, func))
     if not isinstance(schema, str):
         schema_title = schema.__name__
-        schema = json.dumps(schema.schema())
+        parser = JsonSchemaParser(schema.schema_json())
+        parser.parse_raw()
+        raw_schema = parser.results[0].render()
     else:
         schema = cast(str, schema)
         # check if schema is valid json
         try:
-            json.loads(schema)
             schema_title = json.loads(schema)["title"]
+            parser = JsonSchemaParser(schema)
+            parser.parse_raw()
+            raw_schema = parser.results[0].render()
         except json.JSONDecodeError:
             # if not, assume it's python code
             raw_schema = textwrap.dedent(schema)
             schema_title = (
                 raw_schema.split("(BaseModel):")[0].split("class ")[1].strip()
             )
+
     func_requirements = get_requirements(func)
     env = Environment(loader=PackageLoader("autosmith", "templates"))
 
     if not tool_env:
         tool_env = ToolEnv(requirements=func_requirements, tools={})
 
     if not consistent_requirements(tool_env.requirements, func_requirements):
@@ -112,24 +119,30 @@
 
     # convert schema and func to tool
     tool = EncodedTool(
         function=source,
         function_name=get_func_name(func),
         description=get_func_description(func),
         input_class_name=schema_title,
-        input_class_schema=schema,
         input_class_raw_schema=raw_schema,
     )
 
     # add tool to tool_env
     tool_env.tools[func_to_url(tool.function_name)] = tool
 
     # render tool_env
     template = env.get_template("main.py.jinja")
     return template.render(env=tool_env)
 
 
-def template_container(tool_env: ToolEnv) -> str:
+def render_container(tool_env: ToolEnv) -> str:
     """template a container with a tool environment"""
     env = Environment(loader=PackageLoader("autosmith", "templates"))
     template = env.get_template("Dockerfile.jinja")
     return template.render(env=tool_env)
+
+
+def render_requirements(tool_env: ToolEnv) -> str:
+    """Render requirements.txt from tool_env"""
+    env = Environment(loader=PackageLoader("autosmith", "templates"))
+    template = env.get_template("requirements.txt.jinja")
+    return template.render(env=tool_env)
```

### Comparing `autosmith-0.0.1/setup.py` & `autosmith-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,20 @@
     description="Make tools quickly automatically",
     author="Andrew White",
     author_email="white.d.andrew@gmail.com",
     url="https://github.com/whitead/autosmith",
     license="Apache 2.0",
     packages=["autosmith"],
     package_data={"autosmith": ["templates/*"]},
-    install_requires=["jinja2", "pydantic", "importlib_metadata"],
+    install_requires=[
+        "jinja2",
+        "pydantic",
+        "datamodel_code_generator",
+        "importlib_metadata",
+    ],
     test_suite="tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `autosmith-0.0.1/tests/test_env.py` & `autosmith-0.0.2/tests/test_func.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from math import *  # noqa
 
 import pytest
 from numpy import arange
 
-from autosmith.env import (
+from autosmith.func import (
     consistent_requirements,
     get_func_imports,
     get_imports,
     get_requirements_from_imports,
+    merge_requirements,
 )
 
 
 def test_nested_imports():
     source = "import a.b.c\n" "from a.b import c\n" "c.do_something()\n"
     imports, _ = get_imports(source)
     # Assert that the imports list contains the expected modules
@@ -74,34 +75,58 @@
     assert "numpy" in reqs
     assert "pytest" in reqs
     assert "foo" not in reqs
 
 
 def test_consistent_requirements():
     env = """
-    numpy>=1.19.5
+    numpy==1.19.5
     pytest==6.2.2
     """
     proposed = """
     numpy==1.19.5
     pytest==6.2.2
     """
 
     assert consistent_requirements(env, proposed)
 
     proposed = """
-    numpy==1.23
-    pytest==6.2.2
+    numpy==1.19.5
     """
 
     assert consistent_requirements(env, proposed)
 
     proposed = """
     numpy==1.18
-    pytest==6.2.2
+    pytest
     """
 
     assert not consistent_requirements(env, proposed)
 
 
 def test_str_func():
     get_func_imports("def foo(): pass")
+
+
+def test_merge_requirements():
+    env = """
+    numpy==1.19.5
+    pytest==6.2.2
+    """
+    proposed = """
+    numpy==1.19.5
+    pytest==6.2.2
+    """
+
+    assert consistent_requirements(env, merge_requirements(env, proposed))
+
+    proposed = """
+    numpy
+    """
+
+    assert not consistent_requirements(env, merge_requirements(env, proposed))
+
+    proposed = """
+    rdkit
+    """
+
+    assert consistent_requirements(env + "\nrdkit", merge_requirements(env, proposed))
```

### Comparing `autosmith-0.0.1/tests/test_template.py` & `autosmith-0.0.2/tests/test_template.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import ast
 
 import pytest
 from pydantic import BaseModel
 
+from autosmith.env import ToolEnv
 from autosmith.template import (
     func_to_url,
     get_func_description,
     get_func_name,
     make_schema,
-    template_container,
-    template_server,
+    render_container,
+    render_server,
 )
-from autosmith.types import ToolEnv
 
 
 def is_valid_python(code):
     try:
         ast.parse(code)
     except SyntaxError:
         return False
@@ -23,21 +23,54 @@
 
 
 def test_make_schema():
     def func(a: int, b: float) -> int:
         """Add a and b"""
         return int(a + b)
 
+    class Func(BaseModel):
+        """Add a and b"""
+
+        a: int
+        b: float
+
     schema = make_schema(func)
-    foo = schema(a=1, b=2.0)
-    assert foo.a == 1
-    assert foo.b == 2.0
-    assert foo.a.__class__.__name__ == "int"
-    assert foo.description == "Add a and b"
-    assert foo.__class__.__name__ == "func"
+    assert schema.schema() == Func.schema()
+
+
+def test_make_schema_imports():
+    def func(a: int, b: float) -> int:
+        """Add a and b"""
+        return int(a + b)
+
+    class Func(BaseModel):
+        """Add a and b"""
+
+        a: int
+        b: float
+
+    schema = make_schema(func)
+    print(schema.schema())
+    assert schema.schema() == Func.schema()
+
+
+def test_empty_schema():
+    """Test with callable function and make sure schema is empty"""
+
+    def func() -> str:
+        """print hello world"""
+        return "hello world"
+
+    class Func(BaseModel):
+        """print hello world"""
+
+        pass
+
+    schema = make_schema(func)
+    assert schema.schema() == Func.schema()
 
 
 def test_get_func_name():
     def func(a: int, b: float) -> int:
         """Add a and b"""
         return int(a + b)
 
@@ -63,16 +96,18 @@
         """Add a and b"""
         return int(a + b)
 
     class Schema(BaseModel):
         a: int
         b: float
 
-    rendered = template_server(func, schema=Schema)
+    rendered = render_server(func, schema=Schema)
     assert is_valid_python(rendered)
+    print(rendered)
+    assert "Schema(BaseModel):" in rendered
 
 
 def test_template_server_str():
     """Test with callable function and BaseModel schema"""
 
     func = """
     def func(a: int, b: float) -> int:
@@ -80,39 +115,47 @@
         return int(a + b)
     """
     schema = """
     class Schema(BaseModel):
         a: int
         b: float
     """
-    rendered = template_server(func, schema)
+    rendered = render_server(func, schema)
     assert is_valid_python(rendered)
+    assert "Schema(BaseModel):" in rendered
 
 
 def test_template_server_infer():
     """Test with callable function and BaseModel schema"""
 
     def func(a: int, b: float) -> int:
         """Add a and b"""
         return int(a + b)
 
-    rendered = template_server(func)
+    rendered = render_server(func)
     assert is_valid_python(rendered)
+    assert "Func(BaseModel):" in rendered
 
 
 def test_template_server_fail():
     """Test with callable function and BaseModel schema"""
 
     func = """
     def func(a: int, b: float) -> int:
         '''Add a and b'''
         return a + b
     """
     with pytest.raises(ValueError):
-        template_server(func)
+        render_server(func)
+
+    def no_doc():
+        pass
+
+    with pytest.raises(ValueError):
+        render_server(no_doc)
 
 
 def test_template_container():
     """Test templating container"""
     tool_env = ToolEnv(requirements="pytest==6.2.2")
-    rendered = template_container(tool_env)
-    assert tool_env.host in rendered
+    rendered = render_container(tool_env)
+    assert str(tool_env.port) in rendered
```

