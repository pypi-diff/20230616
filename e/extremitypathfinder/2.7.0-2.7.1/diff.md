# Comparing `tmp/extremitypathfinder-2.7.0.tar.gz` & `tmp/extremitypathfinder-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extremitypathfinder-2.7.0.tar", max compression
+gzip compressed data, was "extremitypathfinder-2.7.1.tar", max compression
```

## Comparing `extremitypathfinder-2.7.0.tar` & `extremitypathfinder-2.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      200 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/.editorconfig
--rw-r--r--   0        0        0     2043 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     4782 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/CHANGELOG.rst
--rw-r--r--   0        0        0     3091 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1056 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/LICENSE
--rw-r--r--   0        0        0      772 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/Makefile
--rw-r--r--   0        0        0     2532 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/README.rst
--rw-r--r--   0        0        0      574 2023-06-08 10:11:45.728013 extremitypathfinder-2.7.0/example.json
--rw-r--r--   0        0        0      132 2023-06-08 10:11:45.728013 extremitypathfinder-2.7.0/extremitypathfinder/__init__.py
--rw-r--r--   0        0        0     2234 2023-06-08 10:11:45.728013 extremitypathfinder-2.7.0/extremitypathfinder/command_line.py
--rw-r--r--   0        0        0      198 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/configs.py
--rw-r--r--   0        0        0    14841 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/extremitypathfinder.py
--rw-r--r--   0        0        0      833 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/numba_replacements.py
--rw-r--r--   0        0        0     6902 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/plotting.py
--rw-r--r--   0        0        0      379 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/types.py
--rw-r--r--   0        0        0    44457 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/utils.py
--rw-r--r--   0        0        0     7133 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/utils_numba.py
--rw-r--r--   0        0        0     1970 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/__init__.py
--rw-r--r--   0        0        0      580 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/cli_test.py
--rwxr-xr-x   0        0        0     7211 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/helper_fcts_test.py
--rwxr-xr-x   0        0        0      839 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/helpers.py
--rwxr-xr-x   0        0        0     7351 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/main_test.py
--rw-r--r--   0        0        0    10817 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/test_cases.py
--rw-r--r--   0        0        0    12624 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/test_find_visible.py
--rwxr-xr-x   0        0        0      499 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tox.ini
--rw-r--r--   0        0        0     4137 1970-01-01 00:00:00.000000 extremitypathfinder-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/.editorconfig
+-rw-r--r--   0        0        0     2043 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     5082 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     3091 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1056 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/LICENSE
+-rw-r--r--   0        0        0      772 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/Makefile
+-rw-r--r--   0        0        0     2532 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/README.rst
+-rw-r--r--   0        0        0      574 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/example.json
+-rw-r--r--   0        0        0      132 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/__init__.py
+-rw-r--r--   0        0        0     2234 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/command_line.py
+-rw-r--r--   0        0        0      198 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/configs.py
+-rw-r--r--   0        0        0    14841 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/extremitypathfinder.py
+-rw-r--r--   0        0        0      833 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/numba_replacements.py
+-rw-r--r--   0        0        0     6902 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/plotting.py
+-rw-r--r--   0        0        0      379 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/types.py
+-rw-r--r--   0        0        0    43344 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/utils.py
+-rw-r--r--   0        0        0     8673 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/utils_numba.py
+-rw-r--r--   0        0        0     2082 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/__init__.py
+-rw-r--r--   0        0        0      580 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/cli_test.py
+-rwxr-xr-x   0        0        0     7211 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/helper_fcts_test.py
+-rwxr-xr-x   0        0        0      839 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/helpers.py
+-rwxr-xr-x   0        0        0     7351 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/main_test.py
+-rw-r--r--   0        0        0    10817 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/test_cases.py
+-rw-r--r--   0        0        0    12624 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/test_find_visible.py
+-rwxr-xr-x   0        0        0      499 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tox.ini
+-rw-r--r--   0        0        0     4196 1970-01-01 00:00:00.000000 extremitypathfinder-2.7.1/PKG-INFO
```

### Comparing `extremitypathfinder-2.7.0/.pre-commit-config.yaml` & `extremitypathfinder-2.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/CHANGELOG.rst` & `extremitypathfinder-2.7.1/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+2.7.1 (2023-05-16)
+-------------------
+
+internal:
+
+- JIT compile more utility functions (including numpy.linalg.solve)
+- add scipy dependency for JIT compiling numpy.linalg.solve
+- updated supported python versions to ">=3.8,<3.12" (required by scipy)
+- remove debug print statements and assertions
+
 
 2.7.0 (2023-06-08)
 -------------------
 
 - optional Numba JIT compilation offering significant speedup
 - extra: `pip install extremitypathfinder[numba]`
```

### Comparing `extremitypathfinder-2.7.0/CONTRIBUTING.rst` & `extremitypathfinder-2.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/LICENSE` & `extremitypathfinder-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/Makefile` & `extremitypathfinder-2.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/README.rst` & `extremitypathfinder-2.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/example.json` & `extremitypathfinder-2.7.1/example.json`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/extremitypathfinder/command_line.py` & `extremitypathfinder-2.7.1/extremitypathfinder/command_line.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/extremitypathfinder/extremitypathfinder.py` & `extremitypathfinder-2.7.1/extremitypathfinder/extremitypathfinder.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/extremitypathfinder/numba_replacements.py` & `extremitypathfinder-2.7.1/extremitypathfinder/numba_replacements.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/extremitypathfinder/plotting.py` & `extremitypathfinder-2.7.1/extremitypathfinder/plotting.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/extremitypathfinder/utils.py` & `extremitypathfinder-2.7.1/extremitypathfinder/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from extremitypathfinder.utils_numba import (
     _angle_rep_inverse,
     _compute_repr_n_dist,
     _fill_edge_vertex_idxs,
     _fill_extremity_mask,
     _has_clockwise_numbering,
     _inside_polygon,
+    _lies_behind,
     _no_identical_consequent_vertices,
 )
 
 
 def cmp_reps_n_distances(orig_idx: int, coords: np.ndarray) -> np.ndarray:
     coords_orig = coords[orig_idx]
     coords_translated = coords - coords_orig
@@ -72,46 +73,14 @@
         return 0
     # if np.all(0.0 <= x) and np.all(x <= 1.0):
     #     return 2
     else:
         return 1
 
 
-def _lies_behind_inner(p1: np.ndarray, p2: np.ndarray, v: np.ndarray) -> bool:
-    # special case of get_intersection_status()
-    # solve the set of equations
-    # (p2-p1) lambda + (p1) = (v) mu
-    #  in matrix form A x = b:
-    # [(p1-p2) (v)] (lambda, mu)' = (p1)
-    # because the vertex lies within the angle range between the two edge vertices
-    #    (together with the other conditions on the polygons)
-    #   this set of linear equations is always solvable (the matrix is regular)
-    A = np.array([p1 - p2, v]).T
-    try:
-        x = np.linalg.solve(A, p1)
-    except np.linalg.LinAlgError:
-        # parallel lines -> lie in
-        raise ValueError
-
-    # Debug:
-    # assert np.allclose((p2 - p1) * x[0] + p1, v * x[1])
-    # assert np.allclose(np.dot(A, x), b)
-
-    # vertices on the edge are possibly visible! ( < not <=)
-    return x[1] < 1.0
-
-
-def _lies_behind(idx_p1: int, idx_p2: int, idx_v: int, idx_orig: int, coords: np.ndarray) -> bool:
-    coords_origin = coords[idx_orig]
-    coords_p1_rel = coords[idx_p1] - coords_origin
-    coords_p2_rel = coords[idx_p2] - coords_origin
-    coords_v_rel = coords[idx_v] - coords_origin
-    return _lies_behind_inner(coords_p1_rel, coords_p2_rel, coords_v_rel)
-
-
 def _no_self_intersection(coords):
     polygon_length = len(coords)
     # again_check = []
     for index_p1, index_q1 in combinations(range(polygon_length), 2):
         # always: index_p1 < index_q1
         if index_p1 == index_q1 - 1 or index_p1 == index_q1 + 1:
             # neighbouring edges never have an intersection
@@ -272,38 +241,34 @@
     :param origin: the vertex for which the visibility to the other candidates should be checked.
     :param candidates: the set of all vertex ids which should be checked for visibility.
         IMPORTANT: is being manipulated, so has to be a copy!
         IMPORTANT: must not contain any vertices with equal coordinates (e.g. the origin vertex itself)!
     :param edges_to_check: the set of edges which determine visibility
     :return: a set of all vertices visible from the origin
     """
-    print("\n\nNEW:")
     nr_candidates_total = len(candidates)
     if nr_candidates_total == 0:
         return candidates
     # TODO immutable
     # eliminate candidates with equal representations: only keep the closest (min dist)
     candidates_sorted = _eliminate_eq_candidates(candidates, distances, representations)
-    print(candidates_sorted)
 
     (
         crossing_edges,
         edges_is_crossing,
         edges_max_dist,
         edges_max_rep,
         edges_min_rep,
         non_crossing_edges,
         edge_vertex_idxs,
     ) = _compile_visibility_datastructs(
         distances, edge_vertex_idxs, edges_to_check, extremity_mask, representations, vertex_edge_idxs
     )
 
     # check non-crossing edges
-    print("non-crossing edges")
-
     # TODO skipped edges. argsort
     # sort after the minimum representation
     edge_idxs_sorted = sorted(non_crossing_edges, key=lambda e: edges_min_rep[e])
     # edge_ptr_iter = iter(ptr for ptr in edge_ptrs if not edges_is_crossing[ptr])
     _check_candidates(
         candidates_sorted,
         edge_idxs_sorted,
@@ -341,15 +306,15 @@
         edges_max_dist,
     )
     # TODO avoid conversion?
     candidates_ = set(candidates_sorted)
     return candidates_
 
 
-def _eliminate_eq_candidates(candidates, distances, representations):
+def _eliminate_eq_candidates(candidates: List[int], distances: np.ndarray, representations: np.ndarray) -> List[int]:
     # sort after angle representation, then after distance ascending
     candidates_sorted = sorted(candidates, key=lambda i: (representations[i], distances[i]))
     rep_prev = representations[candidates_sorted[0]]
     i = 1
     while i < len(candidates_sorted):
         candidate = candidates_sorted[i]
         rep = representations[candidate]
@@ -364,16 +329,14 @@
 
     return candidates_sorted
 
 
 def _compile_visibility_datastructs(
     distances, edge_vertex_idxs, edges_to_check, extremity_mask, representations, vertex_edge_idxs
 ):
-    print(edge_vertex_idxs)
-
     edges = list(edges_to_check)
     nr_edges_total = len(edge_vertex_idxs)
     edges_min_rep = np.zeros(nr_edges_total, dtype=float)
     edges_max_rep = np.zeros(nr_edges_total, dtype=float)
     edges_max_dist = np.zeros(nr_edges_total, dtype=float)
     edges_is_crossing = np.zeros(nr_edges_total, dtype=bool)
     edges_to_skip = set()
@@ -420,17 +383,14 @@
             if not copied_indices:
                 edge_vertex_idxs = edge_vertex_idxs.copy()
                 copied_indices = True
 
             # point to the neighbouring vertices (used for looking up the coordinates)
             edge_vertex_idxs[e] = (i1, i2)
 
-            print(e)
-            print(edge_vertex_idxs)
-
             # the "outside the polygon" angle range should be eliminated
             # this angle range is greater than 180 degree if the node identical to the origin is NOT an extremity
             deg_gr_180_exp = not extremity_mask[identical_node]
             deg_gr_180_actual = max_rep - min_rep > 2.0
             # an edge "crosses the origin" (rep: 4.0 -> 0.0)
             # when its vertex representation difference is unlike expected
             is_crossing = deg_gr_180_actual != deg_gr_180_exp
@@ -472,15 +432,14 @@
             non_crossing_edges.add(e)
 
         edges_min_rep[e] = min_rep
         edges_max_rep[e] = max_rep
         edges_max_dist[e] = max_dist
         edges_is_crossing[e] = is_crossing
 
-    print(edge_vertex_idxs)
     return (
         crossing_edges,
         edges_is_crossing,
         edges_max_dist,
         edges_max_rep,
         edges_min_rep,
         non_crossing_edges,
@@ -512,41 +471,42 @@
     edges_max_rep = tmp
     # apply same transformation also to candidate representations
     # TODO avoid large copy. use dict
     representations = representations.copy()  # IMPORTANT: work on independent copy
     representations[candidate_idxs] = (representations[candidate_idxs] + infimum_to_0) % 4.0
     # Note: new sorting is required
     candidate_idxs = sorted(candidate_idxs, key=lambda i: representations[i])
-    non_nan_reps = representations[np.logical_not(np.isnan(representations))]
-    assert np.all(non_nan_reps >= 0.0)
-    assert np.all(non_nan_reps <= 4.0)
-    if not np.all(edges_min_rep >= 0.0):
-        raise ValueError
-    assert np.all(edges_min_rep <= 4.0)
-    assert np.min(edges_min_rep[edges_is_crossing]) == 0.0
-    assert np.all(edges_max_rep >= 0.0)
-    assert np.all(edges_max_rep <= 4.0)
-    for r_min, r_max in zip(edges_min_rep[edges_is_crossing], edges_max_rep[edges_is_crossing]):
-        if r_min > r_max:
-            raise ValueError
+    # TODO move to tests
+    # non_nan_reps = representations[np.logical_not(np.isnan(representations))]
+    # assert np.all(non_nan_reps >= 0.0)
+    # assert np.all(non_nan_reps <= 4.0)
+    # if not np.all(edges_min_rep >= 0.0):
+    #     raise ValueError
+    # assert np.all(edges_min_rep <= 4.0)
+    # assert np.min(edges_min_rep[edges_is_crossing]) == 0.0
+    # assert np.all(edges_max_rep >= 0.0)
+    # assert np.all(edges_max_rep <= 4.0)
+    # for r_min, r_max in zip(edges_min_rep[edges_is_crossing], edges_max_rep[edges_is_crossing]):
+    #     if r_min > r_max:
+    #         raise ValueError
     return candidate_idxs, edges_max_rep, edges_min_rep, representations
 
 
 def check_candidates_one_edge(
-    edge_min_rep,
-    edge_max_rep,
-    edge_max_dist,
-    p1,
-    p2,
-    candidate_ptr,
-    origin,
-    candidate_indices,
-    coords,
-    distances,
-    representations,
+    edge_min_rep: float,
+    edge_max_rep: float,
+    edge_max_dist: float,
+    p1: int,
+    p2: int,
+    candidate_ptr: int,
+    origin: int,
+    candidate_indices: List[int],
+    coords: np.ndarray,
+    distances: np.ndarray,
+    representations: np.ndarray,
 ):
     # start over at the same candidate than the previous edge
     # TODO Note: check within range: edge case, same representation than edge vertex.
     #  do not include (edge does not block view)
     for candidate_idx in candidate_indices[candidate_ptr:]:
         candidate_rep = representations[candidate_idx]
         # a candidate does not have to be considered,
@@ -604,24 +564,24 @@
             # move pointer to the next candidate
             candidate_ptr_curr += 1
 
     return candidate_ptr
 
 
 def _check_candidates(
-    candidate_idxs,
-    edge_idxs_sorted,
-    edges_max_rep,
-    edges_min_rep,
-    origin,
-    distances,
-    representations,
-    coords,
-    edge_vertex_idxs,
-    edges_max_dist,
+    candidate_idxs: List[int],
+    edge_idxs_sorted: List[int],
+    edges_max_rep: np.ndarray,
+    edges_min_rep: np.ndarray,
+    origin: int,
+    distances: np.ndarray,
+    representations: np.ndarray,
+    coords: np.ndarray,
+    edge_vertex_idxs: np.ndarray,
+    edges_max_dist: np.ndarray,
 ):
     candidate_ptr = 0
     for edge_idx in edge_idxs_sorted:
         if len(candidate_idxs) == 0:
             # Note: length is decreasing
             break
```

### Comparing `extremitypathfinder-2.7.0/extremitypathfinder/utils_numba.py` & `extremitypathfinder-2.7.1/extremitypathfinder/utils_numba.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import math
 from typing import Optional, Tuple
 
 import numpy as np
 
+from extremitypathfinder import configs
+
 try:
     from numba import b1, f8, i8, njit, typeof, void
 except ImportError:
     using_numba = False
     # replace Numba functionality with "transparent" implementations
     from extremitypathfinder.numba_replacements import b1, f8, i8, njit, typeof, void
 
@@ -204,7 +206,45 @@
         v2_idx = v2
         edge_vertex_idxs[edge_idx, 0] = v1_idx
         edge_vertex_idxs[edge_idx, 1] = v2_idx
         vertex_edge_idxs[v1_idx, 1] = edge_idx
         vertex_edge_idxs[v2_idx, 0] = edge_idx
         # move to the next vertex/edge
         v1 = v2
+
+
+@njit(b1(f8[:], f8[:], f8[:]), cache=True)
+def _lies_behind_inner(p1: np.ndarray, p2: np.ndarray, v: np.ndarray) -> bool:
+    # special case of get_intersection_status()
+    # solve the set of equations
+    # (p2-p1) lambda + (p1) = (v) mu
+    #  in matrix form A x = b:
+    # [(p1-p2) (v)] (lambda, mu)' = (p1)
+    # because the vertex lies within the angle range between the two edge vertices
+    #    (together with the other conditions on the polygons)
+    #   this set of linear equations is always solvable (the matrix is regular)
+    A = np.empty((2, 2), dtype=configs.DTYPE_FLOAT)
+    A[:, 0] = p1 - p2
+    A[:, 1] = v
+    # A = np.array([p1 - p2, v]).T
+    x = np.linalg.solve(A, p1)
+    # Note: parallel lines are not possible here (singular matrix)
+    # try:
+    #     x = np.linalg.solve(A, p1)
+    # except np.linalg.LinAlgError:
+    #     raise Exception("parallel lines")
+
+    # Debug:
+    # assert np.allclose((p2 - p1) * x[0] + p1, v * x[1])
+    # assert np.allclose(np.dot(A, x), b)
+
+    # vertices on the edge are possibly visible! ( < not <=)
+    return x[1] < 1.0
+
+
+@njit(b1(i8, i8, i8, i8, f8[:, :]), cache=True)
+def _lies_behind(idx_p1: int, idx_p2: int, idx_v: int, idx_orig: int, coords: np.ndarray) -> bool:
+    coords_origin = coords[idx_orig]
+    coords_p1_rel = coords[idx_p1] - coords_origin
+    coords_p2_rel = coords[idx_p2] - coords_origin
+    coords_v_rel = coords[idx_v] - coords_origin
+    return _lies_behind_inner(coords_p1_rel, coords_p2_rel, coords_v_rel)
```

### Comparing `extremitypathfinder-2.7.0/pyproject.toml` & `extremitypathfinder-2.7.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "extremitypathfinder"
-version = "2.7.0"
+version = "2.7.1"
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/jannikmi/extremitypathfinder"
 homepage = "https://extremitypathfinder.readthedocs.io/en/latest/"
 documentation = "https://extremitypathfinder.readthedocs.io/en/latest/"
 keywords = ["path-planning", "path-finding", "shortest-path", "visibility", "graph", "polygon", "grid", "map", "robotics", "navigation", "offline"]
 classifiers = [
@@ -35,18 +35,20 @@
 ]
 #exclude = ["my_package/excluded.py"]
 
 [tool.poetry.scripts]
 extremitypathfinder = "extremitypathfinder.command_line:main"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8,<3.12"
 numpy = "^1.22"
 networkx = "^3"
 numba = {version = "^0.56.0", optional = true}
+# required for jit of np.linalg.solve with numba
+scipy = {version = "^1.10.1", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "*"
 
 [tool.poetry.group.plot.dependencies]
 matplotlib = "*"
 
@@ -55,15 +57,15 @@
 tox = "*"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "*"
 sphinx-rtd-theme = "*"
 
 [tool.poetry.extras]
-numba = ["numba"]
+numba = ["numba", "scipy"]
 plot = ["matplotlib"]
 test = ["pytest", "tox"]
 docs = ["Sphinx", "sphinx-rtd-theme"]
 
 [build-system]
 requires = ["poetry-core>=1.5", "poetry>=1.4"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `extremitypathfinder-2.7.0/tests/cli_test.py` & `extremitypathfinder-2.7.1/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/tests/helper_fcts_test.py` & `extremitypathfinder-2.7.1/tests/helper_fcts_test.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/tests/helpers.py` & `extremitypathfinder-2.7.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/tests/main_test.py` & `extremitypathfinder-2.7.1/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/tests/test_cases.py` & `extremitypathfinder-2.7.1/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/tests/test_find_visible.py` & `extremitypathfinder-2.7.1/tests/test_find_visible.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.0/PKG-INFO` & `extremitypathfinder-2.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: extremitypathfinder
-Version: 2.7.0
+Version: 2.7.1
 Summary: python package for fast shortest path computation on 2D polygon or grid maps
 Home-page: https://extremitypathfinder.readthedocs.io/en/latest/
 License: MIT
 Keywords: path-planning,path-finding,shortest-path,visibility,graph,polygon,grid,map,robotics,navigation,offline
 Author: jannikmi
 Author-email: github@michelfe.it
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -27,14 +27,15 @@
 Provides-Extra: docs
 Provides-Extra: numba
 Provides-Extra: plot
 Provides-Extra: test
 Requires-Dist: networkx (>=3,<4)
 Requires-Dist: numba (>=0.56.0,<0.57.0) ; extra == "numba"
 Requires-Dist: numpy (>=1.22,<2.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0) ; extra == "numba"
 Project-URL: Documentation, https://extremitypathfinder.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/jannikmi/extremitypathfinder
 Description-Content-Type: text/x-rst
 
 ===================
 extremitypathfinder
 ===================
```

