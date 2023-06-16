# Comparing `tmp/UComp-1.0.61.tar.gz` & `tmp/UComp-1.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.61.tar", last modified: Thu Jun 15 07:07:01 2023, max compression
+gzip compressed data, was "UComp-1.0.62.tar", last modified: Fri Jun 16 08:13:33 2023, max compression
```

## Comparing `UComp-1.0.61.tar` & `UComp-1.0.62.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 07:07:01.032080 UComp-1.0.61/
--rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.61/MANIFEST.in
--rw-rw-rw-   0        0        0      343 2023-06-15 07:07:01.032080 UComp-1.0.61/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.61/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 07:07:00.978691 UComp-1.0.61/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.61/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.61/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    11378 2023-06-14 17:01:33.000000 UComp-1.0.61/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0    11790 2023-06-14 14:49:10.000000 UComp-1.0.61/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.61/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.61/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24515 2023-06-14 14:47:37.000000 UComp-1.0.61/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.61/UComp/__init__.py
--rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.61/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.61/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.61/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.61/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    29855 2023-06-14 14:47:37.000000 UComp-1.0.61/UComp/tools.py
--rw-rw-rw-   0        0        0      641 2023-06-15 07:05:30.000000 UComp-1.0.61/UComp/tsfile.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:07:01.032080 UComp-1.0.61/UComp.egg-info/
--rw-rw-rw-   0        0        0      343 2023-06-15 07:07:00.000000 UComp-1.0.61/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-15 07:07:00.000000 UComp-1.0.61/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 07:07:00.000000 UComp-1.0.61/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-15 07:07:00.000000 UComp-1.0.61/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 07:07:00.000000 UComp-1.0.61/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 07:07:01.032080 UComp-1.0.61/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-15 07:06:27.000000 UComp-1.0.61/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:13:33.142972 UComp-1.0.62/
+-rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.62/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2023-06-16 08:13:33.142972 UComp-1.0.62/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.62/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 08:13:33.103465 UComp-1.0.62/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.62/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.62/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    11378 2023-06-16 08:11:50.000000 UComp-1.0.62/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0    11790 2023-06-16 08:11:41.000000 UComp-1.0.62/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.62/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.62/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24515 2023-06-16 08:11:46.000000 UComp-1.0.62/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.62/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.62/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.62/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.62/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.62/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    29875 2023-06-16 08:11:37.000000 UComp-1.0.62/UComp/tools.py
+-rw-rw-rw-   0        0        0      641 2023-06-15 07:05:30.000000 UComp-1.0.62/UComp/tsfile.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:13:33.142972 UComp-1.0.62/UComp.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-16 08:13:32.000000 UComp-1.0.62/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-16 08:13:32.000000 UComp-1.0.62/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 08:13:32.000000 UComp-1.0.62/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-16 08:13:32.000000 UComp-1.0.62/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 08:13:32.000000 UComp-1.0.62/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 08:13:33.142972 UComp-1.0.62/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-16 08:13:10.000000 UComp-1.0.62/setup.py
```

### Comparing `UComp-1.0.61/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.62/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.61/UComp/ETSmodule.py` & `UComp-1.0.62/UComp/ETSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.61/UComp/PTSmodule.py` & `UComp-1.0.62/UComp/PTSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.61/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.62/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.61/UComp/UCmodule.py` & `UComp-1.0.62/UComp/UCmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.61/UComp/airpas.bin` & `UComp-1.0.62/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.61/UComp/gdp.bin` & `UComp-1.0.62/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.61/UComp/ipi.bin` & `UComp-1.0.62/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.61/UComp/libopenblas.dll` & `UComp-1.0.62/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.61/UComp/tools.py` & `UComp-1.0.62/UComp/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     from UComp import UCmodule as uc
     from UComp import ETSmodule as ets
     from UComp import PTSmodule as pts
     from UComp import tsfile
 else:
     import UCmodule as uc
     import ETSmodule as ets
+    import PTSmodule as pts
 
 
 ipi = pd.read_pickle("ipi.bin")
 gdp = pd.read_pickle("gdp.bin")
 airpas = pd.read_pickle("airpas.bin")
 
 
@@ -744,15 +745,15 @@
     plotH = pd.DataFrame(metrics, index=np.arange(1, h + 1))
     plt.plot(plotH)
     plt.ylabel("Error metric")
     plt.show(block=False)
     return outj
 
 
-def Accuracy(py, y, collectFun=np.mean):
+def Accuracy(py, y, s=1, collectFun=np.mean):
     """
     Accuracy for 1 time series y and several forecasting
     methods py and h steps ahead py is h x nMethods x nSeries
     Inputs:
         py:         matrix of forecasts (h x nMethods x nForecasts)
         y:          a matrix of actual values (n x nForecasts)
         s:          seasonal period, number of observations per year
@@ -763,24 +764,25 @@
     Author: Diego J. Pedregal
     """
     # Accuracy for 1 time series y and several forecasting methods py and h steps ahead
     # py is h x nMethods x nSeries
     # y is n x nSeries
     spy = len(py.shape)
     if (isinstance(py, pd.Series) or isinstance(py, pd.DataFrame)) and isinstance(y, pd.Series):
+        s = y.resample('Y').count()[1]
         tpy = py.index
         ty = y.index
-        if min(tpy) - max(ty) > 1e-5:
+        if min(tpy) > max(ty):
             raise ValueError("No errors to estimate, check dates!!!")
-        if max(tpy) - max(ty) > 1e-5:
+        if max(tpy) > max(ty):
             # Cut forecasts
-            py = py.head(np.where(max(ty) == tpy)[0])
-        if max(ty) - max(tpy) > 1e-5:
+            py = py[:, :int(np.where(max(ty) == tpy)[0] + 1)]
+        if max(ty) > max(tpy):
             # Cut time series
-            y = y.head(np.where(max(tpy) == ty)[0])
+            y = y[:int(np.where(max(tpy) == ty)[0] + 1)]
     if spy == 1:
         raise ValueError("Input 'py' should be: h x number of methods x number of series!!!")
     elif spy == 2:
         # aux = np.empty((py.shape[0], py.shape[1], 1))
         # aux[:, :, :] = py
         # aux = np.asmatrix(aux)
         py = np.reshape(py, (py.shape[0], py.shape[1], 1))
@@ -805,30 +807,30 @@
         colnames.extend(["MASE", "RelMAE", "Theil's U"])
     out = np.zeros((len(rownames), len(colnames)))
     # out.index.name = colnames(py)
     for i in range(ny):
         e = py[:, i, :] - y[-h:, :]
         p = 100 * e / y[-h:, :]
         aux = np.stack((np.nanmean(e, axis=0),
-                              np.sqrt(np.nanmean(e * e, axis=0)),
-                              np.nanmean(np.abs(e), axis=0),
-                              np.nanmean(p, axis=0),
-                              np.sqrt(np.nanmean(p * p, axis=0)),
-                              np.nanmean(np.abs(p), axis=0),
-                              np.nanmean(200 * np.abs(e) / (py[:, i, :] + y[-h:, :]), axis=0)),
-                             axis=0)
+                        np.sqrt(np.nanmean(e * e, axis=0)),
+                        np.nanmean(np.abs(e), axis=0),
+                        np.nanmean(p, axis=0),
+                        np.sqrt(np.nanmean(p * p, axis=0)),
+                        np.nanmean(np.abs(p), axis=0),
+                        np.nanmean(200 * np.abs(e) / (py[:, i, :] + y[-h:, :]), axis=0)),
+                        axis=0)
         if insample:
-            theil = 100 * (y[-h:, :] - y[(n - h):(n - 1), :]) / y[-h:, :]
+            theil = 100 * (y[-h:, :] - y[(n - h - 1):(n - 1), :]) / y[-h:, :]
             fRW = y[(s + 1):(n - h), :] - y[1:(n - h - s), :]
             if nSeries == 1:
                 fRW = np.reshape(fRW, (len(fRW), 1))
-            aux = np.column_stack((aux,
-                                   np.nanmean(np.abs(e), axis=0) / np.nanmean(np.abs(fRW), axis=0),
-                                   np.nansum(np.abs(e), axis=0) / np.nansum(np.abs(fRW), axis=0),
-                                   np.sqrt(np.nansum(p * p, axis=0) / np.nansum(theil * theil, axis=0))))
+            aux1 = np.stack((np.nanmean(np.abs(e), axis=0) / np.nanmean(np.abs(fRW), axis=0),
+                             np.nansum(np.abs(e), axis=0) / np.nansum(np.abs(fRW), axis=0),
+                             np.sqrt(np.nansum(p * p, axis=0) / np.nansum(theil * theil, axis=0))), axis=0)
+            aux = np.vstack((aux, aux1))
         out[i, :] = collectFun(aux, axis=1)
     return pd.DataFrame(out, index=rownames, columns=colnames)
 
 
 def tsDisplay(y, nCoef=None, nPar=0):
     """
     tsDisplay
```

### Comparing `UComp-1.0.61/UComp/tsfile.py` & `UComp-1.0.62/UComp/tsfile.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.61/setup.py` & `UComp-1.0.62/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.61',
+    version='1.0.62',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

