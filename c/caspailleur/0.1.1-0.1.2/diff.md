# Comparing `tmp/caspailleur-0.1.1.tar.gz` & `tmp/caspailleur-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caspailleur-0.1.1.tar", last modified: Fri May 26 18:15:04 2023, max compression
+gzip compressed data, was "caspailleur-0.1.2.tar", last modified: Fri Jun 16 14:31:35 2023, max compression
```

## Comparing `caspailleur-0.1.1.tar` & `caspailleur-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-05-26 18:15:04.964982 caspailleur-0.1.1/
--rw-r--r--   0 egordudyrev   (501) staff       (20)    35149 2023-04-11 14:13:18.000000 caspailleur-0.1.1/LICENSE
--rw-r--r--   0 egordudyrev   (501) staff       (20)    53111 2023-05-26 18:15:04.964853 caspailleur-0.1.1/PKG-INFO
--rw-r--r--   0 egordudyrev   (501) staff       (20)    11966 2023-05-26 17:59:35.000000 caspailleur-0.1.1/README.md
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-05-26 18:15:04.962882 caspailleur-0.1.1/caspailleur/
--rw-r--r--   0 egordudyrev   (501) staff       (20)      401 2023-05-26 18:09:18.000000 caspailleur-0.1.1/caspailleur/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     4096 2023-04-11 14:13:18.000000 caspailleur-0.1.1/caspailleur/base_functions.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     4202 2023-04-11 14:13:18.000000 caspailleur-0.1.1/caspailleur/definitions.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     6900 2023-04-11 14:13:18.000000 caspailleur-0.1.1/caspailleur/implication_bases.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     3905 2023-04-11 14:13:18.000000 caspailleur-0.1.1/caspailleur/indices.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     7027 2023-05-25 13:00:43.000000 caspailleur-0.1.1/caspailleur/mine_equivalence_classes.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2386 2023-04-11 14:13:18.000000 caspailleur-0.1.1/caspailleur/orchestrator.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     5982 2023-04-11 14:13:18.000000 caspailleur-0.1.1/caspailleur/order.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-05-26 18:15:04.963583 caspailleur-0.1.1/caspailleur.egg-info/
--rw-r--r--   0 egordudyrev   (501) staff       (20)    53111 2023-05-26 18:15:04.000000 caspailleur-0.1.1/caspailleur.egg-info/PKG-INFO
--rw-r--r--   0 egordudyrev   (501) staff       (20)      605 2023-05-26 18:15:04.000000 caspailleur-0.1.1/caspailleur.egg-info/SOURCES.txt
--rw-r--r--   0 egordudyrev   (501) staff       (20)        1 2023-05-26 18:15:04.000000 caspailleur-0.1.1/caspailleur.egg-info/dependency_links.txt
--rw-r--r--   0 egordudyrev   (501) staff       (20)       48 2023-05-26 18:15:04.000000 caspailleur-0.1.1/caspailleur.egg-info/requires.txt
--rw-r--r--   0 egordudyrev   (501) staff       (20)       12 2023-05-26 18:15:04.000000 caspailleur-0.1.1/caspailleur.egg-info/top_level.txt
--rw-r--r--   0 egordudyrev   (501) staff       (20)      825 2023-05-26 18:14:49.000000 caspailleur-0.1.1/pyproject.toml
--rw-r--r--   0 egordudyrev   (501) staff       (20)       38 2023-05-26 18:15:04.965017 caspailleur-0.1.1/setup.cfg
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-05-26 18:15:04.964600 caspailleur-0.1.1/tests/
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2769 2023-04-11 14:13:18.000000 caspailleur-0.1.1/tests/test_base_functions.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     4679 2023-04-11 14:13:18.000000 caspailleur-0.1.1/tests/test_definitions.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     1423 2023-04-11 14:13:18.000000 caspailleur-0.1.1/tests/test_implication_bases.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     3840 2023-05-25 13:00:43.000000 caspailleur-0.1.1/tests/test_mine_equivalence_classes.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2859 2023-04-11 14:13:18.000000 caspailleur-0.1.1/tests/test_orchestrator.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2334 2023-04-11 14:13:18.000000 caspailleur-0.1.1/tests/test_order.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-16 14:31:35.260237 caspailleur-0.1.2/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    35149 2023-04-11 14:13:18.000000 caspailleur-0.1.2/LICENSE
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    53090 2023-06-16 14:31:35.260106 caspailleur-0.1.2/PKG-INFO
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    11945 2023-06-16 14:29:16.000000 caspailleur-0.1.2/README.md
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-16 14:31:35.258139 caspailleur-0.1.2/caspailleur/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      401 2023-06-16 14:29:16.000000 caspailleur-0.1.2/caspailleur/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     4544 2023-06-16 14:29:16.000000 caspailleur-0.1.2/caspailleur/base_functions.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     4202 2023-04-11 14:13:18.000000 caspailleur-0.1.2/caspailleur/definitions.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     6900 2023-04-11 14:13:18.000000 caspailleur-0.1.2/caspailleur/implication_bases.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     4482 2023-06-16 14:29:16.000000 caspailleur-0.1.2/caspailleur/indices.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     8487 2023-06-16 14:29:16.000000 caspailleur-0.1.2/caspailleur/mine_equivalence_classes.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2386 2023-04-11 14:13:18.000000 caspailleur-0.1.2/caspailleur/orchestrator.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     5982 2023-04-11 14:13:18.000000 caspailleur-0.1.2/caspailleur/order.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-16 14:31:35.258842 caspailleur-0.1.2/caspailleur.egg-info/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    53090 2023-06-16 14:31:35.000000 caspailleur-0.1.2/caspailleur.egg-info/PKG-INFO
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      605 2023-06-16 14:31:35.000000 caspailleur-0.1.2/caspailleur.egg-info/SOURCES.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        1 2023-06-16 14:31:35.000000 caspailleur-0.1.2/caspailleur.egg-info/dependency_links.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)       48 2023-06-16 14:31:35.000000 caspailleur-0.1.2/caspailleur.egg-info/requires.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)       12 2023-06-16 14:31:35.000000 caspailleur-0.1.2/caspailleur.egg-info/top_level.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      825 2023-06-16 14:29:16.000000 caspailleur-0.1.2/pyproject.toml
+-rw-r--r--   0 egordudyrev   (501) staff       (20)       38 2023-06-16 14:31:35.260282 caspailleur-0.1.2/setup.cfg
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-16 14:31:35.259826 caspailleur-0.1.2/tests/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2769 2023-04-11 14:13:18.000000 caspailleur-0.1.2/tests/test_base_functions.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     4679 2023-04-11 14:13:18.000000 caspailleur-0.1.2/tests/test_definitions.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1423 2023-04-11 14:13:18.000000 caspailleur-0.1.2/tests/test_implication_bases.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     5089 2023-06-16 13:27:41.000000 caspailleur-0.1.2/tests/test_mine_equivalence_classes.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2859 2023-04-11 14:13:18.000000 caspailleur-0.1.2/tests/test_orchestrator.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2334 2023-04-11 14:13:18.000000 caspailleur-0.1.2/tests/test_order.py
```

### Comparing `caspailleur-0.1.1/LICENSE` & `caspailleur-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.1/PKG-INFO` & `caspailleur-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caspailleur
-Version: 0.1.1
+Version: 0.1.2
 Summary: Minimalistic python package for mining many concise data representations. Part of SmartFCA project
 Author: Egor Dudyrev
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -697,15 +697,15 @@
 
 # caspailleur
 
 Minimalistic python package for mining many concise data representations. Part of SmartFCA project.
 
 ## Get started
 
-To install the package, please download it from this GitHub page.
+The package can be installed from PyPI with:
 
 ```console
 pip install caspailleur
 ```
 
 ## Run example
```

### Comparing `caspailleur-0.1.1/README.md` & `caspailleur-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # caspailleur
 
 Minimalistic python package for mining many concise data representations. Part of SmartFCA project.
 
 ## Get started
 
-To install the package, please download it from this GitHub page.
+The package can be installed from PyPI with:
 
 ```console
 pip install caspailleur
 ```
 
 ## Run example
```

### Comparing `caspailleur-0.1.1/caspailleur/base_functions.py` & `caspailleur-0.1.2/caspailleur/base_functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,38 +27,45 @@
 
 
 def is_psubset_of(A: FrozenSet[int] or fbarray, B: FrozenSet[int] or fbarray) -> bool:
     """Test whether `A` is a proper subset of `B`"""
     return (A & B == A) and A != B
 
 
-def closure(D: Iterable[int], crosses_per_columns: List[FrozenSet[int]]) -> Iterator[int]:
-    """Iterate indices of all columns whose intersection equals to the intersection of columns `D`
+def extension(description: Iterable[int], crosses_per_columns: List[FrozenSet[int]]) -> FrozenSet[int]:
+    """Select the indices of rows described by `description`"""
+    n_rows = max(max(col) + 1 for col in crosses_per_columns if col)
+    extent = set(range(n_rows))
+    for m in description:
+        extent &= crosses_per_columns[m]
+    return frozenset(extent)
+
+
+def intention(objects: Iterable[int], crosses_per_columns: List[FrozenSet[int]]) -> Iterator[int]:
+    """Iterate the indices of columns that describe the `objects`"""
+    return (m for m, col in enumerate(crosses_per_columns) if is_subset_of(objects, col))
+
+
+def closure(description: Iterable[int], crosses_per_columns: List[FrozenSet[int]]) -> Iterator[int]:
+    """Iterate indices of all columns who describe the same rows as `description`
 
     Parameters
     ----------
-    D: Iterable[int]
+    description: Iterable[int]
         Indices of some columns from `crosses_per_columns`
     crosses_per_columns: List[FrozenSet[int]]
         List of indices of 'True' rows for each column
 
     Returns
     -------
     intent: Iterator[int]
         Indices of All columns with the same intersection as `D`
 
     """
-    n_rows = max(max(col) + 1 for col in crosses_per_columns if col)
-
-    extent = set(range(n_rows))
-    for m in D:
-        extent &= crosses_per_columns[m]
-
-    intent = (m for m, col in enumerate(crosses_per_columns) if is_subset_of(extent, col))
-    return intent
+    return intention(extension(description, crosses_per_columns), crosses_per_columns)
 
 
 ##########################
 # Basic type conversions #
 ##########################
 def np2bas(X: npt.ArrayLike) -> List[fbarray]:
     """Convert numpy boolean matrix to the list of bitarrays (one per row of the matrix)"""
```

### Comparing `caspailleur-0.1.1/caspailleur/definitions.py` & `caspailleur-0.1.2/caspailleur/definitions.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.1/caspailleur/implication_bases.py` & `caspailleur-0.1.2/caspailleur/implication_bases.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.1/caspailleur/indices.py` & `caspailleur-0.1.2/caspailleur/indices.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Iterator
 from collections import deque
 from bitarray import frozenbitarray as fbarray
 from tqdm import tqdm
 
 from caspailleur.order import test_topologically_sorted
 
 
@@ -103,7 +103,22 @@
         n_distr -= 2 * n_intents - 3  # dropping (n-1) rels for top intent and 1 rel. for (n-2) intents
         n_pairs -= 2 * n_intents - 3
 
     if n_distr > n_pairs:
         raise ValueError('Distributivity index is computed in a wrong way (There should be problem with the code)')
 
     return n_distr / n_pairs if n_pairs else 0
+
+
+def delta_stability_index(extents: List[fbarray]) -> Iterator[int]:
+    """Compute the delta stability index: the difference in supports of an extent and its maximal smaller neighbour"""
+    assert test_topologically_sorted(extents)
+
+    for i, extent in enumerate(extents):
+        for smaller_extent in extents[i-1::-1]:
+            if smaller_extent & extent != smaller_extent:
+                continue
+
+            yield (extent & ~smaller_extent).count()
+            break
+        else:  # no break, i.e. no child extent found
+            yield extent.count()
```

### Comparing `caspailleur-0.1.1/caspailleur/mine_equivalence_classes.py` & `caspailleur-0.1.2/caspailleur/mine_equivalence_classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import List, Dict, Iterator, Iterable
 
 from .order import topological_sorting
 from .base_functions import isets2bas, bas2isets
+from .indices import delta_stability_index
 
 from skmine.itemsets import LCM
 from bitarray import bitarray, frozenbitarray as fbarray
 from bitarray.util import zeros as bazeros
 from collections import deque
+from tqdm import tqdm
 
 
 def list_intents_via_LCM(itemsets: List[fbarray], min_supp: float = 1, n_jobs: int = 1) -> List[fbarray]:
     """Get the list of intents by running LCM algorithm from scikit-mine
 
     Parameters
     ----------
@@ -196,7 +198,36 @@
 
 
 def list_passkeys(intents: List[fbarray]) -> Dict[fbarray, int]:
     """List all passkeys for all intents
 
      (i.e. subsets of attributes of minimal size selecting specific subsets of objects)"""
     return list_keys(intents, only_passkeys=True)
+
+
+def list_stable_extents_via_sofia(
+        attribute_extents: Iterable[fbarray],
+        n_stable_extents: int, min_supp: int = -1,
+        use_tqdm: bool = False, n_attributes: int = None
+) -> set[fbarray]:
+    stable_extents = set()
+    for attr_extent in tqdm(attribute_extents, disable=not use_tqdm, total=n_attributes):
+        if not stable_extents:  # Set up the top extent, as soon as we know the number of objects
+            stable_extents.add(fbarray(~bazeros(len(attr_extent))))
+
+        if attr_extent.count() < min_supp:
+            continue
+
+        new_extents = (extent & attr_extent for extent in stable_extents)
+        new_extents = filter(lambda extent: extent.count() >= min_supp and extent not in stable_extents, new_extents)
+        stable_extents |= set(new_extents)
+
+        if len(stable_extents) > n_stable_extents:
+            extents_top_sort = sorted(stable_extents, key=lambda extent: extent.count())
+            delta_stabilities = list(delta_stability_index(extents_top_sort))
+            stab_thold = sorted(delta_stabilities)[-n_stable_extents]
+            stable_extents = {extent for extent, stab in zip(extents_top_sort, delta_stabilities) if stab >= stab_thold}
+
+    if len(stable_extents) > n_stable_extents:
+        stable_extents = {extent for extent, stab in zip(extents_top_sort, delta_stabilities) if stab > stab_thold}
+
+    return stable_extents
```

### Comparing `caspailleur-0.1.1/caspailleur/orchestrator.py` & `caspailleur-0.1.2/caspailleur/orchestrator.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.1/caspailleur/order.py` & `caspailleur-0.1.2/caspailleur/order.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.1/caspailleur.egg-info/PKG-INFO` & `caspailleur-0.1.2/caspailleur.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caspailleur
-Version: 0.1.1
+Version: 0.1.2
 Summary: Minimalistic python package for mining many concise data representations. Part of SmartFCA project
 Author: Egor Dudyrev
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -697,15 +697,15 @@
 
 # caspailleur
 
 Minimalistic python package for mining many concise data representations. Part of SmartFCA project.
 
 ## Get started
 
-To install the package, please download it from this GitHub page.
+The package can be installed from PyPI with:
 
 ```console
 pip install caspailleur
 ```
 
 ## Run example
```

### Comparing `caspailleur-0.1.1/caspailleur.egg-info/SOURCES.txt` & `caspailleur-0.1.2/caspailleur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.1/pyproject.toml` & `caspailleur-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caspailleur"
-version = "0.1.1"
+version = "0.1.2"
 description = "Minimalistic python package for mining many concise data representations. Part of SmartFCA project"
 readme = "README.md"
 authors = [{ name = "Egor Dudyrev" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

### Comparing `caspailleur-0.1.1/tests/test_base_functions.py` & `caspailleur-0.1.2/tests/test_base_functions.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.1/tests/test_definitions.py` & `caspailleur-0.1.2/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.1/tests/test_implication_bases.py` & `caspailleur-0.1.2/tests/test_implication_bases.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.1/tests/test_orchestrator.py` & `caspailleur-0.1.2/tests/test_orchestrator.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.1/tests/test_order.py` & `caspailleur-0.1.2/tests/test_order.py`

 * *Files identical despite different names*

