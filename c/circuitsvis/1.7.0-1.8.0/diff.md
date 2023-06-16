# Comparing `tmp/circuitsvis-1.7.0.tar.gz` & `tmp/circuitsvis-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitsvis-1.7.0.tar", max compression
+gzip compressed data, was "circuitsvis-1.8.0.tar", max compression
```

## Comparing `circuitsvis-1.7.0.tar` & `circuitsvis-1.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1068 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/LICENSE.txt
--rw-r--r--   0        0        0       61 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/README.md
--rw-r--r--   0        0        0      131 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/__init__.py
--rw-r--r--   0        0        0      799 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/activations.py
--rw-r--r--   0        0        0     2636 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/attention.py
--rw-r--r--   0        0        0      416 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/examples.py
--rw-r--r--   0        0        0     4050 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/render.py
--rw-r--r--   0        0        0        0 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/tests/snapshots/__init__.py
--rw-r--r--   0        0        0      583 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/tests/snapshots/snap_test_activations.py
--rw-r--r--   0        0        0      561 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/tests/snapshots/snap_test_attention.py
--rw-r--r--   0        0        0      493 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/tests/snapshots/snap_test_hello.py
--rw-r--r--   0        0        0      497 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/tests/snapshots/snap_test_render.py
--rw-r--r--   0        0        0      538 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/tests/snapshots/snap_test_tokens.py
--rw-r--r--   0        0        0      506 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/tests/test_activations.py
--rw-r--r--   0        0        0      480 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/tests/test_attention.py
--rw-r--r--   0        0        0      357 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/tests/test_hello.py
--rw-r--r--   0        0        0     1949 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/tests/test_render.py
--rw-r--r--   0        0        0      425 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/tests/test_tokens.py
--rw-r--r--   0        0        0     1266 2022-11-28 10:57:30.552419 circuitsvis-1.7.0/circuitsvis/tokens.py
--rw-r--r--   0        0        0      472 2022-11-28 10:57:53.411162 circuitsvis-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 circuitsvis-1.7.0/setup.py
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 circuitsvis-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/LICENSE.txt
+-rw-r--r--   0        0        0       61 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/README.md
+-rw-r--r--   0        0        0      131 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/__init__.py
+-rw-r--r--   0        0        0      799 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/activations.py
+-rw-r--r--   0        0        0     2795 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/attention.py
+-rw-r--r--   0        0        0      416 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/examples.py
+-rw-r--r--   0        0        0     4050 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/render.py
+-rw-r--r--   0        0        0        0 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/tests/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0      583 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/tests/snapshots/snap_test_activations.py
+-rw-r--r--   0        0        0      561 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/tests/snapshots/snap_test_attention.py
+-rw-r--r--   0        0        0      493 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/tests/snapshots/snap_test_hello.py
+-rw-r--r--   0        0        0      497 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/tests/snapshots/snap_test_render.py
+-rw-r--r--   0        0        0      538 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/tests/snapshots/snap_test_tokens.py
+-rw-r--r--   0        0        0      506 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/tests/test_activations.py
+-rw-r--r--   0        0        0      480 2022-11-28 19:16:10.018127 circuitsvis-1.8.0/circuitsvis/tests/test_attention.py
+-rw-r--r--   0        0        0      357 2022-11-28 19:16:10.022127 circuitsvis-1.8.0/circuitsvis/tests/test_hello.py
+-rw-r--r--   0        0        0     1949 2022-11-28 19:16:10.022127 circuitsvis-1.8.0/circuitsvis/tests/test_render.py
+-rw-r--r--   0        0        0      425 2022-11-28 19:16:10.022127 circuitsvis-1.8.0/circuitsvis/tests/test_tokens.py
+-rw-r--r--   0        0        0     1266 2022-11-28 19:16:10.022127 circuitsvis-1.8.0/circuitsvis/tokens.py
+-rw-r--r--   0        0        0      472 2022-11-28 19:16:30.427106 circuitsvis-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 circuitsvis-1.8.0/setup.py
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 circuitsvis-1.8.0/PKG-INFO
```

### Comparing `circuitsvis-1.7.0/LICENSE.txt` & `circuitsvis-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `circuitsvis-1.7.0/circuitsvis/activations.py` & `circuitsvis-1.8.0/circuitsvis/activations.py`

 * *Files identical despite different names*

### Comparing `circuitsvis-1.7.0/circuitsvis/attention.py` & `circuitsvis-1.8.0/circuitsvis/attention.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Attention visualisations"""
 from typing import List, Optional
 from circuitsvis.render import RenderedHTML, render
 import numpy as np
 
 
 def attention_patterns(
     tokens: List[str],
@@ -24,59 +25,63 @@
     return render(
         "AttentionPatterns",
         tokens=tokens,
         attention=attention_list,
         development_mode=development_mode
     )
 
+
 def attention_pattern(
     tokens: List[str],
     attention: np.ndarray,
-    min_value: Optional[float] = None,
+    development_mode: Optional[bool] = None,
     max_value: Optional[float] = None,
+    min_value: Optional[float] = None,
     negative_color: Optional[str] = None,
+    show_axis_labels: Optional[bool] = None,
     positive_color: Optional[str] = None,
-    development_mode: Optional[bool] = None
 ) -> RenderedHTML:
     """Attention Pattern
 
     Attention pattern from destination to source tokens. Displays a heatmap of
     attention values (hover to see the specific values).
 
     Args:
         tokens: List of tokens (e.g. `["A", "person"]`). Must be the same length
-        as the list of values. 
+        as the list of values.
         attention: Attention head activations of the shape [dest_tokens x
         src_tokens]
-        min_value: Minimum value. Used to determine how dark the token color is
-        when negative (i.e. based on how close it is to the minimum value).
         max_value: Maximum value. Used to determine how dark the token color is
         when positive (i.e. based on how close it is to the maximum value).
+        min_value: Minimum value. Used to determine how dark the token color is
+        when negative (i.e. based on how close it is to the minimum value).
         negative_color: Color for negative values. This can be any valid CSS
         color string. Be mindful of color blindness if not using the default
-        here. 
+        here.
+        show_axis_labels: Whether to show axis labels.
         positive_color: Color for positive values. This can be any valid CSS
         color string. Be mindful of color blindness if not using the default
-        here. 
+        here.
 
     Returns:
         Html: Attention pattern visualization
     """
     attention_list = attention.tolist()
-    
+
     kwargs = {
         "tokens": tokens,
         "attention": attention_list,
         "minValue": min_value,
         "maxValue": max_value,
         "negativeColor": negative_color,
         "positiveColor": positive_color,
-        "development_mode": development_mode,
+        "showAxisLabels": show_axis_labels,
     }
-    
+
     # Remove kwargs that are None
     kwargs = {k: v for k, v in kwargs.items() if v is not None}
-    
+
     return render(
         "AttentionPattern",
+        development_mode=development_mode,
         **kwargs
     )
```

### Comparing `circuitsvis-1.7.0/circuitsvis/render.py` & `circuitsvis-1.8.0/circuitsvis/render.py`

 * *Files identical despite different names*

### Comparing `circuitsvis-1.7.0/circuitsvis/tests/snapshots/snap_test_activations.py` & `circuitsvis-1.8.0/circuitsvis/tests/snapshots/snap_test_activations.py`

 * *Files identical despite different names*

### Comparing `circuitsvis-1.7.0/circuitsvis/tests/snapshots/snap_test_attention.py` & `circuitsvis-1.8.0/circuitsvis/tests/snapshots/snap_test_attention.py`

 * *Files identical despite different names*

### Comparing `circuitsvis-1.7.0/circuitsvis/tests/snapshots/snap_test_tokens.py` & `circuitsvis-1.8.0/circuitsvis/tests/snapshots/snap_test_tokens.py`

 * *Files identical despite different names*

### Comparing `circuitsvis-1.7.0/circuitsvis/tests/test_render.py` & `circuitsvis-1.8.0/circuitsvis/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `circuitsvis-1.7.0/circuitsvis/tokens.py` & `circuitsvis-1.8.0/circuitsvis/tokens.py`

 * *Files identical despite different names*

### Comparing `circuitsvis-1.7.0/PKG-INFO` & `circuitsvis-1.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitsvis
-Version: 1.7.0
+Version: 1.8.0
 Summary: Mechanistic Interpretability Visualizations
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

