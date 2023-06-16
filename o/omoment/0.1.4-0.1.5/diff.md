# Comparing `tmp/omoment-0.1.4.tar.gz` & `tmp/omoment-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omoment-0.1.4.tar", last modified: Sun May  7 18:16:01 2023, max compression
+gzip compressed data, was "omoment-0.1.5.tar", last modified: Fri Jun 16 12:35:34 2023, max compression
```

## Comparing `omoment-0.1.4.tar` & `omoment-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0      726 2022-10-29 21:19:55.803580 omoment-0.1.4/.github/workflows/builddoc.yaml
--rw-r--r--   0        0        0     1050 2022-10-29 20:55:31.453855 omoment-0.1.4/.github/workflows/pytest.yaml
--rw-r--r--   0        0        0     1889 2022-10-29 20:12:44.215687 omoment-0.1.4/.gitignore
--rw-r--r--   0        0        0     1074 2022-10-28 11:01:20.166050 omoment-0.1.4/LICENSE
--rw-r--r--   0        0        0     4468 2023-05-07 18:13:50.450480 omoment-0.1.4/README.rst
--rw-r--r--   0        0        0      775 2023-05-07 16:09:56.817015 omoment-0.1.4/changelog.rst
--rw-r--r--   0        0        0       74 2022-10-29 12:10:17.934348 omoment-0.1.4/doc/api/obase.rst
--rw-r--r--   0        0        0       96 2022-10-29 11:38:32.206847 omoment-0.1.4/doc/api/omean.rst
--rw-r--r--   0        0        0      105 2022-10-29 11:40:59.911415 omoment-0.1.4/doc/api/omeanvar.rst
--rw-r--r--   0        0        0       93 2023-05-07 17:57:42.608666 omoment-0.1.4/doc/api/oreg.rst
--rw-r--r--   0        0        0     1730 2022-10-29 20:09:04.562822 omoment-0.1.4/doc/conf.py
--rw-r--r--   0        0        0      487 2022-10-29 11:45:13.624391 omoment-0.1.4/doc/index.rst
--rw-r--r--   0        0        0     4252 2023-05-07 18:06:45.621680 omoment-0.1.4/omoment/__init__.py
--rw-r--r--   0        0        0     4818 2022-11-28 20:16:37.926867 omoment-0.1.4/omoment/obase.py
--rw-r--r--   0        0        0    10368 2023-05-07 16:03:54.284352 omoment-0.1.4/omoment/omean.py
--rw-r--r--   0        0        0    11924 2023-05-07 17:12:45.887940 omoment-0.1.4/omoment/omeanvar.py
--rw-r--r--   0        0        0    11339 2023-05-07 16:59:00.962464 omoment-0.1.4/omoment/oreg.py
--rw-r--r--   0        0        0       17 2023-05-07 15:54:42.967358 omoment-0.1.4/omoment/version.py
--rw-r--r--   0        0        0     1205 2022-11-28 18:35:53.908523 omoment-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       13 2022-10-28 11:24:51.428266 omoment-0.1.4/requirements.txt
--rw-r--r--   0        0        0       19 2023-05-07 17:50:35.679906 omoment-0.1.4/test_requirements.txt
--rw-r--r--   0        0        0     5539 2023-01-21 09:48:09.410903 omoment-0.1.4/tests/test_omean.py
--rw-r--r--   0        0        0     7566 2023-01-21 09:46:18.206640 omoment-0.1.4/tests/test_omeanvar.py
--rw-r--r--   0        0        0    11003 2023-05-07 17:56:42.696559 omoment-0.1.4/tests/test_oreg.py
--rw-r--r--   0        0        0     5522 1970-01-01 00:00:00.000000 omoment-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      726 2022-10-29 21:19:55.803580 omoment-0.1.5/.github/workflows/builddoc.yaml
+-rw-r--r--   0        0        0     1050 2022-10-29 20:55:31.453855 omoment-0.1.5/.github/workflows/pytest.yaml
+-rw-r--r--   0        0        0     1889 2022-10-29 20:12:44.215687 omoment-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1074 2022-10-28 11:01:20.166050 omoment-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4468 2023-05-07 18:13:50.450480 omoment-0.1.5/README.rst
+-rw-r--r--   0        0        0      913 2023-06-16 12:33:34.573313 omoment-0.1.5/changelog.rst
+-rw-r--r--   0        0        0       74 2022-10-29 12:10:17.934348 omoment-0.1.5/doc/api/obase.rst
+-rw-r--r--   0        0        0       96 2022-10-29 11:38:32.206847 omoment-0.1.5/doc/api/omean.rst
+-rw-r--r--   0        0        0      105 2022-10-29 11:40:59.911415 omoment-0.1.5/doc/api/omeanvar.rst
+-rw-r--r--   0        0        0      102 2023-06-16 12:33:34.573313 omoment-0.1.5/doc/api/ominmax.rst
+-rw-r--r--   0        0        0       93 2023-05-07 17:57:42.608666 omoment-0.1.5/doc/api/oreg.rst
+-rw-r--r--   0        0        0     1730 2022-10-29 20:09:04.562822 omoment-0.1.5/doc/conf.py
+-rw-r--r--   0        0        0      487 2022-10-29 11:45:13.624391 omoment-0.1.5/doc/index.rst
+-rw-r--r--   0        0        0     4292 2023-06-16 12:33:34.573313 omoment-0.1.5/omoment/__init__.py
+-rw-r--r--   0        0        0     4674 2023-06-16 12:33:34.573313 omoment-0.1.5/omoment/obase.py
+-rw-r--r--   0        0        0    10426 2023-06-16 12:33:34.573313 omoment-0.1.5/omoment/omean.py
+-rw-r--r--   0        0        0    11924 2023-05-07 17:12:45.887940 omoment-0.1.5/omoment/omeanvar.py
+-rw-r--r--   0        0        0     5426 2023-06-16 12:33:34.573313 omoment-0.1.5/omoment/ominmax.py
+-rw-r--r--   0        0        0    11339 2023-05-07 16:59:00.962464 omoment-0.1.5/omoment/oreg.py
+-rw-r--r--   0        0        0       17 2023-06-16 12:33:34.573313 omoment-0.1.5/omoment/version.py
+-rw-r--r--   0        0        0     1205 2022-11-28 18:35:53.908523 omoment-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       13 2022-10-28 11:24:51.428266 omoment-0.1.5/requirements.txt
+-rw-r--r--   0        0        0       19 2023-05-07 17:50:35.679906 omoment-0.1.5/test_requirements.txt
+-rw-r--r--   0        0        0     5539 2023-01-21 09:48:09.410903 omoment-0.1.5/tests/test_omean.py
+-rw-r--r--   0        0        0     7566 2023-01-21 09:46:18.206640 omoment-0.1.5/tests/test_omeanvar.py
+-rw-r--r--   0        0        0     5351 2023-06-16 12:33:34.573313 omoment-0.1.5/tests/test_ominmax.py
+-rw-r--r--   0        0        0    11003 2023-05-07 17:56:42.696559 omoment-0.1.5/tests/test_oreg.py
+-rw-r--r--   0        0        0     5522 1970-01-01 00:00:00.000000 omoment-0.1.5/PKG-INFO
```

### Comparing `omoment-0.1.4/.github/workflows/builddoc.yaml` & `omoment-0.1.5/.github/workflows/builddoc.yaml`

 * *Files identical despite different names*

### Comparing `omoment-0.1.4/.github/workflows/pytest.yaml` & `omoment-0.1.5/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `omoment-0.1.4/.gitignore` & `omoment-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `omoment-0.1.4/LICENSE` & `omoment-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `omoment-0.1.4/README.rst` & `omoment-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `omoment-0.1.4/changelog.rst` & `omoment-0.1.5/changelog.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+Version 0.1.5 (2023-06-16)
+--------------------------
+
+* Added `OMinMax` class for calculation of minimum, maximum and number of points.
+
 Version 0.1.4 (2023-05-07)
 --------------------------
 
 * Added `OReg` class for handling an univariate regression.
 * Added convenience method `of_frame` for quick computation of pandas dataframes.
 * Explicit `compute` override to play well with intellisense.
```

### Comparing `omoment-0.1.4/doc/conf.py` & `omoment-0.1.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `omoment-0.1.4/omoment/__init__.py` & `omoment-0.1.5/omoment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,10 +99,11 @@
 """
 
 from .version import VERSION as __version__
 from .obase import OBase, HandlingInvalid
 from .omean import OMean
 from .omeanvar import OMeanVar
 from .oreg import OReg
+from .ominmax import OMinMax
 
-__all__ = ['OBase', 'OMean', 'OMeanVar', 'OReg', 'HandlingInvalid']
+__all__ = ['OBase', 'OMean', 'OMeanVar', 'OReg', 'OMinMax', 'HandlingInvalid']
 __author__ = 'Tomas Protivinsky'
```

### Comparing `omoment-0.1.4/omoment/obase.py` & `omoment-0.1.5/omoment/obase.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,18 +26,15 @@
     - string representation
     - conversion objects to dictionaries or tuples (convenient for serialization)
     - combination of objects via addition
     - copying of objects
 
     """
     @abstractmethod
-    def update(self,
-               x: Union[Number, np.ndarray, pd.Series],
-               w: Optional[Union[Number, np.ndarray, pd.Series]] = None,
-               handling_invalid: HandlingInvalid = HandlingInvalid.Drop) -> OBase:
+    def update(self, x: Union[Number, np.ndarray, pd.Series], *args, **kwargs) -> OBase:
         """
         Update the object based on new data. Subclasses have to implement how to aggregate the new data.
         """
         ...
 
     @classmethod
     def compute(cls, *args, **kwargs):
```

### Comparing `omoment-0.1.4/omoment/omean.py` & `omoment-0.1.5/omoment/omean.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
                  mean: Number = np.nan,
                  weight: Number = 0,
                  handling_invalid: HandlingInvalid = HandlingInvalid.Drop) -> OMean:
         """Creates a representation of mean and weight of a part of data. To estimate OMean directly
         from data, use OMean.compute class method.
 
         Raises:
+            TypeError: if mean or weight are not numbers.
             ValueError: if handling invalid is HandlingInvalid.Raise (or 'raise') and invalid values are provided
              in the constructor (such as negative weight or positive weight and infinite mean).
 
         """
         if not (isinstance(mean, Number) and isinstance(weight, Number)):
             raise TypeError(f'Mean and weight have to be numbers in OMean, provided type(mean) ='
                             f' {type(mean).__name__}, type(weight) = {type(weight).__name__}.')
```

### Comparing `omoment-0.1.4/omoment/omeanvar.py` & `omoment-0.1.5/omoment/omeanvar.py`

 * *Files identical despite different names*

### Comparing `omoment-0.1.4/omoment/oreg.py` & `omoment-0.1.5/omoment/oreg.py`

 * *Files identical despite different names*

### Comparing `omoment-0.1.4/pyproject.toml` & `omoment-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `omoment-0.1.4/tests/test_omean.py` & `omoment-0.1.5/tests/test_omean.py`

 * *Files identical despite different names*

### Comparing `omoment-0.1.4/tests/test_omeanvar.py` & `omoment-0.1.5/tests/test_omeanvar.py`

 * *Files identical despite different names*

### Comparing `omoment-0.1.4/tests/test_oreg.py` & `omoment-0.1.5/tests/test_oreg.py`

 * *Files identical despite different names*

### Comparing `omoment-0.1.4/PKG-INFO` & `omoment-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omoment
-Version: 0.1.4
+Version: 0.1.5
 Summary: OMoment package calculates moments of statistical distributions (means, variances, covariance) in online or
 Keywords: statistics,mean,variance,distributed,estimation,efficient,additive
 Author-email: Tomas Protivinsky <tomas.protivinsky@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

