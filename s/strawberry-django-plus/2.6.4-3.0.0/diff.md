# Comparing `tmp/strawberry_django_plus-2.6.4.tar.gz` & `tmp/strawberry_django_plus-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-2.6.4.tar", max compression
+gzip compressed data, was "strawberry_django_plus-3.0.0.tar", max compression
```

## Comparing `strawberry_django_plus-2.6.4.tar` & `strawberry_django_plus-3.0.0.tar`

### file list

```diff
@@ -1,39 +1,37 @@
--rw-r--r--   0        0        0     1094 2023-06-14 19:24:58.798656 strawberry_django_plus-2.6.4/LICENSE
--rw-r--r--   0        0        0     3299 2023-06-14 19:24:58.798656 strawberry_django_plus-2.6.4/README.md
--rw-r--r--   0        0        0     4309 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/pyproject.toml
--rw-r--r--   0        0        0     3001 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5562 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5752 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    26052 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3054 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1657 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1389 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0     6304 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/middlewares/debug_toolbar.py
--rw-r--r--   0        0        0      896 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/middlewares/user_warmup.py
--rw-r--r--   0        0        0        0 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    25062 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14825 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    26108 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1357 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    27526 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0    47691 2023-06-14 19:24:58.802656 strawberry_django_plus-2.6.4/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1107 2023-06-14 19:24:58.806656 strawberry_django_plus-2.6.4/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0     1445 2023-06-14 19:24:58.806656 strawberry_django_plus-2.6.4/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
--rw-r--r--   0        0        0        0 2023-06-14 19:24:58.806656 strawberry_django_plus-2.6.4/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2408 2023-06-14 19:24:58.806656 strawberry_django_plus-2.6.4/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    18649 2023-06-14 19:24:58.806656 strawberry_django_plus-2.6.4/strawberry_django_plus/type.py
--rw-r--r--   0        0        0    10297 2023-06-14 19:24:58.806656 strawberry_django_plus-2.6.4/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-06-14 19:24:58.806656 strawberry_django_plus-2.6.4/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6916 2023-06-14 19:24:58.806656 strawberry_django_plus-2.6.4/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    13223 2023-06-14 19:24:58.806656 strawberry_django_plus-2.6.4/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-06-14 19:24:58.806656 strawberry_django_plus-2.6.4/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-06-14 19:24:58.806656 strawberry_django_plus-2.6.4/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    13142 2023-06-14 19:24:58.806656 strawberry_django_plus-2.6.4/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-06-14 19:24:58.806656 strawberry_django_plus-2.6.4/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-06-15 22:48:01.093610 strawberry_django_plus-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3354 2023-06-15 22:48:01.093610 strawberry_django_plus-3.0.0/README.md
+-rw-r--r--   0        0        0     4208 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3001 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5649 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5752 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    28702 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3033 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1556 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1515 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     1939 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0      896 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/middlewares/user_warmup.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    23947 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14791 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    26439 2023-06-15 22:48:01.097610 strawberry_django_plus-3.0.0/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1340 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    28085 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0     2532 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1027 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2408 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    16382 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0     9889 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6916 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    13223 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     5865 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    16244 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      938 2023-06-15 22:48:01.101610 strawberry_django_plus-3.0.0/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     4875 1970-01-01 00:00:00.000000 strawberry_django_plus-3.0.0/PKG-INFO
```

### Comparing `strawberry_django_plus-2.6.4/LICENSE` & `strawberry_django_plus-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.4/README.md` & `strawberry_django_plus-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
   using schema directives, supporting both
   [django authentication system](https://docs.djangoproject.com/en/4.0/topics/auth/default/),
   direct and per-object permission checking for backends that implement those (e.g.
   [django-guardian](https://django-guardian.readthedocs.io/en/stable/)).
 - [Mutations for Django](https://blb-ventures.github.io/strawberry-django-plus/mutations/),
   with CRUD support and automatic errors validation.
 - [Relay support](https://blb-ventures.github.io/strawberry-django-plus/quickstart/#relay-support)
-  for queries, connections and input mutations, all integrated with django types directly.
+  for queries, connections and input mutations, using the official strawberry's
+  [relay integration](https://strawberry.rocks/docs/guides/relay)
 - [Django Debug Toolbar integration](https://blb-ventures.github.io/strawberry-django-plus/debug-toolbar/)
   with graphiql to display metrics like SQL queries
 - Improved sync/async resolver that priorizes the model's cache to avoid have to use
   [sync_to_async](https://docs.djangoproject.com/en/4.0/topics/async/#asgiref.sync.sync_to_async)
   when not needed.
 
 ## Installation
```

### Comparing `strawberry_django_plus-2.6.4/pyproject.toml` & `strawberry_django_plus-3.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "2.6.4"
+version = "3.0.0"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
@@ -29,18 +29,17 @@
 ]
 packages = [{ include = "strawberry_django_plus" }]
 include = ["strawberry_django_plus/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django = ">= 3.2"
-strawberry-graphql = ">=0.161.0"
-strawberry-graphql-django = ">= 0.8"
+strawberry-graphql = ">=0.184.0"
+strawberry-graphql-django = ">= 0.9.4"
 typing-extensions = ">= 4.2.0"
-django-debug-toolbar = { version = ">=3.4", optional = true }
 django-choices-field = { version = ">=2.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 codecov = "^2.1.12"
 django-types = "^0.17.0"
 pytest = "^7.1.2"
@@ -55,21 +54,20 @@
 django-guardian = "^2.4.0"
 mkdocs = "^1.4.2"
 mkdocs-markdownextradata-plugin = "^0.2.5"
 mkdocs-material = "^9.0.9"
 mkdocs-minify-plugin = "^0.6.2"
 pymdown-extensions = ">=9.5,<11.0"
 Markdown = "^3.3.7"
-ruff = "^0.0.271"
+ruff = "^0.0.272"
 debugpy = "^1.6.7"
 
 
 [tool.poetry.extras]
 enum = ["django-choices-field"]
-debug-toolbar = ["django-debug-toolbar"]
 
 [tool.ruff]
 line-length = 100
 select = [
   "A",
   "ASYNC100",
   "ASYNC101",
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/__init__.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _original_process_type = object_type._process_type
 _original_wrap_dataclass = object_type._wrap_dataclass
 _original_field_init = StrawberryField.__init__
 _original_field_call = StrawberryField.__call__
 _original_enum_init = EnumDefinition.__init__
 _original_from_generic = NameConverter.from_generic
 
-__version__ = "2.6.4"  # x-release-please-version
+__version__ = "3.0.0"  # x-release-please-version
 
 
 def _get_doc(obj):
     if not obj.__doc__:
         return None
     return inspect.cleandoc(obj.__doc__)
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/descriptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Type,
     TypeVar,
     Union,
     overload,
 )
 
 from django.db.models.base import Model
+from strawberry.exceptions import MissingFieldAnnotationError
 from typing_extensions import Self
 
 if TYPE_CHECKING:
     from django.db.models.query import Prefetch
 
     from .optimizer import OptimizerStore, PrefetchType
     from .utils.typing import TypeOrSequence
@@ -57,14 +58,15 @@
         self.store = OptimizerStore.with_hints(
             only=only,
             select_related=select_related,
             prefetch_related=prefetch_related,
         )
 
     def __set_name__(self, owner: Type[_M], name: str):
+        self.origin = owner
         self.name = name
 
     @overload
     def __get__(self, obj: _M, cls: Type[_M]) -> _R:
         ...
 
     @overload
@@ -92,15 +94,15 @@
             return None
         return inspect.cleandoc(self.func.__doc__)
 
     @property
     def type_annotation(self) -> Union[object, str]:
         ret = self.func.__annotations__.get("return")
         if ret is None:
-            raise TypeError(f"missing type annotation from {self.func}")
+            raise MissingFieldAnnotationError(self.name, self.origin)
         return ret
 
 
 @overload
 def model_property(
     func: Callable[[_M], _R],
     *,
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/directives.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/field.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/field.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,70 @@
 import dataclasses
+import inspect
 from functools import cached_property
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
+    Iterable,
     List,
     Literal,
     Mapping,
     Optional,
     Sequence,
     Type,
     TypeVar,
     Union,
     cast,
-    get_args,
     overload,
 )
 
 import strawberry
 from django.db import models
 from django.db.models import QuerySet
 from django.db.models.fields.related_descriptors import (
     ForwardManyToOneDescriptor,
     ReverseManyToOneDescriptor,
     ReverseOneToOneDescriptor,
 )
 from django.db.models.query_utils import DeferredAttribute
-from strawberry import UNSET
+from strawberry import UNSET, relay
 from strawberry.annotation import StrawberryAnnotation
 from strawberry.arguments import StrawberryArgument
-from strawberry.extensions.field_extension import FieldExtension
+from strawberry.auto import StrawberryAuto
+from strawberry.extensions.field_extension import FieldExtension, SyncExtensionResolver
+from strawberry.field import _RESOLVER_TYPE, UNRESOLVED, StrawberryField
 from strawberry.lazy_type import LazyType
 from strawberry.permission import BasePermission
+from strawberry.relay.types import NodeIterableType
 from strawberry.type import StrawberryContainer, StrawberryType
 from strawberry.types.fields.resolver import StrawberryResolver
 from strawberry.types.info import Info
 from strawberry.types.types import TypeDefinition
 from strawberry.union import StrawberryUnion
 from strawberry_django.arguments import argument
 from strawberry_django.fields.field import (
     StrawberryDjangoField as _StrawberryDjangoField,
 )
-from strawberry_django.utils import get_django_model, unwrap_type
+from strawberry_django.fields.types import get_model_field, is_optional
+from strawberry_django.utils import unwrap_type
 
-from . import optimizer, relay
+from strawberry_django_plus.types import resolve_model_field_type
+from strawberry_django_plus.utils import aio
+
+from . import optimizer
 from .descriptors import ModelProperty
 from .permissions import filter_with_perms
 from .utils import resolvers
 from .utils.typing import TypeOrSequence
 
 __all__ = [
     "StrawberryDjangoField",
-    "StrawberryDjangoNodeField",
-    "StrawberryDjangoConnectionField",
+    "StrawberryDjangoConnectionExtension",
     "field",
     "node",
     "connection",
 ]
 
 _T = TypeVar("_T")
 _M = TypeVar("_M", bound=models.Model)
@@ -66,113 +73,134 @@
 class StrawberryDjangoField(_StrawberryDjangoField):
     """A strawberry field for django attributes.
 
     Do not instantiate this directly. Instead, use `@field` decorator.
 
     """
 
-    store: optimizer.OptimizerStore
-
-    def __init__(self, *args, **kwargs):
-        self.disable_optimization = kwargs.pop("disable_optimization", False)
+    def __init__(
+        self,
+        *args,
+        only: Optional[TypeOrSequence[str]] = None,
+        select_related: Optional[TypeOrSequence[str]] = None,
+        prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
+        disable_optimization: bool = False,
+        **kwargs,
+    ):
+        self.disable_optimization = disable_optimization
         self.store = optimizer.OptimizerStore.with_hints(
-            only=kwargs.pop("only", None),
-            select_related=kwargs.pop("select_related", None),
-            prefetch_related=kwargs.pop("prefetch_related", None),
+            only=only,
+            select_related=select_related,
+            prefetch_related=prefetch_related,
         )
         super().__init__(*args, **kwargs)
 
-    @cached_property
-    def is_basic_field(self):
-        return False
-
     @property
     def arguments(self) -> List[StrawberryArgument]:
-        if isinstance(self, relay.NodeField):
-            return []
-
         args = super().arguments
         is_node = isinstance(unwrap_type(self.type), relay.Node)
         return [
             (
                 (
                     argument("ids", List[relay.GlobalID], is_optional=self.is_optional)
                     if self.is_list
                     else argument("id", relay.GlobalID, is_optional=self.is_optional)
                 )
-                if is_node
-                and arg.python_name == "pk"
-                and arg.type_annotation.annotation == strawberry.ID
+                if (
+                    is_node
+                    and arg.python_name == "pk"
+                    and arg.type_annotation.annotation == strawberry.ID
+                )
                 else arg
             )
             for arg in args
         ]
 
+    @arguments.setter
+    def arguments(self, value: List[StrawberryArgument]):
+        return StrawberryField.arguments.fset(self, value)
+
     @property
-    def type(self) -> Union[StrawberryType, type]:  # noqa: A003
-        return super().type
+    def type(self) -> Union[StrawberryType, type, Literal[UNRESOLVED]]:  # type: ignore # noqa: A003
+        resolved = super().type
+        if resolved is UNRESOLVED:
+            return resolved
+
+        if isinstance(resolved, StrawberryAuto) and self.origin_django_type:
+            model_field = get_model_field(
+                self.origin_django_type.model,
+                self.django_name or self.name,
+            )
+            resolved_type = resolve_model_field_type(model_field, self.origin_django_type)
+            if is_optional(
+                model_field,
+                self.origin_django_type.is_input,
+                self.origin_django_type.is_partial,
+            ):
+                resolved_type = Optional[resolved_type]
+
+            self.type_annotation = StrawberryAnnotation(resolved_type)
+            resolved = super().type
+
+        return resolved
 
     @type.setter
     def type(self, type_: Any) -> None:  # noqa: A003
-        if type_ is not None and self.origin_django_type is None:
-            resolved = type_
-            if isinstance(resolved, StrawberryAnnotation):
-                resolved = type_.resolve()
-            while isinstance(resolved, StrawberryContainer):
-                resolved = resolved.of_type
-
-            dj_type = getattr(resolved, "_django_type", None)
-            if dj_type is None:
-                contained = get_args(resolved)
-                if contained:
-                    dj_type = getattr(contained[0], "_django_type", None)
-
-            if dj_type is not None:
-                self.origin_django_type = dj_type
-                if self.filters is UNSET or self.filters is None:
-                    self.filters = dj_type.filters
-                if self.order is UNSET or self.order is None:
-                    self.order = dj_type.order
-                if self.pagination is UNSET or self.pagination is None:
-                    self.pagination = dj_type.pagination
-
         super(StrawberryDjangoField, self.__class__).type.fset(self, type_)  # type: ignore
 
+    def get_order(self) -> Optional[Type]:
+        # FIXME: This should be done on strawberry-graphql-django
+        order = super().get_order()
+        if order in (None, UNSET):
+            t_origin = self.type_origin
+            if (f_origin := getattr(t_origin, "_django_type", None)) is not None:
+                order = f_origin.order
+
+        return order
+
+    def get_filters(self) -> Optional[Type]:
+        # FIXME: This should be done on strawberry-graphql-django
+        filters = super().get_filters()
+        if filters in (None, UNSET):
+            t_origin = self.type_origin
+            if (f_origin := getattr(t_origin, "_django_type", None)) is not None:
+                filters = f_origin.filters
+
+        return filters
+
     @cached_property
-    def model(self) -> Type[models.Model]:
-        type_ = unwrap_type(self.type)
-        model = get_django_model(type_)
-        if model:
-            return model
+    def type_origin(self) -> Type:
+        origin = self.type
 
-        tdef = cast(Optional[TypeDefinition], getattr(type_, "_type_definition", None))
+        tdef = cast(Optional[TypeDefinition], getattr(origin, "_type_definition", None))
         if tdef and tdef.concrete_of and issubclass(tdef.concrete_of.origin, relay.Connection):
-            n_type = tdef.type_var_map[relay.NodeType]  # type: ignore
-            if isinstance(n_type, LazyType):
-                n_type = n_type.resolve_type()
-
-            return cast(Type[models.Model], get_django_model(n_type))
-
-        origin = self.origin_django_type or getattr(self.origin, "_django_type", None)
-        model = origin and origin.model
-
-        if isinstance(self.type, StrawberryUnion):
-            mlist = []
-            for t in self.type.types:
-                dj_type = getattr(t, "_django_type", None)
-                if dj_type:
-                    mlist.append(dj_type.model)
-                else:
-                    model = getattr(t, "model", None)
-                    if model:
-                        mlist.append(model)
-            assert len(mlist) == 1
-            model = mlist[0]
+            origin = tdef.type_var_map[relay.NodeType]  # type: ignore
+            if isinstance(origin, LazyType):
+                origin = origin.resolve_type()
+
+        while isinstance(origin, StrawberryContainer):
+            origin = origin.of_type
+
+        if isinstance(origin, StrawberryUnion):
+            olist = []
+            for t in origin.types:
+                while isinstance(t, StrawberryContainer):
+                    t = t.of_type  # noqa: PLW2901
+
+                if hasattr(t, "_django_type"):
+                    olist.append(t)
+
+            assert len(olist) == 1
+            origin = olist[0]
 
-        return cast(Type[models.Model], model)
+        return origin
+
+    @cached_property
+    def model(self) -> Type[models.Model]:
+        return self.type_origin._django_type.model
 
     @cached_property
     def safe_resolver(self):
         resolver = self.base_resolver
         assert resolver
         if not resolver.is_async:
             return resolvers.async_safe(resolver)
@@ -181,16 +209,18 @@
 
     def get_result(
         self,
         source: Optional[models.Model],
         info: Info,
         args: List[Any],
         kwargs: Dict[str, Any],
+        *,
+        skip_base_resolver: bool = False,
     ) -> Union[Awaitable[Any], Any]:
-        if self.base_resolver is not None:
+        if not skip_base_resolver and self.base_resolver is not None:
             result = self.resolver(source, info, args, kwargs)
         elif source is None:
             result = self.model._default_manager.all()
         else:
             # Small optimization to async resolvers avoid having to call it in an sync_to_async
             # context if the value is already cached, since it will not hit the db anymore
             attname = self.django_name or self.python_name
@@ -215,23 +245,23 @@
                     # This returns a queryset, it is async safe
                     result = getattr(source, attname)
                 else:
                     raise KeyError  # noqa: TRY301
             except KeyError:
                 result = resolvers.getattr_async_safe(source, attname)
 
-        if self.is_list:
-
-            def qs_resolver(qs):  # type: ignore
-                return self.get_queryset_as_list(qs, info, kwargs)
+        def qs_resolver(qs):
+            if self.is_list:
+                retval = self.get_queryset_as_list(qs, info, kwargs)
+            elif isinstance((f_type := self.type), type) and issubclass(f_type, relay.Connection):
+                retval = self.get_queryset_as_list(qs, info, kwargs, skip_fetch=True)
+            else:
+                retval = self.get_queryset_one(qs, info, kwargs)
 
-        else:
-
-            def qs_resolver(qs):
-                return self.get_queryset_one(qs, info, kwargs)
+            return retval
 
         return resolvers.resolve_result(result, info=info, qs_resolver=qs_resolver)
 
     def resolver(
         self,
         source: Any,
         info: Info,
@@ -267,15 +297,17 @@
             nodes: Optional[List[relay.GlobalID]] = kwargs.get("ids")
             if isinstance(nodes, list):
                 if nodes:
                     assert {n.resolve_type(info) for n in nodes} == {unwrap_type(self.type)}
                 qs = qs.filter(pk__in=[n.node_id for n in nodes])
 
         qs = self.get_queryset(filter_with_perms(qs, info), info, **kwargs)
-        if not skip_fetch and not isinstance(self, relay.ConnectionField):
+        if not skip_fetch and not any(
+            isinstance(e, relay.ConnectionExtension) for e in self.extensions
+        ):
             # This is what QuerySet does internally to fetch results.
             # After this, iterating over the queryset should be async safe
             qs._fetch_all()  # type: ignore
         return qs
 
     @resolvers.async_safe
     def get_queryset_one(
@@ -300,46 +332,101 @@
                 raise
         else:
             return qs.get()
 
         return None
 
 
-class StrawberryDjangoNodeField(relay.NodeField, StrawberryDjangoField):
-    ...
-
-
-class StrawberryDjangoConnectionField(relay.ConnectionField, StrawberryDjangoField):
-    @property
-    def arguments(self) -> List[StrawberryArgument]:
-        args = super().arguments
-
+class StrawberryDjangoConnectionExtension(relay.ConnectionExtension):
+    def apply(self, field: StrawberryDjangoField) -> None:
         # NOTE: Because we have a base_resolver defined, our parents will not add
         # order/filters resolvers in here, so we need to add them by hand (unless they
         # are somewhat in there). We are not adding pagination because it doesn't make
         # sense together with a Connection
-        args_names = [a.python_name for a in args]
-        if "order" not in args_names and (order := self.get_order()) not in (None, UNSET):
-            args.append(argument("order", order))
-        if "filters" not in args_names and (filters := self.get_filters()) not in (None, UNSET):
-            args.append(argument("filters", filters))
+        args_names = {a.python_name for a in field.arguments}
 
-        return args
+        if "filters" not in args_names and (filters := field.get_filters()) not in (None, UNSET):
+            field.arguments = [*field.arguments, argument("filters", filters)]
+        if "order" not in args_names and (order := field.get_order()) not in (None, UNSET):
+            field.arguments = [*field.arguments, argument("order", order)]
+
+        if field.base_resolver is None:
+
+            def default_resolver(
+                root: Optional[models.Model],
+                info: Info,
+                **kwargs: Any,
+            ) -> Iterable[Any]:
+                if root is not None:
+                    # If this is a nested field, call get_result instead because we want
+                    # to retrieve the queryset from its RelatedManager
+                    retval = field.get_result(root, info, [], kwargs, skip_base_resolver=True)
+                else:
+                    retval = resolvers.resolve_model_nodes(
+                        field.type_origin,
+                        info=info,
+                        required=True,
+                        filter_perms=True,
+                    )
+
+                # If the type defines a custom get_queryset, use it on top of the returned queryset
+                if (get_queryset := getattr(field.type_origin, "get_queryset", None)) is not None:
+                    retval = aio.resolve(
+                        retval,
+                        lambda resolved: get_queryset(resolved, info),
+                        info=info,
+                    )
 
-    @resolvers.async_safe
-    def resolve_connection(
+                return cast(Iterable[Any], retval)
+
+            field.base_resolver = StrawberryResolver(default_resolver)
+
+        return super().apply(field)
+
+    def resolve(
         self,
-        nodes: QuerySet,
+        next_: SyncExtensionResolver,
+        source: Any,
         info: Info,
-        **kwargs,
-    ):
-        return super().resolve_connection(
-            cast(QuerySet, self.get_queryset_as_list(nodes, info, kwargs, skip_fetch=True)),
-            info,
-            **kwargs,
+        *,
+        before: Optional[str] = None,
+        after: Optional[str] = None,
+        first: Optional[int] = None,
+        last: Optional[int] = None,
+        **kwargs: Any,
+    ) -> Any:
+        assert self.connection_type is not None
+        nodes = cast(Iterable[relay.Node], next_(source, info, **kwargs))
+
+        # We have a single resolver for both sync and async, so we need to check if
+        # nodes is awaitable or not and resolve it accordingly
+        if inspect.isawaitable(nodes):
+
+            async def resolver():
+                resolved = self.connection_type.resolve_connection(
+                    await nodes,
+                    info=info,
+                    before=before,
+                    after=after,
+                    first=first,
+                    last=last,
+                )
+                if inspect.isawaitable(resolved):
+                    resolved = await resolved
+                return resolved
+
+            return resolver()
+
+        return self.connection_type.resolve_connection(
+            nodes,
+            info=info,
+            before=before,
+            after=after,
+            first=first,
+            last=last,
         )
 
 
 @overload
 def field(
     *,
     resolver: Callable[[], _T],
@@ -530,15 +617,16 @@
                 id
                 ...
             }
         }
         ```
 
     """
-    return StrawberryDjangoNodeField(
+    extensions = [*list(extensions), relay.NodeExtension()]
+    return StrawberryDjangoField(
         python_name=None,
         graphql_name=name,
         type_annotation=StrawberryAnnotation.from_annotation(graphql_type),
         description=description,
         is_subscription=is_subscription,
         permission_classes=permission_classes or [],
         deprecation_reason=deprecation_reason,
@@ -552,108 +640,82 @@
         disable_optimization=disable_optimization,
         extensions=extensions,
     )
 
 
 @overload
 def connection(
+    graphql_type: Optional[Type[relay.Connection[relay.NodeType]]] = None,
     *,
-    resolver: Callable[[], _T],
     name: Optional[str] = None,
     is_subscription: bool = False,
     description: Optional[str] = None,
-    init: Literal[False] = False,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
-    graphql_type: Optional[Any] = None,
+    extensions: List[FieldExtension] = (),  # type: ignore
     filters: Optional[type] = UNSET,
     order: Optional[type] = UNSET,
     only: Optional[TypeOrSequence[str]] = None,
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
     disable_optimization: bool = False,
-    extensions: List[FieldExtension] = (),  # type: ignore
-) -> _T:
+) -> Any:
     ...
 
 
 @overload
 def connection(
+    graphql_type: Optional[Type[relay.Connection[relay.NodeType]]] = None,
     *,
+    resolver: Optional[_RESOLVER_TYPE[NodeIterableType[Any]]] = None,
     name: Optional[str] = None,
     is_subscription: bool = False,
     description: Optional[str] = None,
     init: Literal[True] = True,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
-    graphql_type: Optional[Any] = None,
+    extensions: List[FieldExtension] = (),  # type: ignore
     filters: Optional[type] = UNSET,
     order: Optional[type] = UNSET,
     only: Optional[TypeOrSequence[str]] = None,
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
     disable_optimization: bool = False,
-    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> Any:
     ...
 
 
-@overload
 def connection(
-    resolver: Union[StrawberryResolver, Callable, staticmethod, classmethod],
+    graphql_type: Optional[Type[relay.Connection[relay.NodeType]]] = None,
     *,
+    resolver: Optional[_RESOLVER_TYPE[NodeIterableType[Any]]] = None,
     name: Optional[str] = None,
     is_subscription: bool = False,
     description: Optional[str] = None,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
-    graphql_type: Optional[Any] = None,
-    filters: Optional[type] = UNSET,
-    order: Optional[type] = UNSET,
-    only: Optional[TypeOrSequence[str]] = None,
-    select_related: Optional[TypeOrSequence[str]] = None,
-    prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
-    disable_optimization: bool = False,
     extensions: List[FieldExtension] = (),  # type: ignore
-) -> StrawberryDjangoConnectionField:
-    ...
-
-
-def connection(
-    resolver=None,
-    *,
-    name: Optional[str] = None,
-    is_subscription: bool = False,
-    description: Optional[str] = None,
-    permission_classes: Optional[List[Type[BasePermission]]] = None,
-    deprecation_reason: Optional[str] = None,
-    default: Any = dataclasses.MISSING,
-    default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
-    metadata: Optional[Mapping[Any, Any]] = None,
-    directives: Optional[Sequence[object]] = (),
-    graphql_type: Optional[Any] = None,
     filters: Optional[type] = UNSET,
     order: Optional[type] = UNSET,
     only: Optional[TypeOrSequence[str]] = None,
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
     disable_optimization: bool = False,
-    extensions: List[FieldExtension] = (),  # type: ignore
     # This init parameter is used by pyright to determine whether this field
     # is added in the constructor or not. It is not used to change
     # any behavior at the moment.
     init: Literal[True, False, None] = None,
 ) -> Any:
     """Annotate a property or a method to create a relay connection field.
 
@@ -701,15 +763,16 @@
         }
         ```
 
     .. _Relay connections:
         https://relay.dev/graphql/connections.htm
 
     """
-    f = StrawberryDjangoConnectionField(
+    extensions = [*list(extensions), StrawberryDjangoConnectionExtension()]
+    f = StrawberryDjangoField(
         python_name=None,
         graphql_name=name,
         type_annotation=StrawberryAnnotation.from_annotation(graphql_type),
         description=description,
         is_subscription=is_subscription,
         permission_classes=permission_classes or [],
         deprecation_reason=deprecation_reason,
@@ -722,11 +785,11 @@
         only=only,
         select_related=select_related,
         prefetch_related=prefetch_related,
         disable_optimization=disable_optimization,
         extensions=extensions,
     )
 
-    if resolver is not None:
-        return f(resolver)
+    if resolver:
+        f = f(resolver)
 
     return f
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/filters.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from enum import Enum
 from typing import Any, Callable, Optional, Sequence, Type, TypeVar, cast
 
 from django.db.models.base import Model
 from django.db.models.sql.query import get_field_names_from_opts  # type: ignore
-from strawberry import UNSET
+from strawberry import UNSET, relay
 from strawberry.field import StrawberryField
 from strawberry_django import filters as _filters
 from strawberry_django import utils
 from strawberry_django.fields.field import field as _field
 from typing_extensions import dataclass_transform
 
 from . import field
-from .relay import GlobalID, connection, node
 from .type import input
 
 _T = TypeVar("_T")
 
 
 def _normalize_value(value: Any):
     if isinstance(value, list):
         return [_normalize_value(v) for v in value]
-    if isinstance(value, GlobalID):
+    if isinstance(value, relay.GlobalID):
         return value.node_id
 
     return value
 
 
 def _build_filter_kwargs(filters):
     filter_kwargs = {}
@@ -70,16 +69,16 @@
 
 
 @dataclass_transform(
     order_default=True,
     field_specifiers=(
         StrawberryField,
         _field,
-        node,
-        connection,
+        relay.node,
+        relay.connection,
         field.field,
         field.node,
         field.connection,
     ),
 )
 def filter(  # noqa: A001
     model: Type[Model],
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/gql/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,35 +15,33 @@
     experimental,
     federation,
     field,
     input,
     interface,
     lazy,
     mutation,
+    relay,
     scalar,
     schema_directive,
     subscription,
     type,
     union,
 )
-
-from strawberry_django_plus import relay
-from strawberry_django_plus.descriptors import model_cached_property, model_property
-from strawberry_django_plus.relay import (
+from strawberry.relay import (
     Connection,
     Node,
     connection,
-    input_mutation,
     node,
 )
+
+from strawberry_django_plus.descriptors import model_cached_property, model_property
 from strawberry_django_plus.types import (
     ListInput,
     NodeInput,
     NodeInputPartial,
-    NodeType,
     OperationInfo,
     OperationMessage,
 )
 from strawberry_django_plus.utils import aio, resolvers
 
 from . import django
 
@@ -76,21 +74,20 @@
     "union",
     # relay
     "relay",
     "Node",
     "Connection",
     "node",
     "connection",
-    "input_mutation",
     # strawberry_django_plus
     "django",
-    "NodeType",
     "NodeInput",
     "NodeInputPartial",
     "ListInput",
     "OperationInfo",
     "OperationMessage",
     "model_cached_property",
     "model_property",
     "resolvers",
     "aio",
+    "relay",
 ]
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/middlewares/user_warmup.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/middlewares/user_warmup.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/mutations/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 import strawberry
 from django.core.exceptions import (
     NON_FIELD_ERRORS,
     ObjectDoesNotExist,
     PermissionDenied,
     ValidationError,
 )
-from strawberry import UNSET
+from strawberry import UNSET, relay
 from strawberry.annotation import StrawberryAnnotation
 from strawberry.arguments import StrawberryArgument
 from strawberry.extensions.field_extension import FieldExtension
+from strawberry.field_extensions import InputMutationExtension
 from strawberry.permission import BasePermission
 from strawberry.type import StrawberryType
 from strawberry.types.fields.resolver import StrawberryResolver
 from strawberry.types.info import Info
 from strawberry.utils.await_maybe import AwaitableOrValue
 from strawberry.utils.str_converters import to_camel_case
 
-from strawberry_django_plus import relay
 from strawberry_django_plus.field import StrawberryDjangoField
 from strawberry_django_plus.optimizer import DjangoOptimizerExtension
 from strawberry_django_plus.permissions import get_with_perms
 from strawberry_django_plus.types import NodeInput, OperationInfo, OperationMessage
 from strawberry_django_plus.utils import aio
 from strawberry_django_plus.utils.inspect import get_possible_types
 from strawberry_django_plus.utils.resolvers import async_safe
@@ -105,16 +105,16 @@
       if the mutation raises any `PermissionDenied`, `ValidationError` or
       `ObjectDoesNotExist`.
 
     Do not instantiate this directly. Instead, use `@gql.django.mutation`
 
     """
 
-    def __init__(self, *args, **kwargs):
-        self._handle_errors: bool = kwargs.pop("handle_django_errors", True)
+    def __init__(self, *args, handle_django_errors: bool = True, **kwargs):
+        self._handle_errors: bool = handle_django_errors
         super().__init__(*args, **kwargs)
 
     def __call__(self, resolver: Callable[..., Iterable[relay.Node]]):
         if self._handle_errors:
             name = to_camel_case(resolver.__name__)
             cap_name = name[0].upper() + name[1:]
             namespace = sys.modules[resolver.__module__].__dict__
@@ -153,66 +153,52 @@
     def get_result(
         self,
         source: Any,
         info: Info,
         args: List[Any],
         kwargs: Dict[str, Any],
     ) -> AwaitableOrValue[Any]:
-        # FIXME: Any other exception types that we should capture here?
+        # TODO: Any other exception types that we should capture here?
         resolver = aio.resolver(
             self.resolver,
             on_error=_map_exception if self._handle_errors else None,
             info=info,
         )
         return resolver(source, info, args, kwargs)
 
 
-class DjangoInputMutationField(DjangoMutationField, relay.InputMutationField):
-    """Input mutation for django models.
-
-    This fields does 3 things:
-
-    - It ensures that the mutation resolver gets called in an async safe environment.
-    - If `handle_django_errors` is True (the default), the return values gets
-      changed to a union with `OperationMessage`, which will be returned instead
-      if the mutation raises any `PermissionDenied`, `ValidationError` or
-      `ObjectDoesNotExist`.
-    - It transforms the resolver arguments to a new type and receives it in
-      a `input` argument at the graphql side.
-
-    Do not instantiate this directly. Instead, use `@gql.django.input_mutation`
-
-    """
-
-    def __init__(self, *args, **kwargs):
-        input_type: Optional[type] = kwargs.pop("input_type", None)
-
+class DjangoCUDMutationField(DjangoMutationField):
+    def __init__(self, input_type: type, *args, full_clean: bool = True, **kwargs):
         super().__init__(*args, **kwargs)
-
         self.input_type = input_type
-        if self.input_type and not self.base_resolver:
-            namespace = sys.modules[self.input_type.__module__].__dict__
-            type_def = getattr(input_type, "_type_definition", None)
-            self.default_args["input"] = StrawberryArgument(
+        self.full_clean = full_clean
+
+    @property
+    def arguments(self) -> List[StrawberryArgument]:
+        namespace = sys.modules[self.input_type.__module__].__dict__
+        type_def = getattr(self.input_type, "_type_definition", None)
+        return [
+            StrawberryArgument(
                 python_name="input",
                 graphql_name=None,
                 type_annotation=StrawberryAnnotation(self.input_type, namespace=namespace),
                 description=type_def and type_def.description,
-            )
+            ),
+        ]
 
     def get_result(
         self,
         source: Any,
         info: Info,
         args: List[Any],
         kwargs: Dict[str, Any],
     ) -> AwaitableOrValue[Any]:
         input_obj = kwargs.pop("input", None)
 
-        # FIXME: Any other exception types that we should capture here?
+        # TODO: Any other exception types that we should capture here?
         resolver = aio.resolver(
             self.resolver,
             on_error=_map_exception if self._handle_errors else None,
             info=info,
         )
         return resolver(source, info, input_obj, args, kwargs)
 
@@ -223,68 +209,55 @@
         data: Optional[object],
         args: List[Any],
         kwargs: Dict[str, Any],
     ) -> AwaitableOrValue[Any]:
         return self.safe_resolver(*args, **kwargs, **vars(data))
 
 
-class DjangoCreateMutationField(DjangoInputMutationField):
+class DjangoCreateMutationField(DjangoCUDMutationField):
     """Create mutation for django models.
 
     Do not instantiate this directly. Instead, use
     `@gql.django.create_mutation`
 
     """
 
-    def __init__(self, *args, **kwargs):
-        self.full_clean: bool = kwargs.pop("full_clean", True)
-        super().__init__(*args, **kwargs)
-
-    @property
-    def arguments(self) -> List[StrawberryArgument]:
-        # FIXME: We don't have a base_resolve in this case. Make sure StrawberryDjangoFieldFilters
-        # doesn't add a opk argument in here...
-        return [a for a in super().arguments if a.python_name == "input"]
-
     @async_safe
     def resolver(
         self,
         source: Any,
         info: Info,
         data: object,
         args: List[Any],
         kwargs: Dict[str, Any],
     ) -> Any:
         assert data is not None
-        return resolvers.create(
-            info,
-            self.model,
-            resolvers.parse_input(info, vars(data)),
-            full_clean=self.full_clean,
-        )
+        # Do not optimize anything while retrieving the object to update
+        token = DjangoOptimizerExtension.enabled.set(False)
+        try:
+            retval = resolvers.create(
+                info,
+                self.model,
+                resolvers.parse_input(info, vars(data)),
+                full_clean=self.full_clean,
+            )
+        finally:
+            DjangoOptimizerExtension.enabled.reset(token)
+
+        return retval
 
 
-class DjangoUpdateMutationField(DjangoInputMutationField):
+class DjangoUpdateMutationField(DjangoCUDMutationField):
     """Update mutation for django models.
 
     Do not instantiate this directly. Instead, use
     `@gql.django.update_mutation`
 
     """
 
-    def __init__(self, *args, **kwargs):
-        self.full_clean: bool = kwargs.pop("full_clean", True)
-        super().__init__(*args, **kwargs)
-
-    @property
-    def arguments(self) -> List[StrawberryArgument]:
-        # FIXME: We don't have a base_resolve in this case. Make sure StrawberryDjangoFieldFilters
-        # doesn't add a opk argument in here...
-        return [a for a in super().arguments if a.python_name == "input"]
-
     @async_safe
     def resolver(
         self,
         source: Any,
         info: Info,
         data: object,
         args: List[Any],
@@ -309,28 +282,22 @@
             )
         finally:
             DjangoOptimizerExtension.enabled.reset(token)
 
         return retval
 
 
-class DjangoDeleteMutationField(DjangoInputMutationField):
+class DjangoDeleteMutationField(DjangoCUDMutationField):
     """Delete mutation for django models.
 
     Do not instantiate this directly. Instead, use
     `@gql.django.delete_mutation`
 
     """
 
-    @property
-    def arguments(self) -> List[StrawberryArgument]:
-        # FIXME: We don't have a base_resolve in this case. Make sure StrawberryDjangoFieldFilters
-        # doesn't add a opk argument in here...
-        return [a for a in super().arguments if a.python_name == "input"]
-
     @async_safe
     def resolver(
         self,
         source: Any,
         info: Info,
         data: object,
         args: List[Any],
@@ -367,16 +334,16 @@
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
-    handle_django_errors: bool = True,
     extensions: List[FieldExtension] = (),  # type: ignore
+    handle_django_errors: bool = True,
 ) -> _T:
     ...
 
 
 @overload
 def mutation(
     *,
@@ -389,16 +356,16 @@
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
-    handle_django_errors: bool = True,
     extensions: List[FieldExtension] = (),  # type: ignore
+    handle_django_errors: bool = True,
 ) -> Any:
     ...
 
 
 @overload
 def mutation(
     resolver: Union[StrawberryResolver, Callable, staticmethod, classmethod],
@@ -411,17 +378,17 @@
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
-    handle_django_errors: bool = True,
     extensions: List[FieldExtension] = (),  # type: ignore
-) -> DjangoInputMutationField:
+    handle_django_errors: bool = True,
+) -> DjangoMutationField:
     ...
 
 
 def mutation(
     resolver=None,
     *,
     name: Optional[str] = None,
@@ -432,16 +399,16 @@
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
-    handle_django_errors: bool = True,
     extensions: List[FieldExtension] = (),  # type: ignore
+    handle_django_errors: bool = True,
     # This init parameter is used by pyright to determine whether this field
     # is added in the constructor or not. It is not used to change
     # any behavior at the moment.
     init: Literal[True, False, None] = None,
 ) -> Any:
     """Annotate a property or a method to create a mutation field.
 
@@ -477,94 +444,94 @@
 
     return f
 
 
 @overload
 def input_mutation(
     *,
-    input_type: Optional[type] = None,
     resolver: Callable[[], _T],
     name: Optional[str] = None,
     field_name: Optional[str] = None,
     filters: Any = UNSET,
     is_subscription: bool = False,
     description: Optional[str] = None,
     init: Literal[False] = False,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
+    extensions: List[FieldExtension] = (),  # type: ignore
     handle_django_errors: bool = True,
 ) -> _T:
     ...
 
 
 @overload
 def input_mutation(
     *,
-    input_type: Optional[type] = None,
     name: Optional[str] = None,
     field_name: Optional[str] = None,
     filters: Any = UNSET,
     is_subscription: bool = False,
     description: Optional[str] = None,
     init: Literal[True] = True,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
+    extensions: List[FieldExtension] = (),  # type: ignore
     handle_django_errors: bool = True,
 ) -> Any:
     ...
 
 
 @overload
 def input_mutation(
     resolver: Union[StrawberryResolver, Callable, staticmethod, classmethod],
     *,
-    input_type: Optional[type] = None,
     name: Optional[str] = None,
     field_name: Optional[str] = None,
     filters: Any = UNSET,
     is_subscription: bool = False,
     description: Optional[str] = None,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
+    extensions: List[FieldExtension] = (),  # type: ignore
     handle_django_errors: bool = True,
-) -> DjangoInputMutationField:
+) -> DjangoMutationField:
     ...
 
 
 def input_mutation(
     resolver=None,
     *,
-    input_type: Optional[type] = None,
     name: Optional[str] = None,
     field_name: Optional[str] = None,
     filters: Any = UNSET,
     is_subscription: bool = False,
     description: Optional[str] = None,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
+    extensions: List[FieldExtension] = (),  # type: ignore
     handle_django_errors: bool = True,
     # This init parameter is used by pyright to determine whether this field
     # is added in the constructor or not. It is not used to change
     # any behavior at the moment.
     init: Literal[True, False, None] = None,
 ) -> Any:
     """Annotate a property or a method to create an input mutation field.
@@ -576,29 +543,30 @@
           changed to a union with `OperationMessage`, which will be returned instead
           if the mutation raises any `PermissionDenied`, `ValidationError` or
           `ObjectDoesNotExist`.
         - It transforms the resolver arguments to a new type and receives it in
           a `input` argument at the graphql side.
 
     """
-    f = DjangoInputMutationField(
-        input_type=input_type,
+    extensions = [*list(extensions), InputMutationExtension()]
+    f = DjangoMutationField(
         python_name=None,
         django_name=field_name,
         graphql_name=name,
         type_annotation=StrawberryAnnotation.from_annotation(graphql_type),
         description=description,
         is_subscription=is_subscription,
         permission_classes=permission_classes or [],
         deprecation_reason=deprecation_reason,
         default=default,
         default_factory=default_factory,
         metadata=metadata,
         directives=directives,
         filters=filters,
+        extensions=extensions,
         handle_django_errors=handle_django_errors,
     )
 
     if resolver is not None:
         return f(resolver)
 
     return f
@@ -616,14 +584,15 @@
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
+    extensions: List[FieldExtension] = (),  # type: ignore
     handle_django_errors: bool = True,
     full_clean: bool = True,
 ) -> Any:
     """Create mutation for django input fields.
 
     Automatically create data for django input fields.
 
@@ -635,15 +604,15 @@
         ...
         >>> @strawberry.mutation
         >>> class Mutation:
         ...     create_product: ProductType = gql.django.create_mutation(ProductInput)
 
     """
     return DjangoCreateMutationField(
-        input_type=input_type,
+        input_type,
         python_name=None,
         django_name=field_name,
         graphql_name=name,
         type_annotation=StrawberryAnnotation.from_annotation(graphql_type),
         description=description,
         is_subscription=is_subscription,
         permission_classes=permission_classes or [],
@@ -651,14 +620,15 @@
         default=default,
         default_factory=default_factory,
         metadata=metadata,
         directives=directives,
         filters=filters,
         handle_django_errors=handle_django_errors,
         full_clean=full_clean,
+        extensions=extensions or (),
     )
 
 
 def update(
     input_type: type,
     *,
     name: Optional[str] = None,
@@ -670,14 +640,15 @@
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
+    extensions: List[FieldExtension] = (),  # type: ignore
     handle_django_errors: bool = True,
     full_clean: bool = True,
 ) -> Any:
     """Update mutation for django input fields.
 
     Examples:
         >>> @gql.django.input
@@ -687,15 +658,15 @@
         ...
         >>> @strawberry.mutation
         >>> class Mutation:
         ...     create_product: ProductType = gql.django.update_mutation(ProductInput)
 
     """
     return DjangoUpdateMutationField(
-        input_type=input_type,
+        input_type,
         python_name=None,
         django_name=field_name,
         graphql_name=name,
         type_annotation=StrawberryAnnotation.from_annotation(graphql_type),
         description=description,
         is_subscription=is_subscription,
         permission_classes=permission_classes or [],
@@ -703,14 +674,15 @@
         default=default,
         default_factory=default_factory,
         metadata=metadata,
         directives=directives,
         filters=filters,
         handle_django_errors=handle_django_errors,
         full_clean=full_clean,
+        extensions=extensions or (),
     )
 
 
 def delete(
     input_type: type = NodeInput,
     *,
     name: Optional[str] = None,
@@ -721,27 +693,29 @@
     init: Literal[True] = True,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
+    extensions: List[FieldExtension] = (),  # type: ignore
     graphql_type: Optional[Any] = None,
     handle_django_errors: bool = True,
 ) -> Any:
     return DjangoDeleteMutationField(
-        input_type=input_type,
+        input_type,
         python_name=None,
         django_name=field_name,
         graphql_name=name,
         type_annotation=StrawberryAnnotation.from_annotation(graphql_type),
         description=description,
         is_subscription=is_subscription,
         permission_classes=permission_classes or [],
         deprecation_reason=deprecation_reason,
         default=default,
         default_factory=default_factory,
         metadata=metadata,
         directives=directives,
         filters=filters,
         handle_django_errors=handle_django_errors,
+        extensions=extensions or (),
     )
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/mutations/resolvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,25 +22,24 @@
 from django.db.models.fields.related import ManyToManyField
 from django.db.models.fields.reverse_related import (
     ForeignObjectRel,
     ManyToManyRel,
     ManyToOneRel,
     OneToOneRel,
 )
-from strawberry import UNSET
+from strawberry import UNSET, relay
 from strawberry.types.info import Info
 from strawberry_django.fields.types import (
     ManyToManyInput,
     ManyToOneInput,
     OneToManyInput,
     OneToOneInput,
 )
 from typing_extensions import TypeAlias
 
-from strawberry_django_plus import relay
 from strawberry_django_plus.types import ListInput, NodeInput
 from strawberry_django_plus.utils import aio
 from strawberry_django_plus.utils.inspect import get_model_fields
 from strawberry_django_plus.utils.resolvers import resolve_sync
 
 if TYPE_CHECKING:
     from django.db.models.manager import ManyToManyRelatedManager, RelatedManager
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,28 +27,28 @@
     ManyToOneRel,
     OneToOneRel,
 )
 from django.db.models.manager import BaseManager
 from django.db.models.query import QuerySet
 from graphql.language.ast import OperationType
 from graphql.type.definition import GraphQLResolveInfo, get_named_type
+from strawberry import relay
 from strawberry.extensions import SchemaExtension
 from strawberry.lazy_type import LazyType
 from strawberry.schema.schema import Schema
 from strawberry.types.execution import ExecutionContext
 from strawberry.types.info import Info
 from strawberry.types.nodes import InlineFragment, Selection, convert_selections
 from strawberry.types.types import TypeDefinition
 from strawberry.utils.await_maybe import AwaitableOrValue
 from strawberry.utils.typing import eval_type
 from strawberry_django.fields.types import resolve_model_field_name
 from typing_extensions import TypeAlias, assert_never, assert_type
 
 from .descriptors import ModelProperty
-from .relay import Connection, Edge, NodeType
 from .utils import resolvers
 from .utils.inspect import (
     PrefetchInspector,
     get_django_type,
     get_model_fields,
     get_possible_type_definitions,
     get_selections,
@@ -111,26 +111,32 @@
 ) -> "OptimizerStore | None":
     store = OptimizerStore()
     model_cache = model_cache or {}
     typename = schema.config.name_converter.from_object(type_def)
 
     # In case this is a relay field, find the selected edges/nodes, the selected fields
     # are actually inside edges -> node selection...
-    if type_def.concrete_of and issubclass(type_def.concrete_of.origin, Connection):
-        n_type = type_def.type_var_map[NodeType]
+    if type_def.concrete_of and issubclass(type_def.concrete_of.origin, relay.Connection):
+        # TODO: Connections are mostly used for pagination so it doesn't make sense for
+        # us to optimize those, as our prefetch would be thrown away causing an extra
+        # useless query. Is there a way for us to properly optimize this in the future?
+        if level > 0:
+            return None
+
+        n_type = type_def.type_var_map[cast(TypeVar, relay.NodeType)]
         if isinstance(n_type, LazyType):
             n_type = n_type.resolve_type()
 
         n_type_def = cast(TypeDefinition, n_type._type_definition)  # type: ignore
 
         for edges in get_selections(selection, typename=typename).values():
             if edges.name != "edges":
                 continue
 
-            e_type = Edge._type_definition.resolve_generic(Edge[n_type])  # type: ignore
+            e_type = relay.Edge._type_definition.resolve_generic(relay.Edge[n_type])  # type: ignore
             e_typename = schema.config.name_converter.from_object(e_type._type_definition)
             for node in get_selections(edges, typename=e_typename).values():
                 if node.name != "node":
                     continue
 
                 new_store = _get_model_hints(
                     model=model,
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/ordering.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/ordering.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from typing import Callable, Optional, Sequence, Type, TypeVar, cast
 
 import strawberry
 from django.db.models.base import Model
-from strawberry import UNSET
+from strawberry import UNSET, relay
 from strawberry.field import StrawberryField
 from strawberry_django.fields.field import field as _field
 from strawberry_django.ordering import Ordering
 from typing_extensions import dataclass_transform
 
 from strawberry_django_plus.utils.typing import is_auto
 
 from . import field
-from .relay import connection, node
 
 _T = TypeVar("_T")
 
 
 @dataclass_transform(
     order_default=True,
     field_specifiers=(
         StrawberryField,
         _field,
-        node,
-        connection,
+        relay.node,
+        relay.connection,
         field.field,
         field.node,
         field.connection,
     ),
 )
 def order(
     model: Type[Model],
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/permissions.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,24 @@
 )
 
 import strawberry
 from django.core.exceptions import PermissionDenied
 from django.db import models
 from django.db.models import Model, QuerySet
 from graphql.type.definition import GraphQLResolveInfo
+from strawberry import Schema, relay
 from strawberry.django.context import StrawberryDjangoContext
 from strawberry.private import Private
+from strawberry.schema.schema_converter import GraphQLCoreConverter
 from strawberry.schema_directive import Location
 from strawberry.types.info import Info
 from strawberry.utils.await_maybe import AwaitableOrValue
 from typing_extensions import Self, assert_never, final
 
 from .directives import SchemaDirectiveHelper, SchemaDirectiveWithResolver
-from .relay import Connection, GlobalID
 from .types import OperationInfo, OperationMessage
 from .utils import aio, resolvers
 from .utils.query import filter_for_user
 from .utils.typing import UserType
 
 try:
     # Try to use the smaller/faster cache decorator if available
@@ -162,56 +163,56 @@
     model: Type[_M],
 ) -> Optional[_M]:
     ...
 
 
 @overload
 def get_with_perms(
-    pk: GlobalID,
+    pk: relay.GlobalID,
     info: Info,
     *,
     required: Literal[True],
     model: Type[_M],
 ) -> _M:
     ...
 
 
 @overload
 def get_with_perms(
-    pk: GlobalID,
+    pk: relay.GlobalID,
     info: Info,
     *,
     required: bool = ...,
     model: Type[_M],
 ) -> Optional[_M]:
     ...
 
 
 @overload
 def get_with_perms(
-    pk: GlobalID,
+    pk: relay.GlobalID,
     info: Info,
     *,
     required: Literal[True],
 ) -> Any:
     ...
 
 
 @overload
 def get_with_perms(
-    pk: GlobalID,
+    pk: relay.GlobalID,
     info: Info,
     *,
     required: bool = ...,
 ) -> Optional[Any]:
     ...
 
 
 def get_with_perms(pk, info, *, required=False, model=None):
-    if isinstance(pk, GlobalID):
+    if isinstance(pk, relay.GlobalID):
         instance = pk.resolve_node(info, required=required, ensure_type=model)
         if aio.is_awaitable(instance, info=info):
             instance = resolvers.resolve_sync(instance)
         instance = cast(models.Model, instance)
     else:
         assert model
         instance = model._default_manager.get(pk=pk)
@@ -343,17 +344,28 @@
         # If it is a Connection, try to return an empty connection, but only if
         # it is the only possibility available...
         if len(helper.ret_possibilities) == 1:
             type_def = helper.ret_possibilities[0].type_def
             if (
                 type_def
                 and type_def.concrete_of
-                and issubclass(type_def.concrete_of.origin, Connection)
+                and issubclass(type_def.concrete_of.origin, relay.Connection)
             ):
-                return cast(Connection, type_def.origin).from_nodes([], total_count=0)
+                strawberry_schema: Schema = info.schema.extensions[
+                    GraphQLCoreConverter.DEFINITION_BACKREF
+                ]
+                field = strawberry_schema.get_field_for_type(info.field_name, info.parent_type.name)
+                assert field is not None
+                return cast(relay.Connection, type_def.origin).resolve_connection(
+                    [],
+                    info=Info(
+                        _raw_info=info,
+                        _field=field,
+                    ),
+                )
 
         # In last case, raise an error
         raise PermissionDenied(self.message)
 
 
 @dataclasses.dataclass
 class ConditionDirective(AuthDirective):
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/settings.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dataclasses
-from typing import TYPE_CHECKING, Final, List, Optional
+from typing import TYPE_CHECKING, Final, List
 
 from django.conf import settings
 
 __all__ = [
     "NAMESPACE",
     "Config",
     "config",
@@ -18,15 +18,14 @@
 
     The configs here are expected to be set on django like:
 
         "STRAWBERRY_DJANGO_<ATTNAME>"
 
     """
 
-    RELAY_MAX_RESULTS: Optional[int] = dataclasses.field(default=100)
     REMOVE_DUPLICATED_SUFFIX: List[str] = dataclasses.field(
         default_factory=lambda: ["Input", "Partial"],
     )
     FIELDS_USE_GLOBAL_ID: bool = dataclasses.field(default=True)
     GENERATE_ENUMS_FROM_CHOICES: bool = dataclasses.field(default=False)
 
     # Trick type checking into thinking that we only have the defined configs
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/test/client.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/test/client.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/type.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,267 +1,76 @@
 import dataclasses
 import inspect
 import sys
 import types
-from contextlib import suppress
 from functools import cached_property
 from typing import (
     Callable,
+    List,
     Literal,
     Optional,
     Sequence,
     Type,
     TypeVar,
     Union,
     cast,
-    get_args,
-    get_origin,
 )
 
 import strawberry
 from django.contrib.contenttypes.fields import GenericForeignKey, GenericRel
 from django.core.exceptions import FieldDoesNotExist
 from django.db.models.base import Model
 from django.db.models.fields.reverse_related import ManyToManyRel, ManyToOneRel
-from strawberry import UNSET
+from strawberry import UNSET, relay
 from strawberry.annotation import StrawberryAnnotation
-from strawberry.exceptions import MissingFieldAnnotationError, PrivateStrawberryFieldError
-from strawberry.field import UNRESOLVED, StrawberryField
+from strawberry.exceptions import (
+    MissingFieldAnnotationError,
+)
+from strawberry.field import StrawberryField
 from strawberry.private import is_private
-from strawberry.types import Info
-from strawberry.types.fields.resolver import StrawberryResolver
+from strawberry.types.types import TypeDefinition
 from strawberry.unset import UnsetType
-from strawberry.utils.typing import eval_type
 from strawberry_django.fields.field import field as _field
 from strawberry_django.fields.types import get_model_field, resolve_model_field_name
 from strawberry_django.type import StrawberryDjangoType as _StraberryDjangoType
-from strawberry_django.utils import get_annotations, is_similar_django_type
-from typing_extensions import Annotated, dataclass_transform
+from strawberry_django.utils import get_annotations
+from typing_extensions import dataclass_transform
 
 from strawberry_django_plus.optimizer import OptimizerStore, PrefetchType
 from strawberry_django_plus.utils.typing import TypeOrSequence, is_auto
 
 from . import field
 from .descriptors import ModelProperty
 from .field import StrawberryDjangoField, connection, node
-from .relay import Connection, ConnectionField, Node
-from .types import resolve_model_field_type
-from .utils.resolvers import resolve_model_id, resolve_model_node, resolve_model_nodes
+from .utils.resolvers import (
+    resolve_model_id,
+    resolve_model_id_attr,
+    resolve_model_node,
+    resolve_model_nodes,
+)
 
 __all = [
     "StrawberryDjangoType",
     "type",
     "interface",
     "input",
     "partial",
 ]
 
 _T = TypeVar("_T")
 _O = TypeVar("_O", bound=type)
 _M = TypeVar("_M", bound=Model)
 
 
-def _from_django_type(
-    django_type: "StrawberryDjangoType",
-    name: str,
-    *,
-    type_annotation: Optional[StrawberryAnnotation] = None,
-) -> StrawberryDjangoField:
-    origin = django_type.origin
-
-    attr = getattr(origin, name, dataclasses.MISSING)
-    if attr is UNSET or attr is dataclasses.MISSING:
-        attr = getattr(StrawberryDjangoField, "__dataclass_fields__", {}).get(name, UNSET)
-
-    if type_annotation:
-        try:
-            type_origin = get_origin(type_annotation.annotation)
-            is_connection = issubclass(type_origin, Connection) if type_origin else False
-        except Exception:  # noqa: BLE001
-            is_connection = False
-        if is_private(type_annotation.annotation):
-            raise PrivateStrawberryFieldError(name, django_type.origin)
-    else:
-        is_connection = False
-
-    if is_connection or isinstance(attr, ConnectionField):
-        field = attr
-        if not isinstance(field, ConnectionField):
-            field = connection()
-
-        field = cast(StrawberryDjangoField, field)
-
-        if not field.base_resolver:
-
-            def conn_resolver(root, info: Info):
-                qs = getattr(root, name).all()
-                if not type_annotation:
-                    return qs
-                remote_type_defs = get_args(type_annotation.annotation)
-                remote_type = eval_type(remote_type_defs[0], type_annotation.namespace, None)
-                if hasattr(remote_type, "get_queryset"):
-                    qs = remote_type.get_queryset(qs, info)
-                return qs
-
-            field.base_resolver = StrawberryResolver(conn_resolver)
-            if type_annotation is not None:
-                field.type_annotation = type_annotation
-    elif isinstance(attr, StrawberryDjangoField) and not attr.origin_django_type:
-        field = attr
-    elif isinstance(attr, dataclasses.Field):
-        default = getattr(attr, "default", dataclasses.MISSING)
-        default_factory = getattr(attr, "default_factory", dataclasses.MISSING)
-
-        if type_annotation is None:
-            type_annotation = getattr(attr, "type_annotation", None)
-        if type_annotation is None:
-            type_annotation = StrawberryAnnotation(attr.type)
-
-        store = getattr(attr, "store", None)
-        field = StrawberryDjangoField(
-            django_name=getattr(attr, "django_name", None) or attr.name,
-            graphql_name=getattr(attr, "graphql_name", None),
-            origin=getattr(attr, "origin", None),
-            is_subscription=getattr(attr, "is_subscription", False),
-            description=getattr(attr, "description", None),
-            base_resolver=getattr(attr, "base_resolver", None),
-            permission_classes=getattr(attr, "permission_classes", ()),
-            default=default,
-            default_factory=default_factory,
-            deprecation_reason=getattr(attr, "deprecation_reason", None),
-            directives=getattr(attr, "directives", ()),
-            type_annotation=type_annotation,
-            filters=getattr(attr, "filters", UNSET),
-            order=getattr(attr, "order", UNSET),
-            only=store and store.only,
-            select_related=store and store.select_related,
-            prefetch_related=store and store.prefetch_related,
-            disable_optimization=getattr(attr, "disable_optimization", False),
-            extensions=getattr(attr, "extensions", ()),
-        )
-    elif isinstance(attr, StrawberryResolver):
-        field = StrawberryDjangoField(base_resolver=attr)
-    elif callable(attr):
-        field = StrawberryDjangoField()(attr)
-    else:
-        field = StrawberryDjangoField(default=attr)
-
-    field.python_name = name
-    # store origin django type for further usage
-    field.origin_django_type = django_type
-
-    # annotation of field is used as a class type
-    if type_annotation is not None:
-        field.type_annotation = type_annotation
-        field.is_auto = is_auto(field.type_annotation)
-
-    # resolve the django_name and check if it is relation field. django_name
-    # is used to access the field data in resolvers
-    try:
-        model_field = get_model_field(
-            django_type.model,
-            getattr(field, "django_name", None) or name,
-        )
-    except FieldDoesNotExist as e:
-        model_attr = getattr(django_type.model, name, None)
-        namespace = sys.modules[django_type.model.__module__].__dict__
-        if model_attr is not None and isinstance(model_attr, ModelProperty):
-            if field.is_auto:
-                annotation = model_attr.type_annotation
-                if get_origin(annotation) is Annotated:
-                    annotation = get_args(annotation)[0]
-                field.type_annotation = StrawberryAnnotation(annotation, namespace=namespace)
-                field.is_auto = is_auto(field.type_annotation)
-
-            if field.description is None:
-                field.description = model_attr.description
-        elif model_attr is not None and isinstance(model_attr, (property, cached_property)):
-            func = model_attr.fget if isinstance(model_attr, property) else model_attr.func
-            if field.is_auto:
-                annotations = func.__annotations__
-                if (return_type := annotations.get("return")) is None:
-                    raise MissingFieldAnnotationError(name, origin) from e
-
-                field.type_annotation = StrawberryAnnotation(return_type, namespace=namespace)
-                field.is_auto = is_auto(field.type_annotation)
-
-            if field.description is None and func.__doc__:
-                field.description = inspect.cleandoc(func.__doc__)
-        elif field.django_name or field.is_auto:
-            raise  # field should exist, reraise caught exception
-    else:
-        field.is_relation = model_field.is_relation
-        if not field.django_name:
-            field.django_name = resolve_model_field_name(
-                model_field,
-                is_input=django_type.is_input,
-                is_filter=bool(django_type.is_filter),
-            )
-
-        # change relation field type to auto if field is inherited from another
-        # type. for example if field is inherited from output type but we are
-        # configuring field for input type
-        if field.is_relation and not is_similar_django_type(django_type, field.origin_django_type):
-            field.is_auto = True
-
-        # resolve type of auto field
-        if field.is_auto:
-            field.type_annotation = StrawberryAnnotation(
-                resolve_model_field_type(model_field, django_type),
-            )
-
-        if field.description is None:
-            if isinstance(model_field, (GenericRel, GenericForeignKey)):
-                description = None
-            elif isinstance(model_field, (ManyToOneRel, ManyToManyRel)):
-                description = model_field.field.help_text
-            else:
-                description = getattr(model_field, "help_text")  # noqa: B009
-
-            if description:
-                field.description = str(description)
-
-    return field
-
-
-def _get_fields(django_type: "StrawberryDjangoType"):
-    origin = django_type.origin
-    fields = {}
-    seen_fields = set()
-
-    # collect all annotated fields
-    for name, annotation in get_annotations(origin).items():
-        with suppress(PrivateStrawberryFieldError):
-            fields[name] = _from_django_type(
-                django_type,
-                name,
-                type_annotation=annotation,
-            )
-        seen_fields.add(name)
-
-    # collect non-annotated strawberry fields
-    for name in dir(origin):
-        if name in seen_fields:
-            continue
-
-        attr = getattr(origin, name, None)
-        if not isinstance(attr, StrawberryField):
-            continue
-
-        fields[name] = _from_django_type(django_type, name)
-
-    return fields
-
-
 def _has_own_node_resolver(cls, name: str) -> bool:
     resolver = getattr(cls, name, None)
     if resolver is None:
         return False
 
-    if id(resolver.__func__) == id(getattr(Node, name).__func__):
+    if id(resolver.__func__) == id(getattr(relay.Node, name).__func__):
         return False
 
     return True
 
 
 def _process_type(
     cls: _O,
@@ -271,54 +80,64 @@
     filters: Optional[type] = UNSET,
     order: Optional[type] = UNSET,
     pagination: Optional[bool] = UNSET,
     only: Optional[TypeOrSequence[str]] = None,
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[PrefetchType]] = None,
     disable_optimization: bool = False,
+    partial: bool = False,
+    is_filter: Union[Literal["lookups"], bool] = False,
     **kwargs,
 ) -> _O:
-    original_annotations = cls.__dict__.get("__annotations__", {})
-
     django_type = StrawberryDjangoType(
         origin=cls,
         model=model,
         field_cls=field_cls,
+        is_partial=partial,
         is_input=kwargs.get("is_input", False),
-        is_partial=kwargs.pop("partial", False),
-        is_filter=kwargs.pop("is_filter", False),
+        is_filter=is_filter,
         filters=filters,
         order=order,
         pagination=pagination,
         disable_optimization=disable_optimization,
         store=OptimizerStore.with_hints(
             only=only,
             select_related=select_related,
             prefetch_related=prefetch_related,
         ),
     )
 
-    fields = list(_get_fields(django_type).values())
-    cls.__annotations__ = {}
+    if django_type.is_input:
+        # FIXME: For input types it is imported to set the default value to UNSET
+        # Is there a better way of doing this?
+        seen_fields = set()
+        for attr_name, attr in cls.__dict__.items():
+            seen_fields.add(attr_name)
+            if isinstance(attr, dataclasses.Field) and attr.default is dataclasses.MISSING:
+                attr.default = UNSET
+                if isinstance(attr, StrawberryField):
+                    attr.default_value = UNSET
+
+        for field_name, field_annotation in get_annotations(cls).items():
+            if field_name in seen_fields:
+                continue
+
+            annotation = field_annotation.annotation
+            if is_private(annotation):
+                continue
 
-    # update annotations and fields
-    for f in fields:
-        annotation = f.type_annotation.annotation if f.type_annotation is not None else f.type
-        if annotation is UNRESOLVED:
-            annotation = None
-
-        cls.__annotations__[f.name] = annotation
-        setattr(cls, f.name, f)
+            if not hasattr(cls, field_name):
+                setattr(cls, field_name, UNSET)
 
     # Make sure model is also considered a "virtual subclass" of cls
     if "is_type_of" not in cls.__dict__:
         cls.is_type_of = lambda obj, info: isinstance(obj, (cls, model))  # type: ignore
 
     # Default querying methods for relay
-    if issubclass(cls, Node):
+    if issubclass(cls, relay.Node):
         if not _has_own_node_resolver(cls, "resolve_node"):
             cls.resolve_node = types.MethodType(resolve_model_node, cls)
 
         if not _has_own_node_resolver(cls, "resolve_nodes"):
             cls.resolve_nodes = types.MethodType(
                 lambda *args, **kwargs: resolve_model_nodes(
                     *args,
@@ -330,25 +149,141 @@
 
         if not _has_own_node_resolver(cls, "resolve_id"):
             cls.resolve_id = types.MethodType(
                 lambda cls, root, *args, **kwargs: resolve_model_id(cls, root),
                 cls,
             )
 
+        if not _has_own_node_resolver(cls, "resolve_id"):
+            cls.resolve_id = types.MethodType(
+                lambda cls, root, *args, **kwargs: resolve_model_id(cls, root),
+                cls,
+            )
+
+        if not _has_own_node_resolver(cls, "resolve_id_attr"):
+            cls.resolve_id_attr = types.MethodType(
+                resolve_model_id_attr,
+                cls,
+            )
+
         # Adjust types that inherit from other types/interfaces that implement Node
         # to make sure they pass themselves as the node type
         for attr in ["resolve_node", "resolve_nodes", "resolve_id"]:
             meth = getattr(cls, attr)
             if isinstance(meth, types.MethodType) and meth.__self__ is not cls:
                 setattr(cls, attr, types.MethodType(cast(classmethod, meth).__func__, cls))
 
     strawberry.type(cls, **kwargs)
 
-    # restore original annotations for further use
-    cls.__annotations__ = original_annotations
+    # update annotations and fields
+    type_def = cast(TypeDefinition, cls._type_definition)  # type: ignore
+    new_fields: List[StrawberryField] = []
+    for f in type_def._fields:
+        django_name: Optional[str] = getattr(f, "django_name", None) or f.name
+        description: Optional[str] = getattr(f, "description", None)
+        type_annotation: Optional[StrawberryAnnotation] = getattr(f, "type_annotation", None)
+        f_is_auto = type_annotation is not None and is_auto(type_annotation.annotation)
+
+        try:
+            if django_name is None:
+                raise FieldDoesNotExist  # noqa: TRY301
+            model_attr = get_model_field(django_type.model, django_name)
+        except FieldDoesNotExist as e:
+            model_attr = getattr(django_type.model, django_name, None)
+            is_relation = False
+
+            if model_attr is not None and isinstance(model_attr, ModelProperty):
+                if type_annotation is None or f_is_auto:
+                    type_annotation = StrawberryAnnotation(
+                        model_attr.type_annotation,
+                        namespace=sys.modules[model_attr.func.__module__].__dict__,
+                    )
+
+                if description is None:
+                    description = model_attr.description
+            elif model_attr is not None and isinstance(model_attr, (property, cached_property)):
+                func = model_attr.fget if isinstance(model_attr, property) else model_attr.func
+
+                if type_annotation is None or f_is_auto:
+                    if (return_type := func.__annotations__.get("return")) is None:
+                        raise MissingFieldAnnotationError(django_name, type_def.origin) from e
+
+                    type_annotation = StrawberryAnnotation(
+                        return_type,
+                        namespace=sys.modules[func.__module__].__dict__,
+                    )
+
+                if description is None and func.__doc__:
+                    description = inspect.cleandoc(func.__doc__)
+        else:
+            is_relation = model_attr.is_relation
+            if not django_name:
+                django_name = resolve_model_field_name(
+                    model_attr,
+                    is_input=django_type.is_input,
+                    is_filter=bool(django_type.is_filter),
+                )
+
+            if description is None:
+                if isinstance(model_attr, (GenericRel, GenericForeignKey)):
+                    f_description = None
+                elif isinstance(model_attr, (ManyToOneRel, ManyToManyRel)):
+                    f_description = model_attr.field.help_text
+                else:
+                    f_description = getattr(model_attr, "help_text", None)
+
+                if f_description:
+                    description = str(f_description)
+
+        if isinstance(f, StrawberryDjangoField) and not f.origin_django_type:
+            # If the field is a StrawberryDjangoField, just update its annotations/description/etc
+            f.type_annotation = type_annotation
+            f.description = description
+        elif (
+            not isinstance(f, StrawberryDjangoField)
+            and getattr(f, "base_resolver", None) is not None
+        ):
+            # If this is not a StrawberryDjangoField, but has a base_resolver, no need
+            # avoid forcing it to be a StrawberryDjangoField
+            new_fields.append(f)
+            continue
+        else:
+            store = getattr(f, "store", None)
+            f = StrawberryDjangoField(  # noqa: PLW2901
+                django_name=django_name,
+                description=description,
+                type_annotation=type_annotation,
+                python_name=f.python_name,
+                graphql_name=getattr(f, "graphql_name", None),
+                origin=getattr(f, "origin", None),
+                is_subscription=getattr(f, "is_subscription", False),
+                base_resolver=getattr(f, "base_resolver", None),
+                permission_classes=getattr(f, "permission_classes", ()),
+                default=getattr(f, "default", dataclasses.MISSING),
+                default_factory=getattr(f, "default_factory", dataclasses.MISSING),
+                deprecation_reason=getattr(f, "deprecation_reason", None),
+                directives=getattr(f, "directives", ()),
+                filters=getattr(f, "filters", UNSET),
+                order=getattr(f, "order", UNSET),
+                only=store and store.only,
+                select_related=store and store.select_related,
+                prefetch_related=store and store.prefetch_related,
+                disable_optimization=getattr(f, "disable_optimization", False),
+                extensions=getattr(f, "extensions", ()),
+            )
+
+        f.is_relation = is_relation
+        if f.origin_django_type is None:
+            f.origin_django_type = django_type  # type: ignore
+
+        new_fields.append(f)
+        if f.base_resolver and f.python_name:
+            setattr(cls, f.python_name, f)
+
+    cls._type_definition._fields = new_fields  # type: ignore
     cls._django_type = django_type  # type: ignore
 
     return cls
 
 
 @dataclasses.dataclass
 class StrawberryDjangoType(_StraberryDjangoType[_O, _M]):
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/types.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 )
 
 import strawberry
 from django.db import models
 from django.db.models.fields import NOT_PROVIDED
 from django.db.models.fields.related import ManyToManyField
 from django.db.models.fields.reverse_related import ForeignObjectRel
-from strawberry import UNSET
+from strawberry import UNSET, relay
 from strawberry.custom_scalar import ScalarWrapper
 from strawberry.enum import EnumValueDefinition
 from strawberry.file_uploads import Upload
 from strawberry.type import StrawberryType
 from strawberry.utils.str_converters import capitalize_first, to_camel_case
 from strawberry_django.fields.types import (
     DjangoModelType,
@@ -34,15 +34,14 @@
     field_type_map,
     input_field_type_map,
 )
 from strawberry_django.fields.types import resolve_model_field_type as _resolve_model_field
 from strawberry_django.filters import DjangoModelFilterInput, FilterLookup
 from typing_extensions import Self
 
-from . import relay
 from .settings import config
 
 if TYPE_CHECKING:
     from .type import StrawberryDjangoType
 
 try:
     from django_choices_field import IntegerChoicesField, TextChoicesField
@@ -97,29 +96,14 @@
                 field_type_map[f] = type_
 
         return type_
 
     return _wrapper
 
 
-@strawberry.type(
-    description="Generic type for objects that implements the `Node` interface.",
-)
-class NodeType(relay.Node):
-    """Set the value to the selected node."""
-
-    id: relay.GlobalID  # noqa: A003
-
-    def __eq__(self, other: Self):
-        return self.__class__ == other.__class__ and self.id == other.id
-
-    def __hash__(self):
-        return hash((self.__class__, self.id))
-
-
 @strawberry.input(
     description="Input of an object that implements the `Node` interface.",
 )
 class NodeInput:
     """Set the value to the selected node.
 
     Notes:
@@ -296,15 +280,15 @@
                 is_lookup = True
                 retval = get_args(retval)[0]
             else:
                 is_lookup = False
 
             retval = {
                 strawberry.ID: relay.GlobalID,
-                DjangoModelType: NodeType,
+                DjangoModelType: relay.Node,
                 DjangoModelFilterInput: NodeInput,
                 OneToOneInput: NodeInput,
                 OneToManyInput: NodeInput,
                 ManyToOneInput: ListInput[NodeInput],
                 ManyToManyInput: ListInput[NodeInputPartial],
             }.get(
                 retval,
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/utils/resolvers.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 import warnings
 from typing import (
     Any,
     Awaitable,
     Callable,
     Coroutine,
     Iterable,
+    List,
     Literal,
     Optional,
     Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 from asgiref.sync import async_to_sync, sync_to_async
 from django.db.models import Model, QuerySet
 from django.db.models.manager import BaseManager
+from strawberry import relay
+from strawberry.relay.exceptions import NodeIDAnnotationError
 from strawberry.types.fields.resolver import StrawberryResolver
 from strawberry.types.info import Info
 from strawberry.utils.await_maybe import AwaitableOrValue
 from strawberry_django.utils import is_async
 from typing_extensions import ParamSpec
 
-from strawberry_django_plus import relay
-from strawberry_django_plus.relay import GlobalID, Node
-
 from .aio import is_awaitable, resolve_async
 from .inspect import get_django_type
 
 _T = TypeVar("_T")
 _M = TypeVar("_M", bound=Model)
 _R = TypeVar("_R")
 _P = ParamSpec("_P")
@@ -288,32 +288,112 @@
             functools.partial(resolve_result, info=info, qs_resolver=qs_resolver),
             info=info,
         )
 
     return res
 
 
+@overload
+def resolve_model_nodes(
+    source: Union[Type[relay.Node], Type[_M]],
+    *,
+    info: Optional[Info] = None,
+    node_ids: Iterable[Union[str, relay.GlobalID]],
+    required: Literal[True],
+    filter_perms: bool = False,
+) -> AwaitableOrValue[Iterable[_M]]:
+    ...
+
+
+@overload
 def resolve_model_nodes(
-    source: Union[Type[Node], Type[_M]],
+    source: Union[Type[relay.Node], Type[_M]],
     *,
     info: Optional[Info] = None,
-    node_ids: Optional[Iterable[Union[str, GlobalID]]] = None,
+    node_ids: None = None,
+    required: Literal[True],
     filter_perms: bool = False,
 ) -> AwaitableOrValue[QuerySet[_M]]:
+    ...
+
+
+@overload
+def resolve_model_nodes(
+    source: Union[Type[relay.Node], Type[_M]],
+    *,
+    info: Optional[Info] = None,
+    node_ids: Iterable[Union[str, relay.GlobalID]],
+    required: Literal[False],
+    filter_perms: bool = False,
+) -> AwaitableOrValue[Iterable[Optional[_M]]]:
+    ...
+
+
+@overload
+def resolve_model_nodes(
+    source: Union[Type[relay.Node], Type[_M]],
+    *,
+    info: Optional[Info] = None,
+    node_ids: None = None,
+    required: Literal[False],
+    filter_perms: bool = False,
+) -> AwaitableOrValue[Optional[QuerySet[_M]]]:
+    ...
+
+
+@overload
+def resolve_model_nodes(
+    source: Union[Type[relay.Node], Type[_M]],
+    *,
+    info: Optional[Info] = None,
+    node_ids: Optional[Iterable[Union[str, relay.GlobalID]]] = None,
+    required: bool = False,
+    filter_perms: bool = False,
+) -> AwaitableOrValue[
+    Union[
+        Iterable[_M],
+        QuerySet[_M],
+        Iterable[Optional[_M]],
+        Optional[QuerySet[_M]],
+    ]
+]:
+    ...
+
+
+def resolve_model_nodes(
+    source,
+    *,
+    info=None,
+    node_ids=None,
+    required=False,
+    filter_perms=False,
+) -> AwaitableOrValue[
+    Union[
+        Iterable[_M],
+        QuerySet[_M],
+        Iterable[Optional[_M]],
+        Optional[QuerySet[_M]],
+    ]
+]:
     """Resolve model nodes, ensuring those are prefetched in a sync context.
 
     Args:
         source:
             The source model or the model type that implements the `Node` interface
         info:
             Optional gql execution info. Make sure to always provide this or
             otherwise, the queryset cannot be optimized in case DjangoOptimizerExtension
             is enabled. This will also be used for `is_awaitable` check.
         node_ids:
             Optional filter by those node_ids instead of retrieving everything
+        required:
+            If `True`, all `node_ids` requested must exist. If they don't,
+            an error must be raised. If `False`, missing nodes should be
+            returned as `None`. It only makes sense when passing a list of
+            `node_ids`, otherwise it will should ignored.
         filter_perms:
             If we should filter the queryset with the permissions defined in the field
 
     Returns:
         The resolved queryset, already prefetched from the database
 
     """
@@ -327,20 +407,24 @@
         origin = source
         django_type = get_django_type(source, ensure_type=True)
         source = cast(Type[_M], django_type.model)
 
     qs = source._default_manager.all()
 
     if origin and hasattr(origin, "get_queryset"):
-        qs = origin.get_queryset(qs, info)  # type: ignore
+        qs = origin.get_queryset(qs, info)
 
+    id_attr = cast(relay.Node, origin).resolve_id_attr()
     if node_ids is not None:
-        id_attr = getattr(origin, "id_attr", "pk")
         qs = qs.filter(
-            **{f"{id_attr}__in": [i.node_id if isinstance(i, GlobalID) else i for i in node_ids]},
+            **{
+                f"{id_attr}__in": [
+                    i.node_id if isinstance(i, relay.GlobalID) else i for i in node_ids
+                ],
+            },
         )
 
     if filter_perms:
         assert info
         qs = filter_with_perms(qs, info)
 
     qs_resolver = resolve_qs
@@ -355,32 +439,55 @@
             return_type,
             relay.Connection,
         ):
 
             def qs_resolver(qs):
                 return qs
 
-    return resolve_result(qs, info=info, qs_resolver=qs_resolver)
+    retval = cast(
+        AwaitableOrValue[QuerySet[_M]],
+        resolve_result(qs, info=info, qs_resolver=qs_resolver),
+    )
+    if not node_ids:
+        return retval
+
+    def map_results(results: QuerySet[_M]) -> List[_M]:
+        results_map = {str(getattr(obj, id_attr)): obj for obj in results}
+        retval: List[Optional[_M]] = []
+        for node_id in node_ids:
+            if required:
+                retval.append(results_map[str(node_id)])
+            else:
+                retval.append(results_map.get(str(node_id), None))
+
+        return retval  # type: ignore
+
+    if inspect.isawaitable(retval):
+
+        async def resolver():
+            return await sync_to_async(map_results)(await retval)
+
+    return map_results(cast(QuerySet[_M], retval))
 
 
 @overload
 def resolve_model_node(
-    source: Union[Type[Node], Type[_M]],
-    node_id: Union[str, GlobalID],
+    source: Union[Type[relay.Node], Type[_M]],
+    node_id: Union[str, relay.GlobalID],
     *,
     info: Optional[Info] = ...,
     required: Literal[False] = ...,
 ) -> AwaitableOrValue[Optional[_M]]:
     ...
 
 
 @overload
 def resolve_model_node(
-    source: Union[Type[Node], Type[_M]],
-    node_id: Union[str, GlobalID],
+    source: Union[Type[relay.Node], Type[_M]],
+    node_id: Union[str, relay.GlobalID],
     *,
     info: Optional[Info] = ...,
     required: Literal[True],
 ) -> AwaitableOrValue[_M]:
     ...
 
 
@@ -408,45 +515,68 @@
     if issubclass(source, Model):
         origin = None
     else:
         origin = source
         django_type = get_django_type(source, ensure_type=True)
         source = cast(Type[Model], django_type.model)
 
-    if isinstance(node_id, GlobalID):
+    if isinstance(node_id, relay.GlobalID):
         node_id = node_id.node_id
 
-    id_attr = getattr(origin, "id_attr", "pk")
+    id_attr = cast(relay.Node, origin).resolve_id_attr()
 
     qs = source._default_manager.filter(**{id_attr: node_id})
 
     if origin and hasattr(origin, "get_queryset"):
         qs = origin.get_queryset(qs, info)
 
     return resolve_result(
         qs,
         info=info,
         qs_resolver=resolve_qs_get_one if required else resolve_qs_get_first,
     )
 
 
-def resolve_model_id(source: Union[Type[Node], Type[_M]], root: Model) -> AwaitableOrValue[str]:
+def resolve_model_id_attr(source: Type) -> str:
+    """Resolve the model id, ensuring it is retrieved in a sync context.
+
+    Args:
+        source:
+            The source model type that implements the `Node` interface
+
+    Returns:
+        The resolved id attr
+
+    """
+    try:
+        id_attr = super(source, source).resolve_id_attr()
+    except NodeIDAnnotationError:
+        id_attr = "pk"
+
+    return id_attr
+
+
+def resolve_model_id(
+    source: Union[Type[relay.Node], Type[_M]],
+    root: Model,
+) -> AwaitableOrValue[str]:
     """Resolve the model id, ensuring it is retrieved in a sync context.
 
     Args:
         source:
             The source model or the model type that implements the `Node` interface
         root:
             The source model object.
 
     Returns:
         The resolved object id
 
     """
-    id_attr = getattr(source, "id_attr", "pk")
+    id_attr = cast(relay.Node, source).resolve_id_attr()
+
     assert isinstance(root, Model)
     if id_attr == "pk":
         pk = root.__class__._meta.pk
         assert pk
         id_attr = pk.attname
     assert id_attr
     try:
```

### Comparing `strawberry_django_plus-2.6.4/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-3.0.0/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.4/PKG-INFO` & `strawberry_django_plus-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 2.6.4
+Version: 3.0.0
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
@@ -20,21 +20,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: debug-toolbar
 Provides-Extra: enum
 Requires-Dist: django (>=3.2)
 Requires-Dist: django-choices-field (>=2.0) ; extra == "enum"
-Requires-Dist: django-debug-toolbar (>=3.4) ; extra == "debug-toolbar"
-Requires-Dist: strawberry-graphql (>=0.161.0)
-Requires-Dist: strawberry-graphql-django (>=0.8)
+Requires-Dist: strawberry-graphql (>=0.184.0)
+Requires-Dist: strawberry-graphql-django (>=0.9.4)
 Requires-Dist: typing-extensions (>=4.2.0)
 Project-URL: Documentation, https://strawberry-django-plus.readthedocs.io
 Project-URL: Repository, https://github.com/blb-ventures/strawberry-django-plus
 Description-Content-Type: text/markdown
 
 # strawberry-django-plus
 
@@ -68,15 +66,16 @@
   using schema directives, supporting both
   [django authentication system](https://docs.djangoproject.com/en/4.0/topics/auth/default/),
   direct and per-object permission checking for backends that implement those (e.g.
   [django-guardian](https://django-guardian.readthedocs.io/en/stable/)).
 - [Mutations for Django](https://blb-ventures.github.io/strawberry-django-plus/mutations/),
   with CRUD support and automatic errors validation.
 - [Relay support](https://blb-ventures.github.io/strawberry-django-plus/quickstart/#relay-support)
-  for queries, connections and input mutations, all integrated with django types directly.
+  for queries, connections and input mutations, using the official strawberry's
+  [relay integration](https://strawberry.rocks/docs/guides/relay)
 - [Django Debug Toolbar integration](https://blb-ventures.github.io/strawberry-django-plus/debug-toolbar/)
   with graphiql to display metrics like SQL queries
 - Improved sync/async resolver that priorizes the model's cache to avoid have to use
   [sync_to_async](https://docs.djangoproject.com/en/4.0/topics/async/#asgiref.sync.sync_to_async)
   when not needed.
 
 ## Installation
```

