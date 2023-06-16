# Comparing `tmp/bornrule-0.2.1.tar.gz` & `tmp/bornrule-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bornrule-0.2.1.tar", max compression
+gzip compressed data, was "bornrule-0.2.2.tar", max compression
```

## Comparing `bornrule-0.2.1.tar` & `bornrule-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    35149 2022-02-17 15:07:25.514146 bornrule-0.2.1/LICENSE
--rw-r--r--   0        0        0      379 2023-03-28 13:25:05.932038 bornrule-0.2.1/README.min.md
--rw-r--r--   0        0        0       62 2022-11-22 14:45:52.298028 bornrule-0.2.1/bornrule/__init__.py
--rw-r--r--   0        0        0    15645 2022-11-22 12:34:29.983982 bornrule-0.2.1/bornrule/born.py
--rw-r--r--   0        0        0       70 2022-03-18 22:15:10.938536 bornrule-0.2.1/bornrule/sql/__init__.py
--rw-r--r--   0        0        0    15208 2023-06-14 21:08:12.886183 bornrule-0.2.1/bornrule/sql/born.py
--rw-r--r--   0        0        0    18607 2023-06-14 21:39:35.203788 bornrule-0.2.1/bornrule/sql/database.py
--rw-r--r--   0        0        0      120 2023-03-14 10:07:39.656021 bornrule-0.2.1/bornrule/sql/postgresql.py
--rw-r--r--   0        0        0      541 2023-03-14 10:07:46.660157 bornrule-0.2.1/bornrule/sql/sqlite.py
--rw-r--r--   0        0        0       42 2022-02-18 12:44:02.006465 bornrule-0.2.1/bornrule/torch/__init__.py
--rw-r--r--   0        0        0     3111 2023-03-28 13:39:18.510897 bornrule-0.2.1/bornrule/torch/born.py
--rw-r--r--   0        0        0      534 2023-06-14 21:40:32.787890 bornrule-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 bornrule-0.2.1/setup.py
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 bornrule-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-02-17 15:07:25.514146 bornrule-0.2.2/LICENSE
+-rw-r--r--   0        0        0      379 2023-03-28 13:25:05.932038 bornrule-0.2.2/README.min.md
+-rw-r--r--   0        0        0       62 2022-11-22 14:45:52.298028 bornrule-0.2.2/bornrule/__init__.py
+-rw-r--r--   0        0        0    15645 2022-11-22 12:34:29.983982 bornrule-0.2.2/bornrule/born.py
+-rw-r--r--   0        0        0       70 2022-03-18 22:15:10.938536 bornrule-0.2.2/bornrule/sql/__init__.py
+-rw-r--r--   0        0        0    14893 2023-06-16 13:59:08.479958 bornrule-0.2.2/bornrule/sql/born.py
+-rw-r--r--   0        0        0    18607 2023-06-16 12:56:51.226468 bornrule-0.2.2/bornrule/sql/database.py
+-rw-r--r--   0        0        0      120 2023-03-14 10:07:39.656021 bornrule-0.2.2/bornrule/sql/postgresql.py
+-rw-r--r--   0        0        0      541 2023-03-14 10:07:46.660157 bornrule-0.2.2/bornrule/sql/sqlite.py
+-rw-r--r--   0        0        0       42 2022-02-18 12:44:02.006465 bornrule-0.2.2/bornrule/torch/__init__.py
+-rw-r--r--   0        0        0     3111 2023-03-28 13:39:18.510897 bornrule-0.2.2/bornrule/torch/born.py
+-rw-r--r--   0        0        0      536 2023-06-16 14:12:37.855634 bornrule-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 bornrule-0.2.2/PKG-INFO
```

### Comparing `bornrule-0.2.1/LICENSE` & `bornrule-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bornrule-0.2.1/bornrule/born.py` & `bornrule-0.2.2/bornrule/born.py`

 * *Files identical despite different names*

### Comparing `bornrule-0.2.1/bornrule/sql/born.py` & `bornrule-0.2.2/bornrule/sql/born.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 try:
     from sqlalchemy import create_engine, String, Integer
 
 except ModuleNotFoundError:
     raise ModuleNotFoundError(
         "SQLAlchemy required but not installed. "
-        "Please install SQLAlchemy with: pip install sqlalchemy")
+        "Please install SQLAlchemy with e.g. -> pip install sqlalchemy")
 
 from .sqlite import SQLite
 from .postgresql import PostgreSQL
 
 
 class BornClassifierSQL:
     """SQL implementation of Born's Classifier
@@ -113,56 +113,48 @@
             Model's hyper-parameters `a`, `b`, `h`.
 
         """
         if self.params is None:
             with self.db.connect() as con:
                 self.params = self.db.read_params(con)
 
-        return self.params
+        return self.params.copy()
 
-    def set_params(self, **kwargs):
+    def set_params(self, **params):
         """Set parameters
 
         Parameters
         ----------
-        **kwargs
+        **params
              Model's hyper-parameters: `a` (>0), `b` (>=0), and `h` (>=0).
 
         """
-        params = self.get_params()
-        params.update(kwargs)
+        p = self.get_params()
+        p.update(params)
 
-        valid = self.db.default_params.keys()
-        invalid = set(params.keys()) - set(valid)
-        if invalid:
-            raise ValueError(
-                f"Invalid parameter(s): {', '.join(invalid)}. "
-                f"Valid parameters are: {', '.join(valid)}."
-            )
-
-        if params['a'] <= 0:
+        if p['a'] <= 0:
             raise ValueError(
                 "The parameter 'a' must be strictly positive."
             )
 
-        if params['b'] < 0:
+        if p['b'] < 0:
             raise ValueError(
                 "The parameter 'b' must be non-negative."
             )
 
-        if params['h'] < 0:
+        if p['h'] < 0:
             raise ValueError(
                 "The parameter 'h' must be non-negative."
             )
 
         with self.db.connect() as con:
             with con.begin():
                 self.db.check_editable(con)
-                self.db.write_params(con, **params)
-                self.params = params
+                self.db.write_params(con, **p)
+                self.params = p
 
     def fit(self, X, y, sample_weight=None):
         """Fit the classifier according to the training data X, y
 
         Parameters
         ----------
         X : list of dict of length n_samples
```

### Comparing `bornrule-0.2.1/bornrule/sql/database.py` & `bornrule-0.2.2/bornrule/sql/database.py`

 * *Files identical despite different names*

### Comparing `bornrule-0.2.1/bornrule/sql/sqlite.py` & `bornrule-0.2.2/bornrule/sql/sqlite.py`

 * *Files identical despite different names*

### Comparing `bornrule-0.2.1/bornrule/torch/born.py` & `bornrule-0.2.2/bornrule/torch/born.py`

 * *Files identical despite different names*

### Comparing `bornrule-0.2.1/pyproject.toml` & `bornrule-0.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "bornrule"
-version = "0.2.1"
+version = "0.2.2"
 license = "GPL-3.0-or-later"
 description = "Classification with Born's rule"
 authors = ["Emanuele Guidotti <emanuele.guidotti@unine.ch>"]
 readme = "README.min.md"
 repository = "https://github.com/eguidotti/bornrule"
 documentation = "https://bornrule.eguidotti.com"
 
 [tool.poetry.dependencies]
-python = ">=3.6"
+python = ">=3.6.1"
 numpy = ">=1.19.5"
 scipy = ">=1.5.4"
 pandas = ">=1.1.5"
 scikit-learn = ">=0.24.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `bornrule-0.2.1/PKG-INFO` & `bornrule-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: bornrule
-Version: 0.2.1
+Version: 0.2.2
 Summary: Classification with Born's rule
 Home-page: https://github.com/eguidotti/bornrule
 License: GPL-3.0-or-later
 Author: Emanuele Guidotti
 Author-email: emanuele.guidotti@unine.ch
-Requires-Python: >=3.6
+Requires-Python: >=3.6.1
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.19.5)
 Requires-Dist: pandas (>=1.1.5)
```

