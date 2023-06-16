# Comparing `tmp/mykit-2.0.3.tar.gz` & `tmp/mykit-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-sl_442b4/mykit-2.0.3.tar", last modified: Fri Jun 16 07:29:58 2023, max compression
+gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-1_d_1_xn/mykit-2.0.4.tar", last modified: Fri Jun 16 13:06:15 2023, max compression
```

## Comparing `mykit-2.0.3.tar` & `mykit-2.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-16 07:29:33.000000 mykit-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-16 07:29:58.000000 mykit-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-16 07:29:33.000000 mykit-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/app/
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/app/complex/
--rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/complex/biplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    17112 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/complex/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    27007 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/slider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/kit/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/kit/fast_visualizations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/kit/fast_visualizations/static/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/fast_visualizations/static/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/kit/keycrate/
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/keycrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/kit/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/neuralnet/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/neuralnet/genetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-16 07:29:33.000000 mykit-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 07:29:58.000000 mykit-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 07:29:33.000000 mykit-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-16 13:05:51.000000 mykit-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-16 13:06:15.000000 mykit-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-16 13:05:51.000000 mykit-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/app/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/complex/biplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17112 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/complex/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27032 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/kit/fast_visualizations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/kit/fast_visualizations/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/fast_visualizations/static/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/kit/keycrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/keycrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/kit/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/neuralnet/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/neuralnet/genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-16 13:05:51.000000 mykit-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 13:06:15.000000 mykit-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 13:05:51.000000 mykit-2.0.4/setup.py
```

### Comparing `mykit-2.0.3/LICENSE` & `mykit-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/PKG-INFO` & `mykit-2.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -25,14 +25,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # myKit
 
 Python utility toolkit.
 
+The aim of this project is to understand how things work by building them from the ground up, while also providing a lightweight version of something that already exists out there.
+
+<!-- reminder: use this link (don't use relative path to the one in the repo) to be able to display the banner on PyPI -->
 ![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230613-mykit-banner-fhd.png)
 
 [![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 
 ## Installation
@@ -58,14 +61,16 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 2.0.4 (June 16, 2023):
+    - Now `move` method of `Button`, `Label`, `_Slider` and will return self
 - 2.0.3 (June 16, 2023):
     - Now `.app.complex.plot.Plot` and `.app.complex.plot.Biplot` can be used even if no points is specified
     - Added `add_background_processes` to `.app.App`
 - 2.0.2 (June 14, 2023):
     - finished updating all type hints
     - Added visibility functionality to `/app/complex/plot.py`
 - 2.0.1 (June 14, 2023):
```

### Comparing `mykit-2.0.3/README.md` & `mykit-2.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # myKit
 
 Python utility toolkit.
 
+The aim of this project is to understand how things work by building them from the ground up, while also providing a lightweight version of something that already exists out there.
+
+<!-- reminder: use this link (don't use relative path to the one in the repo) to be able to display the banner on PyPI -->
 ![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230613-mykit-banner-fhd.png)
 
 [![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 
 ## Installation
@@ -31,14 +34,16 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 2.0.4 (June 16, 2023):
+    - Now `move` method of `Button`, `Label`, `_Slider` and will return self
 - 2.0.3 (June 16, 2023):
     - Now `.app.complex.plot.Plot` and `.app.complex.plot.Biplot` can be used even if no points is specified
     - Added `add_background_processes` to `.app.App`
 - 2.0.2 (June 14, 2023):
     - finished updating all type hints
     - Added visibility functionality to `/app/complex/plot.py`
 - 2.0.1 (June 14, 2023):
```

### Comparing `mykit-2.0.3/mykit/__main__.py` & `mykit-2.0.4/mykit/__main__.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/app/__init__.py` & `mykit-2.0.4/mykit/app/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/app/arrow.py` & `mykit-2.0.4/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/app/button.py` & `mykit-2.0.4/mykit/app/button.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,21 +354,22 @@
 
     def move(
         self,
         x: int,
         y: int,
         /,
         anchor: _Optional[_Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
-    ) -> None:
+    ) -> 'Button':
         """If `anchor = None`, the current anchor will be used."""
         self.x = x
         self.y = y
         if anchor is not None:
             self.anchor = anchor
         self._redraw()
+        return self
 
     @staticmethod
     def move_by_id(
         id: str,
         x: int,
         y: int,
         /,
```

### Comparing `mykit-2.0.3/mykit/app/complex/biplot.py` & `mykit-2.0.4/mykit/app/complex/biplot.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/app/complex/plot.py` & `mykit-2.0.4/mykit/app/complex/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/app/label.py` & `mykit-2.0.4/mykit/app/label.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,27 +220,28 @@
 
     @staticmethod
     def get_anchor_loc_by_id(id: str, anchor: _Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'], /) -> _Tuple[int, int]:
         return Label.labels[id].get_anchor_loc(anchor)
 
     
     def move(
-            self,
-            x: int,
-            y: int,
-            /,
-            anchor: _Optional[_Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
-    ) -> None:
+        self,
+        x: int,
+        y: int,
+        /,
+        anchor: _Optional[_Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
+    ) -> 'Label':
         """If `anchor = None`, the current anchor will be used."""
         self.x = x
         self.y = y
         if anchor is not None:
             self.anchor = anchor
         # self.label.place(x=x, y=y, anchor=anchor)  # reminder: don't do this because `anchor` could be `None`
         self.label.place(x=x, y=y, anchor=self.anchor)
+        return self
 
     @staticmethod
     def move_by_id(
         id: str,
         x: int,
         y: int,
         /,
```

### Comparing `mykit-2.0.3/mykit/app/slider.py` & `mykit-2.0.4/mykit/app/slider.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,21 +334,22 @@
 
     def move(
         self,
         x: int,
         y: int,
         /,
         anchor: _Optional[_Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
-    ) -> None:
+    ) -> '_Slider':
         """If `anchor = None`, the current anchor will be used."""
         self.x = x
         self.y = y
         if anchor is not None:
             self.anchor = anchor
         self._redraw()
+        return self
 
     @staticmethod
     def move_by_id(
         id: str,
         x: int,
         y: int,
         /,
```

### Comparing `mykit-2.0.3/mykit/kit/color.py` & `mykit-2.0.4/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/kit/fast_visualizations/static/plot.py` & `mykit-2.0.4/mykit/kit/fast_visualizations/static/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/kit/ffmpeg.py` & `mykit-2.0.4/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/kit/keycrate/__init__.py` & `mykit-2.0.4/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/kit/math.py` & `mykit-2.0.4/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/kit/neuralnet/dense.py` & `mykit-2.0.4/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/kit/neuralnet/genetic.py` & `mykit-2.0.4/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/kit/noise.py` & `mykit-2.0.4/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/kit/path.py` & `mykit-2.0.4/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/kit/time.py` & `mykit-2.0.4/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit/kit/utils.py` & `mykit-2.0.4/mykit/kit/utils.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/mykit.egg-info/PKG-INFO` & `mykit-2.0.4/mykit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -25,14 +25,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # myKit
 
 Python utility toolkit.
 
+The aim of this project is to understand how things work by building them from the ground up, while also providing a lightweight version of something that already exists out there.
+
+<!-- reminder: use this link (don't use relative path to the one in the repo) to be able to display the banner on PyPI -->
 ![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230613-mykit-banner-fhd.png)
 
 [![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 
 ## Installation
@@ -58,14 +61,16 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 2.0.4 (June 16, 2023):
+    - Now `move` method of `Button`, `Label`, `_Slider` and will return self
 - 2.0.3 (June 16, 2023):
     - Now `.app.complex.plot.Plot` and `.app.complex.plot.Biplot` can be used even if no points is specified
     - Added `add_background_processes` to `.app.App`
 - 2.0.2 (June 14, 2023):
     - finished updating all type hints
     - Added visibility functionality to `/app/complex/plot.py`
 - 2.0.1 (June 14, 2023):
```

### Comparing `mykit-2.0.3/mykit.egg-info/SOURCES.txt` & `mykit-2.0.4/mykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mykit-2.0.3/pyproject.toml` & `mykit-2.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "2.0.3"
+version = "2.0.4"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

