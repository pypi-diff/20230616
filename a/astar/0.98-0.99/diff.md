# Comparing `tmp/astar-0.98-py3-none-any.whl.zip` & `tmp/astar-0.99-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 6615 bytes, number of entries: 6
--rw-r--r--  2.0 fat     6537 b- defN 80-Jan-01 00:00 astar/__init__.py
--rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 astar/py.typed
--rw-r--r--  2.0 fat     1496 b- defN 80-Jan-01 00:00 astar-0.98.dist-info/LICENSE
--rw-r--r--  2.0 fat     8619 b- defN 80-Jan-01 00:00 astar-0.98.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 astar-0.98.dist-info/WHEEL
-?rw-r--r--  2.0 fat      424 b- defN 16-Jan-01 00:00 astar-0.98.dist-info/RECORD
-6 files, 17164 bytes uncompressed, 5855 bytes compressed:  65.9%
+Zip file size: 6635 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     6637 b- defN 80-Jan-01 00:00 astar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 astar/py.typed
+-rw-r--r--  2.0 unx     1496 b- defN 80-Jan-01 00:00 astar-0.99.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8619 b- defN 80-Jan-01 00:00 astar-0.99.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 astar-0.99.dist-info/WHEEL
+?rw-r--r--  2.0 unx      424 b- defN 16-Jan-01 00:00 astar-0.99.dist-info/RECORD
+6 files, 17264 bytes uncompressed, 5875 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: astar/__init__.py
 Comment: 
 
 Filename: astar/py.typed
 Comment: 
 
-Filename: astar-0.98.dist-info/LICENSE
+Filename: astar-0.99.dist-info/LICENSE
 Comment: 
 
-Filename: astar-0.98.dist-info/METADATA
+Filename: astar-0.99.dist-info/METADATA
 Comment: 
 
-Filename: astar-0.98.dist-info/WHEEL
+Filename: astar-0.99.dist-info/WHEEL
 Comment: 
 
-Filename: astar-0.98.dist-info/RECORD
+Filename: astar-0.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## astar/__init__.py

```diff
@@ -42,30 +42,34 @@
 
 
 ################################################################################
 SNType = TypeVar("SNType", bound=SearchNode)
 
 
 class OpenSet(Generic[SNType]):
-        def __init__(self):
+        
+        def __init__(self) -> None:
             self.sortedlist = sortedcontainers.SortedList(key=lambda x: x.fscore)
 
         def push(self, item: SNType) -> None:
             item.in_openset = True
             self.sortedlist.add(item)
 
         def pop(self) -> SNType:
             item = self.sortedlist.pop(0)
             item.in_openset = False
             return item
 
-        def remove(self, item: SNType):
+        def remove(self, item: SNType) -> None:
             self.sortedlist.remove(item)
             item.in_openset = False
 
+        def __len__(self) -> int:
+            return len(self.sortedlist)
+
 ################################################################################*
 
 class AStar(ABC, Generic[T]):
     __slots__ = ()
 
     @abstractmethod
     def heuristic_cost_estimate(self, current: T, goal: T) -> float:
```

## Comparing `astar-0.98.dist-info/LICENSE` & `astar-0.99.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `astar-0.98.dist-info/METADATA` & `astar-0.99.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astar
-Version: 0.98
+Version: 0.99
 Summary: generic A-Star path searching algorithm
 Home-page: https://github.com/jrialland/python-astar
 License: BSD
 Author: J Rialland
 Author-email: julien.rialland@gmail.com
 Requires-Python: >=3.8,<4.0.0
 Classifier: Intended Audience :: Developers
```

