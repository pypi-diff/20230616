# Comparing `tmp/mecode_viewer-0.1.13.tar.gz` & `tmp/mecode_viewer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecode_viewer-0.1.13.tar", last modified: Thu Jun 15 16:18:06 2023, max compression
+gzip compressed data, was "mecode_viewer-0.2.0.tar", last modified: Fri Jun 16 05:04:14 2023, max compression
```

## Comparing `mecode_viewer-0.1.13.tar` & `mecode_viewer-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-15 16:18:06.426093 mecode_viewer-0.1.13/
--rw-r--r--   0 rtelles    (502) staff       (20)     3602 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/CONTRIBUTING.rst
--rw-r--r--   0 rtelles    (502) staff       (20)       89 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/HISTORY.rst
--rw-r--r--   0 rtelles    (502) staff       (20)     1073 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/LICENSE
--rw-r--r--   0 rtelles    (502) staff       (20)      242 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/MANIFEST.in
--rw-r--r--   0 rtelles    (502) staff       (20)     2062 2023-06-15 16:18:06.426244 mecode_viewer-0.1.13/PKG-INFO
--rw-r--r--   0 rtelles    (502) staff       (20)     1261 2023-06-13 00:32:44.000000 mecode_viewer-0.1.13/README.rst
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-15 16:18:06.403557 mecode_viewer-0.1.13/docs/
--rw-r--r--   0 rtelles    (502) staff       (20)      614 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/docs/Makefile
--rwxr-xr-x   0 rtelles    (502) staff       (20)     4862 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/docs/conf.py
--rw-r--r--   0 rtelles    (502) staff       (20)       33 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/docs/contributing.rst
--rw-r--r--   0 rtelles    (502) staff       (20)       28 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/docs/history.rst
--rw-r--r--   0 rtelles    (502) staff       (20)      299 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/docs/index.rst
--rw-r--r--   0 rtelles    (502) staff       (20)     1170 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/docs/installation.rst
--rw-r--r--   0 rtelles    (502) staff       (20)      811 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/docs/make.bat
--rw-r--r--   0 rtelles    (502) staff       (20)       27 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/docs/readme.rst
--rw-r--r--   0 rtelles    (502) staff       (20)       81 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/docs/usage.rst
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-15 16:18:06.406560 mecode_viewer-0.1.13/mecode_viewer/
--rw-r--r--   0 rtelles    (502) staff       (20)      165 2023-05-31 15:53:14.000000 mecode_viewer-0.1.13/mecode_viewer/__init__.py
--rw-r--r--   0 rtelles    (502) staff       (20)      454 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/mecode_viewer/cli.py
--rw-r--r--   0 rtelles    (502) staff       (20)    20419 2023-06-15 16:16:41.000000 mecode_viewer-0.1.13/mecode_viewer/mecode_viewer.py
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-15 16:18:06.424769 mecode_viewer-0.1.13/mecode_viewer.egg-info/
--rw-r--r--   0 rtelles    (502) staff       (20)     2062 2023-06-15 16:18:05.000000 mecode_viewer-0.1.13/mecode_viewer.egg-info/PKG-INFO
--rw-r--r--   0 rtelles    (502) staff       (20)      610 2023-06-15 16:18:05.000000 mecode_viewer-0.1.13/mecode_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 rtelles    (502) staff       (20)        1 2023-06-15 16:18:05.000000 mecode_viewer-0.1.13/mecode_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 rtelles    (502) staff       (20)       57 2023-06-15 16:18:05.000000 mecode_viewer-0.1.13/mecode_viewer.egg-info/entry_points.txt
--rw-r--r--   0 rtelles    (502) staff       (20)        1 2023-06-12 21:06:47.000000 mecode_viewer-0.1.13/mecode_viewer.egg-info/not-zip-safe
--rw-r--r--   0 rtelles    (502) staff       (20)       39 2023-06-15 16:18:05.000000 mecode_viewer-0.1.13/mecode_viewer.egg-info/requires.txt
--rw-r--r--   0 rtelles    (502) staff       (20)       14 2023-06-15 16:18:05.000000 mecode_viewer-0.1.13/mecode_viewer.egg-info/top_level.txt
--rw-r--r--   0 rtelles    (502) staff       (20)      385 2023-06-15 16:18:06.427115 mecode_viewer-0.1.13/setup.cfg
--rw-r--r--   0 rtelles    (502) staff       (20)     1483 2023-06-15 16:16:48.000000 mecode_viewer-0.1.13/setup.py
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-15 16:18:06.425771 mecode_viewer-0.1.13/tests/
--rw-r--r--   0 rtelles    (502) staff       (20)       43 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/tests/__init__.py
--rw-r--r--   0 rtelles    (502) staff       (20)      417 2022-11-21 22:26:04.000000 mecode_viewer-0.1.13/tests/test_mecode_viewer.py
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-16 05:04:14.738235 mecode_viewer-0.2.0/
+-rw-r--r--   0 rtelles    (502) staff       (20)     3602 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)       89 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/HISTORY.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)     1073 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/LICENSE
+-rw-r--r--   0 rtelles    (502) staff       (20)      242 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/MANIFEST.in
+-rw-r--r--   0 rtelles    (502) staff       (20)     2061 2023-06-16 05:04:14.738402 mecode_viewer-0.2.0/PKG-INFO
+-rw-r--r--   0 rtelles    (502) staff       (20)     1261 2023-06-13 00:32:44.000000 mecode_viewer-0.2.0/README.rst
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-16 05:04:14.726642 mecode_viewer-0.2.0/docs/
+-rw-r--r--   0 rtelles    (502) staff       (20)      614 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/Makefile
+-rwxr-xr-x   0 rtelles    (502) staff       (20)     4862 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/conf.py
+-rw-r--r--   0 rtelles    (502) staff       (20)       33 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/contributing.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)       28 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/history.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)      299 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/index.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)     1170 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/installation.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)      811 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/make.bat
+-rw-r--r--   0 rtelles    (502) staff       (20)       27 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/readme.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)       81 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/usage.rst
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-16 05:04:14.728497 mecode_viewer-0.2.0/mecode_viewer/
+-rw-r--r--   0 rtelles    (502) staff       (20)      165 2023-06-16 05:01:44.000000 mecode_viewer-0.2.0/mecode_viewer/__init__.py
+-rw-r--r--   0 rtelles    (502) staff       (20)      454 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/mecode_viewer/cli.py
+-rw-r--r--   0 rtelles    (502) staff       (20)    21238 2023-06-16 04:54:30.000000 mecode_viewer-0.2.0/mecode_viewer/mecode_viewer.py
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-16 05:04:14.736636 mecode_viewer-0.2.0/mecode_viewer.egg-info/
+-rw-r--r--   0 rtelles    (502) staff       (20)     2061 2023-06-16 05:04:14.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 rtelles    (502) staff       (20)      610 2023-06-16 05:04:14.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)        1 2023-06-16 05:04:14.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)       57 2023-06-16 05:04:14.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)        1 2023-06-12 21:06:47.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/not-zip-safe
+-rw-r--r--   0 rtelles    (502) staff       (20)       39 2023-06-16 05:04:14.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/requires.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)       14 2023-06-16 05:04:14.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/top_level.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)      385 2023-06-16 05:04:14.739132 mecode_viewer-0.2.0/setup.cfg
+-rw-r--r--   0 rtelles    (502) staff       (20)     1482 2023-06-16 05:01:44.000000 mecode_viewer-0.2.0/setup.py
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-16 05:04:14.737818 mecode_viewer-0.2.0/tests/
+-rw-r--r--   0 rtelles    (502) staff       (20)       43 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/tests/__init__.py
+-rw-r--r--   0 rtelles    (502) staff       (20)      417 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/tests/test_mecode_viewer.py
```

### Comparing `mecode_viewer-0.1.13/CONTRIBUTING.rst` & `mecode_viewer-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.13/LICENSE` & `mecode_viewer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.13/PKG-INFO` & `mecode_viewer-0.2.0/mecode_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mecode_viewer
-Version: 0.1.13
+Name: mecode-viewer
+Version: 0.2.0
 Summary: Simple GCode Viewer
 Home-page: https://github.com/rtellez700/mecode_viewer
 Author: Rodrigo Telles
 Author-email: rtelles@g.harvard.edu
 License: MIT license
 Keywords: mecode_viewer
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mecode_viewer-0.1.13/README.rst` & `mecode_viewer-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.13/docs/Makefile` & `mecode_viewer-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.13/docs/conf.py` & `mecode_viewer-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.13/docs/installation.rst` & `mecode_viewer-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.13/docs/make.bat` & `mecode_viewer-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.13/mecode_viewer/mecode_viewer.py` & `mecode_viewer-0.2.0/mecode_viewer/mecode_viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,33 @@
 from os.path import isfile
 from typing import Mapping, List, Optional, Dict
 from mpl_toolkits import mplot3d
 import numpy as np
 import matplotlib.pyplot as plt
 from gcode_helpers import get_accel_decel, get_print_mode, get_pressure_config, get_print_move, are_we_printing
 import numpy as np
-from typing import List, Optional
+from typing import List, Optional, Union, Tuple
+from mpl_toolkits.mplot3d.art3d import Line3DCollection
 
-def mecode_viewer(file_name: str, rel_mode: bool=False, animation: bool=False, verbose: bool=False, raw_gcode: List[str]=None, **kwargs) -> Optional[List[Dict]]:
+def mecode_viewer(file_name: str,
+                  rel_mode: bool=False,
+                  animation: bool=False,
+                  verbose: bool=False,
+                  raw_gcode: List[str]=None,
+                  origin: Union[List[Union[int, float]], Tuple[Union[int, float]]]=(0,0,0),
+                  **kwargs) -> Optional[List[Dict]]:
     '''Visualize gcode file
 
         Args:
             file_name (str): name of gcode file
             rel_mode (bool): True if relative coordinates, False if absolute coordinates
             animation (bool): True for 3D animation, False for static matplotlib figure
             verbose (bool): If True, will return print history as a list of dict's
             raw_gcode (List[str]): Can provide list of gcode str commands in lieu of file_name
+            origin (Union[List[Union[int, float]], Tuple[Union[int, float]]]): Specify origin as initial starting point
 
         Returns:
             Optional[List[Dict]]: If verbose is true, will return print history
 
         Examples:
             >>> mecode_viewer(file_name='gcode_file.pgm') # simplest case
 
@@ -45,15 +53,15 @@
         {
             'REL_MODE': REL_MODE,
             'ACCEL' : ACCEL_RATE,
             'DECEL' : DECEL_RATE,
             'P' : PRESSURE,
             'P_COM_PORT': P_COM_PORT,
             'PRINTING': False,
-            'COORDS': (0,0,0.7),
+            'COORDS': origin,
             'PRINT_SPEED': 0
         }
     ]
 
     move_counter = 1
 
     if raw_gcode is not None:
@@ -105,62 +113,75 @@
         animation(history, **kwargs)
     else:
         raise ValueError("Invalid plotting backend! Choose one of mayavi or matplotlib or matplotlib2d or vpython.")
     
     if verbose:
         return history
 
+
 def plot3d(history: List[dict], outfile:Optional[str] =None, mecode:Optional[bool] =False, **kwargs) -> None:
     '''Generates a 3D matplotlib figure.
 
         Args:
             - history (List[dict]): List of printing, speed, color, extrusion, etc... history
             - outfile (str): If specified, will save 3D matplotlib figure locally at `outfile`
             - mecode (bool): If False will not attempt to calculate absolute coordinates from relative points. Mecode by default does this conversion for us
 
     
     '''
     fig = plt.figure(dpi=150)
     ax = plt.axes(projection='3d')
 
-    x_pos, y_pos, z_pos = history[0]['COORDS']
+    segs = []
 
-    for j, h in enumerate(history[1:]):
-        x_0, y_0, z_0 = history[j-1]['COORDS']
-        x_0 = 0 if x_0 is None else x_0
-        y_0 = 0 if y_0 is None else y_0
-        z_0 = 0 if z_0 is None else z_0
-
-        x_f, y_f, z_f = h['COORDS']
-        x_f = 0 if x_f is None else x_f
-        y_f = 0 if y_f is None else y_f
-        z_f = 0 if z_f is None else z_f
-        
-        fmt = {
-            'ls': '-' if h['PRINTING'] else ':',
-            'c': (0,0,1,0.6) if h['PRINTING'] else 'k',
-            'lw': .5 if h['PRINTING'] else 1
-        }
-        if h['REL_MODE'] and not mecode:
-            x_pts = np.round(np.array([x_0, x_f]) + x_pos, 6)
-            y_pts = np.round(np.array([y_0, y_f]) + y_pos, 6)
-            z_pts = np.round(np.array([z_0, z_f]) + z_pos, 6)
+    # origin
+    x_pts = [history[0]['COORDS'][0]] #[0]
+    y_pts = [history[0]['COORDS'][1]] #[0]
+    z_pts = [history[0]['COORDS'][2]] #[0]
+
+    # for u, v in zip(history[:-1], history[1:]):
+    for j, h in enumerate(history[1:], 1):
+        if h['REL_MODE']:
+            x_pts.append(x_pts[-1] + h['COORDS'][0])
+            y_pts.append(y_pts[-1] + h['COORDS'][1])
+            z_pts.append(z_pts[-1] + h['COORDS'][2])
+
+            segs.append([
+                (x_pts[-2], y_pts[-2], z_pts[-2]),
+                (x_pts[-1], y_pts[-1], z_pts[-1])
+            ])
 
-            x_pos, y_pos, z_pos = x_pos+x_f, y_pos+y_f, z_pos+z_f
         else:
-            x_pts = [x_0, x_f]
-            y_pts = [y_0, y_f]
-            z_pts = [z_0, z_f]
-        
-        # if h['PRINTING']:
-        ax.plot3D(x_pts, y_pts, z_pts, **fmt)
+            x_pts.append(h['COORDS'][0])
+            y_pts.append(h['COORDS'][1])
+            z_pts.append(h['COORDS'][2])
+
+            segs.append(
+                [
+                    (history[j-1]['COORDS'][0], history[j-1]['COORDS'][1], history[j-1]['COORDS'][2]),
+                    (h['COORDS'][0], h['COORDS'][1], h['COORDS'][2])
+                ]
+            )
+
+    linestyles = ['-' if h['PRINTING'] else ':' for h in history[1:]]
+    colors = [(0,0,1,0.6) if h['PRINTING'] else (0,0,0) for h in history[1:]]
+    linewidths = [0.5 if h['PRINTING'] else 1 for h in history[1:]]
+
+    line_segments = Line3DCollection(segs,
+                                     linewidths=linewidths,
+                                     colors=colors,
+                                     linestyles=linestyles
+                                     )
+    
+    ax.add_collection3d(line_segments)
 
     position_history = [d['COORDS'] for d in history]
 
-    X, Y, Z = np.vstack(position_history)[:,0], np.vstack(position_history)[:,1], np.vstack(position_history)[:,2]
+    # X, Y, Z = np.vstack(position_history)[:,0], np.vstack(position_history)[:,1], np.vstack(position_history)[:,2]
+    X, Y, Z = np.vstack([x_pts, y_pts, z_pts])
 
     # Hack to keep 3D plot's aspect ratio square. See SO answer:
     # http://stackoverflow.com/questions/13685386
     max_range = np.array([X.max()-X.min(),
                             Y.max()-Y.min(),
                             Z.max()-Z.min()]).max() / 2.0
 
@@ -175,14 +196,15 @@
     ax.set_zlabel("Z")
 
     if outfile == None:
         plt.show()
     else:
         fig.savefig(outfile, dpi=500)
 
+
 def animation(history: List[dict],
               outfile:Optional[str] =None,
               hide_travel=False,color_on=True,
               nozzle_cam=False,
               fast_forward = 3,
               framerate = 60,
               nozzle_dims=[1.0,20.0],
```

### Comparing `mecode_viewer-0.1.13/mecode_viewer.egg-info/PKG-INFO` & `mecode_viewer-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mecode-viewer
-Version: 0.1.13
+Name: mecode_viewer
+Version: 0.2.0
 Summary: Simple GCode Viewer
 Home-page: https://github.com/rtellez700/mecode_viewer
 Author: Rodrigo Telles
 Author-email: rtelles@g.harvard.edu
 License: MIT license
 Keywords: mecode_viewer
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mecode_viewer-0.1.13/mecode_viewer.egg-info/SOURCES.txt` & `mecode_viewer-0.2.0/mecode_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.13/setup.py` & `mecode_viewer-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,10 +43,10 @@
     include_package_data=True,
     keywords='mecode_viewer',
     name='mecode_viewer',
     packages=find_packages(include=['mecode_viewer', 'mecode_viewer.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rtellez700/mecode_viewer',
-    version='0.1.13',
+    version='0.2.0',
     zip_safe=False,
 )
```

