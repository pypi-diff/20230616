# Comparing `tmp/mdis-0.1.tar.gz` & `tmp/mdis-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ghostmansd/mdis/dist/.tmp-mz8i6m12/mdis-0.1.tar", last modified: Tue Jun 13 20:07:08 2023, max compression
+gzip compressed data, was "/home/ghostmansd/mdis/dist/.tmp-7z_xmyvn/mdis-0.2.tar", last modified: Fri Jun 16 20:12:32 2023, max compression
```

## Comparing `mdis-0.1.tar` & `mdis-0.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-13 20:07:08.000000 mdis-0.1/
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     1272 2023-06-13 20:03:06.000000 mdis-0.1/LICENSE
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4407 2023-06-13 20:07:08.000000 mdis-0.1/PKG-INFO
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     3593 2023-06-13 20:03:06.000000 mdis-0.1/README.md
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      928 2023-06-13 20:03:06.000000 mdis-0.1/pyproject.toml
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)       38 2023-06-13 20:07:08.000000 mdis-0.1/setup.cfg
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-13 20:07:08.000000 mdis-0.1/src/
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-13 20:07:08.000000 mdis-0.1/src/mdis/
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      328 2023-06-13 20:06:37.000000 mdis-0.1/src/mdis/__init__.py
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     1356 2023-06-13 20:03:06.000000 mdis-0.1/src/mdis/core.py
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     1176 2023-06-13 20:03:06.000000 mdis-0.1/src/mdis/dispatcher.py
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      399 2023-06-13 20:03:06.000000 mdis-0.1/src/mdis/visitor.py
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      702 2023-06-13 20:03:06.000000 mdis-0.1/src/mdis/walker.py
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-13 20:07:08.000000 mdis-0.1/src/mdis.egg-info/
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4407 2023-06-13 20:07:08.000000 mdis-0.1/src/mdis.egg-info/PKG-INFO
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      260 2023-06-13 20:07:08.000000 mdis-0.1/src/mdis.egg-info/SOURCES.txt
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        1 2023-06-13 20:07:08.000000 mdis-0.1/src/mdis.egg-info/dependency_links.txt
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        5 2023-06-13 20:07:08.000000 mdis-0.1/src/mdis.egg-info/top_level.txt
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-16 20:12:32.000000 mdis-0.2/
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     1272 2023-06-13 22:23:19.000000 mdis-0.2/LICENSE
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4456 2023-06-16 20:12:32.000000 mdis-0.2/PKG-INFO
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     3642 2023-06-14 10:36:25.000000 mdis-0.2/README.md
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      928 2023-06-16 20:05:13.000000 mdis-0.2/pyproject.toml
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)       38 2023-06-16 20:12:32.000000 mdis-0.2/setup.cfg
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-16 20:12:32.000000 mdis-0.2/src/
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-16 20:12:32.000000 mdis-0.2/src/mdis/
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      328 2023-06-16 20:05:17.000000 mdis-0.2/src/mdis/__init__.py
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     2430 2023-06-14 10:35:12.000000 mdis-0.2/src/mdis/dispatcher.py
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      322 2023-06-14 10:34:25.000000 mdis-0.2/src/mdis/visitor.py
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      624 2023-06-14 10:29:43.000000 mdis-0.2/src/mdis/walker.py
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-16 20:12:32.000000 mdis-0.2/src/mdis.egg-info/
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4456 2023-06-16 20:12:32.000000 mdis-0.2/src/mdis.egg-info/PKG-INFO
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      243 2023-06-16 20:12:32.000000 mdis-0.2/src/mdis.egg-info/SOURCES.txt
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        1 2023-06-16 20:12:32.000000 mdis-0.2/src/mdis.egg-info/dependency_links.txt
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        5 2023-06-16 20:12:32.000000 mdis-0.2/src/mdis.egg-info/top_level.txt
```

### Comparing `mdis-0.1/LICENSE` & `mdis-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdis-0.1/PKG-INFO` & `mdis-0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdis
-Version: 0.1
+Version: 0.2
 Summary: Python dispatching library
 Author-email: Dmitry Selyutin <ghostmansd@gmail.com>
 Project-URL: Homepage, https://repo.or.cz/mdis.git
 Project-URL: Bug Tracker, https://repo.or.cz/mdis.git
 Keywords: dispatch,dispather,map,iterator,iterable,visitor,walker
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -37,20 +37,20 @@
 `dict.__iter__` method yields just keys, and the values have to be got via `__getitem__` calls.
 Also, in order to support nested collections, users will have to write some recursive code with `isinstance` checks.
 With `mdis.Walker`, users can just install the handlers for the types of interest, and change the iteration logic.
 A walker is just a particular example of dispatcher, where the call yields some objects in a class-dependent manner.
 The default `mdis.Walker` already incorporates the logic to walk over some builtin Python objects.
 The example below shows how to override the way the dicts are traversed so that keys and values are swapped.
 
-    import mdis.core
+    import mdis.dispatcher
     import mdis.walker
 
     class CustomWalker(mdis.walker.Walker):
-        @mdis.core.hook(dict)
-        def walk_dict(self, instance):
+        @mdis.dispatcher.hook(dict)
+        def dispatch_dict(self, instance):
             for (key, value) in instance.items():
                 yield (value, key)
                 yield from self((value, key))
 
     collection = {"a": 1, "b": 2}
     walker = CustomWalker()
     for item in walker(collection):
@@ -70,35 +70,35 @@
 In `mdis`, a visitor is just another particular example of dispatcher.
 Whenever the visitor is called, the call is dispatched based on type, and some per-class action is performed.
 The primary scenario is to combine the visitor calls with context managers.
 The example below shows how to execute some arbitrary code upon visiting an object.
 
     import contextlib
 
-    import mdis.core
+    import mdis.dispatcher
     import mdis.visitor
 
     class CustomVisitor(mdis.visitor.Visitor):
-        @mdis.core.hook(int)
+        @mdis.dispatcher.hook(int)
         @contextlib.contextmanager
-        def visit_int(self, instance):
+        def dispatch_int(self, instance):
             print("entering int")
             yield (instance + 42)
             print("leaving int")
 
-        @mdis.core.hook(str)
+        @mdis.dispatcher.hook(str)
         @contextlib.contextmanager
-        def visit_str(self, instance):
+        def dispatch_str(self, instance):
             print("entering str")
             yield f"!!!{instance}!!!"
             print("leaving str")
 
-        @mdis.core.hook(object)
+        @mdis.dispatcher.hook(object)
         @contextlib.contextmanager
-        def visit_object(self, instance):
+        def dispatch_object(self, instance):
             print("entering object")
             yield instance
             print("leaving object")
 
     visitor = CustomVisitor()
     for item in (42, "cocojamboo", 1.5):
         with visitor(item) as result:
```

### Comparing `mdis-0.1/README.md` & `mdis-0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 `dict.__iter__` method yields just keys, and the values have to be got via `__getitem__` calls.
 Also, in order to support nested collections, users will have to write some recursive code with `isinstance` checks.
 With `mdis.Walker`, users can just install the handlers for the types of interest, and change the iteration logic.
 A walker is just a particular example of dispatcher, where the call yields some objects in a class-dependent manner.
 The default `mdis.Walker` already incorporates the logic to walk over some builtin Python objects.
 The example below shows how to override the way the dicts are traversed so that keys and values are swapped.
 
-    import mdis.core
+    import mdis.dispatcher
     import mdis.walker
 
     class CustomWalker(mdis.walker.Walker):
-        @mdis.core.hook(dict)
-        def walk_dict(self, instance):
+        @mdis.dispatcher.hook(dict)
+        def dispatch_dict(self, instance):
             for (key, value) in instance.items():
                 yield (value, key)
                 yield from self((value, key))
 
     collection = {"a": 1, "b": 2}
     walker = CustomWalker()
     for item in walker(collection):
@@ -50,35 +50,35 @@
 In `mdis`, a visitor is just another particular example of dispatcher.
 Whenever the visitor is called, the call is dispatched based on type, and some per-class action is performed.
 The primary scenario is to combine the visitor calls with context managers.
 The example below shows how to execute some arbitrary code upon visiting an object.
 
     import contextlib
 
-    import mdis.core
+    import mdis.dispatcher
     import mdis.visitor
 
     class CustomVisitor(mdis.visitor.Visitor):
-        @mdis.core.hook(int)
+        @mdis.dispatcher.hook(int)
         @contextlib.contextmanager
-        def visit_int(self, instance):
+        def dispatch_int(self, instance):
             print("entering int")
             yield (instance + 42)
             print("leaving int")
 
-        @mdis.core.hook(str)
+        @mdis.dispatcher.hook(str)
         @contextlib.contextmanager
-        def visit_str(self, instance):
+        def dispatch_str(self, instance):
             print("entering str")
             yield f"!!!{instance}!!!"
             print("leaving str")
 
-        @mdis.core.hook(object)
+        @mdis.dispatcher.hook(object)
         @contextlib.contextmanager
-        def visit_object(self, instance):
+        def dispatch_object(self, instance):
             print("entering object")
             yield instance
             print("leaving object")
 
     visitor = CustomVisitor()
     for item in (42, "cocojamboo", 1.5):
         with visitor(item) as result:
```

### Comparing `mdis-0.1/pyproject.toml` & `mdis-0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=46.4.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mdis"
-version = "0.1"
+version = "0.2"
 authors = [
   { name="Dmitry Selyutin", email="ghostmansd@gmail.com" },
 ]
 keywords = [
     "dispatch",
     "dispather",
     "map",
```

### Comparing `mdis-0.1/src/mdis.egg-info/PKG-INFO` & `mdis-0.2/src/mdis.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdis
-Version: 0.1
+Version: 0.2
 Summary: Python dispatching library
 Author-email: Dmitry Selyutin <ghostmansd@gmail.com>
 Project-URL: Homepage, https://repo.or.cz/mdis.git
 Project-URL: Bug Tracker, https://repo.or.cz/mdis.git
 Keywords: dispatch,dispather,map,iterator,iterable,visitor,walker
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -37,20 +37,20 @@
 `dict.__iter__` method yields just keys, and the values have to be got via `__getitem__` calls.
 Also, in order to support nested collections, users will have to write some recursive code with `isinstance` checks.
 With `mdis.Walker`, users can just install the handlers for the types of interest, and change the iteration logic.
 A walker is just a particular example of dispatcher, where the call yields some objects in a class-dependent manner.
 The default `mdis.Walker` already incorporates the logic to walk over some builtin Python objects.
 The example below shows how to override the way the dicts are traversed so that keys and values are swapped.
 
-    import mdis.core
+    import mdis.dispatcher
     import mdis.walker
 
     class CustomWalker(mdis.walker.Walker):
-        @mdis.core.hook(dict)
-        def walk_dict(self, instance):
+        @mdis.dispatcher.hook(dict)
+        def dispatch_dict(self, instance):
             for (key, value) in instance.items():
                 yield (value, key)
                 yield from self((value, key))
 
     collection = {"a": 1, "b": 2}
     walker = CustomWalker()
     for item in walker(collection):
@@ -70,35 +70,35 @@
 In `mdis`, a visitor is just another particular example of dispatcher.
 Whenever the visitor is called, the call is dispatched based on type, and some per-class action is performed.
 The primary scenario is to combine the visitor calls with context managers.
 The example below shows how to execute some arbitrary code upon visiting an object.
 
     import contextlib
 
-    import mdis.core
+    import mdis.dispatcher
     import mdis.visitor
 
     class CustomVisitor(mdis.visitor.Visitor):
-        @mdis.core.hook(int)
+        @mdis.dispatcher.hook(int)
         @contextlib.contextmanager
-        def visit_int(self, instance):
+        def dispatch_int(self, instance):
             print("entering int")
             yield (instance + 42)
             print("leaving int")
 
-        @mdis.core.hook(str)
+        @mdis.dispatcher.hook(str)
         @contextlib.contextmanager
-        def visit_str(self, instance):
+        def dispatch_str(self, instance):
             print("entering str")
             yield f"!!!{instance}!!!"
             print("leaving str")
 
-        @mdis.core.hook(object)
+        @mdis.dispatcher.hook(object)
         @contextlib.contextmanager
-        def visit_object(self, instance):
+        def dispatch_object(self, instance):
             print("entering object")
             yield instance
             print("leaving object")
 
     visitor = CustomVisitor()
     for item in (42, "cocojamboo", 1.5):
         with visitor(item) as result:
```

