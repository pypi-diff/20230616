# Comparing `tmp/example_wise_f1_maximizer-0.1.4-py3-none-any.whl.zip` & `tmp/example_wise_f1_maximizer-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7892 bytes, number of entries: 7
--rw-r--r--  2.0 unx       76 b- defN 23-Jun-13 14:55 example_wise_f1_maximizer/__init__.py
--rw-r--r--  2.0 unx    11802 b- defN 23-Jun-13 14:55 example_wise_f1_maximizer/meta_estimator.py
--rw-r--r--  2.0 unx     6574 b- defN 23-Jun-13 14:55 example_wise_f1_maximizer-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 14:55 example_wise_f1_maximizer-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       26 b- defN 23-Jun-13 14:55 example_wise_f1_maximizer-0.1.4.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-13 14:55 example_wise_f1_maximizer-0.1.4.dist-info/zip-safe
--rw-rw-r--  2.0 unx      667 b- defN 23-Jun-13 14:55 example_wise_f1_maximizer-0.1.4.dist-info/RECORD
-7 files, 19238 bytes uncompressed, 6678 bytes compressed:  65.3%
+Zip file size: 7894 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-16 11:15 example_wise_f1_maximizer/__init__.py
+-rw-r--r--  2.0 unx    11814 b- defN 23-Jun-16 11:15 example_wise_f1_maximizer/meta_estimator.py
+-rw-r--r--  2.0 unx     6574 b- defN 23-Jun-16 11:15 example_wise_f1_maximizer-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 11:15 example_wise_f1_maximizer-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-16 11:15 example_wise_f1_maximizer-0.1.5.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-16 11:15 example_wise_f1_maximizer-0.1.5.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      667 b- defN 23-Jun-16 11:15 example_wise_f1_maximizer-0.1.5.dist-info/RECORD
+7 files, 19250 bytes uncompressed, 6680 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: example_wise_f1_maximizer/__init__.py
 Comment: 
 
 Filename: example_wise_f1_maximizer/meta_estimator.py
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.4.dist-info/METADATA
+Filename: example_wise_f1_maximizer-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.4.dist-info/WHEEL
+Filename: example_wise_f1_maximizer-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.4.dist-info/top_level.txt
+Filename: example_wise_f1_maximizer-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.4.dist-info/zip-safe
+Filename: example_wise_f1_maximizer-0.1.5.dist-info/zip-safe
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.4.dist-info/RECORD
+Filename: example_wise_f1_maximizer-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## example_wise_f1_maximizer/meta_estimator.py

```diff
@@ -41,15 +41,15 @@
     :param max_cardinality: The maximium label cardinality observed in the training data or None, if the maximum label
                             cardinality is unknown
     :return:                An `np.ndarray` of shape (num_relevant_labels) that stores the indices of all relevant
                             labels in the label vector that maximizes the F1-measure
     """
     num_labels = p.shape[0]
     best_quality = p_0
-    best_indices = []
+    best_indices = np.asarray([])
 
     if w is None:
         w = create_gfm_weight_matrix(num_labels)
 
     f = np.matmul(p, w)
 
     for k in range(num_labels if max_cardinality is None else max_cardinality):
```

## Comparing `example_wise_f1_maximizer-0.1.4.dist-info/METADATA` & `example_wise_f1_maximizer-0.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example-wise-f1-maximizer
-Version: 0.1.4
+Version: 0.1.5
 Summary: A scikit-learn meta-estimator for multi-label classification that aims to maximize the example-wise F1 measure
 Home-page: https://github.com/mrapp-ke/ExampleWiseF1Maximizer
 Download-URL: https://github.com/mrapp-ke/ExampleWiseF1Maximizer/releases
 Author: Michael Rapp
 Author-email: michael.rapp.ml@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/mrapp-ke/ExampleWiseF1Maximizer/issues
```

## Comparing `example_wise_f1_maximizer-0.1.4.dist-info/RECORD` & `example_wise_f1_maximizer-0.1.5.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 example_wise_f1_maximizer/__init__.py,sha256=OtJDM5jsXq0XJ3SBlRJ3KYhN2yGWjvb5AKh34vkiCjU,76
-example_wise_f1_maximizer/meta_estimator.py,sha256=n2a56fwEW3WdJoSFxNs4LhKI3hEjd3ajW8NacXx4a1w,11802
-example_wise_f1_maximizer-0.1.4.dist-info/METADATA,sha256=WF0sEmi0-Yk_J2U-BOc9wKEMh5W5Mk_OK16Dv4OrLn8,6574
-example_wise_f1_maximizer-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-example_wise_f1_maximizer-0.1.4.dist-info/top_level.txt,sha256=Y3_hRTvgv8_1Vtj4I0HcBsiANUAJuFfeC2v0x06eRqo,26
-example_wise_f1_maximizer-0.1.4.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-example_wise_f1_maximizer-0.1.4.dist-info/RECORD,,
+example_wise_f1_maximizer/meta_estimator.py,sha256=KmLHIBdP2buSz5TYFIVfMwJPl0Z5LTq2KRW_QsxRzjQ,11814
+example_wise_f1_maximizer-0.1.5.dist-info/METADATA,sha256=_vs7-2uXDYb79mYVpwIBKDhyapFPpC9Yo2NkhKA7kB8,6574
+example_wise_f1_maximizer-0.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+example_wise_f1_maximizer-0.1.5.dist-info/top_level.txt,sha256=Y3_hRTvgv8_1Vtj4I0HcBsiANUAJuFfeC2v0x06eRqo,26
+example_wise_f1_maximizer-0.1.5.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+example_wise_f1_maximizer-0.1.5.dist-info/RECORD,,
```

