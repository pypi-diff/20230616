# Comparing `tmp/Sella-2.3.0.tar.gz` & `tmp/Sella-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sella-2.3.0.tar", last modified: Wed Jun 14 21:21:12 2023, max compression
+gzip compressed data, was "Sella-2.3.1.tar", last modified: Thu Jun 15 23:06:39 2023, max compression
```

## Comparing `Sella-2.3.0.tar` & `Sella-2.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:12.060397 Sella-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-14 21:20:40.000000 Sella-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 21:20:40.000000 Sella-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-14 21:21:12.060397 Sella-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-14 21:20:40.000000 Sella-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:12.060397 Sella-2.3.0/Sella.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-14 21:21:11.000000 Sella-2.3.0/Sella.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-14 21:21:12.000000 Sella-2.3.0/Sella.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:21:11.000000 Sella-2.3.0/Sella.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 21:21:11.000000 Sella-2.3.0/Sella.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 21:21:11.000000 Sella-2.3.0/Sella.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-14 21:20:40.000000 Sella-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 21:20:40.000000 Sella-2.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:12.060397 Sella-2.3.0/sella/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/eigensolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/force_match.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/hessian_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    56037 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:12.060397 Sella-2.3.0/sella/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/optimize/irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/optimize/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/optimize/restricted_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/optimize/stepper.py
--rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/peswrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/samd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:12.060397 Sella-2.3.0/sella/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/utilities/blas.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/utilities/math.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-14 21:21:12.060397 Sella-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-14 21:20:40.000000 Sella-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:06:39.955768 Sella-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-15 23:06:09.000000 Sella-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 23:06:09.000000 Sella-2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-15 23:06:39.955768 Sella-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-15 23:06:09.000000 Sella-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:06:39.951768 Sella-2.3.1/Sella.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-15 23:06:39.000000 Sella-2.3.1/Sella.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-15 23:06:39.000000 Sella-2.3.1/Sella.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 23:06:39.000000 Sella-2.3.1/Sella.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 23:06:39.000000 Sella-2.3.1/Sella.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 23:06:39.000000 Sella-2.3.1/Sella.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-15 23:06:09.000000 Sella-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 23:06:09.000000 Sella-2.3.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:06:39.955768 Sella-2.3.1/sella/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/eigensolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/force_match.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/hessian_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56197 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:06:39.955768 Sella-2.3.1/sella/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/optimize/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/optimize/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/optimize/restricted_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/optimize/stepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/peswrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/samd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:06:39.955768 Sella-2.3.1/sella/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/utilities/blas.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-15 23:06:09.000000 Sella-2.3.1/sella/utilities/math.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 23:06:39.955768 Sella-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-15 23:06:09.000000 Sella-2.3.1/setup.py
```

### Comparing `Sella-2.3.0/LICENSE` & `Sella-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Sella-2.3.0/PKG-INFO` & `Sella-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sella
-Version: 2.3.0
+Version: 2.3.1
 Author: Eric Hermes
 Author-email: ehermes@sandia.gov
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
```

### Comparing `Sella-2.3.0/README.md` & `Sella-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `Sella-2.3.0/Sella.egg-info/PKG-INFO` & `Sella-2.3.1/Sella.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sella
-Version: 2.3.0
+Version: 2.3.1
 Author: Eric Hermes
 Author-email: ehermes@sandia.gov
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
```

### Comparing `Sella-2.3.0/Sella.egg-info/SOURCES.txt` & `Sella-2.3.1/Sella.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Sella-2.3.0/sella/eigensolvers.py` & `Sella-2.3.1/sella/eigensolvers.py`

 * *Files identical despite different names*

### Comparing `Sella-2.3.0/sella/force_match.pyx` & `Sella-2.3.1/sella/force_match.pyx`

 * *Files identical despite different names*

### Comparing `Sella-2.3.0/sella/hessian_update.py` & `Sella-2.3.1/sella/hessian_update.py`

 * *Files identical despite different names*

### Comparing `Sella-2.3.0/sella/internal.py` & `Sella-2.3.1/sella/internal.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,19 +513,19 @@
 Angle.union = Dihedral
 Angle.diff = Bond
 Dihedral.diff = Angle
 
 
 def make_internal(
     name: str,
-    fun: Callable[[jnp.ndarray, ...], float],
+    fun: Callable[..., float],
     nindices: int,
     use_jit: bool = True,
-    jac: Callable[[jnp.ndarray, ...], jnp.ndarray] = None,
-    hess: Callable[[jnp.ndarray, ...], jnp.ndarray] = None,
+    jac: Callable[..., jnp.ndarray] = None,
+    hess: Callable[..., jnp.ndarray] = None,
     **kwargs,
 ) -> Type[Coordinate]:
     if jac is None:
         jac = _gradient(fun)
     if hess is None:
         hess = _hessian(fun)
 
@@ -604,14 +604,18 @@
         return sum(self._active['angles'])
 
     @property
     def ndihedrals(self) -> int:
         return sum(self._active['dihedrals'])
 
     @property
+    def nother(self) -> int:
+        return sum(self._active['other'])
+
+    @property
     def nrotations(self) -> int:
         return sum(self._active['rotations'])
 
     @property
     def _active_mask(self) -> List[bool]:
         active = []
         for name in self._names:
@@ -1046,15 +1050,15 @@
             self._active['other'].append(True)
             self._kind['other'].append(comparator)
         else:
             if replace_ok:
                 self._targets['other'][idx] = target
                 self._kind['other'][idx] = comparator
                 return
-            raise DuplicateCoordinateError(
+            raise DuplicateConstraintError(
                 "Coordinate {} is already fixed to target {}"
                 .format(coord, self._targets['other'][idx])
             )
 
     def merge_ase_constraint(self, ase_cons: FixConstraint) -> None:
         if isinstance(ase_cons, FixAtoms):
             for index in ase_cons.index:
@@ -1249,19 +1253,21 @@
     add_dihedral = partialmethod(_add_internal, Dihedral, 'dihedrals')
 
     def add_other(
         self,
         coord: Coordinate,
     ) -> None:
         try:
-            idx = self.internals['other'].index(coord)
+            self.internals['other'].index(coord)
         except ValueError:
             self.internals['other'].append(coord)
         else:
-            raise DuplicateCoordinateError()
+            raise DuplicateInternalError()
+        self.internals['other'].append(coord)
+        self._active['other'].append(True)
 
     def forbid_translation(
         self,
         index: Union[int, Tuple[int, ...], Translation] = None,
         dim: int = None
     ) -> None:
         if isinstance(index, Translation):
@@ -1530,15 +1536,17 @@
                 new = a1 + a2
             except NoValidInternalError:
                 continue
             # this is a dihedral that has the same exact atom as both
             # the first and last atom.
             if (
                 new.indices[0] == new.indices[3]
-                and np.all(np.sum(new.kwargs['ncvecs'], axis=0) == np.array((0, 0, 0)))
+                and np.all(
+                    np.sum(new.kwargs['ncvecs'], axis=0) == np.array((0, 0, 0))
+                )
             ):
                 continue
             try:
                 self.add_dihedral(new)
             except DuplicateInternalError:
                 continue
```

### Comparing `Sella-2.3.0/sella/linalg.py` & `Sella-2.3.1/sella/linalg.py`

 * *Files identical despite different names*

### Comparing `Sella-2.3.0/sella/optimize/irc.py` & `Sella-2.3.1/sella/optimize/irc.py`

 * *Files identical despite different names*

### Comparing `Sella-2.3.0/sella/optimize/optimize.py` & `Sella-2.3.1/sella/optimize/optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 class Sella(Optimizer):
     def __init__(
         self,
         atoms: Atoms,
         restart: bool = None,
         logfile: str = '-',
-        trajectory: str = None,
+        trajectory: Union[str, Trajectory] = None,
         master: bool = None,
         force_consistent: bool = False,
         delta0: float = None,
         sigma_inc: float = None,
         sigma_dec: float = None,
         rho_dec: float = None,
         rho_inc: float = None,
@@ -201,14 +201,15 @@
                 constraints=constraints,
                 trajectory=trajectory,
                 eta=eta,
                 v0=v0,
                 hessian_function=hessian_function,
                 **kwargs
             )
+        self.trajectory = self.pes.traj
 
     def _predict_step(self):
         if not self.initialized:
             self.pes.get_g()
             if self.eig:
                 if self.pes.hessian_function is not None:
                     self.pes.calculate_hessian()
```

### Comparing `Sella-2.3.0/sella/optimize/restricted_step.py` & `Sella-2.3.1/sella/optimize/restricted_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,31 +149,37 @@
         dval = dsda_mat[index] @ s_mat[index] / val
         return val, dval
 
 
 class MaxInternalStep(BaseRestrictedStep):
     synonyms = ['mis', 'max internal step']
 
-    def __init__(self, pes, *args, wx=1., wb=1., wa=1., wd=1., **kwargs):
+    def __init__(
+        self, pes, *args, wx=1., wb=1., wa=1., wd=1., wo=1., **kwargs
+    ):
         if pes.int is None:
             raise ValueError("Internal coordinates are required for the "
                              "{} trust region method"
                              .format(self.__class__.__name__))
         self.wx = wx
         self.wb = wb
         self.wa = wa
         self.wd = wd
+        self.wo = wo
         BaseRestrictedStep.__init__(self, pes, *args, **kwargs)
 
     def cons(self, s, dsda=None):
-        w = np.array([self.wx] * self.pes.int.ntrans
-                     + [self.wb] * self.pes.int.nbonds
-                     + [self.wa] * self.pes.int.nangles
-                     + [self.wd] * self.pes.int.ndihedrals
-                     + [self.wx] * self.pes.int.nrotations)
+        w = np.array(
+            [self.wx] * self.pes.int.ntrans
+            + [self.wb] * self.pes.int.nbonds
+            + [self.wa] * self.pes.int.nangles
+            + [self.wd] * self.pes.int.ndihedrals
+            + [self.wo] * self.pes.int.nother
+            + [self.wx] * self.pes.int.nrotations
+        )
         assert len(w) == len(s)
 
         sw = np.abs(s * w)
         idx = np.argmax(np.abs(sw))
         val = sw[idx]
 
         if dsda is None:
```

### Comparing `Sella-2.3.0/sella/optimize/stepper.py` & `Sella-2.3.1/sella/optimize/stepper.py`

 * *Files identical despite different names*

### Comparing `Sella-2.3.0/sella/peswrapper.py` & `Sella-2.3.1/sella/peswrapper.py`

 * *Files identical despite different names*

### Comparing `Sella-2.3.0/sella/samd.py` & `Sella-2.3.1/sella/samd.py`

 * *Files identical despite different names*

### Comparing `Sella-2.3.0/sella/utilities/blas.pyx` & `Sella-2.3.1/sella/utilities/blas.pyx`

 * *Files identical despite different names*

### Comparing `Sella-2.3.0/sella/utilities/math.pyx` & `Sella-2.3.1/sella/utilities/math.pyx`

 * *Files identical despite different names*

### Comparing `Sella-2.3.0/setup.py` & `Sella-2.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import os
 
 import numpy as np
 
 from setuptools import setup, Extension, find_packages
 
-VERSION = '2.3.0'
+VERSION = '2.3.1'
 
 debug = '--debug' in sys.argv or '-g' in sys.argv
 
 try:
     from Cython.Build import cythonize
 except ImportError:
     use_cython = False
```

