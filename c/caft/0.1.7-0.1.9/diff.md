# Comparing `tmp/caft-0.1.7.tar.gz` & `tmp/caft-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caft-0.1.7.tar", last modified: Fri May 19 15:46:13 2023, max compression
+gzip compressed data, was "caft-0.1.9.tar", last modified: Fri Jun 16 16:44:28 2023, max compression
```

## Comparing `caft-0.1.7.tar` & `caft-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:46:13.330235 caft-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 15:46:00.000000 caft-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-19 15:46:00.000000 caft-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-19 15:46:13.330235 caft-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-19 15:46:00.000000 caft-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:46:13.330235 caft-0.1.7/caft/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 15:46:00.000000 caft-0.1.7/caft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-19 15:46:00.000000 caft-0.1.7/caft/affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-05-19 15:46:00.000000 caft-0.1.7/caft/equation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-05-19 15:46:00.000000 caft-0.1.7/caft/npoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:46:13.330235 caft-0.1.7/caft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-19 15:46:13.000000 caft-0.1.7/caft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-19 15:46:13.000000 caft-0.1.7/caft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:46:13.000000 caft-0.1.7/caft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-19 15:46:13.000000 caft-0.1.7/caft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 15:46:13.000000 caft-0.1.7/caft.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:46:13.330235 caft-0.1.7/img/
--rw-r--r--   0 runner    (1001) docker     (123)    42606 2023-05-19 15:46:00.000000 caft-0.1.7/img/affine_transformed_scatter.png
--rw-r--r--   0 runner    (1001) docker     (123)    22050 2023-05-19 15:46:00.000000 caft-0.1.7/img/fx_scatter_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-19 15:46:00.000000 caft-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-19 15:46:13.330235 caft-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-19 15:46:00.000000 caft-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:46:13.330235 caft-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:46:00.000000 caft-0.1.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:46:13.330235 caft-0.1.7/tests/tests_caft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:46:00.000000 caft-0.1.7/tests/tests_caft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-19 15:46:00.000000 caft-0.1.7/tests/tests_caft/test_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-19 15:46:00.000000 caft-0.1.7/tests/tests_caft/test_equation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-19 15:46:00.000000 caft-0.1.7/tests/tests_caft/test_npoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:44:28.582640 caft-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-16 16:44:17.000000 caft-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-16 16:44:17.000000 caft-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 16:44:17.000000 caft-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-16 16:44:28.582640 caft-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-06-16 16:44:17.000000 caft-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:44:28.582640 caft-0.1.9/caft/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 16:44:17.000000 caft-0.1.9/caft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-06-16 16:44:17.000000 caft-0.1.9/caft/affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-16 16:44:17.000000 caft-0.1.9/caft/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-06-16 16:44:17.000000 caft-0.1.9/caft/odr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-16 16:44:17.000000 caft-0.1.9/caft/regressors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-16 16:44:17.000000 caft-0.1.9/caft/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:44:28.582640 caft-0.1.9/caft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-16 16:44:28.000000 caft-0.1.9/caft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-16 16:44:28.000000 caft-0.1.9/caft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:44:28.000000 caft-0.1.9/caft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 16:44:28.000000 caft-0.1.9/caft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 16:44:28.000000 caft-0.1.9/caft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:44:28.582640 caft-0.1.9/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    42606 2023-06-16 16:44:17.000000 caft-0.1.9/img/affine_transformed_scatter.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22050 2023-06-16 16:44:17.000000 caft-0.1.9/img/fx_scatter_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-16 16:44:17.000000 caft-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-16 16:44:28.586640 caft-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-16 16:44:17.000000 caft-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:44:28.582640 caft-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:44:17.000000 caft-0.1.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:44:28.582640 caft-0.1.9/tests/tests_caft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:44:17.000000 caft-0.1.9/tests/tests_caft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-16 16:44:17.000000 caft-0.1.9/tests/tests_caft/test_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-16 16:44:17.000000 caft-0.1.9/tests/tests_caft/test_odr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-16 16:44:17.000000 caft-0.1.9/tests/tests_caft/test_regressors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-16 16:44:17.000000 caft-0.1.9/tests/tests_caft/test_utils.py
```

### Comparing `caft-0.1.7/LICENSE` & `caft-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `caft-0.1.7/PKG-INFO` & `caft-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caft
-Version: 0.1.7
+Version: 0.1.9
 Summary: Continuous Affine Feature Transformations for feature mapping.
 Home-page: https://github.com/joshdunnlime/caft
 Author: Joshua Dunn
 Author-email: joshua.t.dunn@hotmail.co.uk
 Project-URL: Documentation, https://github.com/joshdunnlime/caft
 Project-URL: Bug Reports, https://github.com/joshdunnlime/caft/issues
 Project-URL: Source Code, https://github.com/joshdunnlime/caft
@@ -51,15 +51,15 @@
 The main pattern is as follows.
 
 ```python
 import sympy as sp
 import numpy as np
 import matplotlib.pyplot as plt
 
-from caft.equation import SympyODRegressor, ODRegressor
+from caft.odr import SympyODRegressor, ODRegressor
 from caft.affine import ContinuousAffineFeatureTransformer
 
 np.random.seed(42)
 
 n = 10000
 
 # Generate data with some natural noise (not errors)
```

### Comparing `caft-0.1.7/README.md` & `caft-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 The main pattern is as follows.
 
 ```python
 import sympy as sp
 import numpy as np
 import matplotlib.pyplot as plt
 
-from caft.equation import SympyODRegressor, ODRegressor
+from caft.odr import SympyODRegressor, ODRegressor
 from caft.affine import ContinuousAffineFeatureTransformer
 
 np.random.seed(42)
 
 n = 10000
 
 # Generate data with some natural noise (not errors)
```

### Comparing `caft-0.1.7/caft/equation.py` & `caft-0.1.9/caft/odr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Equation based regressors."""
 
 import sympy as sp
-
+from scipy.odr import ODR, Data, Model, exponential, multilinear, polynomial
 from sklearn.base import BaseEstimator, RegressorMixin
-from sklearn.utils.validation import check_is_fitted, column_or_1d
-from scipy.odr import ODR, Model, Data, polynomial, exponential, multilinear
+from sklearn.utils import check_array, check_X_y
+from sklearn.utils.validation import check_is_fitted
 
 
 class SympyODRegressor(BaseEstimator, RegressorMixin):
     """Fit a Sympy equation to data using Orthogonal Distance Regression
 
     Typically used on data that is known to have uncertainty in both the x and
     y variables and when a rough estimate for the function shape is known.
 
     Parameters
     ----------
     equation : str
-        A string that can be parsed by sympy.
+        A string that can be parsed by sympy. By default, a linear model.
     beta0 : dict
-        A dictionary of initial values for the parameters in the equation.
+        A dictionary of initial values for the parameters in the equation. By
+        default, linear model parameters, `a=1` and `c=0`.
     wrt : str, optional
         The variable to fit the equation to, by default "x".
 
     Attributes
     ----------
     sp_equation : sympy expression
         The sympy expression parsed from the equation string.
@@ -56,37 +57,44 @@
     >>> sfr = SympyFunctionRegressor(equation, beta0={"a": 3, "b": 5})
     >>> sfr.fit(X, y)
     >>> y_pred = sfr.predict(X)
 
     >>> sfr.beta
     array([1.60245274, 9.89329657])...
     """
-    def __init__(self, equation: str, beta0: dict, wrt: str = "x",):
+
+    def __init__(
+        self,
+        equation: str = "a*x + c",
+        beta0: dict = {"a": 1, "c": 0},
+        wrt: str = "x",
+    ):
         self.equation = equation
         self.wrt = wrt
         self.beta0 = beta0
 
     def fit(self, X, y):
         """Fit the sympy equation to the data.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             The training input samples.
         y : array-like of shape (n_samples,)
             The target values (real numbers in regression).
         """
-        X_ = column_or_1d(X)
-        y_ = column_or_1d(y)
+        X_, y_ = check_X_y(X, y)
+        X_ = X_[:, 0]
+
         self.sp_equation = sp.parsing.sympy_parser.parse_expr(self.equation)
         self.wrt_symbol = sp.Symbol(self.wrt)
         free_symbols_auto = self.sp_equation.free_symbols
-        self.free_symbols_user = (
-            [sp.Symbol(s) for s in self.beta0.keys()] + [self.wrt_symbol]
-        )
+        self.free_symbols_user = [sp.Symbol(s) for s in self.beta0.keys()] + [
+            self.wrt_symbol
+        ]
 
         if free_symbols_auto != set(self.free_symbols_user):
             raise ValueError("beta0 keys must match equation free symbols")
 
         self.subs_beta0 = [(sp.Symbol(k), v) for k, v in self.beta0.items()]
 
         self.mod = Model(self.odr_function)
@@ -117,15 +125,16 @@
 
         Returns
         -------
         y : ndarray of shape (n_samples,)
             The predicted values.
         """
         check_is_fitted(self, ["beta"])
-        X_ = column_or_1d(X)
+        X_ = check_array(X)
+
         return sp.lambdify(self.wrt_symbol, self.sp_equation)(X_).reshape(-1)
 
     def odr_function(self, beta, x):
         """The function to optimize with scipy.odr."""
         odr_fx_subs = self.sp_equation.subs(
             [(s, b) for s, b in zip(self.free_symbols_user, beta)]
         )
@@ -146,18 +155,20 @@
         for details.
     degree : int, optional
         The degree of the polynomial to fit, by default 3. If model_type is not
         polynomial, this parameter is ignored.
     wrt : str, optional
         The variable to fit the equation with respect to, by default "x".
     """
+
     def __init__(
-            self, model_type: str = "polynomial",
-            degree: int = 3,
-            wrt: str = "x",
+        self,
+        model_type: str = "polynomial",
+        degree: int = 3,
+        wrt: str = "x",
     ):
         self.model_type = model_type
         self.wrt = wrt
         self.degree = degree
 
     def fit(self, X, y):
         """Fit a scipy.odr Model to the data.
@@ -165,16 +176,16 @@
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             The training input samples.
         y : array-like of shape (n_samples,)
             The target values (real numbers in regression).
         """
-        X_ = column_or_1d(X)
-        y_ = column_or_1d(y)
+        X_, y_ = check_X_y(X, y)
+        X_ = X_[:, 0]
 
         if self.model_type == "polynomial":
             self.mod = polynomial(self.degree)
         elif self.model_type == "exponential":
             self.mod = exponential()
         elif self.model_type == "multilinear":
             self.mod = multilinear()
@@ -187,27 +198,24 @@
         self.od = ODR(dat, self.mod)
         self.coefs_ = self.od.run()
         self.beta = self.coefs_.beta
 
         self.wrt_symbol = sp.Symbol(self.wrt)
 
         if self.model_type == "polynomial":
-            self.sp_equation = (
-                sp
-                .Poly
-                .from_list(self.beta[::-1], self.wrt_symbol)
-                .as_expr()
-            )
+            self.sp_equation = sp.Poly.from_list(
+                self.beta[::-1], self.wrt_symbol
+            ).as_expr()
         elif self.model_type == "exponential":
-            self.sp_equation = (
-                self.beta[0] + sp.exp(self.beta[1] * self.wrt_symbol)
+            self.sp_equation = self.beta[0] + sp.exp(
+                self.beta[1] * self.wrt_symbol
             )
         elif self.model_type == "multilinear":
-            self.sp_equation = (
-                sum([b * self.wrt_symbol**i for i, b in enumerate(self.beta)])
+            self.sp_equation = sum(
+                [b * self.wrt_symbol**i for i, b in enumerate(self.beta)]
             )
         return self
 
     def predict(self, X):
         """Predict regression target for X.
 
         Parameters
@@ -217,9 +225,10 @@
 
         Returns
         -------
         y : ndarray of shape (n_samples,)
             The predicted values.
         """
         check_is_fitted(self, ["beta"])
-        X_ = column_or_1d(X)
+        X_ = check_array(X)
+
         return sp.lambdify(self.wrt_symbol, self.sp_equation)(X_).reshape(-1)
```

### Comparing `caft-0.1.7/caft.egg-info/PKG-INFO` & `caft-0.1.9/caft.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caft
-Version: 0.1.7
+Version: 0.1.9
 Summary: Continuous Affine Feature Transformations for feature mapping.
 Home-page: https://github.com/joshdunnlime/caft
 Author: Joshua Dunn
 Author-email: joshua.t.dunn@hotmail.co.uk
 Project-URL: Documentation, https://github.com/joshdunnlime/caft
 Project-URL: Bug Reports, https://github.com/joshdunnlime/caft/issues
 Project-URL: Source Code, https://github.com/joshdunnlime/caft
@@ -51,15 +51,15 @@
 The main pattern is as follows.
 
 ```python
 import sympy as sp
 import numpy as np
 import matplotlib.pyplot as plt
 
-from caft.equation import SympyODRegressor, ODRegressor
+from caft.odr import SympyODRegressor, ODRegressor
 from caft.affine import ContinuousAffineFeatureTransformer
 
 np.random.seed(42)
 
 n = 10000
 
 # Generate data with some natural noise (not errors)
```

### Comparing `caft-0.1.7/img/affine_transformed_scatter.png` & `caft-0.1.9/img/affine_transformed_scatter.png`

 * *Files identical despite different names*

### Comparing `caft-0.1.7/img/fx_scatter_plot.png` & `caft-0.1.9/img/fx_scatter_plot.png`

 * *Files identical despite different names*

### Comparing `caft-0.1.7/setup.py` & `caft-0.1.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,51 @@
+"""Package setup for caft."""
+
 import setuptools
 
-with open('README.md', 'r', encoding='utf-8') as fh:
+with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-short_name = 'caft'
+short_name = "caft"
 author = "Joshua Dunn"
 git_author = "joshdunnlime"
 
 setuptools.setup(
-    name='caft',
+    name="caft",
     author=author,
-    author_email='joshua.t.dunn@hotmail.co.uk',
+    author_email="joshua.t.dunn@hotmail.co.uk",
     description=(
-        'Continuous Affine Feature Transformations for feature mapping.'
+        "Continuous Affine Feature Transformations for feature mapping."
     ),
-    keywords='feature-engineering feature-mapping, anomaly-detection',
+    keywords="feature-engineering feature-mapping, anomaly-detection",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    url=f'https://github.com/{git_author}/{short_name}',
+    long_description_content_type="text/markdown",
+    url=f"https://github.com/{git_author}/{short_name}",
     project_urls={
-        'Documentation': f'https://github.com/{git_author}/{short_name}',
-        'Bug Reports':
-        f'https://github.com/{git_author}/{short_name}/issues',
-        'Source Code': f'https://github.com/{git_author}/{short_name}',
-        # 'Funding': '',
-        # 'Say Thanks!': '',
+        "Documentation": f"https://github.com/{git_author}/{short_name}",
+        "Bug Reports": f"https://github.com/{git_author}/{short_name}/issues",
+        "Source Code": f"https://github.com/{git_author}/{short_name}",
     },
     packages=setuptools.find_packages(),
     classifiers=[
         # see https://pypi.org/classifiers/
-        'Development Status :: 5 - Production/Stable',
-
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3 :: Only',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3 :: Only",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
     ],
-    python_requires='>=3.8',
+    python_requires=">=3.8",
     install_requires=[
-        'sympy>=1.11.0',
-        'pandas>=1.3.0',
-        'scikit-learn>=1.0.0',
+        "sympy>=1.11.0",
+        "pandas>=1.3.0",
+        "scikit-learn>=1.0.0",
     ],
     extras_require={
-        'dev': ['check-manifest'],
+        "dev": ["check-manifest"],
         # 'test': ['coverage'],
     },
-    # entry_points={
-    #     'console_scripts': [  # This can provide executable scripts
-    #         'run=examplepy:main',
-    # You can execute `run` in bash to run `main()` in src/examplepy/__init__.py
-    #     ],
-    # },
 )
```

### Comparing `caft-0.1.7/tests/tests_caft/test_equation.py` & `caft-0.1.9/tests/tests_caft/test_odr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 """Test equation regressors."""
 
-import pytest
-
 import numpy as np
+import pytest
 import sympy as sp
 
-from caft.equation import SympyODRegressor, ODRegressor
+from caft.odr import ODRegressor, SympyODRegressor
 
 
 def sympy_approx_equals(eq1, eq2):
     """Check if two sympy equations are equal. Either an exact match, sp.solve
     returns empty list, or has root 0 in solved list.
 
     """
     solved_eq = sp.solve(eq1 - eq2)
     if (0 in solved_eq) | (solved_eq == []):
         return True
     else:
         return False
 
 
-def test_sympy_function_regressor():
+def test_SympyODRegressor():
     """Test sympy function regressor."""
     sodr = SympyODRegressor("a*x**2 + b", beta0={"a": 3, "b": 5})
     X = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]).reshape(-1, 1)
-    y = 5 * X ** 2 + 10
+    y = (5 * X**2 + 10).reshape(-1)
     sodr.fit(X, y)
     y_pred = sodr.predict(X)
-    wrt = sp.Symbol('x')
+    wrt = sp.Symbol("x")
 
-    check_sp_equation = sodr.beta[0] * wrt ** 2 + sodr.beta[1]
+    check_sp_equation = sodr.beta[0] * wrt**2 + sodr.beta[1]
 
     assert sodr.beta == pytest.approx([5, 10], rel=1e-3)
     assert sodr.sp_equation == check_sp_equation
     assert sodr.wrt_symbol == sp.Symbol("x")
     assert y_pred == pytest.approx(y.reshape(-1), rel=1e-3)
 
 
 def test_odregressor():
     """Test odr regressor."""
-    odr = ODRegressor(degree=2, wrt='s')
+    odr = ODRegressor(degree=2, wrt="s")
     X = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]).reshape(-1, 1)
-    y = (5 * X ** 2) + (2 * X) + 10
+    y = (5 * X**2) + (2 * X) + 10
     odr.fit(X, y)
     y_pred = odr.predict(X)
-    wrt = sp.Symbol('s')
+    wrt = sp.Symbol("s")
 
     check_sp_equation = (
-        odr.beta[2] * wrt ** 2
-        + (odr.beta[1] * wrt)
-        + odr.beta[0]
+        odr.beta[2] * wrt**2 + (odr.beta[1] * wrt) + odr.beta[0]
     )
 
     assert odr.beta == pytest.approx([10, 2, 5], rel=1e-3)
     assert odr.sp_equation == check_sp_equation
     assert odr.wrt_symbol == sp.Symbol("s")
     assert y_pred == pytest.approx(y.reshape(-1), rel=1e-3)
```

