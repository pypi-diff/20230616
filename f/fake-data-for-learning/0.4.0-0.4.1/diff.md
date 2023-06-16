# Comparing `tmp/fake_data_for_learning-0.4.0.tar.gz` & `tmp/fake_data_for_learning-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fake_data_for_learning-0.4.0.tar", last modified: Wed Dec  1 18:16:17 2021, max compression
+gzip compressed data, was "fake_data_for_learning-0.4.1.tar", last modified: Fri Jun 16 07:44:30 2023, max compression
```

## Comparing `fake_data_for_learning-0.4.0.tar` & `fake_data_for_learning-0.4.1.tar`

### file list

```diff
@@ -1,56 +1,26 @@
-drwxr-xr-x   0 pauldev    (503) staff       (20)        0 2021-12-01 18:16:17.202685 fake_data_for_learning-0.4.0/
-drwxr-xr-x   0 pauldev    (503) staff       (20)        0 2021-12-01 18:16:17.147603 fake_data_for_learning-0.4.0/.circleci/
--rw-r--r--   0 pauldev    (503) staff       (20)      466 2021-12-01 09:04:52.000000 fake_data_for_learning-0.4.0/.circleci/config.yml
--rw-r--r--   0 pauldev    (503) staff       (20)      292 2019-06-16 18:53:32.000000 fake_data_for_learning-0.4.0/.editorconfig
--rw-r--r--   0 pauldev    (503) staff       (20)       49 2020-01-02 09:00:34.000000 fake_data_for_learning-0.4.0/.gitattributes
--rw-r--r--   0 pauldev    (503) staff       (20)      897 2020-01-01 11:42:24.000000 fake_data_for_learning-0.4.0/.gitignore
--rw-r--r--   0 pauldev    (503) staff       (20)     1074 2020-01-01 11:42:24.000000 fake_data_for_learning-0.4.0/LICENSE
--rw-r--r--   0 pauldev    (503) staff       (20)     1767 2021-12-01 18:16:17.202855 fake_data_for_learning-0.4.0/PKG-INFO
--rw-r--r--   0 pauldev    (503) staff       (20)     6314 2021-12-01 18:10:11.000000 fake_data_for_learning-0.4.0/README.md
--rw-r--r--   0 pauldev    (503) staff       (20)       30 2020-01-01 11:42:24.000000 fake_data_for_learning-0.4.0/_config.yml
-drwxr-xr-x   0 pauldev    (503) staff       (20)        0 2021-12-01 18:16:17.152533 fake_data_for_learning-0.4.0/docs/
--rw-r--r--   0 pauldev    (503) staff       (20)      825 2020-01-01 16:09:57.000000 fake_data_for_learning-0.4.0/docs/Makefile
-drwxr-xr-x   0 pauldev    (503) staff       (20)        0 2021-12-01 18:16:17.157198 fake_data_for_learning-0.4.0/docs/graphics/
--rw-r--r--   0 pauldev    (503) staff       (20)     8265 2021-12-01 11:00:07.000000 fake_data_for_learning-0.4.0/docs/graphics/graph.png
--rw-r--r--   0 pauldev    (503) staff       (20)     5313 2021-12-01 11:00:07.000000 fake_data_for_learning-0.4.0/docs/graphics/network_sample.png
--rw-r--r--   0 pauldev    (503) staff       (20)       70 2020-01-01 11:42:24.000000 fake_data_for_learning-0.4.0/docs/index.html
--rw-r--r--   0 pauldev    (503) staff       (20)      799 2020-01-01 11:42:24.000000 fake_data_for_learning-0.4.0/docs/make.bat
-drwxr-xr-x   0 pauldev    (503) staff       (20)        0 2021-12-01 18:16:17.161555 fake_data_for_learning-0.4.0/docs/scripts/
--rw-r--r--   0 pauldev    (503) staff       (20)      313 2020-01-01 15:58:56.000000 fake_data_for_learning-0.4.0/docs/scripts/build_docs.sh
--rw-r--r--   0 pauldev    (503) staff       (20)      493 2020-01-01 16:07:19.000000 fake_data_for_learning-0.4.0/docs/scripts/git_docs_change.sh
-drwxr-xr-x   0 pauldev    (503) staff       (20)        0 2021-12-01 18:16:17.168237 fake_data_for_learning-0.4.0/docs/source/
-drwxr-xr-x   0 pauldev    (503) staff       (20)        0 2021-12-01 18:16:17.175398 fake_data_for_learning-0.4.0/docs/source/api/
--rw-r--r--   0 pauldev    (503) staff       (20)      235 2020-01-01 11:42:24.000000 fake_data_for_learning-0.4.0/docs/source/api/fake_data_for_learning.fake_data_for_learning.rst
--rw-r--r--   0 pauldev    (503) staff       (20)      297 2020-04-17 04:54:22.000000 fake_data_for_learning-0.4.0/docs/source/api/fake_data_for_learning.rst
--rw-r--r--   0 pauldev    (503) staff       (20)      178 2020-01-01 11:42:24.000000 fake_data_for_learning-0.4.0/docs/source/api/fake_data_for_learning.utils.rst
--rw-r--r--   0 pauldev    (503) staff       (20)      103 2020-01-01 11:42:24.000000 fake_data_for_learning-0.4.0/docs/source/api/modules.rst
--rw-r--r--   0 pauldev    (503) staff       (20)      127 2020-01-01 11:42:24.000000 fake_data_for_learning-0.4.0/docs/source/api.rst
--rw-r--r--   0 pauldev    (503) staff       (20)     2070 2020-01-01 11:42:24.000000 fake_data_for_learning-0.4.0/docs/source/conf.py
--rw-r--r--   0 pauldev    (503) staff       (20)     1892 2020-04-17 06:47:37.000000 fake_data_for_learning-0.4.0/docs/source/index.rst
-drwxr-xr-x   0 pauldev    (503) staff       (20)        0 2021-12-01 18:16:17.185034 fake_data_for_learning-0.4.0/fake_data_for_learning/
--rw-r--r--   0 pauldev    (503) staff       (20)        0 2021-12-01 18:04:05.000000 fake_data_for_learning-0.4.0/fake_data_for_learning/__init__.py
--rw-r--r--   0 pauldev    (503) staff       (20)     2343 2021-12-01 16:58:18.000000 fake_data_for_learning-0.4.0/fake_data_for_learning/contingency_tables.py
--rw-r--r--   0 pauldev    (503) staff       (20)    15086 2020-04-16 15:35:21.000000 fake_data_for_learning-0.4.0/fake_data_for_learning/fake_data_for_learning.py
--rw-r--r--   0 pauldev    (503) staff       (20)    13482 2021-12-01 09:04:52.000000 fake_data_for_learning-0.4.0/fake_data_for_learning/probability_polytopes.py
--rw-r--r--   0 pauldev    (503) staff       (20)      895 2021-12-01 09:04:52.000000 fake_data_for_learning-0.4.0/fake_data_for_learning/utils.py
-drwxr-xr-x   0 pauldev    (503) staff       (20)        0 2021-12-01 18:16:17.190682 fake_data_for_learning-0.4.0/fake_data_for_learning.egg-info/
--rw-r--r--   0 pauldev    (503) staff       (20)     1767 2021-12-01 18:16:17.000000 fake_data_for_learning-0.4.0/fake_data_for_learning.egg-info/PKG-INFO
--rw-r--r--   0 pauldev    (503) staff       (20)     1298 2021-12-01 18:16:17.000000 fake_data_for_learning-0.4.0/fake_data_for_learning.egg-info/SOURCES.txt
--rw-r--r--   0 pauldev    (503) staff       (20)        1 2021-12-01 18:16:17.000000 fake_data_for_learning-0.4.0/fake_data_for_learning.egg-info/dependency_links.txt
--rw-r--r--   0 pauldev    (503) staff       (20)        1 2019-06-16 18:57:10.000000 fake_data_for_learning-0.4.0/fake_data_for_learning.egg-info/not-zip-safe
--rw-r--r--   0 pauldev    (503) staff       (20)       80 2021-12-01 18:16:17.000000 fake_data_for_learning-0.4.0/fake_data_for_learning.egg-info/requires.txt
--rw-r--r--   0 pauldev    (503) staff       (20)       23 2021-12-01 18:16:17.000000 fake_data_for_learning-0.4.0/fake_data_for_learning.egg-info/top_level.txt
-drwxr-xr-x   0 pauldev    (503) staff       (20)        0 2021-12-01 18:16:17.193049 fake_data_for_learning-0.4.0/notebooks/
--rw-r--r--   0 pauldev    (503) staff       (20)    56247 2021-12-01 14:33:55.000000 fake_data_for_learning-0.4.0/notebooks/bayesian-network.ipynb
--rw-r--r--   0 pauldev    (503) staff       (20)    18808 2021-12-01 09:04:52.000000 fake_data_for_learning-0.4.0/notebooks/conditional-probability-tables-with-constraints.ipynb
--rw-r--r--   0 pauldev    (503) staff       (20)      183 2021-12-01 09:04:52.000000 fake_data_for_learning-0.4.0/requirements.txt
--rw-r--r--   0 pauldev    (503) staff       (20)      302 2021-12-01 18:16:17.203692 fake_data_for_learning-0.4.0/setup.cfg
--rw-r--r--   0 pauldev    (503) staff       (20)     2293 2021-12-01 18:10:26.000000 fake_data_for_learning-0.4.0/setup.py
-drwxr-xr-x   0 pauldev    (503) staff       (20)        0 2021-12-01 18:16:17.200848 fake_data_for_learning-0.4.0/tests/
--rw-r--r--   0 pauldev    (503) staff       (20)     5218 2021-12-01 09:04:52.000000 fake_data_for_learning-0.4.0/tests/test_bayesian_node_rv.py
--rw-r--r--   0 pauldev    (503) staff       (20)     5353 2021-12-01 16:48:26.000000 fake_data_for_learning-0.4.0/tests/test_contingency_tables.py
--rw-r--r--   0 pauldev    (503) staff       (20)     1281 2021-12-01 09:04:52.000000 fake_data_for_learning-0.4.0/tests/test_demo_notebooks.py
--rw-r--r--   0 pauldev    (503) staff       (20)     8741 2021-12-01 09:04:52.000000 fake_data_for_learning-0.4.0/tests/test_fake_data_bn.py
--rw-r--r--   0 pauldev    (503) staff       (20)    10959 2021-12-01 09:04:52.000000 fake_data_for_learning-0.4.0/tests/test_probability_polytopes.py
--rw-r--r--   0 pauldev    (503) staff       (20)      577 2021-12-01 09:04:52.000000 fake_data_for_learning-0.4.0/tests/test_utils.py
--rw-r--r--   0 pauldev    (503) staff       (20)      476 2021-11-30 14:34:32.000000 fake_data_for_learning-0.4.0/tox.ini
+drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-06-16 07:44:30.870174 fake_data_for_learning-0.4.1/
+-rw-r--r--   0 paullarsen   (501) staff       (20)     1074 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/LICENSE
+-rw-r--r--   0 paullarsen   (501) staff       (20)     1711 2023-06-16 07:44:30.870234 fake_data_for_learning-0.4.1/PKG-INFO
+-rw-r--r--   0 paullarsen   (501) staff       (20)     6455 2023-06-16 06:42:55.000000 fake_data_for_learning-0.4.1/README.md
+drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-06-16 07:44:30.867721 fake_data_for_learning-0.4.1/fake_data_for_learning/
+-rw-r--r--   0 paullarsen   (501) staff       (20)        0 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/fake_data_for_learning/__init__.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)     2339 2023-06-15 12:49:41.000000 fake_data_for_learning-0.4.1/fake_data_for_learning/contingency_tables.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)    15082 2023-06-15 12:48:16.000000 fake_data_for_learning-0.4.1/fake_data_for_learning/fake_data_for_learning.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)    13482 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/fake_data_for_learning/probability_polytopes.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)      895 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/fake_data_for_learning/utils.py
+drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-06-16 07:44:30.868849 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/
+-rw-r--r--   0 paullarsen   (501) staff       (20)     1711 2023-06-16 07:44:30.000000 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/PKG-INFO
+-rw-r--r--   0 paullarsen   (501) staff       (20)      695 2023-06-16 07:44:30.000000 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 paullarsen   (501) staff       (20)        1 2023-06-16 07:44:30.000000 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 paullarsen   (501) staff       (20)        1 2023-06-15 12:43:35.000000 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/not-zip-safe
+-rw-r--r--   0 paullarsen   (501) staff       (20)       80 2023-06-16 07:44:30.000000 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/requires.txt
+-rw-r--r--   0 paullarsen   (501) staff       (20)       23 2023-06-16 07:44:30.000000 fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/top_level.txt
+-rw-r--r--   0 paullarsen   (501) staff       (20)      302 2023-06-16 07:44:30.870450 fake_data_for_learning-0.4.1/setup.cfg
+-rw-r--r--   0 paullarsen   (501) staff       (20)     2293 2023-06-15 15:14:49.000000 fake_data_for_learning-0.4.1/setup.py
+drwxr-xr-x   0 paullarsen   (501) staff       (20)        0 2023-06-16 07:44:30.870012 fake_data_for_learning-0.4.1/tests/
+-rw-r--r--   0 paullarsen   (501) staff       (20)     5218 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/tests/test_bayesian_node_rv.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)     5353 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/tests/test_contingency_tables.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)     1281 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/tests/test_demo_notebooks.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)     8721 2023-06-16 06:45:18.000000 fake_data_for_learning-0.4.1/tests/test_fake_data_bn.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)    10959 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/tests/test_probability_polytopes.py
+-rw-r--r--   0 paullarsen   (501) staff       (20)      577 2023-04-11 08:11:23.000000 fake_data_for_learning-0.4.1/tests/test_utils.py
```

### Comparing `fake_data_for_learning-0.4.0/LICENSE` & `fake_data_for_learning-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.0/PKG-INFO` & `fake_data_for_learning-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: fake_data_for_learning
-Version: 0.4.0
-Summary: UNKNOWN
-Home-page: UNKNOWN
+Version: 0.4.1
 Author: Paul Larsen
 Author-email: munichpavel@gmail.com
 License: MIT license
 Project-URL: Homepage, https://munichpavel.github.io/fake-data-for-learning/
 Project-URL: Bug Tracker, https://github.com/munichpavel/fake-data-for-learning/issues
 Project-URL: Documentation, https://munichpavel.github.io/fake-data-docs/html/index.html
 Project-URL: Source Code, https://github.com/munichpavel/fake-data-for-learning/
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >3.6
@@ -32,9 +29,7 @@
 For machine learning experimentation, it is useful to have an unlimited supply
  of interesting fake data, where by interesting I mean that we know certain
  properties of the data and want to test if the algorithm can pick this up. A
  great potential source of such data is graphical models.
 
 In the current release, we generate fake data with discrete Bayesian networks
  (also known as directed graphical models).
-
-
```

### Comparing `fake_data_for_learning-0.4.0/README.md` & `fake_data_for_learning-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # fake-data-for-learning
 
+![ci](https://github.com/munichpavel/fake-data-for-learning/actions/workflows/ci.yml/badge.svg)
+
 Interesting fake multivariate data is harder to generate than it should be. Textbooks typically give definitions, two standard examples (multinomial and multivariate normal) and then proceed to proving theorems and propositions. True, one dimensional distributions can be combined, but here as well the source of examples is also sparse, e.g. products of distributions or copulas (typically Gaussian or t-copulas) applied to these 1-d examples.
 
 For machine learning experimentation, it is useful to have an unlimited supply of interesting fake data, where by interesting I mean that we know certain properties of the data and want to test if the algorithm can pick this up. A great potential source of such data is graphical models.
 
 The goal of this package is to make it easy to generate interesting fake data. In the current release, we generate fake data with discrete Bayesian networks (also known as directed graphical models).
 
 * **Website**: [https://munichpavel.github.io/fake-data-for-learning](https://munichpavel.github.io/fake-data-for-learning)
@@ -35,26 +37,26 @@
 # 0.4
 
 # Sample from Y given Gender
 Y.rvs({'Gender': SampleValue('male', label_encoder=Gender.label_encoder)}, seed=42)
 # array([0])
 ```
 
-Combine into a Bayesian network. Sample and calculate the probability mass function of each sample.
+Combine into a Bayesian network; sample and calculate the probability mass function of each sample:
 
 ```python
 from fake_data_for_learning.fake_data_for_learning import FakeDataBayesianNetwork
 samples = bn.rvs(size=5)
 # Rounding of pmf is only for display purposes
 samples['pmf'] = samples[['Gender', 'Y']].apply(lambda sample: round(bn.pmf(sample), 3), axis=1)
 ```
 
 ![docs/graphics/network_sample.png](docs/graphics/network_sample.png)
 
-Visualize the Bayesian network
+Visualize the Bayesian network:
 
 ```python
 bn.draw_graph()
 ```
 
 ![docs/graphics/graph.png](docs/graphics/graph.png)
 
@@ -91,10 +93,14 @@
 
 * [pyagrum](https://pyagrum.readthedocs.io) is a Python wrapper around the C++ library [aGrUM](http://agrum.org/), and has similar funcionality with a larger scope. Unlike `pgmpy`, `pyagrum` has a similar API for specifying conditional probability tables to the one used here.
 
 * [causalgraphicalmodels](https://github.com/ijmbarr/causalgraphicalmodels)'s class `StructuralCausalModel` allows sampling from Bayesian network where the variables are related as functions of one another, rather than via the conditional probability tables used here.
 
 ## Change log
 
+### v0.4.1
+
+Fix dependencies' API changes
+
 ### v0.4.0
 
 This release adds a method for generating categorical data whose (multidimensional) contingency table equals a given one. The motivation is to generate fake data exhibiting [Simpson's paradox](https://en.wikipedia.org/wiki/Simpson%27s_paradox).
```

### Comparing `fake_data_for_learning-0.4.0/docs/source/index.rst` & `fake_data_for_learning-0.4.1/fake_data_for_learning.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-Welcome to fake-data-for-learning's documentation!
-==================================================
+Metadata-Version: 2.1
+Name: fake-data-for-learning
+Version: 0.4.1
+Author: Paul Larsen
+Author-email: munichpavel@gmail.com
+License: MIT license
+Project-URL: Homepage, https://munichpavel.github.io/fake-data-for-learning/
+Project-URL: Bug Tracker, https://github.com/munichpavel/fake-data-for-learning/issues
+Project-URL: Documentation, https://munichpavel.github.io/fake-data-docs/html/index.html
+Project-URL: Source Code, https://github.com/munichpavel/fake-data-for-learning/
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+Interesting fake multivariate data is harder to generate than it should be.
+ Textbooks typically give definitions, two standard examples (multinomial and
+ multivariate normal) and then proceed to proving theorems and propositions.
+ True, one dimensional distributions can be combined, but here as well the
+ source of examples is also sparse, e.g. products of distributions or copulas
+ (typically Gaussian or t-copulas) applied to these 1-d examples.
+
+For machine learning experimentation, it is useful to have an unlimited supply
+ of interesting fake data, where by interesting I mean that we know certain
+ properties of the data and want to test if the algorithm can pick this up. A
+ great potential source of such data is graphical models.
 
-Interesting fake multivariate data is harder to generate than it should be. Textbooks typically give definitions, two standard examples (multinomial and multivariate normal) and then proceed to proving theorems and propositions. True, one dimensional distributions can be combined, but here as well the source of examples is also sparse, e.g. products of distributions or copulas (typically Gaussian or t-copulas) applied to these 1-d examples.
-
-For machine learning experimentation, it is useful to have an unlimited supply of interesting fake data, where by interesting I mean that we know certain properties of the data and want to test if the algorithm can pick this up. A great potential source of such data is graphical models.
-
-In the current release, we generate fake data with discrete Bayesian networks (also known as directed graphical models).
-
-.. toctree::
-   :maxdepth: 1
-   :caption: Contents:
-
-   api
-
-Installation
-------------
-
-Install from `pypi`_: ``pip install fake-data-for-learning``
-
-.. _pypi: https://pypi.org/project/fake-data-for-learning/
-
-Note that the methods of `utils.ProbabilityPolytope` that use polytope calculatations to generate conditional probability tables subject to constraints on expectation value uses the non-pure-python library `pypoman`_. See the installation `instructions`_ for external dependencies.
-
-.. _pypoman: https://github.com/stephane-caron/pypoman
-.. _instructions: https://github.com/stephane-caron/pypoman#installation
-
-Links
------
-
-**Website**: https://munichpavel.github.io/fake-data-for-learning
-
-**GitHub Repository**: https://github.com/munichpavel/fake-data-for-learning
-
-**PyPI**: https://pypi.org/project/fake-data-for-learning/
-
-
-Indices and tables
-==================
-
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+In the current release, we generate fake data with discrete Bayesian networks
+ (also known as directed graphical models).
```

### Comparing `fake_data_for_learning-0.4.0/fake_data_for_learning/contingency_tables.py` & `fake_data_for_learning-0.4.1/fake_data_for_learning/contingency_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         try:
             flat_contingency_table[event] = contingency_table[event]
         except TypeError:
             msg = f'Only integer coordinate values supported, entered coord was {event}'
             raise NotImplementedError(msg)
 
     samples = []
-    for idx, count in flat_contingency_table.iteritems():
+    for idx, count in flat_contingency_table.items():
         samples += count * [idx]
     res = pd.DataFrame(samples, columns=dims)
     # Shuffle rows uniformly so it looks better
     res = res.sample(
         res.shape[0], replace=False, random_state=seed
     ).reset_index(drop=True)
     return res
```

### Comparing `fake_data_for_learning-0.4.0/fake_data_for_learning/fake_data_for_learning.py` & `fake_data_for_learning-0.4.1/fake_data_for_learning/fake_data_for_learning.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
                 return value
 
     @staticmethod
     def possible_default_value(x):
         """
         Check conditions that rule-out a default (i.e. natural number) value.
         """
-        if isinstance(x, np.int) or isinstance(x, np.int64):
+        if isinstance(x, int) or isinstance(x, np.int64):
             return x >= 0
         else:
             return False
 
     def __str_(self):
         return 'SampleValue({}, {})'.format(self.value, self.label_encoder)
 
@@ -376,15 +376,15 @@
         """Return 1 if name is in list l, else 0."""
         if l is None:
             return 0
         res = name in l
         return res
 
     def get_graph(self):
-        g = nx.from_numpy_matrix(
+        g = nx.from_numpy_array(
             self.adjacency_matrix, create_using=nx.DiGraph
         )
         # Add node labels
         labels = {n: self.node_names[n] for n in range(len(self.node_names))}
         g = nx.relabel_nodes(g, labels)
         return g
```

### Comparing `fake_data_for_learning-0.4.0/fake_data_for_learning/probability_polytopes.py` & `fake_data_for_learning-0.4.1/fake_data_for_learning/probability_polytopes.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.0/fake_data_for_learning/utils.py` & `fake_data_for_learning-0.4.1/fake_data_for_learning/utils.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.0/setup.py` & `fake_data_for_learning-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     'xarray',
     'pypoman'
 ]
 
 
 setup(
     name='fake_data_for_learning',
-    version='0.4.0',
+    version='0.4.1',
     long_description=description,
     long_description_content_type='text/markdown',
     project_urls={
         "Homepage": "https://munichpavel.github.io/fake-data-for-learning/",
         "Bug Tracker": "https://github.com/munichpavel/fake-data-for-learning/issues",
         "Documentation": "https://munichpavel.github.io/fake-data-docs/html/index.html",
         "Source Code": "https://github.com/munichpavel/fake-data-for-learning/",
```

### Comparing `fake_data_for_learning-0.4.0/tests/test_bayesian_node_rv.py` & `fake_data_for_learning-0.4.1/tests/test_bayesian_node_rv.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.0/tests/test_contingency_tables.py` & `fake_data_for_learning-0.4.1/tests/test_contingency_tables.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.0/tests/test_demo_notebooks.py` & `fake_data_for_learning-0.4.1/tests/test_demo_notebooks.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.0/tests/test_fake_data_bn.py` & `fake_data_for_learning-0.4.1/tests/test_fake_data_bn.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,10 +338,9 @@
         [(0, 0), (0, 1), (1, 0), (1, 1)],
         names=['X0', 'X1'])
     expected_ratios = pd.Series(
         [0.125, 0.375, 0.375, 0.125],
         index=expected_index
     )
     pd.testing.assert_series_equal(
-        sample_ratios, expected_ratios,
-        check_exact=False, check_less_precise=0
+        sample_ratios, expected_ratios, check_exact=False, rtol=0.1
     )
```

### Comparing `fake_data_for_learning-0.4.0/tests/test_probability_polytopes.py` & `fake_data_for_learning-0.4.1/tests/test_probability_polytopes.py`

 * *Files identical despite different names*

### Comparing `fake_data_for_learning-0.4.0/tests/test_utils.py` & `fake_data_for_learning-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

