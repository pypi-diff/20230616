# Comparing `tmp/error-parity-0.1.2.tar.gz` & `tmp/error-parity-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-parity-0.1.2.tar", last modified: Tue Jun  6 12:00:15 2023, max compression
+gzip compressed data, was "error-parity-0.1.3.tar", last modified: Fri Jun 16 14:07:05 2023, max compression
```

## Comparing `error-parity-0.1.2.tar` & `error-parity-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:00:15.044356 error-parity-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-06 12:00:05.000000 error-parity-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-06 12:00:05.000000 error-parity-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-06 12:00:15.040356 error-parity-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-06 12:00:05.000000 error-parity-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:00:15.040356 error-parity-0.1.2/error_parity/
--rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-06-06 12:00:05.000000 error-parity-0.1.2/error_parity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-06 12:00:05.000000 error-parity-0.1.2/error_parity/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-06-06 12:00:05.000000 error-parity-0.1.2/error_parity/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-06-06 12:00:05.000000 error-parity-0.1.2/error_parity/cvxpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-06-06 12:00:05.000000 error-parity-0.1.2/error_parity/equal_odds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-06 12:00:05.000000 error-parity-0.1.2/error_parity/roc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:00:15.040356 error-parity-0.1.2/error_parity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-06 12:00:15.000000 error-parity-0.1.2/error_parity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-06 12:00:15.000000 error-parity-0.1.2/error_parity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:00:15.000000 error-parity-0.1.2/error_parity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-06 12:00:15.000000 error-parity-0.1.2/error_parity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 12:00:15.000000 error-parity-0.1.2/error_parity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:00:15.040356 error-parity-0.1.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 12:00:05.000000 error-parity-0.1.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 12:00:05.000000 error-parity-0.1.2/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-06 12:00:05.000000 error-parity-0.1.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:00:15.044356 error-parity-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-06 12:00:05.000000 error-parity-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:00:15.040356 error-parity-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:00:05.000000 error-parity-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-06 12:00:05.000000 error-parity-0.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-06 12:00:05.000000 error-parity-0.1.2/tests/test_equal_odds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:07:05.620197 error-parity-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-16 14:06:55.000000 error-parity-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 14:06:55.000000 error-parity-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-16 14:07:05.620197 error-parity-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-16 14:06:55.000000 error-parity-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:07:05.620197 error-parity-0.1.3/error_parity/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-06-16 14:06:55.000000 error-parity-0.1.3/error_parity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-16 14:06:55.000000 error-parity-0.1.3/error_parity/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-06-16 14:06:55.000000 error-parity-0.1.3/error_parity/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-06-16 14:06:55.000000 error-parity-0.1.3/error_parity/cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-06-16 14:06:55.000000 error-parity-0.1.3/error_parity/equal_odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-16 14:06:55.000000 error-parity-0.1.3/error_parity/roc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:07:05.620197 error-parity-0.1.3/error_parity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-16 14:07:05.000000 error-parity-0.1.3/error_parity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-16 14:07:05.000000 error-parity-0.1.3/error_parity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:07:05.000000 error-parity-0.1.3/error_parity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-16 14:07:05.000000 error-parity-0.1.3/error_parity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 14:07:05.000000 error-parity-0.1.3/error_parity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:07:05.620197 error-parity-0.1.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 14:06:55.000000 error-parity-0.1.3/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 14:06:55.000000 error-parity-0.1.3/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 14:06:55.000000 error-parity-0.1.3/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 14:07:05.620197 error-parity-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-16 14:06:55.000000 error-parity-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:07:05.620197 error-parity-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:06:55.000000 error-parity-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-16 14:06:55.000000 error-parity-0.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-16 14:06:55.000000 error-parity-0.1.3/tests/test_equal_odds.py
```

### Comparing `error-parity-0.1.2/LICENSE` & `error-parity-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.2/PKG-INFO` & `error-parity-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-parity
-Version: 0.1.2
+Version: 0.1.3
 Summary: Achieve error-rate parity between protected groups for any predictor
 Home-page: https://github.com/AndreFCruz/error-parity
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness,error-parity,equal-odds
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `error-parity-0.1.2/README.md` & `error-parity-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.2/error_parity/classifiers.py` & `error-parity-0.1.3/error_parity/classifiers.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.2/error_parity/cvxpy_utils.py` & `error-parity-0.1.3/error_parity/equal_odds.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,438 +1,440 @@
-"""A set of helper functions for using cvxpy.
+"""Solver for the relaxed equal odds problem.
+
+TODO
+- Add option for constraining only equality of FPR or TPR (currently it must be 
+both -> equal odds);
+- Add option for constraining equality of positive predictions (independence
+criterion, aka demographic parity);
+
 """
 import logging
-import operator
 from itertools import product
-from typing import Dict, Tuple, List
+from typing import Callable
 
 import numpy as np
-import cvxpy as cp
-from cvxpy.expressions.variable import Variable
-from cvxpy.expressions.expression import Expression
-
-from .roc_utils import calc_cost_of_point, compute_global_roc_from_groupwise
-
-
-def compute_line(p1, p2):
-    """Computes the slope and intercept of the line that passes
-    through the two given points.
-    
-    The intercept is the value at x=0!
-    (or NaN for vertical lines)
-    
-    For vertical lines just use the x-value of one of the points
-    to find the intercept at y=0.
-    """
-    p1x, p1y = p1
-    p2x, p2y = p2
-    if all(p1 == p2):
-        raise ValueError("Invalid points: p1==p2;")
-
-    # Vertical line
-    if np.isclose(p2x, p1x):
-        slope = np.inf
-        intercept = np.nan
-
-    # Diagonal or horizontal line
-    else:
-        slope = (p2y - p1y) / (p2x - p1x)
-        intercept = p1y - slope * p1x
-
-    return slope, intercept
-
-
-def compute_halfspace_inequality(p1, p2):
-    """Computes the halfspace inequality defined by the vector p1->p2;
-    -> input points must be in COUNTER CLOCK-WISE order (right-hand rule);
-    -> as such, the inequality enforces that points must lie on the right
-    of the line defined by the p1->p2 vector;
-    -> where "right" depends on the direction of the vector;
-    
-    Return
-    ------
-    Returns an array of size=(n_dims + 1), with format [A; b],
-    representing the inequality Ax + b <= 0.
-    """
-    slope, intercept = compute_line(p1, p2)
-
-    # Unpack the points for ease of use
-    p1x, p1y = p1
-    p2x, p2y = p2
-
-    # if slope is infinity, the constraint only applies to the values of x
-    # - the b intercept value will correspond to this value of x;
-    # - the sign of the constraint will depend on the vector p1->p2 pointing
-    # downards (x <= b) or upwards (x >= b);
-    if np.isinf(slope):
-        assert np.isclose(p1x, p2x)
-        
-        # Vector pointing downards? then, x >= b
-        if p2y < p1y:
-            return [-1, 0, p1x]
-        
-        # Vector pointing upwards? then, x <= b
-        elif p2y > p1y:
-            return [1, 0, -p1x]
-        
-    # elif slope is zero, the constraint only applies to the values of y
-    # - we still need to figure out the sign of y in the inequality;
-    # - may be y <= b or y >= b, depending on whether p1->p2 points
-    # rightwards (y <= b) or leftwards (y >= b);
-    elif np.isclose(slope, 0.0):
-        assert np.isclose(p1y, p2y)
-        assert np.isclose(p1y, intercept)
-
-        # Vector pointing leftwards? then, y <= b
-        if p2x < p1x:
-            return [0, 1, -p1y]
-        
-        # Vector pointing rightwards? then, y >= b
-        elif p2x > p1x:
-            return [0, -1, p1y]
-
-    # else, we have a standard diagonal line
-    else:
-        
-        # Vector points left?
-        # then, y <= mx + b <=> -mx + y - b <= 0
-        if p2x < p1x:
-            return [-slope, 1, -intercept]
-        
-        # Vector points right?
-        # then, y >= mx + b <=> mx - y + b <= 0
-        elif p2x > p1x:
-            return [slope, -1, intercept]
-        
-    logging.error(f"No constraint can be concluded from points p1={p1} and p2={p2};")
-    return [0, 0, 0]
+from sklearn.metrics import roc_curve
 
-
-def polygon_halfspace_inequalities(points: np.ndarray) -> np.ndarray:
-    """Parses the given points of a polygon, in COUNTER CLOCK-WISE order,
-    and constructs halfspaces from each consecutive pair of points.
-    
-    Output is in scipy.spatial.HalfspaceIntersection format;
-    i.e., an ndarray of format [A; b], for Ax + b <= 0.
+from .cvxpy_utils import compute_equal_odds_optimum
+from .roc_utils import (
+    roc_convex_hull,
+    plot_polygon_edges,
+    calc_cost_of_point,
+)
+from .classifiers import (
+    Classifier,
+    RandomizedClassifier,
+    EnsembleGroupwiseClassifiers,
+)
+
+
+class RelaxedEqualOdds(Classifier):
+    """Class to encapsulate all the logic needed to compute the optimal equal
+    odds classifier (with possibly relaxed constraints).
     """
-    # Array of shape (num_inequalities, num_dims + 1)
-    halfspaces = np.ndarray(shape=(len(points), points.shape[-1] + 1), dtype=float)
-
-    for i in range(len(points)):
-        p1 = np.ravel(points[i])
-        p2 = np.ravel(points[(i+1) % len(points)])
 
-        halfspaces[i] = compute_halfspace_inequality(p1, p2)
+    def __init__(
+            self,
+            predictor: Callable[[np.ndarray], np.ndarray],
+            tolerance: float,
+            false_pos_cost: float = 1.0,
+            false_neg_cost: float = 1.0,
+            max_roc_ticks: int = 1000,
+            seed: int = 42,
+            # distance: str = 'max',    # TODO: add option to use l1 or linf distances
+        ):
+        """Initializes the relaxed equal odds wrapper.
+
+        Parameters
+        ----------
+        predictor : callable[(np.ndarray), float]
+            A trained score predictor that takes in samples, X, in shape
+            (num_samples, num_features), and outputs real-valued scores, R, in
+            shape (num_samples,).
+        tolerance : float
+            The absolute tolerance for the equal odds fairness constraint.
+            Will allow for `tolerance` difference between group-wise ROC points.
+        false_pos_cost : float, optional
+            The cost of a FALSE POSITIVE error, by default 1.0.
+        false_neg_cost : float, optional
+            The cost of a FALSE NEGATIVE error, by default 1.0.
+        max_roc_ticks : int, optional
+            The maximum number of ticks (points) in each group's ROC, when
+            computing the optimal fair classifier, by default 1000.
+        seed : int
+            A random seed used for reproducibility when producing randomized
+            classifiers.
+        """
+        # Save arguments
+        self.predictor = predictor
+        self.tolerance = tolerance
+        self.false_pos_cost = false_pos_cost
+        self.false_neg_cost = false_neg_cost
+        self.max_roc_ticks = max_roc_ticks
+        self.seed = seed
+
+        # Initialize instance variables
+        self._all_roc_data: dict = None
+        self._all_roc_hulls: dict = None
+        self._groupwise_roc_points: np.ndarray = None
+        self._global_roc_point: np.ndarray = None
+        self._global_prevalence: float = None
+        self._realized_classifier: EnsembleGroupwiseClassifiers = None
+
+    @property
+    def groupwise_roc_points(self) -> np.ndarray:
+        return self._groupwise_roc_points
+
+    @property
+    def global_roc_point(self) -> np.ndarray:
+        return self._global_roc_point
+
+    def cost(
+            self,
+            false_pos_cost: float = None,
+            false_neg_cost: float = None,
+        ) -> float:
+        """Computes the theoretical cost of the solution found.
+
+        NOTE: use false_pos_cost==false_neg_cost==1 for the 0-1 loss (the 
+        standard error rate), which is equal to `1 - accuracy`.
+
+        Parameters
+        ----------
+        false_pos_cost : float, optional
+            The cost of a FALSE POSITIVE error, by default will take the value
+            given in the object's constructor.
+        false_neg_cost : float, optional
+            The cost of a FALSE NEGATIVE error, by default will take the value
+            given in the object's constructor.
+
+        Returns
+        -------
+        float
+            The cost of the solution found.
+        """
+        self._check_fit_status()
+        global_fpr, global_tpr = self.global_roc_point
+
+        return calc_cost_of_point(
+            fpr=global_fpr,
+            fnr=1 - global_tpr,
+            prevalence=self._global_prevalence,
+            false_pos_cost=false_pos_cost or self.false_pos_cost,
+            false_neg_cost=false_neg_cost or self.false_neg_cost,
+        )
     
-    return halfspaces
-
+    def constraint_violation(self) -> float:
+        """This method should be part of a common interface between different
+        relaxed-constraint classes.
+
+        Returns
+        -------
+        float
+            The fairness constraint violation.
+        """
+        return self.equal_odds_violation()
+
+    def equal_odds_violation(self) -> float:
+        """Computes the theoretical violation of the equal odds constraint 
+        (i.e., the maximum l-inf distance between the ROC point of any pair
+        of groups).
+
+        Returns
+        -------
+        float
+            The equal-odds constraint violation.
+        """
+        self._check_fit_status()
+
+        n_groups = len(self.groupwise_roc_points)
+
+        # Compute l-inf distance between each pair of groups
+        linf_constraint_violation = [
+            (np.linalg.norm(
+                self.groupwise_roc_points[i] - self.groupwise_roc_points[j],
+                ord=np.inf), (i, j))
+            for i, j in product(range(n_groups), range(n_groups))
+            if i < j
+        ]
+
+        # Return the maximum
+        max_violation, (groupA, groupB) = max(linf_constraint_violation)
+        logging.info(
+            f"Maximum fairness violation is between "
+            f"group={groupA} (p={self.groupwise_roc_points[groupA]}) and "
+            f"group={groupB} (p={self.groupwise_roc_points[groupB]});"
+        )
 
-def make_cvxpy_halfspace_inequality(p1, p2, cvxpy_point: Variable):
-    """Points sorted in counter clock-wise order!
-    """
-    x_coeff, y_coeff, b = compute_halfspace_inequality(p1, p2)
-    return np.array([x_coeff, y_coeff]) @ cvxpy_point + b <= 0
+        return max_violation
 
 
-def make_cvxpy_point_in_polygon_constraints(
-        polygon_vertices: np.ndarray,
-        cvxpy_point: Variable
-    ) -> Expression:
-    """Creates the set of cvxpy constraints that force the given cvxpy variables
-    to lie within the polygon defined by the given vertices.
-    
-    Polygon points sorted in COUNTER CLOCK-WISE order!
-    """
-    return [
-        make_cvxpy_halfspace_inequality(
-            polygon_vertices[i], polygon_vertices[(i+1) % len(polygon_vertices)],
-            cvxpy_point,
+    def fit(self, X: np.ndarray, y: np.ndarray, group: np.ndarray, y_scores: np.ndarray = None):
+        """Fit this predictor to achieve the (possibly relaxed) equal odds 
+        constraint on the provided data.
+
+        Parameters
+        ----------
+        X : np.ndarray
+            The input features.
+        y : np.ndarray
+            The input labels.
+        group : np.ndarray
+            The group membership of each sample.
+            Assumes groups are numbered [0, 1, ..., num_groups-1].
+        y_scores : np.ndarray, optional
+            The pre-computed model predictions on this data.
+        
+        Returns
+        -------
+        callable
+            Returns self.
+        """
+
+        # Compute group stats
+        self._global_prevalence = np.sum(y) / len(y)
+
+        unique_groups = np.unique(group)
+        num_groups = len(unique_groups)
+        if np.max(unique_groups) > num_groups-1:
+            raise ValueError(
+                f"Groups should be numbered starting at 0, and up to "
+                f"num_groups-1. Got {num_groups} groups, but max value is "
+                f"{np.max(unique_groups)} != num_groups-1 == {num_groups-1}."
+            )
+
+        # Relative group sizes for LN and LP samples
+        group_sizes_label_neg = np.array([
+            np.sum(1 - y[group == g]) for g in unique_groups
+        ])
+        group_sizes_label_pos = np.array([
+            np.sum(y[group == g]) for g in unique_groups
+        ])
+        assert np.sum(group_sizes_label_neg) + np.sum(group_sizes_label_pos) == len(y)
+
+        # Convert to relative sizes
+        group_sizes_label_neg = group_sizes_label_neg.astype(float) / np.sum(group_sizes_label_neg)
+        group_sizes_label_pos = group_sizes_label_pos.astype(float) / np.sum(group_sizes_label_pos)
+
+        # Compute group-wise ROC curves
+        if y_scores is None:
+            y_scores = self.predictor(X)
+
+        self._all_roc_data = dict()
+        for g in unique_groups:
+            group_filter = group == g
+
+            roc_curve_data = roc_curve(
+                y[group_filter],
+                y_scores[group_filter],
+            )
+
+            # Check if max_roc_ticks is exceeded
+            fpr, tpr, thrs = roc_curve_data
+            if self.max_roc_ticks is not None and len(fpr) > self.max_roc_ticks:
+                indices_to_keep = np.arange(0, len(fpr), len(fpr) / self.max_roc_ticks).astype(int)
+
+                # Bottom-left (0,0) and top-right (1,1) points must be kept
+                indices_to_keep[-1] = len(fpr) - 1
+                roc_curve_data = (fpr[indices_to_keep], tpr[indices_to_keep], thrs[indices_to_keep])
+
+            self._all_roc_data[g] = roc_curve_data
+
+        # Compute convex hull of each ROC curve
+        self._all_roc_hulls = dict()
+        for g in unique_groups:
+            group_fpr, group_tpr, _group_thresholds = self._all_roc_data[g]
+
+            curr_roc_points = np.stack((group_fpr, group_tpr), axis=1)
+            curr_roc_points = np.vstack((curr_roc_points, [1, 0]))  # Add point (1, 0) to ROC curve
+
+            self._all_roc_hulls[g] = roc_convex_hull(curr_roc_points)
+
+        # Find the group-wise optima that fulfill the fairness criteria
+        self._groupwise_roc_points, self._global_roc_point = compute_equal_odds_optimum(
+            groupwise_roc_hulls=self._all_roc_hulls,
+            fairness_tolerance=self.tolerance,
+            group_sizes_label_pos=group_sizes_label_pos,
+            group_sizes_label_neg=group_sizes_label_neg,
+            global_prevalence=self._global_prevalence,
+            false_positive_cost=self.false_pos_cost,
+            false_negative_cost=self.false_neg_cost,
         )
-        for i in range(len(polygon_vertices))
-    ]
 
+        # Construct each group-specific classifier
+        all_rand_clfs = {
+            g: RandomizedClassifier.construct_at_target_ROC(
+                predictor=self.predictor,
+                roc_curve_data=self._all_roc_data[g],
+                target_roc_point=self._groupwise_roc_points[g],
+                seed=self.seed,
+            )
+            for g in unique_groups
+        }
+
+        # Construct the global classifier (can be used for all groups)
+        self._realized_classifier = EnsembleGroupwiseClassifiers(group_to_clf=all_rand_clfs)
+        return self
+    
+    def _check_fit_status(self, raise_error: bool = True) -> bool:
+        """Checks whether this classifier has been fit on some data.
+        
+        Parameters
+        ----------
+        raise_error : bool, optional
+            Whether to raise an error if the classifier is uninitialized 
+            (otherwise will just return False), by default True.
+
+        Returns
+        -------
+        is_fit : bool
+            Whether the classifier was already fit on some data.
+
+        Raises
+        ------
+        RuntimeError
+            If `raise_error==True`, raises an error if the classifier is
+            uninitialized.
+        """
+        if self._realized_classifier is None:
+            if not raise_error:
+                return False
+
+            raise RuntimeError(
+                "There's nothing to plot: this classifier has not yet been "
+                "fitted to any data. Call clf.fit(...) before clf.plot().")
+
+        return True
+
+    def plot(
+            self,
+            plot_roc_curves: bool = False,
+            plot_roc_hulls: bool = True,
+            plot_group_optima: bool = True,
+            plot_group_triangulation: bool = True,
+            plot_global_optimum: bool = True,
+            plot_diagonal: bool = True,
+            plot_relaxation: bool = False,
+            group_name_map: dict = None,
+            figure = None,
+            **fig_kwargs,
+        ):
+        self._check_fit_status()
+    
+        from matplotlib import pyplot as plt
+        from matplotlib.patches import Rectangle
+        import seaborn as sns
+
+        n_groups = len(self._all_roc_hulls)
+
+        # Set group-wise colors and global color
+        palette = sns.color_palette(n_colors=n_groups + 1)
+        global_color = palette[0]
+        all_group_colors = palette[1:]
+
+        fig = figure if figure is not None else plt.figure(**fig_kwargs)
+
+        # For each group `idx`
+        for idx in range(n_groups):
+            group_ls = (['--', ':', '-.'] * (1 + n_groups // 3))[idx]
+            group_color = all_group_colors[idx]
+
+            # Plot group-wise (actual) ROC curves
+            if plot_roc_curves:
+                roc_points = np.stack(self._all_roc_data[idx], axis=1)[:, 0:2]
+                plot_polygon_edges(
+                    np.vstack((roc_points, [1, 0])),
+                    color=group_color,
+                    ls=group_ls,
+                    alpha=0.5,
+                )
+
+            # Plot group-wise ROC hulls
+            if plot_roc_hulls:
+                plot_polygon_edges(
+                    self._all_roc_hulls[idx],
+                    color=group_color,
+                    ls=group_ls,
+                )
+
+            # Plot group-wise fair optimum
+            group_optimum = self._groupwise_roc_points[idx]
+            if plot_group_optima:
+                plt.plot(
+                    group_optimum[0], group_optimum[1],
+                    label=group_name_map[idx] if group_name_map else f"group {idx}",
+                    color=group_color,
+                    marker="^", markersize=5,
+                    lw=0,
+                )
+
+            # Plot triangulation of target point
+            if plot_group_triangulation:
+                _weights, triangulated_points = RandomizedClassifier.find_points_for_target_ROC(
+                    roc_curve_data=self._all_roc_data[idx],
+                    target_roc_point=group_optimum,
+                )
+                plt.plot(
+                    triangulated_points[:, 0], triangulated_points[:, 1],
+                    color=group_color,
+                    marker='x', lw=0,
+                )
+
+                plt.fill(
+                    triangulated_points[:, 0], triangulated_points[:, 1],
+                    color=group_color,
+                    alpha=0.1,
+                )
+
+
+        # Plot global optimum
+        if plot_global_optimum:
+            plt.plot(
+                self._global_roc_point[0], self._global_roc_point[1],
+                label="global",
+                marker="*", color=global_color, alpha=0.6,
+                markersize=5, lw=0,
+            )
+
+        # Plot rectangle to visualize constraint relaxation
+        if plot_relaxation:
+
+            # Get rectangle points
+            min_x, max_x = np.min(self._groupwise_roc_points[:, 0]), np.max(self._groupwise_roc_points[:, 0])
+            min_y, max_y = np.min(self._groupwise_roc_points[:, 1]), np.max(self._groupwise_roc_points[:, 1])
+
+            # Draw relaxation rectangle
+            rect = Rectangle(
+                xy=(min_x, min_y),
+                width=max_x - min_x,
+                height=max_y - min_y,
+                facecolor="grey",
+                alpha=0.3,
+                label="relaxation",
+            )
+
+            # Add the patch to the Axes
+            ax = plt.gca()
+            ax.add_patch(rect)
+
+        # Plot diagonal
+        if plot_diagonal:
+            plt.plot(
+                [0, 1], [0, 1],
+                ls='--', color="grey", alpha=0.5,
+                label="random clf.",
+            )
+
+        # Set axis settings
+        plt.title(f"Solution to {self.tolerance}-relaxed equal odds optimum")
+        plt.xlabel("False Positive Rate")
+        plt.ylabel("True Positive Rate")
+
+        plt.legend(loc="lower right", borderaxespad=2)
 
+        # plt.show()
 
-def compute_equal_odds_optimum(
-        groupwise_roc_hulls: Dict[int, np.ndarray],
-        fairness_tolerance: float,
-        group_sizes_label_pos: np.ndarray,
-        group_sizes_label_neg: np.ndarray,
-        global_prevalence: float,
-        false_positive_cost: float = 1.,
-        false_negative_cost: float = 1.,
-    ) -> Tuple[np.ndarray, np.ndarray]:
-    """Computes the solution to finding the optimal fair (equal odds) classifier.
-
-    Can relax the equal odds constraint by some given tolerance.
-
-    Parameters
-    ----------
-    groupwise_roc_hulls : dict[int, np.ndarray]
-        A dict mapping each group to the convex hull of the group's ROC curve.
-        The convex hull is an np.array of shape (n_points, 2), containing the 
-        points that form the convex hull of the ROC curve, sorted in COUNTER
-        CLOCK-WISE order.
-    fairness_tolerance : float
-        A value for the tolerance when enforcing the equal odds fairness 
-        constraint, i.e., equality of TPR and FPR among groups.
-    group_sizes_label_pos : np.ndarray
-        The relative or absolute number of positive samples in each group.
-    group_sizes_label_neg : np.ndarray
-        The relative or absolute number of negative samples in each group.
-    global_prevalence : float
-        The global prevalence of positive samples.
-    false_positive_cost : float, optional
-        The cost of a FALSE POSITIVE error, by default 1.
-    false_negative_cost : float, optional
-        The cost of a FALSE NEGATIVE error, by default 1.
-
-    Returns
-    -------
-    (groupwise_roc_points, global_roc_point) : tuple[np.ndarray, np.ndarray]
-        A pair tuple, (<1>, <2>), containing:
-        1: an array with the group-wise ROC points for the solution.
-        2: an array with the single global ROC point for the solution.
-    """
-    n_groups = len(groupwise_roc_hulls)
-    assert n_groups == len(group_sizes_label_neg) == len(group_sizes_label_pos)
+    def __call__(self, X: np.ndarray, group: np.ndarray) -> int:
+        return self._realized_classifier(X, group)
 
-    # Group-wise ROC points
-    groupwise_roc_points_vars = [
-        cp.Variable(shape=2, name=f"ROC point for group {i}", nonneg=True)
-        for i in range(n_groups)
-    ]
-
-    # Define global ROC point as a linear combination of the group-wise ROC points
-    global_roc_point_var = cp.Variable(shape=2, name="Global ROC point", nonneg=True)
-    constraints = [
-        # Global FPR is the average of group FPRs weighted by LNs in each group
-        global_roc_point_var[0] == group_sizes_label_neg @ np.array([p[0] for p in groupwise_roc_points_vars]),
-
-        # Global TPR is the average of group TPRs weighted by LPs in each group
-        global_roc_point_var[1] == group_sizes_label_pos @ np.array([p[1] for p in groupwise_roc_points_vars]),
-    ]
-
-    # Relaxed equal odds constraints
-    # 1st option - CONSTRAINT FOR: l-inf distance between any two group's ROCs being less than epsilon
-    constraints += [
-        cp.norm_inf(groupwise_roc_points_vars[i] - groupwise_roc_points_vars[j]) <= fairness_tolerance
-        for i, j in product(range(n_groups), range(n_groups))
-        if i < j
-        # if i != j
-    ]
-
-    # Constraints for points in respective group-wise ROC curves
-    for idx in range(n_groups):
-        constraints += make_cvxpy_point_in_polygon_constraints(
-            polygon_vertices=groupwise_roc_hulls[idx],
-            cvxpy_point=groupwise_roc_points_vars[idx])
-
-    # Define cost function
-    obj = cp.Minimize(calc_cost_of_point(
-        fpr=global_roc_point_var[0],
-        fnr=1 - global_roc_point_var[1],
-        prevalence=global_prevalence,
-        false_pos_cost=false_positive_cost,
-        false_neg_cost=false_negative_cost,
-    ))
-
-    # Define cvxpy problem
-    prob = cp.Problem(obj, constraints)
-
-    # _plot_polygons([groupwise_roc_hulls[i] for i in range(n_groups)]) # NOTE: just for debugging
-
-    # Run solver
-    prob.solve(solver=cp.ECOS, abstol=1e-9, feastol=1e-9)
-    # NOTE: these tolerances are supposed to be smaller than the default np.isclose tolerances
-    # (useful when comparing if two points are the same, within the cvxpy accuracy tolerance)
-
-    # Log solution
-    logging.info(f"cvxpy solver took {prob.solver_stats.solve_time}s; status is {prob.status}.")
-
-    if prob.status not in ["infeasible", "unbounded"]:
-        # Otherwise, problem.value is inf or -inf, respectively.
-        logging.info(f"Optimal solution value: {prob.value}")
-        for variable in prob.variables():
-            logging.info(f"Variable {variable.name()}: value {variable.value}")
-    else:
-        import ipdb; ipdb.set_trace()   # TODO
-        raise ValueError(f"cvxpy problem has no solution; status={prob.status}")
-
-    groupwise_roc_points = np.vstack([p.value for p in groupwise_roc_points_vars])
-    global_roc_point = global_roc_point_var.value
-
-    # Sanity check solution cost
-    assert np.isclose(
-        prob.value,
-        calc_cost_of_point(
-            fpr=global_roc_point[0],
-            fnr=1-global_roc_point[1],
-            prevalence=global_prevalence,
-            false_pos_cost=false_positive_cost,
-            false_neg_cost=false_negative_cost,
-        ))
-
-    # Sanity check congruency between group-wise ROC points and global ROC point
-    global_roc_from_groupwise = compute_global_roc_from_groupwise(
-        groupwise_roc_points=groupwise_roc_points,
-        groupwise_label_pos_weight=group_sizes_label_pos,
-        groupwise_label_neg_weight=group_sizes_label_neg,
-    )
-    assert all(np.isclose(global_roc_from_groupwise, global_roc_point))
-
-    return groupwise_roc_points, global_roc_point
-
-
-def compute_equal_odds_unfair_optimum(
-        groupwise_roc_hulls: Dict[int, np.ndarray],
-        fairness_tolerance: float,
-        group_sizes_label_pos: np.ndarray,
-        group_sizes_label_neg: np.ndarray,
-        global_prevalence: float,
-        false_positive_cost: float = 1.,
-        false_negative_cost: float = 1.,
-    ) -> Tuple[np.ndarray, np.ndarray]:
-    """Computes the solution to finding the optimally UNFAIR (equal odds) classifier.
-
-    Can relax the equal odds constraint by some given tolerance.
-
-    Parameters
-    ----------
-    groupwise_roc_hulls : dict[int, np.ndarray]
-        A dict mapping each group to the convex hull of the group's ROC curve.
-        The convex hull is an np.array of shape (n_points, 2), containing the 
-        points that form the convex hull of the ROC curve, sorted in COUNTER
-        CLOCK-WISE order.
-    fairness_tolerance : float
-        A value for the tolerance when enforcing the equal odds fairness 
-        constraint, i.e., equality of TPR and FPR among groups.
-    group_sizes_label_pos : np.ndarray
-        The relative or absolute number of positive samples in each group.
-    group_sizes_label_neg : np.ndarray
-        The relative or absolute number of negative samples in each group.
-    global_prevalence : float
-        The global prevalence of positive samples.
-    false_positive_cost : float, optional
-        The cost of a FALSE POSITIVE error, by default 1.
-    false_negative_cost : float, optional
-        The cost of a FALSE NEGATIVE error, by default 1.
-
-    Returns
-    -------
-    (groupwise_roc_points, global_roc_point) : tuple[np.ndarray, np.ndarray]
-        A pair tuple, (<1>, <2>), containing:
-        1: an array with the group-wise ROC points for the solution.
-        2: an array with the single global ROC point for the solution.
-    """
-    raise NotImplementedError("Not currently implemented; the problem is not convex!")
-
-    logging.warning("> compute_equal_odds_unfair_optimum :: USE WITH CARE!")
-    n_groups = len(groupwise_roc_hulls)
-    assert n_groups == len(group_sizes_label_neg) == len(group_sizes_label_pos)
-
-    # Group-wise ROC points
-    groupwise_roc_points_vars = [
-        cp.Variable(shape=2, name=f"ROC point for group {i}", nonneg=True)
-        for i in range(n_groups)
-    ]
-
-    # Define global ROC point as a linear combination of the group-wise ROC points
-    global_roc_point_var = cp.Variable(shape=2, name="Global ROC point", nonneg=True)
-    constraints = [
-        # Global FPR is the average of group FPRs weighted by LNs in each group
-        global_roc_point_var[0] == group_sizes_label_neg @ np.array([p[0] for p in groupwise_roc_points_vars]),
-
-        # Global TPR is the average of group TPRs weighted by LPs in each group
-        global_roc_point_var[1] == group_sizes_label_pos @ np.array([p[1] for p in groupwise_roc_points_vars]),
-    ]
-
-    # Relaxed equal odds constraints (UNFAIR VERSION!)
-    groupwise_disparities = [
-        cp.norm_inf(groupwise_roc_points_vars[i] - groupwise_roc_points_vars[j])
-        for i, j in product(range(n_groups), range(n_groups))
-        if i < j
-    ]
-
-    # Constraint: the minimum disparity must be above `tolerance`
-    constraints.append(
-        cp.minimum(*groupwise_disparities) >= fairness_tolerance
-    )
-
-    # Constraints for points in respective group-wise ROC curves
-    for idx in range(n_groups):
-        constraints += make_cvxpy_point_in_polygon_constraints(
-            polygon_vertices=groupwise_roc_hulls[idx],
-            cvxpy_point=groupwise_roc_points_vars[idx])
-
-    # Define cost function
-    obj = cp.Minimize(calc_cost_of_point(
-        fpr=global_roc_point_var[0],
-        fnr=1 - global_roc_point_var[1],
-        prevalence=global_prevalence,
-        false_pos_cost=false_positive_cost,
-        false_neg_cost=false_negative_cost,
-    ))
-
-    # Define cvxpy problem
-    prob = cp.Problem(obj, constraints)
-
-    # _plot_polygons([groupwise_roc_hulls[i] for i in range(n_groups)]) # NOTE: just for debugging
-
-    # Run solver
-    prob.solve(solver=cp.ECOS, abstol=1e-9, feastol=1e-9)
-    # NOTE: these tolerances are supposed to be smaller than the default np.isclose tolerances
-    # (useful when comparing if two points are the same, within the cvxpy accuracy tolerance)
-
-    # Log solution
-    logging.info(f"cvxpy solver took {prob.solver_stats.solve_time}s; status is {prob.status}.")
-
-    if prob.status not in ["infeasible", "unbounded"]:
-        # Otherwise, problem.value is inf or -inf, respectively.
-        logging.info(f"Optimal solution value: {prob.value}")
-        for variable in prob.variables():
-            logging.info(f"Variable {variable.name()}: value {variable.value}")
-    else:
-        import ipdb; ipdb.set_trace()   # TODO
-        raise ValueError(f"cvxpy problem has no solution; status={prob.status}")
-
-    groupwise_roc_points = np.vstack([p.value for p in groupwise_roc_points_vars])
-    global_roc_point = global_roc_point_var.value
-
-    # Sanity check solution cost
-    assert np.isclose(
-        prob.value,
-        calc_cost_of_point(
-            fpr=global_roc_point[0],
-            fnr=1-global_roc_point[1],
-            prevalence=global_prevalence,
-            false_pos_cost=false_positive_cost,
-            false_neg_cost=false_negative_cost,
-        ))
-
-    # Sanity check congruency between group-wise ROC points and global ROC point
-    global_roc_from_groupwise = compute_global_roc_from_groupwise(
-        groupwise_roc_points=groupwise_roc_points,
-        groupwise_label_pos_weight=group_sizes_label_pos,
-        groupwise_label_neg_weight=group_sizes_label_neg,
-    )
-    assert all(np.isclose(global_roc_from_groupwise, global_roc_point))
-
-    return groupwise_roc_points, global_roc_point
-
-
-def _plot_polygons(polygons: List[np.ndarray]):
-    from matplotlib import pyplot as plt
-    fig = plt.figure(dpi=200, figsize=(5, 5))
-
-    for i, poly in enumerate(polygons):
-
-        # Plot ROC curve
-        plt.fill(
-            poly[:, 0], poly[:, 1],
-            alpha=0.2,
-            label=f"poly {i}",
-        )
-        
-        plt.legend(loc='lower right')
-    
-    plt.plot()
+    def predict(self, X: np.ndarray, group: np.ndarray) -> int:
+        return self(X, group)
```

### Comparing `error-parity-0.1.2/error_parity/roc_utils.py` & `error-parity-0.1.3/error_parity/roc_utils.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.2/error_parity.egg-info/PKG-INFO` & `error-parity-0.1.3/error_parity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-parity
-Version: 0.1.2
+Version: 0.1.3
 Summary: Achieve error-rate parity between protected groups for any predictor
 Home-page: https://github.com/AndreFCruz/error-parity
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness,error-parity,equal-odds
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `error-parity-0.1.2/setup.py` & `error-parity-0.1.3/setup.py`

 * *Files identical despite different names*

