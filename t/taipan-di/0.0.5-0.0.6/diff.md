# Comparing `tmp/taipan_di-0.0.5.tar.gz` & `tmp/taipan_di-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipan_di-0.0.5.tar", max compression
+gzip compressed data, was "taipan_di-0.0.6.tar", max compression
```

## Comparing `taipan_di-0.0.5.tar` & `taipan_di-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,28 @@
--rw-r--r--   0        0        0     1063 2023-06-13 15:12:31.390871 taipan_di-0.0.5/LICENSE
--rw-r--r--   0        0        0     2988 2023-06-13 15:12:31.390871 taipan_di-0.0.5/README.md
--rw-r--r--   0        0        0     1004 2023-06-13 15:12:31.390871 taipan_di-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      534 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/__init__.py
--rw-r--r--   0        0        0      196 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/__init__.py
--rw-r--r--   0        0        0     4331 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/dependency_collection.py
--rw-r--r--   0        0        0      703 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/dependency_container.py
--rw-r--r--   0        0        0      736 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/dependency_provider.py
--rw-r--r--   0        0        0     3689 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/instanciate_service.py
--rw-r--r--   0        0        0      130 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/scopes/__init__.py
--rw-r--r--   0        0        0      503 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/scopes/factory_scope.py
--rw-r--r--   0        0        0      625 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/scopes/singleton_scope.py
--rw-r--r--   0        0        0      559 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/__init__.py
--rw-r--r--   0        0        0      929 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/chain_of_responsibility_factory.py
--rw-r--r--   0        0        0      590 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/chain_of_responsibility_link.py
--rw-r--r--   0        0        0     2047 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/chain_of_responsibility_registrator.py
--rw-r--r--   0        0        0      811 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/pipeline_factory.py
--rw-r--r--   0        0        0      665 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/pipeline_link.py
--rw-r--r--   0        0        0     1775 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/classes/tools/pipeline_registrator.py
--rw-r--r--   0        0        0      415 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/errors/__init__.py
--rw-r--r--   0        0        0       67 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/errors/taipan_error.py
--rw-r--r--   0        0        0      142 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/errors/taipan_injection_error.py
--rw-r--r--   0        0        0      148 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/errors/taipan_registration_error.py
--rw-r--r--   0        0        0      132 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/errors/taipan_type_error.py
--rw-r--r--   0        0        0      148 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/errors/taipan_unregistered_error.py
--rw-r--r--   0        0        0      236 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/interfaces/__init__.py
--rw-r--r--   0        0        0      963 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/interfaces/base_dependency_container.py
--rw-r--r--   0        0        0     1059 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/interfaces/base_dependency_provider.py
--rw-r--r--   0        0        0      544 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/interfaces/base_scope.py
--rw-r--r--   0        0        0        0 2023-06-13 15:12:31.390871 taipan_di-0.0.5/taipan_di/py.typed
--rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 taipan_di-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-16 20:14:24.052799 taipan_di-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3022 2023-06-16 20:14:24.052799 taipan_di-0.0.6/README.md
+-rw-r--r--   0        0        0     1004 2023-06-16 20:14:24.052799 taipan_di-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/__init__.py
+-rw-r--r--   0        0        0      140 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/__init__.py
+-rw-r--r--   0        0        0     3730 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/dependency_collection.py
+-rw-r--r--   0        0        0      673 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/dependency_container.py
+-rw-r--r--   0        0        0      733 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/dependency_provider.py
+-rw-r--r--   0        0        0     3689 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/instanciate_service.py
+-rw-r--r--   0        0        0      130 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/scopes/__init__.py
+-rw-r--r--   0        0        0      503 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/scopes/factory_scope.py
+-rw-r--r--   0        0        0      625 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/scopes/singleton_scope.py
+-rw-r--r--   0        0        0      225 2023-06-16 20:14:24.052799 taipan_di-0.0.6/taipan_di/classes/tools/__init__.py
+-rw-r--r--   0        0        0      811 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/classes/tools/pipeline_factory.py
+-rw-r--r--   0        0        0      705 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/classes/tools/pipeline_link.py
+-rw-r--r--   0        0        0     1775 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/classes/tools/pipeline_registrator.py
+-rw-r--r--   0        0        0      415 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/errors/__init__.py
+-rw-r--r--   0        0        0       67 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/errors/taipan_error.py
+-rw-r--r--   0        0        0      142 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/errors/taipan_injection_error.py
+-rw-r--r--   0        0        0      148 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/errors/taipan_registration_error.py
+-rw-r--r--   0        0        0      132 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/errors/taipan_type_error.py
+-rw-r--r--   0        0        0      148 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/errors/taipan_unregistered_error.py
+-rw-r--r--   0        0        0      236 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/interfaces/__init__.py
+-rw-r--r--   0        0        0      933 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/interfaces/base_dependency_container.py
+-rw-r--r--   0        0        0     1056 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/interfaces/base_dependency_provider.py
+-rw-r--r--   0        0        0      544 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/interfaces/base_scope.py
+-rw-r--r--   0        0        0        0 2023-06-16 20:14:24.056800 taipan_di-0.0.6/taipan_di/py.typed
+-rw-r--r--   0        0        0     3944 1970-01-01 00:00:00.000000 taipan_di-0.0.6/PKG-INFO
```

### Comparing `taipan_di-0.0.5/LICENSE` & `taipan_di-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.5/README.md` & `taipan_di-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
  - Lightweight
  - No decorators
  - No hidden behaviour (what you write is what you get)
  - Automatic dependency injection on service resolving
  - Type hinting
  - No global container by default
  - Singleton and factory scopes
- - Register pipelines and chains of responsibility easily
+ - Register pipelines easily
 
 
 ## Constraints
 
  - Based purely on types (not on strings)
  - No automatic registration
  - It is necessary to write an `__init__` function or use `@dataclass`
@@ -50,15 +50,15 @@
 
 You can also provide a creator method or an instance (for singletons only) that will be used when resolving the services :
 
  - `services.register_factory_creator(Type, lambda provider: create(provider))`
  - `services.register_singleton_creator(Type, lambda provider: create(provider))`
  - `services.register_singleton_instance(Type, instance)`
 
-You can also register chains of responsibility and pipelines. Examples are given in the test files.
+You can also register pipelines. Examples are given in the test files.
 
 Once your services are registered, you have to build a dependency provider which will be used to resolve services : 
 
 > `provider = services.build()`<br/>
 > `resolved = provider.resolve(InterfaceType)`
 
 If `ImplementationType` has a constructor dependency, it will be automatically resolved, as long as the dependency has been registered in the `DependencyCollection`.
@@ -74,9 +74,10 @@
 ## TODO
 
 This library isn't stable yet and a lot of things can still be improved.
 If there is something you want to see added or if something does not work as you want it to, feel free to open an issue.
 
 Here is a list of features I have in mind and will be working on :
 
+ - Modify the registration process / methods to better handle type conditions and protocols
  - Create configuration from environment or configuration files
```

### Comparing `taipan_di-0.0.5/pyproject.toml` & `taipan_di-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Taipan-DI"
-version = "0.0.5"
+version = "0.0.6"
 description = "Truly Amazing Inversion of control Python library Analogous to .Net's DI"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 
 keywords = ["taipan", "dependency injection", "dependency", "python"]
```

### Comparing `taipan_di-0.0.5/taipan_di/classes/dependency_collection.py` & `taipan_di-0.0.6/taipan_di/classes/dependency_collection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-from typing import Callable, Type, TypeVar
+from typing import Callable, Optional, Type, TypeVar
 
 from taipan_di.interfaces import BaseDependencyProvider
 
 from .dependency_container import DependencyContainer
 from .instanciate_service import instanciate_service
 from .scopes import FactoryScope, SingletonScope
-from .tools import (
-    PipelineLink,
-    PipelineRegistrator,
-    ChainOfResponsibilityLink,
-    ChainOfResponsibilityRegistrator,
-)
+from .tools import PipelineLink, PipelineRegistrator
 
 __all__ = ["DependencyCollection"]
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
@@ -39,15 +34,15 @@
         """
         Registers a service as a singleton by providing the instance to return.
         """
         creator = lambda provider: instance
         self.register_singleton_creator(type, creator)
 
     def register_singleton(
-        self, interface_type: Type[T], implementation_type: Type[T] = None
+        self, interface_type: Type[T], implementation_type: Optional[Type[T]] = None
     ) -> None:
         """
         Register a service as a singleton by specifying the implementation type to use.
 
         On resolve, the implementation will be instanciated with its dependencies automatically resolved.
 
         If the implementation type isn't provided, the interface type will be used as the implementation type.
@@ -68,15 +63,15 @@
         """
         Registers a service as a factory by specifying how to create its instances.
         """
         service = FactoryScope(creator)
         self._container.register(type, service)
 
     def register_factory(
-        self, interface_type: Type[T], implementation_type: Type[T] = None
+        self, interface_type: Type[T], implementation_type: Optional[Type[T]] = None
     ) -> None:
         """
         Register a service as a factory by specifying the implementation type to use.
 
         On resolve, the implementation will be instanciated with its dependencies automatically resolved.
 
         If the implementation type isn't provided, the interface type will be used as the implementation type.
@@ -85,29 +80,14 @@
         """
         if implementation_type is None:
             implementation_type = interface_type
 
         creator = lambda provider: instanciate_service(implementation_type, provider)
         self.register_factory_creator(interface_type, creator)
 
-    ## Chain of Responsibility
-
-    def register_chain_of_responsibility(
-        self, interface_type: Type[ChainOfResponsibilityLink[T, U]], as_singleton=False
-    ) -> ChainOfResponsibilityRegistrator[T, U]:
-        """
-        Initiate the registration of a service as a chain of responsibility.
-
-        Returns a registrator to be used to add the links and then register the service.
-        """
-        registrator = ChainOfResponsibilityRegistrator[T, U](
-            interface_type, self, as_singleton
-        )
-        return registrator
-
     ## Pipeline
 
     def register_pipeline(
         self, interface_type: Type[PipelineLink[T, U]], as_singleton=False
     ) -> PipelineRegistrator[T, U]:
         """
         Initiate the registration of a service as a pipeline.
```

### Comparing `taipan_di-0.0.5/taipan_di/classes/dependency_provider.py` & `taipan_di-0.0.6/taipan_di/classes/dependency_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 T = TypeVar("T")
 
 
 class DependencyProvider(BaseDependencyProvider):
     def __init__(self, services: Dict[Type, BaseScope]) -> None:
         self._services = services.copy()
 
-    def contains(self, type: Type[T]) -> bool:
+    def contains(self, type: Type) -> bool:
         return type in self._services
 
     def resolve(self, type: Type[T]) -> T:
         if not type in self._services:
             raise TaipanUnregisteredError(f"Service {str(type)} is not registered")
 
         service = self._services[type]
```

### Comparing `taipan_di-0.0.5/taipan_di/classes/instanciate_service.py` & `taipan_di-0.0.6/taipan_di/classes/instanciate_service.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.5/taipan_di/classes/scopes/singleton_scope.py` & `taipan_di-0.0.6/taipan_di/classes/scopes/singleton_scope.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.5/taipan_di/classes/tools/chain_of_responsibility_registrator.py` & `taipan_di-0.0.6/taipan_di/classes/tools/pipeline_registrator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,53 @@
 from __future__ import annotations
 from typing import Generic, List, Type, TypeVar, TYPE_CHECKING
 
-from taipan_di.classes.tools import ChainOfResponsibilityLink, ChainOfResponsibilityFactory
+from taipan_di.classes.tools import PipelineLink, PipelineFactory
 from taipan_di.errors import TaipanRegistrationError
 from taipan_di.interfaces import BaseDependencyProvider
 
 from taipan_di.classes import instanciate_service
 
 if TYPE_CHECKING:
     from taipan_di.classes import DependencyCollection
 
-__all__ = ["ChainOfResponsibilityRegistrator"]
+__all__ = ["PipelineRegistrator"]
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
-class ChainOfResponsibilityRegistrator(Generic[T, U]):
+class PipelineRegistrator(Generic[T, U]):
     def __init__(
         self,
-        interface_type: Type[ChainOfResponsibilityLink[T, U]],
+        interface_type: Type[PipelineLink[T, U]],
         services: DependencyCollection,
         as_singleton=False,
     ) -> None:
         self._interface_type = interface_type
         self._services = services
         self._as_singleton = as_singleton
-        self._link_types: List[Type[ChainOfResponsibilityLink[T, U]]] = []
+        self._link_types: List[Type[PipelineLink[T, U]]] = []
 
-    def add(
-        self, link: Type[ChainOfResponsibilityLink[T, U]]
-    ) -> ChainOfResponsibilityRegistrator[T, U]:
+    def add(self, link: Type[PipelineLink[T, U]]) -> PipelineRegistrator[T, U]:
         self._link_types.append(link)
         return self
 
     def register(self) -> None:
         if len(self._link_types) == 0:
             raise TaipanRegistrationError(
                 f"Pipeline[{str(T)}, {str(U)}] is empty ! Add at least one link"
             )
 
-        def create_chain_of_responsibility(
-            provider: BaseDependencyProvider,
-        ) -> ChainOfResponsibilityLink[T, U]:
-            factory = ChainOfResponsibilityFactory[T, U]()
+        def create_pipeline(provider: BaseDependencyProvider) -> PipelineLink[T, U]:
+            factory = PipelineFactory[T, U]()
 
             for link_type in self._link_types:
                 link = instanciate_service.instanciate_service(link_type, provider)
                 factory.add(link)
 
             return factory.build()
 
         if self._as_singleton:
-            self._services.register_singleton_creator(
-                self._interface_type, create_chain_of_responsibility
-            )
+            self._services.register_singleton_creator(self._interface_type, create_pipeline)
         else:
-            self._services.register_factory_creator(
-                self._interface_type, create_chain_of_responsibility
-            )
+            self._services.register_factory_creator(self._interface_type, create_pipeline)
```

### Comparing `taipan_di-0.0.5/taipan_di/classes/tools/pipeline_factory.py` & `taipan_di-0.0.6/taipan_di/classes/tools/pipeline_factory.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.5/taipan_di/classes/tools/pipeline_link.py` & `taipan_di-0.0.6/taipan_di/classes/tools/pipeline_link.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import abc
-from typing import Callable, Generic, TypeVar
+from typing import Callable, Generic, Optional, TypeVar
 
 __all__ = ["PipelineLink"]
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
@@ -11,15 +11,15 @@
     def __init__(self) -> None:
         self._next = None
 
     def _set_next(self, next: "PipelineLink[T, U]") -> "PipelineLink[T, U]":
         self._next = next
         return self._next
 
-    def exec(self, request: T) -> U:
+    def exec(self, request: T) -> Optional[U]:
         next_function = self._next.exec if self._next is not None else lambda req: None
 
         return self._handle(request, next_function)
 
     @abc.abstractmethod
-    def _handle(self, request: T, next: Callable[[T], U]) -> U:
+    def _handle(self, request: T, next: Callable[[T], Optional[U]]) -> Optional[U]:
         return next(request)
```

### Comparing `taipan_di-0.0.5/taipan_di/interfaces/base_dependency_container.py` & `taipan_di-0.0.6/taipan_di/interfaces/base_dependency_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import abc
-from typing import Type, TypeVar
+from typing import Type
 
 from .base_dependency_provider import BaseDependencyProvider
 from .base_scope import BaseScope
 
 __all__ = ["BaseDependencyContainer"]
 
-T = TypeVar("T")
-
 
 class BaseDependencyContainer(metaclass=abc.ABCMeta):
     @classmethod
     def __subclasshook__(cls, subclass):
         return (
             hasattr(subclass, "contains")
             and callable(subclass.contains)
@@ -19,15 +17,15 @@
             and callable(subclass.register)
             and hasattr(subclass, "build")
             and callable(subclass.build)
             or NotImplemented
         )
 
     @abc.abstractmethod
-    def contains(self, type: Type[T]) -> bool:
+    def contains(self, type: Type) -> bool:
         raise NotImplementedError
 
     @abc.abstractmethod
     def register(self, type: Type, service: BaseScope) -> None:
         raise NotImplementedError
 
     @abc.abstractmethod
```

### Comparing `taipan_di-0.0.5/taipan_di/interfaces/base_dependency_provider.py` & `taipan_di-0.0.6/taipan_di/interfaces/base_dependency_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             and callable(subclass.contains)
             and hasattr(subclass, "resolve")
             and callable(subclass.resolve)
             or NotImplemented
         )
 
     @abc.abstractmethod
-    def contains(self, type: Type[T]) -> bool:
+    def contains(self, type: Type) -> bool:
         """
         Checks if the requested type is registered in the provider's services
         """
         raise NotImplementedError
 
     @abc.abstractmethod
     def resolve(self, type: Type[T]) -> T:
```

### Comparing `taipan_di-0.0.5/taipan_di/interfaces/base_scope.py` & `taipan_di-0.0.6/taipan_di/interfaces/base_scope.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.5/PKG-INFO` & `taipan_di-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipan-di
-Version: 0.0.5
+Version: 0.0.6
 Summary: Truly Amazing Inversion of control Python library Analogous to .Net's DI
 Home-page: https://github.com/Billuc/Taipan-DI
 License: MIT
 Keywords: taipan,dependency injection,dependency,python
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
@@ -32,15 +32,15 @@
  - Lightweight
  - No decorators
  - No hidden behaviour (what you write is what you get)
  - Automatic dependency injection on service resolving
  - Type hinting
  - No global container by default
  - Singleton and factory scopes
- - Register pipelines and chains of responsibility easily
+ - Register pipelines easily
 
 
 ## Constraints
 
  - Based purely on types (not on strings)
  - No automatic registration
  - It is necessary to write an `__init__` function or use `@dataclass`
@@ -72,15 +72,15 @@
 
 You can also provide a creator method or an instance (for singletons only) that will be used when resolving the services :
 
  - `services.register_factory_creator(Type, lambda provider: create(provider))`
  - `services.register_singleton_creator(Type, lambda provider: create(provider))`
  - `services.register_singleton_instance(Type, instance)`
 
-You can also register chains of responsibility and pipelines. Examples are given in the test files.
+You can also register pipelines. Examples are given in the test files.
 
 Once your services are registered, you have to build a dependency provider which will be used to resolve services : 
 
 > `provider = services.build()`<br/>
 > `resolved = provider.resolve(InterfaceType)`
 
 If `ImplementationType` has a constructor dependency, it will be automatically resolved, as long as the dependency has been registered in the `DependencyCollection`.
@@ -96,10 +96,11 @@
 ## TODO
 
 This library isn't stable yet and a lot of things can still be improved.
 If there is something you want to see added or if something does not work as you want it to, feel free to open an issue.
 
 Here is a list of features I have in mind and will be working on :
 
+ - Modify the registration process / methods to better handle type conditions and protocols
  - Create configuration from environment or configuration files
```

