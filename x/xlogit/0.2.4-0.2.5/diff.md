# Comparing `tmp/xlogit-0.2.4.tar.gz` & `tmp/xlogit-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlogit-0.2.4.tar", last modified: Mon Nov 28 23:39:54 2022, max compression
+gzip compressed data, was "xlogit-0.2.5.tar", last modified: Fri Jun 16 08:15:00 2023, max compression
```

## Comparing `xlogit-0.2.4.tar` & `xlogit-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxr-xr-x   0 das       (1000) das       (1000)        0 2022-11-28 23:39:54.072516 xlogit-0.2.4/
--rw-rw-r--   0 das       (1000) das       (1000)    35149 2022-03-23 01:15:13.000000 xlogit-0.2.4/LICENSE
--rw-r--r--   0 das       (1000) das       (1000)    10329 2022-11-28 23:39:54.072516 xlogit-0.2.4/PKG-INFO
--rw-r--r--   0 das       (1000) das       (1000)     9987 2022-07-05 05:52:11.000000 xlogit-0.2.4/README.rst
--rw-r--r--   0 das       (1000) das       (1000)       38 2022-11-28 23:39:54.072516 xlogit-0.2.4/setup.cfg
--rw-r--r--   0 das       (1000) das       (1000)      872 2022-11-28 23:36:47.000000 xlogit-0.2.4/setup.py
-drwxr-xr-x   0 das       (1000) das       (1000)        0 2022-11-28 23:39:54.072516 xlogit-0.2.4/xlogit/
--rw-rw-r--   0 das       (1000) das       (1000)      112 2022-03-23 01:15:13.000000 xlogit-0.2.4/xlogit/__init__.py
--rwxr-xr-x   0 das       (1000) das       (1000)    10858 2022-11-28 22:51:03.000000 xlogit-0.2.4/xlogit/_choice_model.py
--rwxrwxr-x   0 das       (1000) das       (1000)     1983 2022-06-01 05:55:09.000000 xlogit-0.2.4/xlogit/_device.py
--rw-r--r--   0 das       (1000) das       (1000)     3098 2022-06-25 05:00:58.000000 xlogit-0.2.4/xlogit/_optimize.py
--rw-r--r--   0 das       (1000) das       (1000)    31216 2022-10-20 21:53:38.000000 xlogit-0.2.4/xlogit/mixed_logit.py
--rw-r--r--   0 das       (1000) das       (1000)    13220 2022-10-20 21:53:21.000000 xlogit-0.2.4/xlogit/multinomial_logit.py
--rwxrwxr-x   0 das       (1000) das       (1000)     3851 2022-06-25 05:23:47.000000 xlogit-0.2.4/xlogit/utils.py
-drwxr-xr-x   0 das       (1000) das       (1000)        0 2022-11-28 23:39:54.072516 xlogit-0.2.4/xlogit.egg-info/
--rw-r--r--   0 das       (1000) das       (1000)    10329 2022-11-28 23:39:54.000000 xlogit-0.2.4/xlogit.egg-info/PKG-INFO
--rw-r--r--   0 das       (1000) das       (1000)      352 2022-11-28 23:39:54.000000 xlogit-0.2.4/xlogit.egg-info/SOURCES.txt
--rw-r--r--   0 das       (1000) das       (1000)        1 2022-11-28 23:39:54.000000 xlogit-0.2.4/xlogit.egg-info/dependency_links.txt
--rw-r--r--   0 das       (1000) das       (1000)        1 2022-06-25 05:41:05.000000 xlogit-0.2.4/xlogit.egg-info/not-zip-safe
--rw-r--r--   0 das       (1000) das       (1000)       27 2022-11-28 23:39:54.000000 xlogit-0.2.4/xlogit.egg-info/requires.txt
--rw-r--r--   0 das       (1000) das       (1000)        7 2022-11-28 23:39:54.000000 xlogit-0.2.4/xlogit.egg-info/top_level.txt
+drwxr-xr-x   0 das       (1000) das       (1000)        0 2023-06-16 08:15:00.841240 xlogit-0.2.5/
+-rw-rw-r--   0 das       (1000) das       (1000)    35149 2022-03-23 01:15:13.000000 xlogit-0.2.5/LICENSE
+-rw-r--r--   0 das       (1000) das       (1000)    10383 2023-06-16 08:15:00.841240 xlogit-0.2.5/PKG-INFO
+-rw-r--r--   0 das       (1000) das       (1000)    10041 2023-06-16 08:10:09.000000 xlogit-0.2.5/README.rst
+-rw-r--r--   0 das       (1000) das       (1000)       38 2023-06-16 08:15:00.841240 xlogit-0.2.5/setup.cfg
+-rw-r--r--   0 das       (1000) das       (1000)      872 2023-06-16 08:10:30.000000 xlogit-0.2.5/setup.py
+drwxr-xr-x   0 das       (1000) das       (1000)        0 2023-06-16 08:15:00.841240 xlogit-0.2.5/tests/
+-rwxr-xr-x   0 das       (1000) das       (1000)     3091 2022-06-11 06:21:48.000000 xlogit-0.2.5/tests/test__choice_model.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     1761 2022-06-01 07:42:17.000000 xlogit-0.2.5/tests/test__device.py
+-rw-rw-r--   0 das       (1000) das       (1000)     5214 2023-06-16 03:10:49.000000 xlogit-0.2.5/tests/test_mixed_logit.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     3518 2023-06-16 03:10:49.000000 xlogit-0.2.5/tests/test_multinomial_logit.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     1940 2022-06-25 05:26:01.000000 xlogit-0.2.5/tests/test_utils.py
+drwxr-xr-x   0 das       (1000) das       (1000)        0 2023-06-16 08:15:00.841240 xlogit-0.2.5/xlogit/
+-rw-rw-r--   0 das       (1000) das       (1000)      112 2022-03-23 01:15:13.000000 xlogit-0.2.5/xlogit/__init__.py
+-rwxrwxr-x   0 das       (1000) das       (1000)    11115 2023-06-16 03:10:49.000000 xlogit-0.2.5/xlogit/_choice_model.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     1983 2022-06-01 05:55:09.000000 xlogit-0.2.5/xlogit/_device.py
+-rw-r--r--   0 das       (1000) das       (1000)     3098 2022-06-25 05:00:58.000000 xlogit-0.2.5/xlogit/_optimize.py
+-rw-rw-r--   0 das       (1000) das       (1000)    31981 2023-06-16 03:12:49.000000 xlogit-0.2.5/xlogit/mixed_logit.py
+-rw-rw-r--   0 das       (1000) das       (1000)    13869 2023-06-16 03:13:14.000000 xlogit-0.2.5/xlogit/multinomial_logit.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     3851 2022-06-25 05:23:47.000000 xlogit-0.2.5/xlogit/utils.py
+drwxr-xr-x   0 das       (1000) das       (1000)        0 2023-06-16 08:15:00.841240 xlogit-0.2.5/xlogit.egg-info/
+-rw-r--r--   0 das       (1000) das       (1000)    10383 2023-06-16 08:15:00.000000 xlogit-0.2.5/xlogit.egg-info/PKG-INFO
+-rw-r--r--   0 das       (1000) das       (1000)      480 2023-06-16 08:15:00.000000 xlogit-0.2.5/xlogit.egg-info/SOURCES.txt
+-rw-r--r--   0 das       (1000) das       (1000)        1 2023-06-16 08:15:00.000000 xlogit-0.2.5/xlogit.egg-info/dependency_links.txt
+-rw-r--r--   0 das       (1000) das       (1000)        1 2022-06-25 05:41:05.000000 xlogit-0.2.5/xlogit.egg-info/not-zip-safe
+-rw-r--r--   0 das       (1000) das       (1000)       27 2023-06-16 08:15:00.000000 xlogit-0.2.5/xlogit.egg-info/requires.txt
+-rw-r--r--   0 das       (1000) das       (1000)        7 2023-06-16 08:15:00.000000 xlogit-0.2.5/xlogit.egg-info/top_level.txt
```

### Comparing `xlogit-0.2.4/LICENSE` & `xlogit-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.4/PKG-INFO` & `xlogit-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlogit
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python package for GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/arteagac/xlogit
 Author: Cristian Arteaga
 Author-email: cristiandavidarteaga@gmail.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
@@ -13,15 +13,15 @@
 ===========================================================================================
 xlogit: A Python Package for GPU-Accelerated Estimation of Mixed Logit Models.
 ===========================================================================================
 
 .. image:: https://raw.githubusercontent.com/arteagac/xlogit/master/docs/xlogit_logo_1000px.png
   :width: 400
 
-|Travis| |Coverage| |Community| |Docs| |PyPi| |License|
+|Build| |Coverage| |Community| |Docs| |PyPi| |License|
 
 .. _Mixed Logit: https://xlogit.readthedocs.io/en/latest/api/mixed_logit.html
 .. _Multinomial Logit: https://xlogit.readthedocs.io/en/latest/api/multinomial_logit.html
 
 `Examples <https://xlogit.readthedocs.io/en/latest/examples.html>`__ | `Docs <https://xlogit.readthedocs.io/en/latest/index.html>`__ | `Installation <https://xlogit.readthedocs.io/en/latest/install.html>`__ | `API Reference <https://xlogit.readthedocs.io/en/latest/api/index.html>`__ | `Contributing <https://xlogit.readthedocs.io/en/latest/contributing.html>`__ | `Contact <https://xlogit.readthedocs.io/en/latest/index.html#contact>`__ 
 
 Quick start
@@ -173,16 +173,16 @@
         pages = {100339},
         year = {2022},
         issn = {1755-5345},
         doi = {https://doi.org/10.1016/j.jocm.2021.100339},
     }
 
 
-.. |Travis| image:: https://travis-ci.com/arteagac/xlogit.svg?branch=master
-   :target: https://travis-ci.com/arteagac/xlogit
+.. |Build| image:: https://github.com/arteagac/xlogit/actions/workflows/python-tests.yml/badge.svg
+   :target: https://github.com/arteagac/xlogit/actions/workflows/python-tests.yml
 
 .. |Docs| image:: https://readthedocs.org/projects/xlogit/badge/?version=latest
    :target: https://xlogit.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. |Community| image:: https://badges.gitter.im/xlogit/community.svg
    :target: https://gitter.im/xlogit/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
```

### Comparing `xlogit-0.2.4/README.rst` & `xlogit-0.2.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ===========================================================================================
 xlogit: A Python Package for GPU-Accelerated Estimation of Mixed Logit Models.
 ===========================================================================================
 
 .. image:: https://raw.githubusercontent.com/arteagac/xlogit/master/docs/xlogit_logo_1000px.png
   :width: 400
 
-|Travis| |Coverage| |Community| |Docs| |PyPi| |License|
+|Build| |Coverage| |Community| |Docs| |PyPi| |License|
 
 .. _Mixed Logit: https://xlogit.readthedocs.io/en/latest/api/mixed_logit.html
 .. _Multinomial Logit: https://xlogit.readthedocs.io/en/latest/api/multinomial_logit.html
 
 `Examples <https://xlogit.readthedocs.io/en/latest/examples.html>`__ | `Docs <https://xlogit.readthedocs.io/en/latest/index.html>`__ | `Installation <https://xlogit.readthedocs.io/en/latest/install.html>`__ | `API Reference <https://xlogit.readthedocs.io/en/latest/api/index.html>`__ | `Contributing <https://xlogit.readthedocs.io/en/latest/contributing.html>`__ | `Contact <https://xlogit.readthedocs.io/en/latest/index.html#contact>`__ 
 
 Quick start
@@ -161,16 +161,16 @@
         pages = {100339},
         year = {2022},
         issn = {1755-5345},
         doi = {https://doi.org/10.1016/j.jocm.2021.100339},
     }
 
 
-.. |Travis| image:: https://travis-ci.com/arteagac/xlogit.svg?branch=master
-   :target: https://travis-ci.com/arteagac/xlogit
+.. |Build| image:: https://github.com/arteagac/xlogit/actions/workflows/python-tests.yml/badge.svg
+   :target: https://github.com/arteagac/xlogit/actions/workflows/python-tests.yml
 
 .. |Docs| image:: https://readthedocs.org/projects/xlogit/badge/?version=latest
    :target: https://xlogit.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. |Community| image:: https://badges.gitter.im/xlogit/community.svg
    :target: https://gitter.im/xlogit/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
```

### Comparing `xlogit-0.2.4/setup.py` & `xlogit-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import codecs
 
 with codecs.open('README.rst', encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='xlogit',
-                 version='0.2.4',
+                 version='0.2.5',
                  description='A Python package for GPU-accelerated ' +
                  'estimation of mixed logit models.',
                  long_description=long_description,
                  long_description_content_type="text/x-rst",
                  url='https://github.com/arteagac/xlogit',
                  author='Cristian Arteaga',
                  author_email='cristiandavidarteaga@gmail.com',
```

### Comparing `xlogit-0.2.4/xlogit/_choice_model.py` & `xlogit-0.2.5/xlogit/_choice_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,26 +39,27 @@
         self.pvalues = None
         self.loglikelihood = None
         self.total_fun_eval = 0
         self.verbose = 1
         self.robust = False
 
     def _as_array(self, X, y, varnames, alts, isvars, ids, weights, panels,
-                  avail, scale_factor):
+                  avail, scale_factor, addit):
         X = np.asarray(X)
         y = np.asarray(y)
         varnames = np.asarray(varnames) if varnames is not None else None
         alts = np.asarray(alts) if alts is not None else None
         isvars = np.asarray(isvars) if isvars is not None else None
         ids = np.asarray(ids) if ids is not None else None
         weights = np.asarray(weights) if weights is not None else None
         panels = np.asarray(panels) if panels is not None else None
         avail = np.asarray(avail) if avail is not None else None
         scale_factor = np.asarray(scale_factor) if scale_factor is not None else None
-        return X, y, varnames, alts, isvars, ids, weights, panels, avail, scale_factor
+        addit = np.asarray(addit) if addit is not None else None
+        return X, y, varnames, alts, isvars, ids, weights, panels, avail, scale_factor, addit
 
     def _pre_fit(self, alts, varnames, isvars, base_alt,
                  fit_intercept, maxiter):
         self._reset_attributes()
         self._fit_start_time = time()
         self._isvars = [] if isvars is None else list(isvars)
         self._asvars = [v for v in varnames if v not in self._isvars]
@@ -247,16 +248,18 @@
         print("Significance:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1")
         print("")
         print("Log-Likelihood= {:.3f}".format(self.loglikelihood))
         print("AIC= {:.3f}".format(self.aic))
         print("BIC= {:.3f}".format(self.bic))
 
 
-def diff_nonchosen_chosen(X, y, scale, avail):
+def diff_nonchosen_chosen(X, y, scale, addit, avail):
     # Setup Xd as Xij - Xi* (difference between non-chosen and chosen alternatives)
     N, J, K = X.shape
     X, y = X.reshape(N*J, K), y.astype(bool).reshape(N*J, )
     Xd =  X[~y, :].reshape(N, J - 1, K) - X[y, :].reshape(N, 1, K)
     scale = scale.reshape(N*J, ) if scale is not None else None
     scale_d = scale[~y].reshape(N, J - 1) - scale[y].reshape(N, 1) if scale is not None else None
+    addit = addit.reshape(N*J, ) if addit is not None else None
+    addit_d = addit[~y].reshape(N, J - 1) - addit[y].reshape(N, 1) if addit is not None else None
     avail = avail.reshape(N*J)[~y].reshape(N, J - 1) if avail is not None else None
-    return Xd, scale_d, avail
+    return Xd, scale_d, addit_d, avail
```

### Comparing `xlogit-0.2.4/xlogit/_device.py` & `xlogit-0.2.5/xlogit/_device.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.4/xlogit/_optimize.py` & `xlogit-0.2.5/xlogit/_optimize.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.4/xlogit/mixed_logit.py` & `xlogit-0.2.5/xlogit/mixed_logit.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         super(MixedLogit, self).__init__()
         self._rvidx = None  # Index of random variables (True when random var)
         self._rvdist = None  # List of mixing distributions of rand vars
 
     def fit(self, X, y, varnames, alts, ids, randvars, isvars=None, weights=None, avail=None,  panels=None,
             base_alt=None, fit_intercept=False, init_coeff=None, maxiter=2000, random_state=None, n_draws=1000,
             halton=True, verbose=1, batch_size=None, halton_opts=None, tol_opts=None, robust=False, num_hess=False,
-            scale_factor=None, optim_method="BFGS", mnl_init=True):
+            scale_factor=None, optim_method="BFGS", mnl_init=True, addit=None):
         """Fit Mixed Logit models.
 
         Parameters
         ----------
         X : array-like, shape (n_samples*n_alts, n_variables)
             Input data for explanatory variables in long format
 
@@ -154,14 +154,17 @@
         batch_size : int, default=None
             Size of batches used to avoid GPU memory overflow.
             
         scale_factor : array-like, shape (n_samples*n_alts, ), default=None
             Scaling variable used for non-linear models. For WTP models, this is usually the negative of 
             the price variable.
             
+        addit : array-like, shape (n_samples*n_alts, ), default=None
+            Additive term to model coefficients kept fixed during estimation.
+            
         optim_method : str, default='BFGS'
             Optimization method to use for model estimation. It can be `BFGS` or `L-BFGS-B`.
             For non-linear (WTP-like) models, `L-BFGS-B` is used by default.
 
         robust: bool, default=False
             Whether robust standard errors should be computed
 
@@ -171,41 +174,41 @@
         mnl_init: bool, default=True
             Whether to initialize coefficients using estimates from a multinomial logit
         Returns
         -------
         None.
         """
         # Handle array-like inputs by converting everything to numpy arrays
-        X, y, varnames, alts, isvars, ids, weights, panels, avail, scale_factor \
-            = self._as_array(X, y, varnames, alts, isvars, ids, weights, panels, avail, scale_factor)
+        X, y, varnames, alts, isvars, ids, weights, panels, avail, scale_factor, addit \
+            = self._as_array(X, y, varnames, alts, isvars, ids, weights, panels, avail, scale_factor, addit)
 
         self._validate_inputs(X, y, alts, varnames, isvars, ids, weights)
 
         if mnl_init and init_coeff is None:
             # Initialize coefficients using a multinomial logit model
             mnl = MultinomialLogit()
-            mnl.fit(X, y, varnames, alts, ids, isvars=isvars, weights=weights,
+            mnl.fit(X, y, varnames, alts, ids, isvars=isvars, weights=weights, addit=addit,
                     avail=avail, base_alt=base_alt, fit_intercept=fit_intercept)
             init_coeff = np.concatenate((mnl.coeff_, np.repeat(.1, len(randvars))))
             init_coeff = init_coeff if scale_factor is None else np.append(init_coeff, 1.)
 
         self._pre_fit(alts, varnames, isvars, base_alt, fit_intercept, maxiter)
 
-        betas, X, y, panels, draws, weights, avail, Xnames, scale = \
+        betas, X, y, panels, draws, weights, avail, Xnames, scale, addit = \
             self._setup_input_data(X, y, varnames, alts, ids, randvars, isvars=isvars, weights=weights, avail=avail,
                                    panels=panels, init_coeff=init_coeff, random_state=random_state, n_draws=n_draws,
                                    halton=halton, verbose=verbose, predict_mode=False, halton_opts=halton_opts,
-                                   scale_factor=scale_factor)
+                                   scale_factor=scale_factor, addit=addit)
 
         tol = {'ftol': 1e-10, 'gtol': 1e-6}
         if tol_opts is not None:
             tol.update(tol_opts)
 
-        Xd, scale_d, avail = diff_nonchosen_chosen(X, y, scale, avail)  # Setup Xd as Xij - Xi*
-        fargs = (Xd, panels, draws, weights, avail, scale_d, batch_size)
+        Xd, scale_d, addit_d, avail = diff_nonchosen_chosen(X, y, scale, addit, avail)  # Setup Xd as Xij - Xi*
+        fargs = (Xd, panels, draws, weights, avail, scale_d, addit_d, batch_size)
         if scale_factor is not None:
             optim_method = "L-BFGS-B"
         optim_res = _minimize(self._loglik_gradient, betas, args=fargs, method=optim_method, tol=tol['ftol'],
                               options={'gtol': tol['gtol'], 'maxiter': maxiter, 'disp': verbose > 1})        
 
         coef_names = np.append(Xnames, np.char.add("sd.", Xnames[self._rvidx]))
 
@@ -221,15 +224,15 @@
         
         self._post_fit(optim_res, coef_names, X.shape[0], verbose, robust)
 
 
 
     def predict(self, X, varnames, alts, ids, isvars=None, weights=None, avail=None,  panels=None, random_state=None,
                 n_draws=1000, halton=True, verbose=1, batch_size=None, return_proba=False, return_freq=False,
-                halton_opts=None, scale_factor=None):
+                halton_opts=None, scale_factor=None, addit=None):
         """Predict chosen alternatives.
 
         Parameters
         ----------
         X : array-like, shape (n_samples*n_alts, n_variables)
             Input data for explanatory variables in long format
 
@@ -279,15 +282,18 @@
             Verbosity of messages to show during estimation. 0: No messages, 1: Some messages, 2: All messages
 
         batch_size : int, default=None
             Size of batches used to GPU avoid memory overflow. 
             
         scale_factor : array-like, shape (n_samples*n_alts, ), default=None
             Scaling variable used for non-linear WTP-like models. This is usually the negative of the price variable..
-
+            
+        addit : array-like, shape (n_samples*n_alts, ), default=None
+            Additive term to model coefficients kept fixed during estimation.
+            
         return_proba : bool, default=False
             If True, also return the choice probabilities
 
         return_freq : bool, default=False
             If True, also return the frequency of the chosen the alternatives
 
 
@@ -301,54 +307,55 @@
             appear in ``self.alternatives``. Only provided if `return_proba` is True.
 
         freq : dict, optional
             Choice frequency for each alternative. Only provided if `return_freq` is True.
         """
         # Handle array-like inputs by converting everything to numpy arrays
         #=== 1. Preprocess inputs
-        X, _, varnames, alts, isvars, ids, weights, panels, avail, scale_factor \
-            = self._as_array(X, None, varnames, alts, isvars, ids, weights, panels, avail, scale_factor)
+        X, _, varnames, alts, isvars, ids, weights, panels, avail, scale_factor, addit \
+            = self._as_array(X, None, varnames, alts, isvars, ids, weights, panels, avail, scale_factor, addit)
         
         self._validate_inputs(X, None, alts, varnames, isvars, ids, weights)
         
-        betas, X, _, panels, draws, weights, avail, Xnames, scale = \
+        betas, X, _, panels, draws, weights, avail, Xnames, scale, addit = \
             self._setup_input_data(X, None, varnames, alts, ids, self.randvars,  isvars=isvars, weights=weights,
                                    avail=avail, panels=panels, init_coeff=self.coeff_, random_state=random_state,
                                    n_draws=n_draws, halton=halton, verbose=verbose, predict_mode=True,
-                                   halton_opts=halton_opts, scale_factor=scale_factor)
+                                   halton_opts=halton_opts, scale_factor=scale_factor, addit=addit)
         
         coeff_names = np.append(Xnames, np.char.add("sd.", Xnames[self._rvidx]))
         coeff_names = coeff_names if scale_factor is None else np.append(coeff_names, "_scale_factor")
         if not np.array_equal(coeff_names, self.coeff_names):
             raise ValueError("The provided 'varnames' yield coefficient names that are inconsistent with the stored "
                              "in 'self.coeff_names'")
         
         
         lambdac = 1 if scale_factor is None else betas[-1]
         sca = 0 if scale_factor is None else scale[:, :, None]
+        addit = 0 if addit is None else addit[:, :, None]
         
         #=== 2. Compute choice probabilities
         Xf = X[:, :, ~self._rvidx]  # Data for fixed parameters
         Xr = X[:, :, self._rvidx]  # Data for random parameters
         betas, Xr, avail = dev.to_gpu(betas), dev.to_gpu(Xr), dev.to_gpu(avail)
-        lambdac, sca = dev.to_gpu(lambdac), dev.to_gpu(sca)
+        lambdac, sca, addit = dev.to_gpu(lambdac), dev.to_gpu(sca), dev.to_gpu(addit)
         
         # Utility for fixed parameters
         Bf = betas[np.where(~self._rvidx)[0]]  # Fixed betas
         Vf = dev.np.einsum('njk,k -> nj', Xf, Bf)  # (N, J-1)
         
         proba = []  # Temp batching storage
         for batch_start, batch_end in batches_idx(batch_size, n_draws):
             draws_ = dev.to_gpu(draws[:, :, batch_start: batch_end])
 
             # Utility for random parameters 
             Br = self._transform_rand_betas(betas, draws_)  # Get random coefficients
             Vr = dev.cust_einsum("njk,nkr -> njr", Xr, Br)  # (N,J-1,R)
             
-            eV = dev.np.exp(lambdac*(Vf[:, :, None] + Vr - sca))
+            eV = dev.np.exp(lambdac*(Vf[:, :, None] + Vr - sca + addit))
             Vdr, Br = None, None # Release memory
 
             eV = eV if avail is None else eV*avail[:, :, None]  
             proba_ = eV/dev.np.sum(eV, axis=1, keepdims=True)  # (N,J,R)
             # proba_ = self._prob_product_across_panels(proba_, panels)  # (Np,J,R)
 
             proba.append(dev.to_cpu(proba_))
@@ -372,15 +379,15 @@
             output += (freq, )
       
         return _unpack_tuple(output) # Unpack before returning
      
  
     def _setup_input_data(self, X, y, varnames, alts, ids, randvars, isvars=None, weights=None, avail=None,
                           panels=None, init_coeff=None, random_state=None, n_draws=200, halton=True, verbose=1,
-                          predict_mode=False, halton_opts=None, scale_factor=None):
+                          predict_mode=False, halton_opts=None, scale_factor=None, addit=None):
         if random_state is not None:
             np.random.seed(random_state)
 
         self._check_long_format_consistency(ids, alts)
         y = self._format_choice_var(y, alts) if not predict_mode else None
         X, Xnames = self._setup_design_matrix(X)
         self._model_specific_validations(randvars, Xnames)
@@ -423,59 +430,61 @@
             betas = np.repeat(.1, K + Kr)
         else:
             betas = init_coeff
             if len(init_coeff) != (K + Kr + Ks):
                 raise ValueError("The length of init_coeff must be: {}".format(K + Kr + Ks))
         
         scale = None if scale_factor is None else scale_factor.reshape(N, J)
+        addit = None if addit is None else addit.reshape(N, J)
 
         if dev.using_gpu and verbose > 0:
             print("GPU processing enabled.")
-        return betas, X, y, panels, draws, weights, avail, Xnames, scale
+        return betas, X, y, panels, draws, weights, avail, Xnames, scale, addit
 
     def _setup_randvars_info(self, randvars, Xnames):
         self.randvars = randvars
         self._rvidx, self._rvdist = [], []
         for var in Xnames:
             if var in self.randvars.keys():
                 self._rvidx.append(True)
                 self._rvdist.append(self.randvars[var])
             else:
                 self._rvidx.append(False)
         self._rvidx = np.array(self._rvidx)
 
-    def _loglik_gradient(self, betas, Xd, panels, draws, weights, avail, scale_d, batch_size, return_gradient=True):
+    def _loglik_gradient(self, betas, Xd, panels, draws, weights, avail, scale_d, addit_d, batch_size, return_gradient=True):
         """Compute the log-likelihood and gradient.
 
         Fixed and random parameters are handled separately to speed up the estimation and the results are concatenated.
         """
         N, R, Kr, Kf = Xd.shape[0], draws.shape[2], np.sum(self._rvidx), np.sum(~self._rvidx)
         
         lambdac = 1 if scale_d is None else betas[-1]
         Xd = Xd if scale_d is None else Xd*lambdac  # Multiply data by lambda coefficient when scaling is in use
         
         Xdf = Xd[:, :, ~self._rvidx]  # Data for fixed parameters
         Xdr = Xd[:, :, self._rvidx]  # Data for random parameters
         
-        sca = 0 if scale_d is None else (lambdac*scale_d)[:, :, None]
-        betas, Xdf, Xdr, avail, sca = dev.to_gpu(betas), dev.to_gpu(Xdf), dev.to_gpu(Xdr), dev.to_gpu(avail), dev.to_gpu(sca)
+        scad = 0 if scale_d is None else (lambdac*scale_d)[:, :, None]
+        additd = 0 if addit_d is None else (lambdac*addit_d)[:, :, None]
+        betas, Xdf, Xdr, avail, scad, additd = dev.to_gpu(betas), dev.to_gpu(Xdf), dev.to_gpu(Xdr), dev.to_gpu(avail), dev.to_gpu(scad), dev.to_gpu(additd)
 
         # Utility for fixed parameters
         Bf = betas[np.where(~self._rvidx)[0]]  # Fixed betas
         Vdf = dev.np.einsum('njk,k -> nj', Xdf, Bf)  # (N, J-1)
         
         proba, gr_f, gr_u, gr_s, gr_l = [], np.zeros((N, Kf)), np.zeros((N, Kr)), np.zeros((N, Kr)), np.zeros((N, 1))  # Temp batching storage
         for batch_start, batch_end in batches_idx(batch_size, n_samples=R):
             draws_ = dev.to_gpu(draws[:, :, batch_start: batch_end])
 
             # Utility for random parameters 
             Br = self._transform_rand_betas(betas, draws_)  # Get random coefficients
             Vdr = dev.cust_einsum("njk,nkr -> njr", Xdr, Br)  # (N,J-1,R)
             
-            eVd = dev.np.exp(Vdf[:, :, None] + Vdr - sca)
+            eVd = dev.np.exp(Vdf[:, :, None] + Vdr - scad + additd)
             Vdr, Br = None, None # Release memory
             eVd = eVd if avail is None else eVd*avail[:, :, None]  # Availablity of alts.
             # TODO: Handle availability
             proba_n = 1/(1+eVd.sum(axis=1)) # (N,R)
             proba_ = self._prob_product_across_panels(proba_n, panels) # (Np,R)
             
             if return_gradient:
@@ -668,15 +677,15 @@
             betas = np.array([.1, .1, .1, .1])
             Xd =  X[~y, :].reshape(N, J - 1, K) - X[y, :].reshape(N, 1, K) 
 
             # Compute log likelihood using xlogit
             model = MixedLogit()
             model._rvidx,  model._rvdist = np.array([True, True]), np.array(['n', 'n'])
             draws = model._generate_halton_draws(N, R, K)  # (N,Kr,R)
-            model._loglik_gradient(betas, Xd, None, draws, None, None, None,
+            model._loglik_gradient(betas, Xd, None, draws, None, None, None, None,
                                    batch_size=R, return_gradient=False)
 
             print("{} GPU device(s) available. xlogit will use GPU processing".format(n_gpus))
             return True
         else:
             print("*** No GPU device found. Verify CuPy is properly installed")
             return False
```

### Comparing `xlogit-0.2.4/xlogit/multinomial_logit.py` & `xlogit-0.2.5/xlogit/multinomial_logit.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         bic : float
             Bayesian information criteria of the estimated model
     """
 
     def fit(self, X, y, varnames, alts, ids, isvars=None,
             weights=None, avail=None, base_alt=None, fit_intercept=False,
             init_coeff=None, maxiter=2000, random_state=None, tol_opts=None, verbose=1,
-            robust=False, num_hess=False, scale_factor=None):
+            robust=False, num_hess=False, scale_factor=None, addit=None):
         """Fit multinomial and/or conditional logit models.
 
         Parameters
         ----------
         X : array-like, shape (n_samples*n_alts, n_variables)
             Input data for explanatory variables in long format
 
@@ -87,15 +87,18 @@
 
         weights : array-like, shape (n_variables,), default=None
             Weights for the choice situations in long format.
 
         avail: array-like, shape (n_samples*n_alts,), default=None
             Availability of alternatives for the samples. One when
             available or zero otherwise.
-
+            
+        addit : array-like, shape (n_samples*n_alts, ), default=None
+            Additive term to model coefficients kept fixed during estimation.
+            
         base_alt : int, float or str, default=None
             Base alternative
 
         fit_intercept : bool, default=False
             Whether to include an intercept in the model.
 
         init_coeff : numpy array, shape (n_variables,), default=None
@@ -124,49 +127,48 @@
             1: Some messages, 2: All messages
 
 
         Returns
         -------
         None.
         """
-        X, y, varnames, alts, isvars, ids, weights, _, avail, scale_factor\
-            = self._as_array(X, y, varnames, alts, isvars, ids, weights,
-                             None, avail, scale_factor)
+        X, y, varnames, alts, isvars, ids, weights, _, avail, scale_factor, addit \
+            = self._as_array(X, y, varnames, alts, isvars, ids, weights, None, avail, scale_factor, addit)
         self._validate_inputs(X, y, alts, varnames, isvars, ids, weights)
 
         self._pre_fit(alts, varnames, isvars, base_alt, fit_intercept, maxiter)
         
-        betas, X, y, weights, avail, Xnames, scale = \
+        betas, X, y, weights, avail, Xnames, scale, addit = \
             self._setup_input_data(X, y, varnames, alts, ids, 
                                    isvars=isvars, weights=weights, avail=avail,
                                    init_coeff=init_coeff,
                                    random_state=random_state, verbose=verbose,
-                                   predict_mode=False, scale_factor=scale_factor)
+                                   predict_mode=False, scale_factor=scale_factor, addit=addit)
 
         tol = {'ftol': 1e-10}
         if tol_opts is not None:
             tol.update(tol_opts)
 
         # Call optimization routine
-        Xd, scale_d, avail = diff_nonchosen_chosen(X, y, scale, avail)  # Setup Xd as Xij - Xi*
-        fargs = (Xd, scale_d, weights, avail)
+        Xd, scale_d, addit_d, avail = diff_nonchosen_chosen(X, y, scale, addit, avail)  # Setup Xd as Xij - Xi*
+        fargs = (Xd, scale_d, addit_d, weights, avail)
         optim_res = _minimize(self._loglik_gradient, betas, args=fargs, method="BFGS", tol=tol['ftol'],
                               options={'maxiter': maxiter, 'disp': verbose > 1})
         coef_names = Xnames
         if scale_factor is not None:
             coef_names = np.append(coef_names, "_scale_factor")
 
         if num_hess or True:
             optim_res['hess_inv'] = _numerical_hessian(optim_res['x'], self._loglik_gradient, args=fargs)
         self._post_fit(optim_res, coef_names, X.shape[0], verbose, robust)
 
 
     def predict(self, X, varnames, alts, ids, isvars=None, weights=None,
                 avail=None, random_state=None, verbose=1,
-                return_proba=False, return_freq=False, scale_factor=None):
+                return_proba=False, return_freq=False, scale_factor=None, addit=None):
         """Predict chosen alternatives.
 
         Parameters
         ----------
         X : array-like, shape (n_samples*n_alts, n_variables)
             Input data for explanatory variables in long format
 
@@ -185,15 +187,18 @@
 
         weights : array-like, shape (n_variables,), default=None
             Sample weights in long format.
 
         avail: array-like, shape (n_samples*n_alts,), default=None
             Availability of alternatives for the samples. One when
             available or zero otherwise.
-
+            
+        addit : array-like, shape (n_samples*n_alts, ), default=None
+            Additive term to model coefficients kept fixed during estimation.
+            
         random_state : int, default=None
             Random seed for numpy random generator
 
         verbose : int, default=1
             Verbosity of messages to show during estimation. 0: No messages,
             1: Some messages, 2: All messages
 
@@ -217,38 +222,39 @@
 
         freq : dict, optional
             Choice frequency for each alternative. Only provided
             if `return_freq` is True.
         """
         #=== 1. Preprocess inputs
         # Handle array-like inputs by converting everything to numpy arrays
-        X, _, varnames, alts, isvars, ids, weights, _, avail, scale_factor\
-            = self._as_array(X, None, varnames, alts, isvars, ids, weights, None, avail, scale_factor)
+        X, _, varnames, alts, isvars, ids, weights, _, avail, scale_factor, addit \
+            = self._as_array(X, None, varnames, alts, isvars, ids, weights, None, avail, scale_factor, addit)
 
         self._validate_inputs(X, None, alts, varnames, isvars, ids, weights)
        
-        betas, X, _, weights, avail, Xnames, scale = \
+        betas, X, _, weights, avail, Xnames, scale, addit = \
             self._setup_input_data(X, None, varnames, alts, ids, 
                                    isvars=isvars, weights=weights, avail=avail,
                                    init_coeff=self.coeff_,
                                    random_state=random_state, verbose=verbose,
-                                   predict_mode=True, scale_factor=scale_factor)
+                                   predict_mode=True, scale_factor=scale_factor, addit=addit)
             
         coeff_names = Xnames
         coeff_names = coeff_names if scale_factor is None else np.append(coeff_names, "_scale_factor")
         if not np.array_equal(coeff_names, self.coeff_names):
             raise ValueError("The provided 'varnames' yield coefficient names that are inconsistent with the stored "
                              "in 'self.coeff_names'")
         
         lambdac = 1 if scale_factor is None else betas[-1]
         sca = 0 if scale_factor is None else scale
+        addit = 0 if addit is None else addit
         betas = betas if scale_factor is None else betas[:-1]
 
         #=== 2. Compute choice probabilities
-        eV = np.exp(lambdac*(X.dot(betas) - sca))
+        eV = np.exp(lambdac*(X.dot(betas) - sca + addit))
         eV = eV if avail is None else eV*avail
         proba = eV/np.sum(eV, axis=1, keepdims=True)  # (N,J)
         
         #=== 3. Compute choices
         idx_max_proba = np.argmax(proba, axis=1)
         choices = self.alternatives[idx_max_proba]
         
@@ -267,15 +273,15 @@
         
         return _unpack_tuple(output) # Unpack before returning
 
 
     def _setup_input_data(self, X, y, varnames, alts, ids, isvars=None,
             weights=None, avail=None, base_alt=None, fit_intercept=False,
             init_coeff=None, random_state=None, verbose=1, predict_mode=False,
-            scale_factor=None):
+            scale_factor=None, addit=None):
         self._check_long_format_consistency(ids, alts)
         y = self._format_choice_var(y, alts) if not predict_mode else None
         X, Xnames = self._setup_design_matrix(X)
         N, J, K = X.shape
         y = y.reshape(N, J)  if not predict_mode else None
         
         if random_state is not None:
@@ -292,26 +298,28 @@
             betas = betas if scale_factor is None else np.append(betas, 1.)
         else:
             betas = init_coeff
             n_coeff = K + (0 if scale_factor is None else 1)
             if len(init_coeff) != n_coeff:
                 raise ValueError(f"The size of initial_coeff must be: {n_coeff}")
         scale = None if scale_factor is None else scale_factor.reshape(N, J)
+        addit = None if addit is None else addit.reshape(N, J)
         
-        return betas, X, y, weights, avail, Xnames, scale
+        return betas, X, y, weights, avail, Xnames, scale, addit
 
 
-    def _loglik_gradient(self, betas, Xd, scale_d, weights, avail, return_gradient=True):
+    def _loglik_gradient(self, betas, Xd, scale_d, addit_d, weights, avail, return_gradient=True):
         """Compute log-likelihood, gradient, and hessian."""
         lambdac = 1 if scale_d is None else betas[-1]
         betas = betas if scale_d is None else betas[:-1]
         Xd = Xd if scale_d is None else lambdac*Xd
-        sca = 0 if scale_d is None else lambdac*scale_d
+        scad = 0 if scale_d is None else lambdac*scale_d
+        additd = 0 if addit_d is None else lambdac*addit_d
         #p = self._compute_probabilities(betas, X, avail)
-        Vd = np.einsum('njk,k -> nj', Xd, betas) - sca
+        Vd = np.einsum('njk,k -> nj', Xd, betas) - scad + additd
         eVd = np.exp(Vd)
         eVd = eVd if avail is None else eVd*avail # Availablity of alts.
         proba = 1/(1+eVd.sum(axis=1))  # (N, )
         
         # Log likelihood
         lik = proba
         loglik = np.log(lik) if weights is None else np.log(lik)*weights
```

### Comparing `xlogit-0.2.4/xlogit/utils.py` & `xlogit-0.2.5/xlogit/utils.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.4/xlogit.egg-info/PKG-INFO` & `xlogit-0.2.5/xlogit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlogit
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python package for GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/arteagac/xlogit
 Author: Cristian Arteaga
 Author-email: cristiandavidarteaga@gmail.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
@@ -13,15 +13,15 @@
 ===========================================================================================
 xlogit: A Python Package for GPU-Accelerated Estimation of Mixed Logit Models.
 ===========================================================================================
 
 .. image:: https://raw.githubusercontent.com/arteagac/xlogit/master/docs/xlogit_logo_1000px.png
   :width: 400
 
-|Travis| |Coverage| |Community| |Docs| |PyPi| |License|
+|Build| |Coverage| |Community| |Docs| |PyPi| |License|
 
 .. _Mixed Logit: https://xlogit.readthedocs.io/en/latest/api/mixed_logit.html
 .. _Multinomial Logit: https://xlogit.readthedocs.io/en/latest/api/multinomial_logit.html
 
 `Examples <https://xlogit.readthedocs.io/en/latest/examples.html>`__ | `Docs <https://xlogit.readthedocs.io/en/latest/index.html>`__ | `Installation <https://xlogit.readthedocs.io/en/latest/install.html>`__ | `API Reference <https://xlogit.readthedocs.io/en/latest/api/index.html>`__ | `Contributing <https://xlogit.readthedocs.io/en/latest/contributing.html>`__ | `Contact <https://xlogit.readthedocs.io/en/latest/index.html#contact>`__ 
 
 Quick start
@@ -173,16 +173,16 @@
         pages = {100339},
         year = {2022},
         issn = {1755-5345},
         doi = {https://doi.org/10.1016/j.jocm.2021.100339},
     }
 
 
-.. |Travis| image:: https://travis-ci.com/arteagac/xlogit.svg?branch=master
-   :target: https://travis-ci.com/arteagac/xlogit
+.. |Build| image:: https://github.com/arteagac/xlogit/actions/workflows/python-tests.yml/badge.svg
+   :target: https://github.com/arteagac/xlogit/actions/workflows/python-tests.yml
 
 .. |Docs| image:: https://readthedocs.org/projects/xlogit/badge/?version=latest
    :target: https://xlogit.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. |Community| image:: https://badges.gitter.im/xlogit/community.svg
    :target: https://gitter.im/xlogit/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
```

