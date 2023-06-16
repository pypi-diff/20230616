# Comparing `tmp/mykit-2.0.2.tar.gz` & `tmp/mykit-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-87idpf5o/mykit-2.0.2.tar", last modified: Wed Jun 14 07:07:29 2023, max compression
+gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-sl_442b4/mykit-2.0.3.tar", last modified: Fri Jun 16 07:29:58 2023, max compression
```

## Comparing `mykit-2.0.2.tar` & `mykit-2.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-14 07:07:05.000000 mykit-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-14 07:07:29.000000 mykit-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-14 07:07:05.000000 mykit-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/app/
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/app/complex/
--rw-r--r--   0 runner    (1001) docker     (123)    20724 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/complex/biplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16684 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/complex/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    27007 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/app/slider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/kit/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/kit/fast_visualizations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/kit/fast_visualizations/static/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/fast_visualizations/static/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/kit/keycrate/
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/keycrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit/kit/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/neuralnet/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/neuralnet/genetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-14 07:07:05.000000 mykit-2.0.2/mykit/kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 07:07:29.000000 mykit-2.0.2/mykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-14 07:07:05.000000 mykit-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-14 07:07:29.000000 mykit-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-14 07:07:05.000000 mykit-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-16 07:29:33.000000 mykit-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-16 07:29:58.000000 mykit-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-16 07:29:33.000000 mykit-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/app/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/complex/biplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17112 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/complex/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27007 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/app/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/kit/fast_visualizations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/kit/fast_visualizations/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/fast_visualizations/static/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/kit/keycrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/keycrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit/kit/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/neuralnet/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/neuralnet/genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-16 07:29:33.000000 mykit-2.0.3/mykit/kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 07:29:58.000000 mykit-2.0.3/mykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-16 07:29:33.000000 mykit-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 07:29:58.000000 mykit-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 07:29:33.000000 mykit-2.0.3/setup.py
```

### Comparing `mykit-2.0.2/LICENSE` & `mykit-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/PKG-INFO` & `mykit-2.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -58,14 +58,17 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 2.0.3 (June 16, 2023):
+    - Now `.app.complex.plot.Plot` and `.app.complex.plot.Biplot` can be used even if no points is specified
+    - Added `add_background_processes` to `.app.App`
 - 2.0.2 (June 14, 2023):
     - finished updating all type hints
     - Added visibility functionality to `/app/complex/plot.py`
 - 2.0.1 (June 14, 2023):
     - Updated all type hints to make them work on Python 3.8 and 3.9
     - Added visibility functionality to `/app/complex/biplot.py`
 - 2.0.0 (June 13, 2023):
```

### Comparing `mykit-2.0.2/README.md` & `mykit-2.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 2.0.3 (June 16, 2023):
+    - Now `.app.complex.plot.Plot` and `.app.complex.plot.Biplot` can be used even if no points is specified
+    - Added `add_background_processes` to `.app.App`
 - 2.0.2 (June 14, 2023):
     - finished updating all type hints
     - Added visibility functionality to `/app/complex/plot.py`
 - 2.0.1 (June 14, 2023):
     - Updated all type hints to make them work on Python 3.8 and 3.9
     - Added visibility functionality to `/app/complex/biplot.py`
 - 2.0.0 (June 13, 2023):
```

### Comparing `mykit-2.0.2/mykit/__main__.py` & `mykit-2.0.3/mykit/__main__.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/app/__init__.py` & `mykit-2.0.3/mykit/app/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -44,16 +44,18 @@
 
 
         ## <runtime>
         self._left_mouse_press = []
         self._left_mouse_hold = []
         self._left_mouse_release = []
 
-        self._setup = None
-        self._teardown = None
+        self._background_processes = {}
+
+        self._setup = []
+        self._teardown = []
         ## </runtime>
 
     def listen(self, to: str, do: _Callable[[_tk.Event], None]):
         """
         Add event listener.
 
         ---
@@ -69,14 +71,24 @@
             self._left_mouse_press.append(do)
         elif to == 'left-mouse-hold':
             self._left_mouse_hold.append(do)
         elif to == 'left-mouse-release':
             self._left_mouse_release.append(do)
         else:
             ValueError(f'Invalid event: {repr(to)}.')
+    
+    def add_background_processes(self, every: int, do: _Callable[[], None]) -> None:
+        """
+        Execute `do` every `every` milliseconds.
+        The first execution occurs immediately after the app runs.
+        """
+        if every in self._background_processes:
+            self._background_processes[every].append(do)
+        else:
+            self._background_processes[every] = [do]
 
     def setup(self, funcs: _List[_Callable[[], None]]):
         self._setup = funcs
 
     def teardown(self, funcs: _List[_Callable[[], None]]):
         self._teardown = funcs
 
@@ -120,31 +132,39 @@
 
         self.root.bind('<Escape>', lambda e: self.root.destroy())
 
         ## </listeners>
 
 
         ## <background processes>
-        
+
+        ## internal
         def repeat50():
             _Button.hover_listener()
             _Slider.hover_listener()
             self.root.after(50, repeat50)
-        repeat50()
+        # self.root.after(50, repeat50)  # start after 50ms
+        repeat50()  # start immediately
+
+        ## users
+        def setup_background_processes():
+            def wrapper(dur, funcs):
+                def inner():
+                    for fn in funcs: fn()
+                    self.root.after(dur, inner)
+                return inner
+            for dur, funcs in self._background_processes.items():
+                fn = wrapper(dur, funcs)
+                fn()  # start immediately
+        setup_background_processes()
         
         ## </background processes>
 
 
         ## setup
-        if self._setup is not None:
-            for fn in self._setup:
-                fn()
-
+        for fn in self._setup: fn()
 
         ## run
         self.root.mainloop()
 
-
         ## teardown
-        if self._teardown is not None:
-            for fn in self._teardown:
-                fn()
+        for fn in self._teardown: fn()
```

### Comparing `mykit-2.0.2/mykit/app/arrow.py` & `mykit-2.0.3/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/app/button.py` & `mykit-2.0.3/mykit/app/button.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/app/complex/biplot.py` & `mykit-2.0.3/mykit/app/complex/biplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 class Biplot(_Rt):
 
     biplots: _Dict[str, 'Biplot'] = {}
     biplot_tags: _Dict[str, _List['Biplot']] = {}
 
     def __init__(
         self,
-        points1: _List[_Tuple[float, float]],
-        points2: _List[_Tuple[float, float]],
-        /,
+        points1: _List[_Tuple[float, float]] = [],
+        points2: _List[_Tuple[float, float]] = [],
+
         xmin: _Optional[float] = None,
         xmax: _Optional[float] = None,
         ymin: _Optional[float] = None,
         ymax: _Optional[float] = None,
 
         width: int = 300,
         height: int = 200,
@@ -89,18 +89,20 @@
 
         visible: bool = True,
 
         id: _Optional[str] = None,
         tags: _Optional[_Union[str, _List[str]]] = None,
     ):
         """
-        To display this graph, there should be a minimum of 2 pairs of points in `points`.
+        Please ensure that `points1` and `points2` always have the same length.
+        The graph can be displayed without any given points,
+        but in order to show the plot, two points need to be specified.
 
         ---
-
+        
         ## Params
         - `xrange`: if `None` -> using the x-range from `points`
         - `yrange`: if `None` -> using the y-range from `points`
         """
 
         if Biplot.page is None:
             raise AssertionError('App has not been initialized.')
@@ -211,14 +213,19 @@
 
         ## init
         self._redraw()
 
     def _redraw(self):
         """redraw the entire graph"""
 
+        ## 2 points need to be specified in order to draw the graph
+        if len(self.points1) < 3:
+            self.points1 = [(0, 0), (1, 0)]
+            self.points2 = [(0, 0), (1, 0)]
+
         x_values = [p[0] for p in self.points1]
         if self.xmin is None:
             XMIN = min(x_values)
         else:
             XMIN = self.xmin
         if self.xmax is None:
             XMAX = max(x_values)
@@ -422,19 +429,26 @@
             )
 
     def redraw_plot(self, points1: _List[_Tuple[float, float]], points2: _List[_Tuple[float, float]], /) -> None:
         """
         Redraws the plot and updates the tick labels with a new set of given points.
         """
 
+        ## reminder: to optimize things, only redraw the necessary part
+        ##           so the code below is duplicated from `_redraw`.
+        ##           it's redundant, but currently the easiest way to
+        ##           achieve the desired functionality
+
         self.points1 = points1
         self.points2 = points2
 
-        ## The code below is duplicated from `_redraw`. While it may seem redundant,
-        ## it's currently the easiest way to achieve the desired functionality.
+        ## 2 points need to be specified in order to draw the graph
+        if len(self.points1) < 3:
+            self.points1 = [(0, 0), (1, 0)]
+            self.points2 = [(0, 0), (1, 0)]
 
         x_values = [p[0] for p in self.points1]
         if self.xmin is None:
             XMIN = min(x_values)
         else:
             XMIN = self.xmin
         if self.xmax is None:
```

### Comparing `mykit-2.0.2/mykit/app/complex/plot.py` & `mykit-2.0.3/mykit/app/complex/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 class Plot(_Rt):
 
     plots: _Dict[str, 'Plot'] = {}
     plot_tags: _Dict[str, _List['Plot']] = {}
 
     def __init__(
         self,
-        points: _List[_Tuple[float, float]],
-        /,
+        points: _List[_Tuple[float, float]] = [],
+
         xmin: _Optional[float] = None,
         xmax: _Optional[float] = None,
         ymin: _Optional[float] = None,
         ymax: _Optional[float] = None,
 
         width: int = 300,
         height: int = 200,
@@ -76,15 +76,16 @@
 
         visible: bool = True,
 
         id: _Optional[str] = None,
         tags: _Optional[_Union[str, _List[str]]] = None,
     ):
         """
-        To display this graph, there should be a minimum of 2 pairs of points in `points`.
+        The graph can be displayed without any given points,
+        but in order to show the plot, two points need to be specified.
 
         ---
 
         ## Params
         - `xrange`: if `None` -> using the x-range from `points`
         - `yrange`: if `None` -> using the y-range from `points`
         """
@@ -185,14 +186,18 @@
 
         ## init
         self._redraw()
 
     def _redraw(self):
         """redraw the entire graph"""
 
+        ## 2 points need to be specified in order to draw the graph
+        if len(self.points) < 3:
+            self.points = [(0, 0), (1, 0)]
+
         x_values = [p[0] for p in self.points]
         if self.xmin is None:
             XMIN = min(x_values)
         else:
             XMIN = self.xmin
         if self.xmax is None:
             XMAX = max(x_values)
@@ -355,18 +360,24 @@
                 )
     
     def redraw_plot(self, points: _List[_Tuple[float, float]], /) -> None:
         """
         Redraws the plot and updates the tick labels with a new set of given `points`.
         """
 
+        ## reminder: to optimize things, only redraw the necessary part
+        ##           so the code below is duplicated from `_redraw`.
+        ##           it's redundant, but currently the easiest way to
+        ##           achieve the desired functionality
+
         self.points = points
 
-        ## The code below is duplicated from `_redraw`. While it may seem redundant,
-        ## it's currently the easiest way to achieve the desired functionality.
+        ## 2 points need to be specified in order to draw the graph
+        if len(self.points) < 3:
+            self.points = [(0, 0), (1, 0)]
 
         x_values = [p[0] for p in self.points]
         if self.xmin is None:
             XMIN = min(x_values)
         else:
             XMIN = self.xmin
         if self.xmax is None:
```

### Comparing `mykit-2.0.2/mykit/app/label.py` & `mykit-2.0.3/mykit/app/label.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/app/slider.py` & `mykit-2.0.3/mykit/app/slider.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/kit/color.py` & `mykit-2.0.3/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/kit/fast_visualizations/static/plot.py` & `mykit-2.0.3/mykit/kit/fast_visualizations/static/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/kit/ffmpeg.py` & `mykit-2.0.3/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/kit/keycrate/__init__.py` & `mykit-2.0.3/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/kit/math.py` & `mykit-2.0.3/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/kit/neuralnet/dense.py` & `mykit-2.0.3/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/kit/neuralnet/genetic.py` & `mykit-2.0.3/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/kit/noise.py` & `mykit-2.0.3/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/kit/path.py` & `mykit-2.0.3/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/kit/time.py` & `mykit-2.0.3/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit/kit/utils.py` & `mykit-2.0.3/mykit/kit/utils.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/mykit.egg-info/PKG-INFO` & `mykit-2.0.3/mykit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -58,14 +58,17 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 2.0.3 (June 16, 2023):
+    - Now `.app.complex.plot.Plot` and `.app.complex.plot.Biplot` can be used even if no points is specified
+    - Added `add_background_processes` to `.app.App`
 - 2.0.2 (June 14, 2023):
     - finished updating all type hints
     - Added visibility functionality to `/app/complex/plot.py`
 - 2.0.1 (June 14, 2023):
     - Updated all type hints to make them work on Python 3.8 and 3.9
     - Added visibility functionality to `/app/complex/biplot.py`
 - 2.0.0 (June 13, 2023):
```

### Comparing `mykit-2.0.2/mykit.egg-info/SOURCES.txt` & `mykit-2.0.3/mykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mykit-2.0.2/pyproject.toml` & `mykit-2.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "2.0.2"
+version = "2.0.3"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

