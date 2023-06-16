# Comparing `tmp/UComp-1.0.64.tar.gz` & `tmp/UComp-1.0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.64.tar", last modified: Fri Jun 16 08:40:51 2023, max compression
+gzip compressed data, was "UComp-1.0.65.tar", last modified: Fri Jun 16 10:58:09 2023, max compression
```

## Comparing `UComp-1.0.64.tar` & `UComp-1.0.65.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 08:40:51.563177 UComp-1.0.64/
--rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.64/MANIFEST.in
--rw-rw-rw-   0        0        0      343 2023-06-16 08:40:51.564174 UComp-1.0.64/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.64/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 08:40:51.525236 UComp-1.0.64/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.64/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.64/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    11378 2023-06-16 08:39:21.000000 UComp-1.0.64/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0    11790 2023-06-16 08:39:11.000000 UComp-1.0.64/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.64/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.64/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24515 2023-06-16 08:39:16.000000 UComp-1.0.64/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.64/UComp/__init__.py
--rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.64/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.64/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.64/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.64/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    29804 2023-06-16 08:39:05.000000 UComp-1.0.64/UComp/tools.py
--rw-rw-rw-   0        0        0      641 2023-06-15 07:05:30.000000 UComp-1.0.64/UComp/tsfile.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:40:51.562178 UComp-1.0.64/UComp.egg-info/
--rw-rw-rw-   0        0        0      343 2023-06-16 08:40:51.000000 UComp-1.0.64/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-16 08:40:51.000000 UComp-1.0.64/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 08:40:51.000000 UComp-1.0.64/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-16 08:40:51.000000 UComp-1.0.64/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 08:40:51.000000 UComp-1.0.64/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 08:40:51.566172 UComp-1.0.64/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-16 08:40:37.000000 UComp-1.0.64/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 10:58:09.116861 UComp-1.0.65/
+-rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.65/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2023-06-16 10:58:09.117860 UComp-1.0.65/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.65/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 10:58:09.092900 UComp-1.0.65/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.65/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.65/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    11378 2023-06-16 08:39:21.000000 UComp-1.0.65/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0    11787 2023-06-16 10:57:22.000000 UComp-1.0.65/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.65/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.65/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24515 2023-06-16 08:39:16.000000 UComp-1.0.65/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.65/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.65/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.65/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.65/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.65/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    29804 2023-06-16 08:39:05.000000 UComp-1.0.65/UComp/tools.py
+-rw-rw-rw-   0        0        0      641 2023-06-15 07:05:30.000000 UComp-1.0.65/UComp/tsfile.py
+drwxrwxrwx   0        0        0        0 2023-06-16 10:58:09.115864 UComp-1.0.65/UComp.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-16 10:58:08.000000 UComp-1.0.65/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-16 10:58:08.000000 UComp-1.0.65/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 10:58:08.000000 UComp-1.0.65/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-16 10:58:08.000000 UComp-1.0.65/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 10:58:08.000000 UComp-1.0.65/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 10:58:09.119857 UComp-1.0.65/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-16 10:58:02.000000 UComp-1.0.65/setup.py
```

### Comparing `UComp-1.0.64/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.65/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.64/UComp/ETSmodule.py` & `UComp-1.0.65/UComp/ETSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.64/UComp/PTSmodule.py` & `UComp-1.0.65/UComp/PTSmodule.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,16 +181,16 @@
         self.modelUCmodel = None
         if s < 2:
             periods = np.array([1])
         else:
             periods = np.array(s) / range(1, int(s / 2) + 1)
         mUC = uc.UCmodel(y, s, u, self.modelUC, h, lambdaBoxCox=lambdaBoxCox,
                          criterion=criterion, periods=periods,
-                         verbose=verbose, trendOptions="none/rw/llt/dt",
-                         seasonalOptions="none/equal/different", irregularOptions="none/arma(0,0)",
+                         verbose=verbose, trendOptions="rw/llt/srw",
+                         seasonalOptions="none/linear/different", irregularOptions="none/arma(0,0)",
                          MSOE=True, PTSnames=True)
         if mUC.model == "error":
             self.model = "error"
             return
         self.armaOrders = modelUC2arma(mUC.model)
         self.model = modelUC2PTS(mUC.model)
         self.p0 = mUC.p0
```

### Comparing `UComp-1.0.64/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.65/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.64/UComp/UCmodule.py` & `UComp-1.0.65/UComp/UCmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.64/UComp/airpas.bin` & `UComp-1.0.65/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.64/UComp/gdp.bin` & `UComp-1.0.65/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.64/UComp/ipi.bin` & `UComp-1.0.65/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.64/UComp/libopenblas.dll` & `UComp-1.0.65/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.64/UComp/tools.py` & `UComp-1.0.65/UComp/tools.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.64/UComp/tsfile.py` & `UComp-1.0.65/UComp/tsfile.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.64/setup.py` & `UComp-1.0.65/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.64',
+    version='1.0.65',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

