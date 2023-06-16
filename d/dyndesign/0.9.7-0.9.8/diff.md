# Comparing `tmp/dyndesign-0.9.7.tar.gz` & `tmp/dyndesign-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyndesign-0.9.7.tar", max compression
+gzip compressed data, was "dyndesign-0.9.8.tar", max compression
```

## Comparing `dyndesign-0.9.7.tar` & `dyndesign-0.9.8.tar`

### file list

```diff
@@ -1,8 +1,14 @@
--rw-r--r--   0        0        0    13552 2023-04-26 08:04:11.677638 dyndesign-0.9.7/README.rst
--rw-r--r--   0        0        0      172 2023-04-26 08:04:11.677638 dyndesign-0.9.7/dyndesign/__init__.py
--rw-r--r--   0        0        0     7497 2023-04-26 08:04:11.677638 dyndesign-0.9.7/dyndesign/classmerger.py
--rw-r--r--   0        0        0      643 2023-04-26 08:04:11.677638 dyndesign-0.9.7/dyndesign/dynloader.py
--rw-r--r--   0        0        0     5948 2023-04-26 08:04:11.677638 dyndesign-0.9.7/dyndesign/dynmethod.py
--rw-r--r--   0        0        0     1512 2023-04-26 08:04:11.677638 dyndesign-0.9.7/dyndesign/singletonmeta.py
--rw-r--r--   0        0        0     1160 2023-04-26 08:04:11.677638 dyndesign-0.9.7/pyproject.toml
--rw-r--r--   0        0        0    14914 1970-01-01 00:00:00.000000 dyndesign-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-16 10:55:23.850464 dyndesign-0.9.8/LICENSE.txt
+-rw-r--r--   0        0        0    15826 2023-06-16 10:55:23.850464 dyndesign-0.9.8/README.rst
+-rw-r--r--   0        0        0      282 2023-06-16 10:55:23.850464 dyndesign-0.9.8/dyndesign/__init__.py
+-rw-r--r--   0        0        0     7151 2023-06-16 10:55:23.850464 dyndesign-0.9.8/dyndesign/classmerger.py
+-rw-r--r--   0        0        0      851 2023-06-16 10:55:23.850464 dyndesign-0.9.8/dyndesign/dyninherit.py
+-rw-r--r--   0        0        0     6057 2023-06-16 10:55:23.850464 dyndesign-0.9.8/dyndesign/dyninherit_base.py
+-rw-r--r--   0        0        0     2425 2023-06-16 10:55:23.850464 dyndesign-0.9.8/dyndesign/dyninherit_locked_instances.py
+-rw-r--r--   0        0        0     1185 2023-06-16 10:55:23.850464 dyndesign-0.9.8/dyndesign/dynloader.py
+-rw-r--r--   0        0        0     5903 2023-06-16 10:55:23.850464 dyndesign-0.9.8/dyndesign/dynmethod.py
+-rw-r--r--   0        0        0      203 2023-06-16 10:55:23.850464 dyndesign-0.9.8/dyndesign/exceptions.py
+-rw-r--r--   0        0        0     1512 2023-06-16 10:55:23.850464 dyndesign-0.9.8/dyndesign/singletonmeta.py
+-rw-r--r--   0        0        0      483 2023-06-16 10:55:23.850464 dyndesign-0.9.8/dyndesign/utils.py
+-rw-r--r--   0        0        0     1140 2023-06-16 10:55:23.850464 dyndesign-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0    16921 1970-01-01 00:00:00.000000 dyndesign-0.9.8/PKG-INFO
```

### Comparing `dyndesign-0.9.7/README.rst` & `dyndesign-0.9.8/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 DynDesign
 =========
 
 |Build Status| |PyPi Version Status| |Python Version Status| |License|
 
-A set of tools for Dynamic Design Patterns in Python.
+A set of tools for Dynamic Design in Python.
+
+
+Documentation
+-------------
+
+DynDesign's full documentation can be found at
+https://dyndesign.readthedocs.io/en/latest/
 
 
 Install
 -------
 
 Dyndesign is on the Python Package Index (PyPI):
 
@@ -15,42 +22,63 @@
 
     pip install dyndesign
 
 
 Overview
 --------
 
+Dynamically add parent classes:
+
+.. code:: python
+
+    from dyndesign import DynInheritance
+
+    class Child(DynInheritance):
+        ...
+
+    Child.dynparents_add(Parent1)
+    c = Child()
+    c.method_of_Parent1()
+
+
 Merge two or more classes:
 
 .. code:: python
 
     from dyndesign import mergeclasses
 
-    MergedClass = mergeclasses(Base, Ext1, Ext2, ...)
+    MergedClass = mergeclasses(Base, Ext1)
+    m = MergedClass()
+    m.method_of_Ext1()
 
 Decorate a method with one or more instance methods loaded at runtime:
 
 .. code:: python
 
     from dyndesign import decoratewith
 
     @decoratewith("decorator_1", "component.decorator_2", ...)
     def decorated_method(self, ...):
         ...
 
-Safely invoke functions or methods from a ``safezone`` context manager:
+Safely invoke functions or methods from a ``safezone`` context manager or by
+using the ``safeinvoke`` API:
 
 .. code:: python
 
-    from dyndesign import safezone
+    from dyndesign import safezone, safeinvoke
 
     with safezone():
         ...
         function_possibly_non_existent()
-        ...
+
+    ...
+
+    def method(self):
+        safeinvoke("method_possibly_non_existent", self)
 
 Create and destroy Singleton classes:
 
 .. code:: python
 
     from dyndesign import SingletonMeta
 
@@ -67,22 +95,88 @@
 .. code:: python
 
     from dyndesign import importclass
 
     ImportedClass = importclass("directory.module.class_name")
 
 
-Merging Classes
----------------
+Dynamic Inheritance
+-------------------
+
+With Dynamic Inheritance, it becomes possible to dynamically modify the
+superclass set of classes that inherit from special class ``DynInheritance``. This
+allows the addition of parent classes to those classes, and the modification is
+also instantly reflected in all their instances.
+
+.. code:: python
+
+    from dyndesign import DynInheritance
+
+    class Parent:
+        def m1(self):
+            print("Method `m1` from `Parent`")
+
+    class Child(DynInheritance):
+        def __init__(self):
+            print("Constructor of `Child`")
+
+    child_instance = Child()
+
+    # Constructor of `Child`
+
+    Child.dynparents_add(Parent)
+    child_instance.m1()
+
+    # Method `m1` from `Parent`
+
+When the special class ``DynInheritanceLockedInstances`` is utilized instead of
+``DynInheritance``, the superclass set is locked within each class instance,
+meaning that it remains unchanged even when there are modifications to the
+class's superclasses.
+
+.. code:: python
+
+    class Parent:
+        def __init__(self):
+            print("Constructor of `Parent`")
+
+        def mtd(self):
+            print("Method `mtd` of `Parent`")
+
+    class Child(DynInheritanceLockedInstances):
+        def __init__(self):
+            super(DynInheritanceLockedInstances, self).__init__()
+            print("Constructor of `Child`")
+
+    orphan_child = Child()
+
+    # Constructor of `Child`
+
+    Child.dynparents_add(Parent)
+    child_with_parent = Child()
+
+    # Constructor of `Parent`
+    # Constructor of `Child`
+
+    child_with_parent.mtd()
+
+    # Method `mtd` of `Parent`
+
+    orphan_child.mtd()
+
+    # AttributeError: 'Child' object has no attribute 'mtd'
+
+Class Merging
+-------------
 
 Dyndesign provides API ``mergeclasses`` to merge two or more classes as if they
-were dictionaries, so that the merged class has the attributes and methods of
-the base class and of the extension classes. If two or more classes have the
-same attributes/methods, the attributes/methods from the rightmost classes (in
-the order in which the classes are passed to ``mergeclasses``) overload the
+were dictionaries. As a result, the newly created class has the same properties
+from both its base class and any added extensions. If two or more classes have
+the same attributes/methods, the attributes/methods from the rightmost classes
+(in the order in which the classes are passed to ``mergeclasses``) overload the
 ones from the leftmost classes, similarly to what happens when merging
 dictionaries.
 
 .. code:: python
 
     from dyndesign import mergeclasses
 
@@ -138,43 +232,44 @@
 
     # No argument passed to class `A`
     # Argument a='Alpha' passed to class `B`
     # Argument a='Alpha', b='Beta' and kw1='kwarg #1' passed to class `C`
     # Argument kw2='kwarg #2' passed to class `D`
 
 On the other hand, if any required positional argument is missing, an exception
-is raised. If `MergedClass` of the above example is initialized with no
-parameters, and exception is raised when the constructor of class `B` is called:
+is raised. If ``MergedClass`` of the above example is initialized with no
+parameters, and exception is raised when the constructor of class ``B`` is
+called:
 
 .. code:: python
 
     ...
     MergedClass()
 
     # ...
     # TypeError: B.__init__() missing 1 required positional argument: 'a'
 
 So as to have constructor instances with missing positional arguments silently
-skipped, `strict_merged_args` can be set to False in `mergeclasses`. In the
-above example, constructors of class `B` and `C` are skipped:
+skipped, ``strict_merged_args`` can be set to False in ``mergeclasses``. In the
+above example, constructors of class ``B`` and ``C`` are skipped:
 
 .. code:: python
 
     ...
     MergedClass = mergeclasses(A, B, C, D, strict_merged_args=False)
     MergedClass()
 
     # No argument passed to class `A`
     # Argument kw2=None passed to class `D`
 
 
 It is also possible to extend the same behavior of the constructor ``__init__``
 (i.e., all the methods from all the merged classes are invoked rather than being
 overloaded by the same name method from the rightmost class) to other methods. A
-list of method names whose instances have to be all invoked can be specified in
+list of method names whose instances must be all invoked can be specified in
 the ``invoke_all`` argument of ``mergeclasses``. Adaptive filtering of the
 arguments of the method instances is performed as well.
 
 .. code:: python
 
     class E:
         def method(self):
@@ -190,24 +285,24 @@
     # No argument passed to `method` of class `E`
     # Argument a='Alpha' passed to `method` of class `F`
 
 
 Dynamic Decorators
 ------------------
 
-Meta decorator ``decoratewith`` decorates a class method with one or more
-pipelined instance decorators (regardless whether they statically exist or not).
-The syntax of the dynamic decorators aims to get rid of the boilerplate for
-wrapping and returning the decorator code, leaving just the wrapper's code. For
-example, dynamic decorators can be used to decorate a method from a base class
-with a method from an extension class:
+Meta decorator ``decoratewith`` can be used to decorate a class method with one
+or more chained dynamic decorators, regardless whether they statically exist
+or not. Additionally, the syntax of the dynamic decorators aims to get rid of
+the boilerplate for wrapping and returning the decorator code, leaving just the
+wrapper's code. For example, dynamic decorators can be used to decorate a method
+of a base class with a method of an extension class:
 
 .. code:: python
 
-    from dyndesign import decoratewith
+    from dyndesign import decoratewith, mergeclasses
 
     class Base:
         @decoratewith("decorator")
         def m(self):
             print(f"Method `m` of class `Base`")
 
     class Ext:
@@ -221,15 +316,15 @@
 
     # Beginning of method decoration from Ext.
     # Method `m` of class `Base`
     # End of method decoration from Ext.
 
 If a decorator name is passed in the ``invoke_all`` argument of
 ``mergeclasses``, then multiple decorator instances with the same name from
-different extension classes may be used in pipeline:
+different extension classes may be used in chain:
 
 .. code:: python
 
     class Ext2:
         def decorator(self, func):
             print("Beginning of method decoration from Ext2.")
             func(self)
@@ -301,15 +396,15 @@
 protection is restricted to the functions having that/those name(s). For
 example, ``safezone`` can be used to safely call functions that may or may not
 exist at runtime:
 
 .. code:: python
 
     from dyndesign import safezone
-    
+
     def fallback():
         print("Fallback function")
 
     def function_a():
         print("Function `a`")
 
     with safezone(fallback=fallback):
@@ -348,17 +443,17 @@
     # Method `m` of class `Base` standalone
     # Fallback method
 
 
 Invoking methods safely
 -----------------------
 
-As alternative to ``safezone`` context manager, ``safeinvoke`` can be used to
-safely invoke methods that may or may not exist at runtime. To this end, method
-``m`` of class ``Base`` of the example above can be replaced as follows:
+As an alternative to ``safezone`` context manager, ``safeinvoke`` API can be
+used to safely invoke methods that may or may not exist at runtime. To this end,
+method ``m`` of class ``Base`` of the example above can be replaced as follows:
 
 .. code:: python
 
     from dyndesign import safeinvoke
 
     ...
 
@@ -366,16 +461,16 @@
             print(f"Method `m` of {class_desc}")
             safeinvoke("optional_method", self, fallback=self.fallback)
 
 
 Singleton classes
 -----------------
 
-Singleton classes can be swiftly created and destroyed with
-``destroy_singleton``:
+Singleton classes can be swiftly created with `SingletonMeta` metaclass and then
+destroyed with `destroy_singleton`:
 
 .. code:: python
 
     from dyndesign import SingletonMeta
 
     class Singleton(metaclass=SingletonMeta):
         def __init__(self, instance_id = None):
@@ -384,23 +479,27 @@
             print(f"Created a {instance_id} instance of `Singleton`")
 
         def where_points(self, object_name):
             print(f"Object `{object_name}` points to the {self.instance_id} instance")
 
     s_A = Singleton("first")
     s_A.where_points("s_A")
-    s_B = Singleton()
+
+    # Created a first instance of `Singleton`
+    # Object `s_A` points to the first instance
+
+    s_B = Singleton("second")
     s_B.where_points("s_B")
+
+    # Object `s_B` points to the first instance
+
     Singleton().destroy_singleton()
     s_C = Singleton("second")
     s_C.where_points("s_C")
 
-    # Created a first instance of `Singleton`
-    # Object `s_A` points to the first instance
-    # Object `s_B` points to the first instance
     # Created a second instance of `Singleton`
     # Object `s_C` points to the second instance
 
 The class method ``destroy`` of SingletonMeta can be invoked to destroy all the
 Singleton classes at once. As a further alternative to the instance call
 ``destroy_singleton``, the names of the Singleton classes to destroy can be
 passed to the class method ``destroy``:
@@ -423,22 +522,22 @@
     from dyndesign import importclass
 
     ClassA = importclass('package_A', 'ClassA')
     ClassB = importclass('directory_B.package_B.ClassB')
 
 
 Running tests
---------------
+-------------
 
-To run the tests using your default python:
+To run the tests using your default python interpreter:
 
 ::
 
     pip install -U pytest
-    python3 -m pytest test
+    python -m pytest test
 
 
 .. |Build Status| image:: https://github.com/amarula/dyndesign/actions/workflows/python-app.yml/badge.svg
     :target: https://github.com/amarula/dyndesign/actions
 .. |Python Version Status| image:: https://img.shields.io/badge/python-3.8_3.9_3.10_3.11-blue.svg
     :target: https://github.com/amarula/dyndesign/actions
 .. |PyPi Version Status| image:: https://badge.fury.io/py/dyndesign.svg
```

### Comparing `dyndesign-0.9.7/dyndesign/classmerger.py` & `dyndesign-0.9.8/dyndesign/classmerger.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from functools import wraps
 from typing import Any, Callable, Dict, List, Tuple, Type, Union
 from collections import deque
 import re
 import inspect
 
-from dyndesign.dynloader import importclass
+from dyndesign.dynloader import preprocess_classes
 
 __all__ = ["mergeclasses"]
 
 
 DECORATED_STACK_FUNCTION_NAME = 'dynamic_decorator_func'
 
 
@@ -77,30 +77,30 @@
     decorator_instance: Callable,
     is_last_decorator: bool = False
 ) -> Callable:
     """Build a single decorator wrapper around a method using an instance of decorator.
 
     :param func: method to be decorated.
     :param decorator_instance: instance of decorator.
-    :param is_last_decorator: whether the decorator is the last in the pipeline or not.
+    :param is_last_decorator: whether the decorator is the last in the chain or not.
     :return: decorator wrapper.
     """
     args_from = 2 if is_last_decorator else 1
     @wraps(func)
     def dynamic_decorator_func(*args, **kwargs) -> Any:
         filtered_args, filtered_kwargs = __adapt_arguments(decorator_instance, func, *args[args_from:], **kwargs)
         return decorator_instance(args[0], *filtered_args, **filtered_kwargs)
     return dynamic_decorator_func
 
 
 def __merged_decorator_builder(
     func: Callable,
     decorator_instances: List[Callable]
 ) -> Callable:
-    """Build a merged decorator wrapper from two or more instances of decorator (called in pipeline).
+    """Build a merged decorator wrapper from two or more instances of decorator (called in chain).
 
     :param func: method to be decorated.
     :param decorator_instances: two or more instances of decorator.
     :return: merged decorator wrapper.
     """
     decorator_instance =  decorator_instances.pop()
     if decorator_instances:
@@ -109,20 +109,20 @@
             decorator_instances=decorator_instances
         )
     else:
         return __decorator_builder(func, decorator_instance, is_last_decorator=True)
 
 
 def __merge_not_overloaded(
-    classes: List[Type],
+    classes: Tuple[Type, ...],
     method: str,
     strict_merged_args: bool
 ) -> Union[Callable, None]:
     """Build a merged method by calling all the same-name method instances from the merged classes. If the method is
-    used as a decorator (via `decoratewith`), then all the decorator instances are merged and called in pipeline.
+    used as a decorator (via `decoratewith`), then all the decorator instances are merged and called in chain.
 
     :param classes: merged classes.
     :param method: name of the method to be merged.
     :param strict_merged_args: whether a `TypeError` exception is raised or not in case one or more positional
                                arguments are missing.
     :return: merged method if two or more method instances are found, None otherwise.
     """
@@ -146,38 +146,31 @@
                         if strict_merged_args or not __is_missing_arguments_exception(e, method_instance):
                             raise e
         return returned_value
 
     return call_all_method_instances
 
 
-def __preprocess_classes(all_classes: Any) -> List[Type]:
-    """Dynamically import classes if passed as strings."""
-    return [importclass(class_id) if type(class_id) == str else class_id for class_id in all_classes]
-
-
+@preprocess_classes
 def mergeclasses(
-    base_class: Any,
-    *extension_classes: Any,
+    *all_classes: Type,
     invoke_all: Union[List[str], None] = None,
     strict_merged_args = True
 ) -> Type:
-    """Merge (i.e., extend) a base class with one or more extension classes. If more than one extension classes are
-    provided, then the classes are extended in sequence following the order of `extension_classes`.
+    """Merge a base class with one or more extension classes. If more than one extension classes are
+    provided, then the classes are merged in sequence following the order of `extension_classes`.
 
-    :param base_class: base class.
-    :param extension_classes: extension classes.
+    :param all_classes: base and extension classes.
     :param invoke_all: list of methods (in addition to `__init__`) whose instances are invoked (if present) from all
                        the merged classes, rather than being overloaded by the instance from the rightmost class.
     :param strict_merged_args: controls whether a `TypeError` exception is raised or not in case one or more positional
                                arguments are missing in the `invoke_all` methods. If it is set to True (default value)
                                an exception is raised, otherwise methods with missing arguments are silently skipped.
     :return: merged class.
     """
-    all_classes = __preprocess_classes((base_class,) + extension_classes)
     invoke_all = ["__init__"] + (invoke_all or [])
     methods_not_oveloaded = {
         method: merged for method in invoke_all if (
             merged := __merge_not_overloaded(all_classes, method, strict_merged_args)
         )
     }
     return type(
```

### Comparing `dyndesign-0.9.7/dyndesign/dynmethod.py` & `dyndesign-0.9.8/dyndesign/dynmethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from contextlib import AbstractContextManager
 from functools import wraps
 from operator import attrgetter
 import re
 from typing import Any, Callable, List, Union
 
+from dyndesign.exceptions import ErrorMethodNotFound
+
 __all__ = ["decoratewith", "safeinvoke", "safezone"]
 
 
 def __is_sub_object(method_name: str):
     return '.' in method_name
 
 
@@ -57,15 +59,15 @@
     if method_sub_instance:
         method_names = [f"{method_sub_instance}.{m}" for m in method_names]
 
     def dynamic_decorator_wrapper(
         func: Callable,
         method_names: List[str] = method_names
     ) -> Callable:
-        """Decorator wrapper using one or more decorator methods in pipeline to decorate a function `func`.
+        """Decorator wrapper using one or more decorator methods in chain to decorate a function `func`.
 
         :param func: function to decorate.
         :param method_names: method name(s) of the one or more decorator methods.
         :return: decorated method.
         """
         method_name = method_names.pop()
 
@@ -153,11 +155,7 @@
             exctype is not None and
             issubclass(exctype, expected_exception) and
             self.__is_protected_name(excinst)
         )
         if result and self.__fallback:
             self.__fallback()
         return result
-
-
-class ErrorMethodNotFound(Exception):
-    """Raised when a dynamic method cannot be found."""
```

### Comparing `dyndesign-0.9.7/dyndesign/singletonmeta.py` & `dyndesign-0.9.8/dyndesign/singletonmeta.py`

 * *Files identical despite different names*

### Comparing `dyndesign-0.9.7/pyproject.toml` & `dyndesign-0.9.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "dyndesign"
-version = "0.9.7"
-description = "Toolset for Dynamic Design Patterns in Python."
+version = "0.9.8"
+description = "Toolset for Dynamic Design in Python."
 authors = ["Patrizio Gelosi <patrizio.gelosi@amarulasolutions.com>"]
 maintainers = ["Patrizio Gelosi <patrizio.gelosi@amarulasolutions.com>"]
 repository = "https://github.com/amarula/dyndesign"
 license = "MIT"
 readme = "README.rst"
-keywords = ["design", "pattern", "dynamic", "decorator", "inheritance"]
+keywords = ["design", "dynamic", "decorator", "inheritance"]
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `dyndesign-0.9.7/PKG-INFO` & `dyndesign-0.9.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dyndesign
-Version: 0.9.7
-Summary: Toolset for Dynamic Design Patterns in Python.
+Version: 0.9.8
+Summary: Toolset for Dynamic Design in Python.
 Home-page: https://github.com/amarula/dyndesign
 License: MIT
-Keywords: design,pattern,dynamic,decorator,inheritance
+Keywords: design,dynamic,decorator,inheritance
 Author: Patrizio Gelosi
 Author-email: patrizio.gelosi@amarulasolutions.com
 Maintainer: Patrizio Gelosi
 Maintainer-email: patrizio.gelosi@amarulasolutions.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -16,30 +16,32 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/amarula/dyndesign
 Description-Content-Type: text/x-rst
 
 DynDesign
 =========
 
 |Build Status| |PyPi Version Status| |Python Version Status| |License|
 
-A set of tools for Dynamic Design Patterns in Python.
+A set of tools for Dynamic Design in Python.
+
+
+Documentation
+-------------
+
+DynDesign's full documentation can be found at
+https://dyndesign.readthedocs.io/en/latest/
 
 
 Install
 -------
 
 Dyndesign is on the Python Package Index (PyPI):
 
@@ -47,42 +49,63 @@
 
     pip install dyndesign
 
 
 Overview
 --------
 
+Dynamically add parent classes:
+
+.. code:: python
+
+    from dyndesign import DynInheritance
+
+    class Child(DynInheritance):
+        ...
+
+    Child.dynparents_add(Parent1)
+    c = Child()
+    c.method_of_Parent1()
+
+
 Merge two or more classes:
 
 .. code:: python
 
     from dyndesign import mergeclasses
 
-    MergedClass = mergeclasses(Base, Ext1, Ext2, ...)
+    MergedClass = mergeclasses(Base, Ext1)
+    m = MergedClass()
+    m.method_of_Ext1()
 
 Decorate a method with one or more instance methods loaded at runtime:
 
 .. code:: python
 
     from dyndesign import decoratewith
 
     @decoratewith("decorator_1", "component.decorator_2", ...)
     def decorated_method(self, ...):
         ...
 
-Safely invoke functions or methods from a ``safezone`` context manager:
+Safely invoke functions or methods from a ``safezone`` context manager or by
+using the ``safeinvoke`` API:
 
 .. code:: python
 
-    from dyndesign import safezone
+    from dyndesign import safezone, safeinvoke
 
     with safezone():
         ...
         function_possibly_non_existent()
-        ...
+
+    ...
+
+    def method(self):
+        safeinvoke("method_possibly_non_existent", self)
 
 Create and destroy Singleton classes:
 
 .. code:: python
 
     from dyndesign import SingletonMeta
 
@@ -99,22 +122,88 @@
 .. code:: python
 
     from dyndesign import importclass
 
     ImportedClass = importclass("directory.module.class_name")
 
 
-Merging Classes
----------------
+Dynamic Inheritance
+-------------------
+
+With Dynamic Inheritance, it becomes possible to dynamically modify the
+superclass set of classes that inherit from special class ``DynInheritance``. This
+allows the addition of parent classes to those classes, and the modification is
+also instantly reflected in all their instances.
+
+.. code:: python
+
+    from dyndesign import DynInheritance
+
+    class Parent:
+        def m1(self):
+            print("Method `m1` from `Parent`")
+
+    class Child(DynInheritance):
+        def __init__(self):
+            print("Constructor of `Child`")
+
+    child_instance = Child()
+
+    # Constructor of `Child`
+
+    Child.dynparents_add(Parent)
+    child_instance.m1()
+
+    # Method `m1` from `Parent`
+
+When the special class ``DynInheritanceLockedInstances`` is utilized instead of
+``DynInheritance``, the superclass set is locked within each class instance,
+meaning that it remains unchanged even when there are modifications to the
+class's superclasses.
+
+.. code:: python
+
+    class Parent:
+        def __init__(self):
+            print("Constructor of `Parent`")
+
+        def mtd(self):
+            print("Method `mtd` of `Parent`")
+
+    class Child(DynInheritanceLockedInstances):
+        def __init__(self):
+            super(DynInheritanceLockedInstances, self).__init__()
+            print("Constructor of `Child`")
+
+    orphan_child = Child()
+
+    # Constructor of `Child`
+
+    Child.dynparents_add(Parent)
+    child_with_parent = Child()
+
+    # Constructor of `Parent`
+    # Constructor of `Child`
+
+    child_with_parent.mtd()
+
+    # Method `mtd` of `Parent`
+
+    orphan_child.mtd()
+
+    # AttributeError: 'Child' object has no attribute 'mtd'
+
+Class Merging
+-------------
 
 Dyndesign provides API ``mergeclasses`` to merge two or more classes as if they
-were dictionaries, so that the merged class has the attributes and methods of
-the base class and of the extension classes. If two or more classes have the
-same attributes/methods, the attributes/methods from the rightmost classes (in
-the order in which the classes are passed to ``mergeclasses``) overload the
+were dictionaries. As a result, the newly created class has the same properties
+from both its base class and any added extensions. If two or more classes have
+the same attributes/methods, the attributes/methods from the rightmost classes
+(in the order in which the classes are passed to ``mergeclasses``) overload the
 ones from the leftmost classes, similarly to what happens when merging
 dictionaries.
 
 .. code:: python
 
     from dyndesign import mergeclasses
 
@@ -170,43 +259,44 @@
 
     # No argument passed to class `A`
     # Argument a='Alpha' passed to class `B`
     # Argument a='Alpha', b='Beta' and kw1='kwarg #1' passed to class `C`
     # Argument kw2='kwarg #2' passed to class `D`
 
 On the other hand, if any required positional argument is missing, an exception
-is raised. If `MergedClass` of the above example is initialized with no
-parameters, and exception is raised when the constructor of class `B` is called:
+is raised. If ``MergedClass`` of the above example is initialized with no
+parameters, and exception is raised when the constructor of class ``B`` is
+called:
 
 .. code:: python
 
     ...
     MergedClass()
 
     # ...
     # TypeError: B.__init__() missing 1 required positional argument: 'a'
 
 So as to have constructor instances with missing positional arguments silently
-skipped, `strict_merged_args` can be set to False in `mergeclasses`. In the
-above example, constructors of class `B` and `C` are skipped:
+skipped, ``strict_merged_args`` can be set to False in ``mergeclasses``. In the
+above example, constructors of class ``B`` and ``C`` are skipped:
 
 .. code:: python
 
     ...
     MergedClass = mergeclasses(A, B, C, D, strict_merged_args=False)
     MergedClass()
 
     # No argument passed to class `A`
     # Argument kw2=None passed to class `D`
 
 
 It is also possible to extend the same behavior of the constructor ``__init__``
 (i.e., all the methods from all the merged classes are invoked rather than being
 overloaded by the same name method from the rightmost class) to other methods. A
-list of method names whose instances have to be all invoked can be specified in
+list of method names whose instances must be all invoked can be specified in
 the ``invoke_all`` argument of ``mergeclasses``. Adaptive filtering of the
 arguments of the method instances is performed as well.
 
 .. code:: python
 
     class E:
         def method(self):
@@ -222,24 +312,24 @@
     # No argument passed to `method` of class `E`
     # Argument a='Alpha' passed to `method` of class `F`
 
 
 Dynamic Decorators
 ------------------
 
-Meta decorator ``decoratewith`` decorates a class method with one or more
-pipelined instance decorators (regardless whether they statically exist or not).
-The syntax of the dynamic decorators aims to get rid of the boilerplate for
-wrapping and returning the decorator code, leaving just the wrapper's code. For
-example, dynamic decorators can be used to decorate a method from a base class
-with a method from an extension class:
+Meta decorator ``decoratewith`` can be used to decorate a class method with one
+or more chained dynamic decorators, regardless whether they statically exist
+or not. Additionally, the syntax of the dynamic decorators aims to get rid of
+the boilerplate for wrapping and returning the decorator code, leaving just the
+wrapper's code. For example, dynamic decorators can be used to decorate a method
+of a base class with a method of an extension class:
 
 .. code:: python
 
-    from dyndesign import decoratewith
+    from dyndesign import decoratewith, mergeclasses
 
     class Base:
         @decoratewith("decorator")
         def m(self):
             print(f"Method `m` of class `Base`")
 
     class Ext:
@@ -253,15 +343,15 @@
 
     # Beginning of method decoration from Ext.
     # Method `m` of class `Base`
     # End of method decoration from Ext.
 
 If a decorator name is passed in the ``invoke_all`` argument of
 ``mergeclasses``, then multiple decorator instances with the same name from
-different extension classes may be used in pipeline:
+different extension classes may be used in chain:
 
 .. code:: python
 
     class Ext2:
         def decorator(self, func):
             print("Beginning of method decoration from Ext2.")
             func(self)
@@ -333,15 +423,15 @@
 protection is restricted to the functions having that/those name(s). For
 example, ``safezone`` can be used to safely call functions that may or may not
 exist at runtime:
 
 .. code:: python
 
     from dyndesign import safezone
-    
+
     def fallback():
         print("Fallback function")
 
     def function_a():
         print("Function `a`")
 
     with safezone(fallback=fallback):
@@ -380,17 +470,17 @@
     # Method `m` of class `Base` standalone
     # Fallback method
 
 
 Invoking methods safely
 -----------------------
 
-As alternative to ``safezone`` context manager, ``safeinvoke`` can be used to
-safely invoke methods that may or may not exist at runtime. To this end, method
-``m`` of class ``Base`` of the example above can be replaced as follows:
+As an alternative to ``safezone`` context manager, ``safeinvoke`` API can be
+used to safely invoke methods that may or may not exist at runtime. To this end,
+method ``m`` of class ``Base`` of the example above can be replaced as follows:
 
 .. code:: python
 
     from dyndesign import safeinvoke
 
     ...
 
@@ -398,16 +488,16 @@
             print(f"Method `m` of {class_desc}")
             safeinvoke("optional_method", self, fallback=self.fallback)
 
 
 Singleton classes
 -----------------
 
-Singleton classes can be swiftly created and destroyed with
-``destroy_singleton``:
+Singleton classes can be swiftly created with `SingletonMeta` metaclass and then
+destroyed with `destroy_singleton`:
 
 .. code:: python
 
     from dyndesign import SingletonMeta
 
     class Singleton(metaclass=SingletonMeta):
         def __init__(self, instance_id = None):
@@ -416,23 +506,27 @@
             print(f"Created a {instance_id} instance of `Singleton`")
 
         def where_points(self, object_name):
             print(f"Object `{object_name}` points to the {self.instance_id} instance")
 
     s_A = Singleton("first")
     s_A.where_points("s_A")
-    s_B = Singleton()
+
+    # Created a first instance of `Singleton`
+    # Object `s_A` points to the first instance
+
+    s_B = Singleton("second")
     s_B.where_points("s_B")
+
+    # Object `s_B` points to the first instance
+
     Singleton().destroy_singleton()
     s_C = Singleton("second")
     s_C.where_points("s_C")
 
-    # Created a first instance of `Singleton`
-    # Object `s_A` points to the first instance
-    # Object `s_B` points to the first instance
     # Created a second instance of `Singleton`
     # Object `s_C` points to the second instance
 
 The class method ``destroy`` of SingletonMeta can be invoked to destroy all the
 Singleton classes at once. As a further alternative to the instance call
 ``destroy_singleton``, the names of the Singleton classes to destroy can be
 passed to the class method ``destroy``:
@@ -455,22 +549,22 @@
     from dyndesign import importclass
 
     ClassA = importclass('package_A', 'ClassA')
     ClassB = importclass('directory_B.package_B.ClassB')
 
 
 Running tests
---------------
+-------------
 
-To run the tests using your default python:
+To run the tests using your default python interpreter:
 
 ::
 
     pip install -U pytest
-    python3 -m pytest test
+    python -m pytest test
 
 
 .. |Build Status| image:: https://github.com/amarula/dyndesign/actions/workflows/python-app.yml/badge.svg
     :target: https://github.com/amarula/dyndesign/actions
 .. |Python Version Status| image:: https://img.shields.io/badge/python-3.8_3.9_3.10_3.11-blue.svg
     :target: https://github.com/amarula/dyndesign/actions
 .. |PyPi Version Status| image:: https://badge.fury.io/py/dyndesign.svg
```

