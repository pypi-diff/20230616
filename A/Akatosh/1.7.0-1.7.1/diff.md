# Comparing `tmp/Akatosh-1.7.0.tar.gz` & `tmp/Akatosh-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-1.7.0.tar", last modified: Tue Apr  4 13:54:20 2023, max compression
+gzip compressed data, was "Akatosh-1.7.1.tar", last modified: Fri Jun 16 07:32:38 2023, max compression
```

## Comparing `Akatosh-1.7.0.tar` & `Akatosh-1.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 13:54:20.757705 Akatosh-1.7.0/
-drwxrwxrwx   0        0        0        0 2023-04-04 13:54:20.739706 Akatosh-1.7.0/Akatosh/
--rw-rw-rw-   0        0        0      129 2023-03-29 05:49:42.000000 Akatosh-1.7.0/Akatosh/__init__.py
--rw-rw-rw-   0        0        0    18109 2023-03-29 05:49:42.000000 Akatosh-1.7.0/Akatosh/actor.py
--rw-rw-rw-   0        0        0     1073 2023-03-29 05:49:42.000000 Akatosh-1.7.0/Akatosh/event.py
--rw-rw-rw-   0        0        0     6678 2023-03-29 05:49:42.000000 Akatosh-1.7.0/Akatosh/producer.py
--rw-rw-rw-   0        0        0    11540 2023-04-04 13:52:47.000000 Akatosh-1.7.0/Akatosh/resource.py
--rw-rw-rw-   0        0        0     2042 2023-03-29 05:49:42.000000 Akatosh-1.7.0/Akatosh/timeline.py
--rw-rw-rw-   0        0        0     1723 2023-03-29 05:49:42.000000 Akatosh-1.7.0/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-04-04 13:54:20.747207 Akatosh-1.7.0/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2011 2023-04-04 13:54:20.000000 Akatosh-1.7.0/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-04-04 13:54:20.000000 Akatosh-1.7.0/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 13:54:20.000000 Akatosh-1.7.0/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-04 13:54:20.000000 Akatosh-1.7.0/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2011 2023-04-04 13:54:20.756206 Akatosh-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1482 2023-03-29 05:49:42.000000 Akatosh-1.7.0/README.md
--rw-rw-rw-   0        0        0      585 2023-04-04 13:54:01.000000 Akatosh-1.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-04 13:54:20.757705 Akatosh-1.7.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-04 13:54:20.754206 Akatosh-1.7.0/test/
--rw-rw-rw-   0        0        0      688 2023-03-29 05:49:42.000000 Akatosh-1.7.0/test/test_actor.py
--rw-rw-rw-   0        0        0      245 2023-03-29 05:49:42.000000 Akatosh-1.7.0/test/test_decorator.py
--rw-rw-rw-   0        0        0      298 2023-04-04 13:52:59.000000 Akatosh-1.7.0/test/test_resource.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:32:38.761060 Akatosh-1.7.1/
+drwxrwxrwx   0        0        0        0 2023-06-16 07:32:38.739063 Akatosh-1.7.1/Akatosh/
+-rw-rw-rw-   0        0        0      129 2023-05-17 02:07:37.000000 Akatosh-1.7.1/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0    17075 2023-05-17 02:07:37.000000 Akatosh-1.7.1/Akatosh/actor.py
+-rw-rw-rw-   0        0        0     1073 2023-05-17 02:07:37.000000 Akatosh-1.7.1/Akatosh/event.py
+-rw-rw-rw-   0        0        0     6678 2023-05-17 02:07:37.000000 Akatosh-1.7.1/Akatosh/producer.py
+-rw-rw-rw-   0        0        0    11540 2023-05-17 02:07:37.000000 Akatosh-1.7.1/Akatosh/resource.py
+-rw-rw-rw-   0        0        0     2042 2023-05-17 02:07:37.000000 Akatosh-1.7.1/Akatosh/timeline.py
+-rw-rw-rw-   0        0        0     1959 2023-06-16 07:29:25.000000 Akatosh-1.7.1/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:32:38.747063 Akatosh-1.7.1/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2011 2023-06-16 07:32:38.000000 Akatosh-1.7.1/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-06-16 07:32:38.000000 Akatosh-1.7.1/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 07:32:38.000000 Akatosh-1.7.1/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 07:32:38.000000 Akatosh-1.7.1/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2011 2023-06-16 07:32:38.759060 Akatosh-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1482 2023-05-17 02:07:37.000000 Akatosh-1.7.1/README.md
+-rw-rw-rw-   0        0        0      669 2023-06-16 07:29:39.000000 Akatosh-1.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 07:32:38.761060 Akatosh-1.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 07:32:38.756060 Akatosh-1.7.1/test/
+-rw-rw-rw-   0        0        0      169 2023-05-17 02:07:37.000000 Akatosh-1.7.1/test/test_actor.py
+-rw-rw-rw-   0        0        0      245 2023-05-17 02:07:37.000000 Akatosh-1.7.1/test/test_decorator.py
+-rw-rw-rw-   0        0        0      298 2023-05-17 02:07:37.000000 Akatosh-1.7.1/test/test_resource.py
```

### Comparing `Akatosh-1.7.0/Akatosh/actor.py` & `Akatosh-1.7.1/Akatosh/actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from __future__ import annotations
-from typing import Generator, List, Optional, Union, Callable, TYPE_CHECKING
+from typing import List, Optional, Union, Callable, TYPE_CHECKING
 from uuid import uuid4
-from math import inf
 import warnings
 
 from Akatosh import Mundus
 
 if TYPE_CHECKING:
     from .resource import Resource
     from .producer import Producer
-    from .timeline import Timeline
 
 
 class Actor:
     def __init__(
         self,
         action: Optional[Callable] = None,
         at: Union[int, float, Callable] = 0,
@@ -392,54 +390,31 @@
         step (Optional[int  |  float  |  Callable], optional): how frequently the event should occur, till must also be given. Defaults to None.
         till (Optional[int  |  float  |  Callable], optional): when the event should end, step must also be given. Defaults to None.
         after (Optional[List[Actor]  |  Actor], optional): the event(s) that must happens before this event. Defaults to None.
         priority (int, optional): the priority of the event, if multiple event should happen at the same time, then the event with lower value as priority happens first. Defaults to 0.
         active (bool, optional): whether the event should be active upon creation. Defaults to True.
         label (Optional[str], optional): the short description of this event. Defaults to None.
         on_call (bool, optional): if ture, the event will not be created until the decorated function is called. If false, the event will be create directly without need for calling the decorated function. Defaults to False.
-    """    
+    """
+
     def create_event(func):
         def _event(*args, **kwargs):
-            # class Event(Actor):
-            #     def __init__(
-            #         self,
-            #         at: Union[int, float, Callable] = 0,
-            #         step: Optional[int | float | Callable] = None,
-            #         till: Optional[int | float | Callable] = None,
-            #         after: Optional[Actor | List[Actor]] = None,
-            #         priority: int = 0,
-            #         active: bool = True,
-            #         label: Optional[str] = None,
-            #     ) -> None:
-            #         super().__init__(
-            #             at=at,
-            #             step=step,
-            #             till=till,
-            #             after=after,
-            #             priority=priority,
-            #             active=active,
-            #             label=label,
-            #         )
-
-            #     def action(self):
-            #         func(*args, **kwargs)
-
             actor = Actor(
                 action=func,
                 at=at,
                 step=step,
                 till=till,
                 after=after,
                 priority=priority,
                 active=active,
                 label=label,
                 **kwargs,
             )
 
             return actor
+
         if on_call:
             return _event
         else:
             return _event()
 
     return create_event
-
```

### Comparing `Akatosh-1.7.0/Akatosh/event.py` & `Akatosh-1.7.1/Akatosh/event.py`

 * *Files identical despite different names*

### Comparing `Akatosh-1.7.0/Akatosh/producer.py` & `Akatosh-1.7.1/Akatosh/producer.py`

 * *Files identical despite different names*

### Comparing `Akatosh-1.7.0/Akatosh/resource.py` & `Akatosh-1.7.1/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `Akatosh-1.7.0/Akatosh/timeline.py` & `Akatosh-1.7.1/Akatosh/timeline.py`

 * *Files identical despite different names*

### Comparing `Akatosh-1.7.0/Akatosh/universe.py` & `Akatosh-1.7.1/Akatosh/universe.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,23 +19,27 @@
 
     def __init__(self, accuracy:int=3) -> None:
         """The universe in which the simulation takes place. Should not be instantiated directly."""
         self._id = uuid4().int
         self._timeline = Timeline()
         self._till = int()
         self._accuracy = accuracy
+        self._early_stop = False
 
     def simulate(self, till: Union[int, float] = inf) -> None:
         """Simulate the universe to a given time."""
         self._till = till
-        while self.timeline.now <= self.till:
+        while self.timeline.now <= self.till and self.early_stop is False:
             self.timeline.forward(self.till)
             if len(self.timeline.events) == 0:
                 break
-
+            
+    def stop(self) -> None:
+        self._early_stop = True
+        
     @property
     def timeline(self) -> Timeline:
         """The timeline of the universe."""
         return self._timeline
 
     @property
     def till(self) -> Union[int, float]:
@@ -52,8 +56,12 @@
         """The accuracy of the universe in term of minimum time step. e.g., 3 means 0.001s."""
         return self._accuracy
 
     @accuracy.setter
     def accuracy(self, value: int) -> None:
         self._accuracy = value
 
+    @property
+    def early_stop(self) -> bool:
+        return self._early_stop
+    
 Mundus = Universe()
```

### Comparing `Akatosh-1.7.0/Akatosh.egg-info/PKG-INFO` & `Akatosh-1.7.1/Akatosh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 1.7.0
+Version: 1.7.1
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `Akatosh-1.7.0/PKG-INFO` & `Akatosh-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 1.7.0
+Version: 1.7.1
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `Akatosh-1.7.0/README.md` & `Akatosh-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-1.7.0/pyproject.toml` & `Akatosh-1.7.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [project]
 name = "Akatosh"
-version = "1.7.0"
-authors = [
-  { name="Yifei Ren", email="ryf0510@live.com" },
-]
+version = "1.7.1"
+authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+  "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ulfaric/Akatosh"
 "Bug Tracker" = "https://github.com/ulfaric/Akatosh/issues"
 
 [tool.setuptools]
-packages = ["Akatosh"]
+packages = ["Akatosh"]
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = "-ra -q"
+testpaths = ["test"]
```

