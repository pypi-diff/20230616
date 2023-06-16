# Comparing `tmp/wongutils-0.1.1.tar.gz` & `tmp/wongutils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wongutils-0.1.1.tar", last modified: Sun Mar 26 01:49:26 2023, max compression
+gzip compressed data, was "wongutils-0.1.2.tar", last modified: Fri Jun 16 02:55:45 2023, max compression
```

## Comparing `wongutils-0.1.1.tar` & `wongutils-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 georgewong   (501) staff       (20)        0 2023-03-26 01:49:26.000000 wongutils-0.1.1/
--rw-r--r--   0 georgewong   (501) staff       (20)      213 2023-03-26 01:49:26.000000 wongutils-0.1.1/PKG-INFO
--rw-r--r--   0 georgewong   (501) staff       (20)       35 2023-03-14 02:21:36.000000 wongutils-0.1.1/README.md
--rw-r--r--   0 georgewong   (501) staff       (20)      290 2023-03-26 01:49:26.000000 wongutils-0.1.1/setup.cfg
--rw-r--r--   0 georgewong   (501) staff       (20)      298 2023-03-26 01:46:40.000000 wongutils-0.1.1/setup.py
-drwxr-xr-x   0 georgewong   (501) staff       (20)        0 2023-03-26 01:49:26.000000 wongutils-0.1.1/wongutils/
--rw-r--r--   0 georgewong   (501) staff       (20)     1102 2023-03-14 03:38:09.000000 wongutils-0.1.1/wongutils/__init__.py
-drwxr-xr-x   0 georgewong   (501) staff       (20)        0 2023-03-26 01:49:26.000000 wongutils-0.1.1/wongutils/geometry/
--rw-r--r--   0 georgewong   (501) staff       (20)     1101 2023-03-14 04:58:22.000000 wongutils-0.1.1/wongutils/geometry/__init__.py
--rw-r--r--   0 georgewong   (501) staff       (20)     4189 2023-03-25 19:38:04.000000 wongutils-0.1.1/wongutils/geometry/coordinates.py
--rw-r--r--   0 georgewong   (501) staff       (20)     4516 2023-03-25 19:21:34.000000 wongutils-0.1.1/wongutils/geometry/metrics.py
-drwxr-xr-x   0 georgewong   (501) staff       (20)        0 2023-03-26 01:49:26.000000 wongutils-0.1.1/wongutils/grmhd/
--rw-r--r--   0 georgewong   (501) staff       (20)     1101 2023-03-14 04:58:33.000000 wongutils-0.1.1/wongutils/grmhd/__init__.py
--rw-r--r--   0 georgewong   (501) staff       (20)     4547 2023-03-25 19:30:02.000000 wongutils-0.1.1/wongutils/grmhd/athenak.py
--rw-r--r--   0 georgewong   (501) staff       (20)     1101 2023-03-25 19:29:37.000000 wongutils-0.1.1/wongutils/grmhd/babel.py
--rw-r--r--   0 georgewong   (501) staff       (20)     3665 2023-03-26 01:44:08.000000 wongutils-0.1.1/wongutils/grmhd/fluids.py
--rw-r--r--   0 georgewong   (501) staff       (20)     4506 2023-03-25 17:29:58.000000 wongutils-0.1.1/wongutils/grmhd/iharm.py
-drwxr-xr-x   0 georgewong   (501) staff       (20)        0 2023-03-26 01:49:26.000000 wongutils-0.1.1/wongutils.egg-info/
--rw-r--r--   0 georgewong   (501) staff       (20)      213 2023-03-26 01:49:26.000000 wongutils-0.1.1/wongutils.egg-info/PKG-INFO
--rw-r--r--   0 georgewong   (501) staff       (20)      440 2023-03-26 01:49:26.000000 wongutils-0.1.1/wongutils.egg-info/SOURCES.txt
--rw-r--r--   0 georgewong   (501) staff       (20)        1 2023-03-26 01:49:26.000000 wongutils-0.1.1/wongutils.egg-info/dependency_links.txt
--rw-r--r--   0 georgewong   (501) staff       (20)        1 2023-03-14 02:18:26.000000 wongutils-0.1.1/wongutils.egg-info/not-zip-safe
--rw-r--r--   0 georgewong   (501) staff       (20)       10 2023-03-26 01:49:26.000000 wongutils-0.1.1/wongutils.egg-info/top_level.txt
+drwxr-xr-x   0 georgewong   (501) staff       (20)        0 2023-06-16 02:55:45.412234 wongutils-0.1.2/
+-rw-r--r--   0 georgewong   (501) staff       (20)     1071 2023-03-14 02:02:50.000000 wongutils-0.1.2/LICENSE
+-rw-r--r--   0 georgewong   (501) staff       (20)      179 2023-06-16 02:55:45.412430 wongutils-0.1.2/PKG-INFO
+-rw-r--r--   0 georgewong   (501) staff       (20)       35 2023-03-14 02:21:36.000000 wongutils-0.1.2/README.md
+-rw-r--r--   0 georgewong   (501) staff       (20)      289 2023-06-16 02:55:45.413240 wongutils-0.1.2/setup.cfg
+-rw-r--r--   0 georgewong   (501) staff       (20)      298 2023-06-16 02:51:39.000000 wongutils-0.1.2/setup.py
+drwxr-xr-x   0 georgewong   (501) staff       (20)        0 2023-06-16 02:55:45.400792 wongutils-0.1.2/wongutils/
+-rw-r--r--   0 georgewong   (501) staff       (20)     1102 2023-03-14 03:38:09.000000 wongutils-0.1.2/wongutils/__init__.py
+drwxr-xr-x   0 georgewong   (501) staff       (20)        0 2023-06-16 02:55:45.404455 wongutils-0.1.2/wongutils/geometry/
+-rw-r--r--   0 georgewong   (501) staff       (20)     1101 2023-03-14 04:58:22.000000 wongutils-0.1.2/wongutils/geometry/__init__.py
+-rw-r--r--   0 georgewong   (501) staff       (20)     4189 2023-03-25 19:38:04.000000 wongutils-0.1.2/wongutils/geometry/coordinates.py
+-rw-r--r--   0 georgewong   (501) staff       (20)     8857 2023-06-16 02:49:03.000000 wongutils-0.1.2/wongutils/geometry/metrics.py
+drwxr-xr-x   0 georgewong   (501) staff       (20)        0 2023-06-16 02:55:45.411606 wongutils-0.1.2/wongutils/grmhd/
+-rw-r--r--   0 georgewong   (501) staff       (20)     1101 2023-03-14 04:58:33.000000 wongutils-0.1.2/wongutils/grmhd/__init__.py
+-rw-r--r--   0 georgewong   (501) staff       (20)     7562 2023-04-29 02:50:46.000000 wongutils-0.1.2/wongutils/grmhd/athenak.py
+-rw-r--r--   0 georgewong   (501) staff       (20)     1101 2023-03-25 19:29:37.000000 wongutils-0.1.2/wongutils/grmhd/babel.py
+-rw-r--r--   0 georgewong   (501) staff       (20)     9110 2023-04-29 01:07:52.000000 wongutils-0.1.2/wongutils/grmhd/fluids.py
+-rw-r--r--   0 georgewong   (501) staff       (20)     1382 2023-04-29 00:05:06.000000 wongutils-0.1.2/wongutils/grmhd/grids.py
+-rw-r--r--   0 georgewong   (501) staff       (20)     6575 2023-06-16 02:49:03.000000 wongutils-0.1.2/wongutils/grmhd/iharm.py
+drwxr-xr-x   0 georgewong   (501) staff       (20)        0 2023-06-16 02:55:45.402769 wongutils-0.1.2/wongutils.egg-info/
+-rw-r--r--   0 georgewong   (501) staff       (20)      179 2023-06-16 02:55:45.000000 wongutils-0.1.2/wongutils.egg-info/PKG-INFO
+-rw-r--r--   0 georgewong   (501) staff       (20)      473 2023-06-16 02:55:45.000000 wongutils-0.1.2/wongutils.egg-info/SOURCES.txt
+-rw-r--r--   0 georgewong   (501) staff       (20)        1 2023-06-16 02:55:45.000000 wongutils-0.1.2/wongutils.egg-info/dependency_links.txt
+-rw-r--r--   0 georgewong   (501) staff       (20)        1 2023-03-14 02:18:26.000000 wongutils-0.1.2/wongutils.egg-info/not-zip-safe
+-rw-r--r--   0 georgewong   (501) staff       (20)       10 2023-06-16 02:55:45.000000 wongutils-0.1.2/wongutils.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wongutils-0.1.1/wongutils/__init__.py` & `wongutils-0.1.2/wongutils/__init__.py`

 * *Files identical despite different names*

### Comparing `wongutils-0.1.1/wongutils/geometry/__init__.py` & `wongutils-0.1.2/wongutils/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `wongutils-0.1.1/wongutils/geometry/coordinates.py` & `wongutils-0.1.2/wongutils/geometry/coordinates.py`

 * *Files identical despite different names*

### Comparing `wongutils-0.1.1/wongutils/grmhd/__init__.py` & `wongutils-0.1.2/wongutils/grmhd/__init__.py`

 * *Files identical despite different names*

### Comparing `wongutils-0.1.1/wongutils/grmhd/babel.py` & `wongutils-0.1.2/wongutils/grmhd/babel.py`

 * *Files identical despite different names*

### Comparing `wongutils-0.1.1/wongutils/grmhd/iharm.py` & `wongutils-0.1.2/wongutils/grmhd/iharm.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
 import numpy as np
 import h5py
+from wongutils.geometry import metrics
 
 
 def get_native_grid(fname, verbose=False, corners=True, array3d=False):
     """Get native grid underlying iharm-style snapshot file."""
 
     coordinate_info = get_header_coordinates(fname, verbose=verbose)
 
@@ -105,7 +106,58 @@
                 coordinate_info['poly_xt'] = poly_xt
                 coordinate_info['poly_norm'] = poly_norm
 
         else:
             raise NotImplementedError(f"unknown metric {metric}")
 
     return coordinate_info
+
+
+def load_snapshot(fname, gcov=None, gcon=None):
+    """Load fluid information from iharm-style snapshot file."""
+
+    if gcov is None:
+        coordinate_info = get_header_coordinates(fname)
+        x1, x2, x3 = get_native_grid(fname, corners=False)
+        X1, X2, X3 = np.meshgrid(x1, x2, x3, indexing='ij')
+        gcov = metrics.get_gcov_fmks_from_fmks(coordinate_info, X1, X2, X3=X3)
+
+    if gcon is None:
+        n3 = gcov.shape[2]
+        if np.allclose(gcov[:, :, 0], gcov[:, :, n3//3]) and \
+           np.allclose(gcov[:, :, 0], gcov[:, :, n3//2]):
+            gcov2d = gcov[:, :, 0, :, :]
+            gcon2d = np.linalg.inv(gcov2d)
+            gcon = np.zeros_like(gcov)
+            gcon[:, :, :, :, :] = gcon2d[:, :, None, :, :]
+        else:
+            gcon = np.linalg.inv(gcov)
+
+    # load fluid data from snapshot file
+    hfp = h5py.File(fname, 'r')
+    rho = np.array(hfp['prims'][:, :, :, 0])
+    UU = np.array(hfp['prims'][:, :, :, 1])
+    U = np.array(hfp['prims'][:, :, :, 2:5])
+    B = np.array(hfp['prims'][:, :, :, 5:8])
+    hfp.close()
+
+    N1, N2, N3 = rho.shape
+
+    # compute velocity four-vectors
+    alpha = 1. / np.sqrt(-gcon[:, :, :, 0, 0])
+    gamma = np.sqrt(1. + np.einsum('abci,abci->abc', np.einsum('abcij,abci->abcj',
+                                                               gcov[:, :, :, 1:, 1:],
+                                                               U), U))
+    ucon = np.zeros((N1, N2, N3, 4))
+    ucon[:, :, :, 1:] = -gamma[:, :, :, None]*alpha[:, :, :, None]*gcon[:, :, :, 0, 1:]
+    ucon[:, :, :, 1:] += U
+    ucon[:, :, :, 0] = gamma / alpha
+    ucov = np.einsum('abcij,abci->abcj', gcov, ucon)
+
+    # compute magnetic field four-vectors
+    bcon = np.zeros_like(ucon)
+    bcon[:, :, :, 0] = np.einsum('abci,abci->abc', B, ucov[:, :, :, 1:])
+    bcon[:, :, :, 1:] = B + ucon[:, :, :, 1:] * bcon[:, :, :, 0, None]
+    bcon[:, :, :, 1:] /= ucon[:, :, :, 0, None]
+    bcov = np.einsum('abcij,abci->abcj', gcov, bcon)
+
+    return (rho, UU, U, B, ucon, ucov, bcon, bcov)
```

