# Comparing `tmp/symlib-1.3.4.tar.gz` & `tmp/symlib-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symlib-1.3.4.tar", last modified: Wed Jun 14 22:30:24 2023, max compression
+gzip compressed data, was "symlib-1.3.5.tar", last modified: Fri Jun 16 17:54:04 2023, max compression
```

## Comparing `symlib-1.3.4.tar` & `symlib-1.3.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-14 22:30:24.781653 symlib-1.3.4/
--rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.4/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-14 22:30:24.781537 symlib-1.3.4/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.4/README.md
--rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.4/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-06-14 22:30:24.781685 symlib-1.3.4/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      885 2023-06-14 22:30:22.000000 symlib-1.3.4/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-14 22:30:24.780836 symlib-1.3.4/symlib/
--rw-r--r--   0 phil       (501) staff       (20)     1658 2023-05-25 11:19:28.000000 symlib-1.3.4/symlib/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.4/symlib/file_management.py
--rw-r--r--   0 phil       (501) staff       (20)    53111 2023-06-14 22:30:07.000000 symlib-1.3.4/symlib/lib.py
--rw-r--r--   0 phil       (501) staff       (20)    36176 2023-06-02 20:23:27.000000 symlib-1.3.4/symlib/star_tagging.py
--rw-r--r--   0 phil       (501) staff       (20)     9876 2023-06-14 22:30:07.000000 symlib-1.3.4/symlib/util.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-14 22:30:24.781359 symlib-1.3.4/symlib.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-14 22:30:24.000000 symlib-1.3.4/symlib.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      287 2023-06-14 22:30:24.000000 symlib-1.3.4/symlib.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-06-14 22:30:24.000000 symlib-1.3.4/symlib.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       41 2023-06-14 22:30:24.000000 symlib-1.3.4/symlib.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2023-06-14 22:30:24.000000 symlib-1.3.4/symlib.egg-info/top_level.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-16 17:54:04.171974 symlib-1.3.5/
+-rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.5/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-16 17:54:04.171862 symlib-1.3.5/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.5/README.md
+-rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.5/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-06-16 17:54:04.172009 symlib-1.3.5/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      885 2023-06-16 17:54:01.000000 symlib-1.3.5/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-16 17:54:04.171151 symlib-1.3.5/symlib/
+-rw-r--r--   0 phil       (501) staff       (20)     1715 2023-06-16 17:53:43.000000 symlib-1.3.5/symlib/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.5/symlib/file_management.py
+-rw-r--r--   0 phil       (501) staff       (20)    53185 2023-06-16 17:53:43.000000 symlib-1.3.5/symlib/lib.py
+-rw-r--r--   0 phil       (501) staff       (20)     9008 2023-06-16 17:53:43.000000 symlib-1.3.5/symlib/match.py
+-rw-r--r--   0 phil       (501) staff       (20)    36176 2023-06-02 20:23:27.000000 symlib-1.3.5/symlib/star_tagging.py
+-rw-r--r--   0 phil       (501) staff       (20)     9876 2023-06-14 22:30:07.000000 symlib-1.3.5/symlib/util.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-16 17:54:04.171686 symlib-1.3.5/symlib.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-16 17:54:04.000000 symlib-1.3.5/symlib.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      303 2023-06-16 17:54:04.000000 symlib-1.3.5/symlib.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-06-16 17:54:04.000000 symlib-1.3.5/symlib.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       41 2023-06-16 17:54:04.000000 symlib-1.3.5/symlib.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2023-06-16 17:54:04.000000 symlib-1.3.5/symlib.egg-info/top_level.txt
```

### Comparing `symlib-1.3.4/LICENSE` & `symlib-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `symlib-1.3.4/PKG-INFO` & `symlib-1.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.4
+Version: 1.3.5
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `symlib-1.3.4/setup.py` & `symlib-1.3.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-version = "1.3.4"
+version = "1.3.5"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="symlib",
     version=version,
```

### Comparing `symlib-1.3.4/symlib/__init__.py` & `symlib-1.3.5/symlib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .lib import SUBHALO_DTYPE, HISTORY_DTYPE, BRANCH_DTYPE, CORE_DTYPE, UM_DTYPE, PARTICLE_DTYPE
 # I/O function
 from .lib import read_subhalos, read_cores, read_branches, read_tree, read_particles, ParticleInfo
 from .lib import Particles
 # Utilities
 from .lib import simulation_parameters, parameter_table, scale_factors, pristine_merger_indices, merger_stats, propagate_parent_indices, colossus_parameters, suite_names, merger_lookup_table, find_merger_branch, find_all_merger_branches, is_real_confirmed, read_um, read_symfind, read_rockstar
 # TODO: better names for pristine_merger_indices and propagate_parent_indices
+from .match import match_subhalos, plot_matched_subhalos
 
 # Abstract models
 from .star_tagging import ProfileModel, RHalfModel, MStarModel, AbstractRanking
 # Profile models
 from .star_tagging import PlummerProfile
 # R_half models
 from .star_tagging import Nadler2020RHalf, Jiang2019RHalf, FixedRHalf
```

### Comparing `symlib-1.3.4/symlib/file_management.py` & `symlib-1.3.5/symlib/file_management.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.4/symlib/lib.py` & `symlib-1.3.5/symlib/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,16 +488,16 @@
 
     return mpeak, m_snap, ratio, sub_idx
 
 ROCKSTAR_DTYPE = [("id", "i4"), ("m", "f4"), ("vmax", "f4"), ("rvmax", "f4"),
                  ("x", "f4", (3,)), ("v", "f4", (3,)), ("ok", "?"),
                  ("rvir", "f4"), ("cvir", "f4")]
 
-def read_rockstar(dir_name):
-    h, hist = read_subhalos(dir_name)
+def read_rockstar(dir_name, comoving=False):
+    h, hist = read_subhalos(dir_name, comoving=comoving)
     r = np.zeros(h.shape, dtype=ROCKSTAR_DTYPE)
     r["id"], r["m"], r["vmax"] = h["id"], h["mvir"], h["vmax"]
     r["rvmax"], r["x"], r["v"] = h["rvmax"], h["x"], h["v"]
     r["ok"], r["rvir"], r["cvir"] = h["ok"], h["rvir"], h["cvir"]
     return r, hist
 
 def read_subhalos(dir_name, comoving=False, include_false_selections=False):
@@ -615,14 +615,16 @@
                                         h["first_infall_snap"][i])
 
         infall_snap = h["first_infall_snap"][i]
         mpeak_infall = np.max(s[i,:infall_snap+1]["mvir"])
         h["mpeak_pre"][i] = mpeak_infall
         h["false_selection"][i] = mpeak_infall < 300*param["mp"]
 
+    h["mpeak_pre"][0] = h["mpeak"][0]
+
     (snap_discrete, snap_eps,
      snap_relax, snap_relax_hydro,
      disrupt_snap, disrupt_snap_rs) = read_convergence_limits(dir_name)
     if snap_discrete is not None:
         ok = ~h["false_selection"]
         h["conv_snap_discrete"][ok] = snap_discrete
         h["conv_snap_eps"][ok] = snap_eps
```

### Comparing `symlib-1.3.4/symlib/star_tagging.py` & `symlib-1.3.5/symlib/star_tagging.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.4/symlib/util.py` & `symlib-1.3.5/symlib/util.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.4/symlib.egg-info/PKG-INFO` & `symlib-1.3.5/symlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.4
+Version: 1.3.5
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

