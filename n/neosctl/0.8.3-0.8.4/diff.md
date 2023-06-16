# Comparing `tmp/neosctl-0.8.3.tar.gz` & `tmp/neosctl-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosctl-0.8.3.tar", max compression
+gzip compressed data, was "neosctl-0.8.4.tar", max compression
```

## Comparing `neosctl-0.8.3.tar` & `neosctl-0.8.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2655 2023-06-13 11:01:13.522248 neosctl-0.8.3/README.md
--rw-r--r--   0        0        0       22 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/__init__.py
--rw-r--r--   0        0        0     1723 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/auth.py
--rw-r--r--   0        0        0     3853 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/cli.py
--rw-r--r--   0        0        0      224 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/constant.py
--rw-r--r--   0        0        0     4528 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/profile.py
--rw-r--r--   0        0        0     2432 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/schema.py
--rw-r--r--   0        0        0      138 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/services/__init__.py
--rw-r--r--   0        0        0      947 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/services/gateway/__init__.py
--rw-r--r--   0        0        0    14331 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/services/gateway/data_product.py
--rw-r--r--   0        0        0     5584 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/services/gateway/data_source.py
--rw-r--r--   0        0        0     3962 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/services/gateway/data_system.py
--rw-r--r--   0        0        0     6290 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/data_unit.py
--rw-r--r--   0        0        0     5271 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/entity.py
--rw-r--r--   0        0        0     2655 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/link.py
--rw-r--r--   0        0        0     4556 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/output.py
--rw-r--r--   0        0        0     3388 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/schema.py
--rw-r--r--   0        0        0     2526 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/secret.py
--rw-r--r--   0        0        0     1409 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/spark.py
--rw-r--r--   0        0        0     1678 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/tag.py
--rw-r--r--   0        0        0       55 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/iam/__init__.py
--rw-r--r--   0        0        0     3764 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/iam/iam.py
--rw-r--r--   0        0        0      664 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/iam/schema.py
--rw-r--r--   0        0        0       65 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/registry/__init__.py
--rw-r--r--   0        0        0     3067 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/registry/registry.py
--rw-r--r--   0        0        0      141 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/registry/schema.py
--rw-r--r--   0        0        0       63 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/storage/__init__.py
--rw-r--r--   0        0        0     8556 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/storage/storage.py
--rw-r--r--   0        0        0    12292 2023-06-13 11:01:13.525248 neosctl-0.8.3/neosctl/util.py
--rw-r--r--   0        0        0     3050 2023-06-13 11:01:13.525248 neosctl-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     2655 2023-06-16 12:39:32.840874 neosctl-0.8.4/README.md
+-rw-r--r--   0        0        0       22 2023-06-16 12:39:32.841874 neosctl-0.8.4/neosctl/__init__.py
+-rw-r--r--   0        0        0     1723 2023-06-16 12:39:32.841874 neosctl-0.8.4/neosctl/auth.py
+-rw-r--r--   0        0        0     3853 2023-06-16 12:39:32.841874 neosctl-0.8.4/neosctl/cli.py
+-rw-r--r--   0        0        0      224 2023-06-16 12:39:32.841874 neosctl-0.8.4/neosctl/constant.py
+-rw-r--r--   0        0        0     4528 2023-06-16 12:39:32.841874 neosctl-0.8.4/neosctl/profile.py
+-rw-r--r--   0        0        0     2432 2023-06-16 12:39:32.841874 neosctl-0.8.4/neosctl/schema.py
+-rw-r--r--   0        0        0      138 2023-06-16 12:39:32.841874 neosctl-0.8.4/neosctl/services/__init__.py
+-rw-r--r--   0        0        0      947 2023-06-16 12:39:32.841874 neosctl-0.8.4/neosctl/services/gateway/__init__.py
+-rw-r--r--   0        0        0    14331 2023-06-16 12:39:32.841874 neosctl-0.8.4/neosctl/services/gateway/data_product.py
+-rw-r--r--   0        0        0     5584 2023-06-16 12:39:32.841874 neosctl-0.8.4/neosctl/services/gateway/data_source.py
+-rw-r--r--   0        0        0     3962 2023-06-16 12:39:32.841874 neosctl-0.8.4/neosctl/services/gateway/data_system.py
+-rw-r--r--   0        0        0     6290 2023-06-16 12:39:32.841874 neosctl-0.8.4/neosctl/services/gateway/data_unit.py
+-rw-r--r--   0        0        0     5491 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/gateway/entity.py
+-rw-r--r--   0        0        0     2655 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/gateway/link.py
+-rw-r--r--   0        0        0     4556 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/gateway/output.py
+-rw-r--r--   0        0        0     3388 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/gateway/schema.py
+-rw-r--r--   0        0        0     2526 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/gateway/secret.py
+-rw-r--r--   0        0        0     1409 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/gateway/spark.py
+-rw-r--r--   0        0        0     1678 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/gateway/tag.py
+-rw-r--r--   0        0        0       55 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/iam/__init__.py
+-rw-r--r--   0        0        0     3764 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/iam/iam.py
+-rw-r--r--   0        0        0      664 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/iam/schema.py
+-rw-r--r--   0        0        0       65 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/registry/__init__.py
+-rw-r--r--   0        0        0     3067 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/registry/registry.py
+-rw-r--r--   0        0        0      141 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/registry/schema.py
+-rw-r--r--   0        0        0       63 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/storage/__init__.py
+-rw-r--r--   0        0        0     8556 2023-06-16 12:39:32.842874 neosctl-0.8.4/neosctl/services/storage/storage.py
+-rw-r--r--   0        0        0    12292 2023-06-16 12:39:32.843874 neosctl-0.8.4/neosctl/util.py
+-rw-r--r--   0        0        0     3050 2023-06-16 12:39:32.843874 neosctl-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.4/PKG-INFO
```

### Comparing `neosctl-0.8.3/README.md` & `neosctl-0.8.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Core CLI v0.8.3
+# Core CLI v0.8.4
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

### Comparing `neosctl-0.8.3/neosctl/auth.py` & `neosctl-0.8.4/neosctl/auth.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/cli.py` & `neosctl-0.8.4/neosctl/cli.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/profile.py` & `neosctl-0.8.4/neosctl/profile.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/schema.py` & `neosctl-0.8.4/neosctl/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/gateway/__init__.py` & `neosctl-0.8.4/neosctl/services/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/gateway/data_product.py` & `neosctl-0.8.4/neosctl/services/gateway/data_product.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/gateway/data_source.py` & `neosctl-0.8.4/neosctl/services/gateway/data_source.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/gateway/data_system.py` & `neosctl-0.8.4/neosctl/services/gateway/data_system.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/gateway/data_unit.py` & `neosctl-0.8.4/neosctl/services/gateway/data_unit.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/gateway/entity.py` & `neosctl-0.8.4/neosctl/services/gateway/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass
 from typing import List, Optional
 
 import typer
-from pydantic import typing
 
 from neosctl import util
 from neosctl.services.gateway import schema
 
 
 @dataclass
 class EntityArgGenerator:
@@ -65,19 +64,26 @@
     url_prefix: str,
     label: str,
     name: str,
     description: str,
     owner: Optional[str],
     contacts: List[str],
     links: List[str],
-    entity_schema: typing.Optional[schema.CreateElement] = None,
+    entity_schema: Optional[schema.CreateEntity] = None,
 ) -> None:
     """Create entity."""
-    info = None
-    if owner is not None:
+    if owner is None:
+        if len(contacts) == 0 and len(links) == 0:
+            info = None
+        else:
+            raise util.exit_with_output(
+                msg="Set info fields: owner (required), constacts (optional) and links (optional).",
+                exit_code=1,
+            )
+    else:
         info = schema.EntityInfo(
             owner=owner,
             contact_ids=contacts,
             links=links,
         )
 
     if entity_schema is None:
@@ -117,15 +123,15 @@
 def update_entity(
     ctx: typer.Context,
     url_prefix: str,
     identifier: str,
     label: str,
     name: str,
     description: str,
-    entity_schema: typing.Optional[schema.CreateElement] = None,
+    entity_schema: Optional[schema.CreateEntity] = None,
 ) -> None:
     """Update entity."""
     if entity_schema is None:
         entity_schema = schema.CreateEntity(
             name=name,
             label=label,
             description=description,
```

### Comparing `neosctl-0.8.3/neosctl/services/gateway/link.py` & `neosctl-0.8.4/neosctl/services/gateway/link.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/gateway/output.py` & `neosctl-0.8.4/neosctl/services/gateway/output.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -100,17 +100,17 @@
 
 
 @app.command(name="update")
 def update_entity(
     ctx: typer.Context,
     identifier: str = arg_generator.identifier,
     label: str = arg_generator.label,
-    output_type: OutputType = typer.Argument(OutputType.application, help="Output type"),
     name: str = arg_generator.name,
     description: str = arg_generator.description,
+    output_type: OutputType = typer.Argument(OutputType.application, help="Output type"),
 ) -> None:
     """Update output."""
     entity_schema = schema.CreateOutput(
         name=name,
         label=label,
         description=description,
         output_type=output_type.value,
```

### Comparing `neosctl-0.8.3/neosctl/services/gateway/schema.py` & `neosctl-0.8.4/neosctl/services/gateway/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/gateway/secret.py` & `neosctl-0.8.4/neosctl/services/gateway/secret.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/gateway/spark.py` & `neosctl-0.8.4/neosctl/services/gateway/spark.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/gateway/tag.py` & `neosctl-0.8.4/neosctl/services/gateway/tag.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/iam/iam.py` & `neosctl-0.8.4/neosctl/services/iam/iam.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/iam/schema.py` & `neosctl-0.8.4/neosctl/services/iam/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/registry/registry.py` & `neosctl-0.8.4/neosctl/services/registry/registry.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/services/storage/storage.py` & `neosctl-0.8.4/neosctl/services/storage/storage.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/neosctl/util.py` & `neosctl-0.8.4/neosctl/util.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.3/pyproject.toml` & `neosctl-0.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neosctl"
-version = "0.8.3"
+version = "0.8.4"
 description = "Nortal Core CLI"
 authors = []
 license = "closed"
 repository="https://github.com/NEOS-Critical/neos-platform-cli"
 homepage="https://github.com/NEOS-Critical/neos-platform-cli"
 readme = "README.md"
```

### Comparing `neosctl-0.8.3/PKG-INFO` & `neosctl-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosctl
-Version: 0.8.3
+Version: 0.8.4
 Summary: Nortal Core CLI
 Home-page: https://github.com/NEOS-Critical/neos-platform-cli
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Requires-Dist: minio (>=7.1.14,<8.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: typing_extensions (<4.6.0) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-cli
 Description-Content-Type: text/markdown
 
-# Core CLI v0.8.3
+# Core CLI v0.8.4
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

