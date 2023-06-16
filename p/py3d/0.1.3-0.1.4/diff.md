# Comparing `tmp/py3d-0.1.3.tar.gz` & `tmp/py3d-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.1.3.tar", last modified: Thu Jun 15 01:10:55 2023, max compression
+gzip compressed data, was "py3d-0.1.4.tar", last modified: Fri Jun 16 15:15:19 2023, max compression
```

## Comparing `py3d-0.1.3.tar` & `py3d-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 01:10:55.788986 py3d-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-15 01:10:55.788986 py3d-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-15 01:10:34.000000 py3d-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 01:10:55.784986 py3d-0.1.3/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-15 01:09:50.000000 py3d-0.1.3/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28901 2023-06-15 01:09:50.000000 py3d-0.1.3/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22729 2023-06-15 01:09:50.000000 py3d-0.1.3/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 01:10:55.788986 py3d-0.1.3/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-15 01:10:55.000000 py3d-0.1.3/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-15 01:10:55.000000 py3d-0.1.3/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 01:10:55.000000 py3d-0.1.3/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-15 01:10:55.000000 py3d-0.1.3/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-15 01:10:55.000000 py3d-0.1.3/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-15 01:10:55.788986 py3d-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-15 01:09:50.000000 py3d-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 15:15:19.218850 py3d-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-16 15:15:19.218850 py3d-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-16 15:14:54.000000 py3d-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 15:15:19.218850 py3d-0.1.4/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-16 15:14:00.000000 py3d-0.1.4/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28904 2023-06-16 15:14:00.000000 py3d-0.1.4/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22729 2023-06-16 15:14:00.000000 py3d-0.1.4/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 15:15:19.218850 py3d-0.1.4/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-16 15:15:19.000000 py3d-0.1.4/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-16 15:15:19.000000 py3d-0.1.4/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 15:15:19.000000 py3d-0.1.4/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-16 15:15:19.000000 py3d-0.1.4/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-16 15:15:19.000000 py3d-0.1.4/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 15:15:19.218850 py3d-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-16 15:14:00.000000 py3d-0.1.4/setup.py
```

### Comparing `py3d-0.1.3/PKG-INFO` & `py3d-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.3
+Version: 0.1.4
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.3/README.md` & `py3d-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.1.3/py3d/core.py` & `py3d-0.1.4/py3d/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,14 +259,31 @@
         return super().min(axis=self.ndim-2)
 
     def max(self) -> Vector:
         return super().max(axis=self.ndim-2)
 
     def diff(self, n=1) -> Vector:
         return numpy.diff(self, n, axis=self.ndim-2)
+    
+    def lerp(self, x, xp) -> Vector:
+        '''
+        linear interpolation
+        x: 1-D array, the data to be interpolated.
+        xp: 1-D array, the data to interpolate into. For example, time series.
+        '''
+        x = numpy.array(x)
+        xp = numpy.array(xp)
+        assert x.ndim <= xp.ndim == 1
+        i = numpy.searchsorted(xp, x).clip(1, len(xp)-1)
+        x0 = xp[i-1]
+        x1 = xp[i]
+        d = ((x-x0)/(x1-x0)).reshape(-1, 1)
+        f0 = self[i-1]
+        f1 = self[i]
+        return (1-d)*f0+d*f1
 
     def to_pcd(self, path, fields=""):
         w = self.shape[-1]
         pcd = self.reshape(-1, w)
         width = len(pcd)
         size = " ".join(["4"] * w)
         tp = " ".join(["F"] * w)
@@ -386,31 +403,14 @@
         return p0 + (self - p0).vector_projection(p1 - p0)
 
     def projection_on_plane(self, plane) -> numpy.ndarray:
         return self + (plane.position[:, numpy.newaxis] - self).vector_projection(
             plane.normal[:, numpy.newaxis]
         )
 
-    def lerp(self, x, xp) -> Vector3:
-        '''
-        linear interpolation
-        x: 1-D array, the data to be interpolated.
-        xp: 1-D array, the data to interpolate into. For example, time series.
-        '''
-        x = numpy.array(x)
-        xp = numpy.array(xp)
-        assert x.ndim <= xp.ndim == 1
-        i = numpy.searchsorted(xp, x).clip(1, len(xp)-1)
-        x0 = xp[i-1]
-        x1 = xp[i]
-        d = ((x-x0)/(x1-x0)).reshape(-1, 1)
-        f0 = self[i-1]
-        f1 = self[i]
-        return (1-d)*f0+d*f1
-
     def as_scaling(self) -> Transform:
         ret = Transform
         ret[..., 0, 0] = self[..., 0]
         ret[..., 1, 1] = self[..., 1]
         ret[..., 2, 2] = self[..., 2]
         return ret.view(Transform)
```

### Comparing `py3d-0.1.3/py3d/viewer.html` & `py3d-0.1.4/py3d/viewer.html`

 * *Files identical despite different names*

### Comparing `py3d-0.1.3/py3d.egg-info/PKG-INFO` & `py3d-0.1.4/py3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.3
+Version: 0.1.4
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.3/setup.py` & `py3d-0.1.4/setup.py`

 * *Files identical despite different names*

