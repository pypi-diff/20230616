# Comparing `tmp/EclipsingBinaries-2.8.4a9.tar.gz` & `tmp/EclipsingBinaries-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-2.8.4a9.tar", last modified: Tue Jun 13 02:29:56 2023, max compression
+gzip compressed data, was "EclipsingBinaries-3.0.0a1.tar", last modified: Fri Jun 16 18:03:20 2023, max compression
```

## Comparing `EclipsingBinaries-2.8.4a9.tar` & `EclipsingBinaries-3.0.0a1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:29:56.091896 EclipsingBinaries-2.8.4a9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:29:56.087896 EclipsingBinaries-2.8.4a9/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    20561 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17365 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:29:56.091896 EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/multi_aperture_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:29:56.091896 EclipsingBinaries-2.8.4a9/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:29:56.091896 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-13 02:29:56.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-13 02:29:56.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:29:56.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 02:29:56.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 02:29:56.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 02:29:56.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-13 02:29:56.091896 EclipsingBinaries-2.8.4a9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:29:56.091896 EclipsingBinaries-2.8.4a9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:03:20.657333 EclipsingBinaries-3.0.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:03:20.653333 EclipsingBinaries-3.0.0a1/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17365 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:03:20.657333 EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/multi_aperture_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:03:20.657333 EclipsingBinaries-3.0.0a1/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:03:20.657333 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-16 18:03:20.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-16 18:03:20.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:03:20.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-16 18:03:20.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-16 18:03:20.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 18:03:20.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-16 18:03:20.657333 EclipsingBinaries-3.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:03:20.657333 EclipsingBinaries-3.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/setup.py
```

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/IRAF_Reduction.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/OC_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Author: Kyle Koeller
 Created: 12/19/2022
-Last Edited: 06/12/2023
+Last Edited: 06/13/2023
 
 This calculates O-C values and produces an O-C plot.
 """
 
-from math import sqrt
+from math import sqrt, floor
 import pandas as pd
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy.polynomial import Polynomial
 import statsmodels.formula.api as smf
 import seaborn as sns
 from numba import jit
+import time
 
 
 def main(period=None, loop=0, num=None, nights=None):
     if loop == 0:
         print("\n\nThe format of these input files should be the of the raw form given from Dr. Robert Berrginton's"
               " 'find_minimum' C program.")
         print("Run TESS data by itself through the TESS option and filtered SARA/BSUO data through the BSU option.\n"
@@ -105,15 +106,15 @@
     E_est = []
     O_C = []
     O_C_err = []
 
     # this for loop, loops through the min_strict list and calculates a variety of values
     for count, val in enumerate(min_strict):
         # call the function to calculate the O-C values
-        e, OC, OC_err, T0, To_err = calcualte_oc(val, min_strict_err[count], T0, To_err, period)
+        e, OC, OC_err, T0, To_err = calculate_oc(val, min_strict_err[count], T0, To_err, period)
 
         E_est.append(e)
         O_C.append(OC)
         O_C_err.append(OC_err)
 
     # create a dataframe for all outputs to be places in for easy output
     dp = pd.DataFrame({
@@ -160,15 +161,15 @@
         minimum = (val + strict_V[count] + strict_R[count]) / 3
         err = sqrt(strict_B_err[count] ** 2 + strict_V_err[count] ** 2 + strict_R_err[count] ** 2) / 3
 
         average_min.append("%.5f" % minimum)
         average_err.append(err)
 
         # call the function to calculate the O-C values
-        e, OC, OC_err, T0, To_err = calcualte_oc(minimum, err, T0, To_err, period)
+        e, OC, OC_err, T0, To_err = calculate_oc(minimum, err, T0, To_err, period)
         E_est.append(e)
         O_C.append(OC)
         O_C_err.append(OC_err)
 
     # create a dataframe for all outputs to be places in for easy output
     dp = pd.DataFrame({
         "Minimums": average_min,
@@ -190,29 +191,27 @@
 def all_data(nights, period, loop):
     """
     Merges all the data into a singular file for ease of use
 
     :param nights: number of files there are for the first time through
     :param period: period of the system
     :param loop: number of loops through the program either o or 1
-
     :return: None
     """
     count = 0
 
     minimum_list = []
     e_list = []
     o_c_list = []
     o_c_err_list = []
 
     while True:
-        print(
-            "\n\nPlease make sure that the very first line for each and every file that you have starts with the following\n"
-            "'Minimums	Epoch	O-C	O-C_Error'\n"
-            "With each space entered as a space.\n")
+        print("\n\nPlease make sure that the very first line for each and every file that you have starts with the following\n"
+              "'Minimums	Epoch	O-C	O-C_Error'\n"
+              "With each space entered as a space.\n")
         fname = input("Please enter a file name and pathway (i.e. C:\\folder1\\folder2\\[file name]): ")
         df = pd.read_csv(fname, header=None, skiprows=[0], delim_whitespace=True)
         minimum = np.array(df[0])
         e = np.array(df[1])
         o_c = np.array(df[2])
         o_c_err = np.array(df[3])
 
@@ -250,16 +249,16 @@
     table_header += '$BJD_{\\rm TDB}$ & E & O-C \\\ \n'
     table_header += '\\hline\n' + '\\endhead\n' + '\\hline\n'
     table_header += '\\multicolumn{3}{c}{\\textit{Continued on next page}} \\\ \n'
     table_header += '\\endfoot\n' + '\\endlastfoot\n'
 
     minimum_lines = []
     for i in range(len(minimum)):
-        line = str("%.5f" % minimum[i]) + ' & ' + str(e[i]) + ' & $' + str("%.5f" % o_c[i]) + ' \pm ' + str(
-            "%.5f" % o_c_err[i]) + '$ ' + "\\\ \n"
+        line = str("%.5f" % minimum[i]) + ' & ' + str(e[i]) + ' & $' + str("%.5f" % o_c[i]) + ' \pm ' + \
+               str("%.5f" % o_c_err[i]) + '$ ' + "\\\ \n"
         minimum_lines.append(line)
 
     output = table_header
     for count, line in enumerate(minimum_lines):
         output += line
 
     output += '\\hline\n' + '\\caption{NSVS 896797 O-C. The first column is the \n' \
@@ -297,15 +296,15 @@
             break
         except ValueError:
             print("You have entered an invalid value. Please only enter float values and please try again.\n")
     return T0, To_err, period
 
 
 @jit(forceobj=True)
-def calcualte_oc(m, err, T0, T0_err, p):
+def calculate_oc(m, err, T0, T0_err, p):
     """
     Calculates O-C values and errors and find the eclipse number for primary and secondary eclipses
     :param m: ToM
     :param err: ToM error
     :param T0: first ToM
     :param T0_err: error for the T0
     :param p: period of the system
@@ -314,15 +313,15 @@
     """
     if T0 == 0:
         T0 = m
         T0_err = err
     # get the exact E value
     E_act = (m - T0) / p
     # estimate for the primary or secondary eclipse by rounding to the nearest 0.5
-    e = round(E_act * 2) / 2
+    e = floor(E_act * 2) / 2
     # calculate the calculated ToM and find the O-C value
     T_calc = T0 + (e * p)
     OC = "%.5f" % (m - T_calc)
 
     # determine the error of the O-C
     OC_err = "%.5f" % sqrt(T0_err ** 2 + err ** 2)
 
@@ -345,15 +344,16 @@
     df = pd.read_csv(input_file, header=0, delim_whitespace=True)
 
     # append values to their respective lists for further and future potential use
     x = df["Epoch"]
     y = df["O-C"]
     y_err = df["O-C_Error"]
 
-    weights = 1/(y_err**2)
+    # weights for least squares fitting
+    weights = 1 / (y_err ** 2)
 
     # these next parts are mainly for O-C data as I just want to plot primary minima's and not both primary/secondary
     x1_prim = []
     y1_prim = []
     y_err_new_prim = []
 
     x1_sec = []
@@ -393,16 +393,15 @@
             \\usepackage{booktabs}
             \\begin{document}"""
     endtex = "\end{document}"
 
     # opens a file with this name to begin writing to the file
     output_test = None
     while not output_test:
-        output_file = input(
-            "\nWhat is the output file name and pathway for the regression tables (either .txt or .tex): ")
+        output_file = input("\nWhat is the output file name and pathway for the regression tables (either .txt or .tex): ")
         if output_file.endswith((".txt", ".tex")):
             output_test = True
         else:
             print("This is not an allowed file output. Please make sure the file has the extension .txt or .tex.\n")
 
     # noinspection PyUnboundLocalVariable
     f = open(output_file, 'w')
@@ -449,18 +448,17 @@
     f.close()
     print("\nFinished saving latex/text file.\n\n")
 
     fontsize = 14
     plt.errorbar(x1_prim, y1_prim, yerr=y_err_new_prim, fmt="o", color="blue", label="Primary")
     plt.errorbar(x1_sec, y1_sec, yerr=y_err_new_sec, fmt="s", color="green", label="Secondary")
     # allows the legend to be moved wherever the user wants the legend to be placed rather than in a fixed location
-    print("\n\nNOTE:")
-    print(
-        "You can drag the legend to move it wherever you would like, the default is the top right. Just click and drag"
-        " to move around the figure.\n")
+    print("\n\n\033[1m" + "\033[93m" + "NOTE" + "\033[00m" + ":")
+    print("You can drag the legend to move it wherever you would like, the default is the top right. Just click and drag"
+          " to move around the figure.\n")
     plt.legend(loc="upper right", fontsize=fontsize).set_draggable(True)
 
     x_label = "Epoch"
     y_label = "O-C (days)"
 
     if loop == 0:
         print("\nThe figure just plotted is with the original period. The program will start over using a "
@@ -469,14 +467,15 @@
     # noinspection PyUnboundLocalVariable
     plt.xlabel(x_label, fontsize=fontsize)
     plt.xticks(fontsize=fontsize)
     # noinspection PyUnboundLocalVariable
     plt.ylabel(y_label, fontsize=fontsize)
     plt.yticks(fontsize=fontsize)
     plt.grid()
+    time.sleep(1)
     plt.show()
 
     if loop == 0:
         loop += 1
         main(new_period, loop, nights)
 
     # residuals(x1_prim, y1_prim, x_label, y_label, degree, model, xs)
@@ -511,14 +510,20 @@
 
     # allows for easy change of the format of the subplots
     rows = 2
     cols = 1
     # creates the figure subplot for appending next
     fig, (ax1, ax2) = plt.subplots(rows, cols)
     # adds gridlines to both subplots
+    """
+    a[0].grid(visible=True, which='major', color='black', linewidth=1.0)
+    a[0].grid(visible=True, which='minor', color='black', linewidth=0.5)
+    a[1].grid(visible=True, which='major', color='black', linewidth=1.0)
+    a[1].grid(visible=True, which='minor', color='black', linewidth=0.5)
+    """
     ax1.grid()
     ax2.grid()
     # creates the model line fit
     sns.lineplot(x=x_label, y=y_label, data=model_dat, ax=ax1, color="red")
     # plots the original data to the same subplot as the model fit
     # edge color is removed to any sort of weird visual overlay on the plots as the normal edge color is white
     sns.scatterplot(x=x_label, y=y_label, data=raw_dat, ax=ax1, color="black", edgecolor="none")
```

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/apass.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/apass.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/color_light_curve.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_B.txt` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_R.txt` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_V.txt` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_minimums.txt` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/find_min.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/find_min.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 """
 Created:  07/03/2021
 Original Author: Alec Neal
 
 Last Edits Done By: Kyle Koeller
-Last Edited: 05/14/2023
+Last Edited: 06/15/2023
 """
 
-# import vseq  # testing purposes
-from . import vseq_updated as vseq
+# from vseq_updated import calc, FT, io, plot  # testing purposes
+from .vseq_updated import calc, FT, io, plot
 from os import environ, path
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy
 # from tkinter import *
 from collections import Counter
 import statistics
@@ -61,15 +61,15 @@
     dcoef = []
     for n in range(1, len(coef)):
         dcoef.append(n * coef[n])
     allroots = np.unique(np.real(np.roots(dcoef[::-1])))
     # print(allroots)
     goodroots = []
     for root in range(len(allroots)):
-        if lb < allroots[root] < rb and -1e-2 < vseq.calc.poly.result(dcoef, allroots[root]) < 1e-2:
+        if lb < allroots[root] < rb and -1e-2 < calc.poly.result(dcoef, allroots[root]) < 1e-2:
             goodroots.append(allroots[root])
     root_est = (lb + rb) / 2
     try:
         bestroot = min(list(zip(abs(np.array(goodroots) - root_est), goodroots)))[1]
     except ValueError:
         print("\nAn error ocurred with your last boundary entry. Please try again.\n")
         plot_obs(filter_files, day=day, lb=last_lb, rb=last_rb, order=order, resolution=resolution, npairs=npairs,
@@ -106,14 +106,30 @@
     S = sum((interp(guess_min - klist * step) - interp(guess_min + klist * step)) ** 2)
 
     return S, K
 
 
 def KvW(fracHJD, flux, discard=0.1, resolution=100, para_range=None, plot=False,
         need_error=False, ax=None, npairs=20, entire_S=False):
+    """
+    KvW is the Kwee-van Woerden method for finding the minimum of a light curve.
+
+    fracHJD: list of fractional HJDs
+    flux: list of fluxes
+    discard: fraction of the light curve to discard from the edges
+    resolution: number of guesses to try
+    para_range: range of guesses to try
+    plot: whether or not to plot the results
+    need_error: whether or not to return the error
+    ax: axis to plot on
+    npairs: number of pairs to use
+    entire_S: whether or not to return the entire S list
+
+    returns: best guess and corresponding error of the Kwee van Woerdan method
+    """
     guess_range = (max(fracHJD) - min(fracHJD))
     guesses = np.linspace(guess_range * discard + min(fracHJD), guess_range * (1 - discard) + min(fracHJD), resolution)
     guesses = np.linspace(sorted(fracHJD)[1], sorted(fracHJD)[-2], resolution)
     Slist = []
     Klist = []
     for guess in guesses:
         # interp=scipy.interpolate.interp1d(fracHJD,flux)
@@ -134,34 +150,34 @@
     for n in range(1, para_range + 1):
         paraHJD.append(guesses[best_index + n])
         paraHJD.append(guesses[best_index - n])
         paraS.append(Slist[best_index + n])
         paraS.append(Slist[best_index - n])
 
     np.seterr(divide='ignore')
-    parabola = vseq.calc.poly.regr_polyfit(np.array(paraHJD), np.array(paraS), 2)
+    parabola = calc.poly.regr_polyfit(np.array(paraHJD), np.array(paraS), 2)
     coef, err, R2, results = parabola[:4]
     a, b, c = coef[::-1]
     if c - b ** 2 / (4 * a) < 0 or calc_S(fracHJD, flux, -b / (2 * a), npairs=npairs)[0] > paraS[0]:
         with np.errstate(divide='ignore'):
-            p2 = vseq.calc.poly.regr_polyfit(paraHJD[:3], paraS[:3], 2)
+            p2 = calc.poly.regr_polyfit(paraHJD[:3], paraS[:3], 2)
         # coef, err, R2, results = parabola[:4]
         a2, b2, c2 = p2[0][::-1]
         if c2 - b2 ** 2 / (4 * a2) < 0 or calc_S(fracHJD, flux, -b2 / (2 * a2), npairs=npairs)[0] > paraS[0]:
             T_kw = T_BF
         else:
             T_kw = -b2 / (2 * a2)
     else:
         T_kw = -b / (2 * a)
     S_at_tkw, Z = calc_S(fracHJD, flux, T_kw, npairs=npairs)
     Z /= 2
     if need_error:
         if Z <= 1:
             # print(Z)
-            print('Too few observations!')
+            print('\033[1m' + '\033[95m' + 'Too few observations!' + '\033[0m')
         sigt_kw = np.sqrt(S_at_tkw / (a * (Z - 1)))
 
         print('S(T_BF) =', paraS[0])
         print('S(T_KW) =', calc_S(fracHJD, flux, T_kw, npairs=npairs))
     else:
         sigt_kw = 1
 
@@ -169,15 +185,15 @@
         Srange = max(paraS) - min(paraS)
         HJDrange = max(paraHJD) - min(paraHJD)
         if not entire_S:
             ax.set_ylim(min(paraS) - Srange * 0.07, max(paraS) + Srange * 0.07)
             ax.set_xlim(min(paraHJD) - HJDrange * 0.025, max(paraHJD) + HJDrange * 0.025)
 
         ax.plot(guesses, np.array(Slist), 'ok', ms=5)
-        polyx, polyy = vseq.calc.poly.polylist(coef, min(paraHJD), max(paraHJD), 100)
+        polyx, polyy = calc.poly.polylist(coef, min(paraHJD), max(paraHJD), 100)
         ax.plot(polyx, polyy, 'b', lw=1)
         # plt.plot(paraHJD,results,'b',lw=1,label=r'${S}^{\prime}$')
         ax.axvline(T_kw, color='b', label=r'$T_{\rm KW}=' + str(round(T_kw, 6)) + '$', linewidth=1, ls='--')
         # ax.axvline(best_min[1], color='gray', label=r'$T_{\rm BF}=' + str(round(best_min[1], 6)) + '$', linewidth=1,
         #            ls='-.')
 
         ax.set_ylabel(r'$S$', fontsize=fontsize, usetex=False)
@@ -191,34 +207,34 @@
             Kstr = npairs
         # ax.text(xt, yt, r'$S_{\rm fit}/a=' + 'T^2' + str(strcoef[1]) + 'T+' + str(strcoef[0]) + '$'
         #                                                                                         '\n $R^2=' + str(
         #     round(R2, 5)) + '$'
         #                     r', $K=' + str(Kstr) + '~(' + str(int(Z * 2)) + ')$', fontsize=7)
         ax.text(xt, yt, '$R^2=' + str(round(R2, 5)) + '$, $K=' + str(Kstr) + '~(' + str(int(Z * 2)) + ')$', fontsize=7)
 
-    return T_kw, sigt_kw
+    return T_kw, sigt_kw, Z
 
 
 def sim_min(filter_HJD, filter_flux, filter_fluxerr, order, sims, filter_files):
     filters = len(filter_HJD)
     all_sims = []
     for sim in range(sims):
         all_sims.append([])
     filter_results = []
     HJD_inbounds = []
     for band in range(filters):
-        poly = vseq.calc.poly.regr_polyfit(filter_HJD[band], filter_flux[band], order)
+        poly = calc.poly.regr_polyfit(filter_HJD[band], filter_flux[band], order)
         filter_results.append(poly[3])
         HJD_inbounds += list(filter_HJD[band])
         for sim in range(sims):
-            all_sims[sim] += list(vseq.FT.sim_ob_flux(filter_results[band], filter_fluxerr[band], lower=-10, upper=10))
+            all_sims[sim] += list(FT.sim_ob_flux(filter_results[band], filter_fluxerr[band], lower=-10, upper=10))
     rootlist = []
     # kweelist = []
     for sim in tqdm(range(sims), position=0):
-        rootlist.append(best_root(vseq.calc.poly.regr_polyfit(HJD_inbounds, all_sims[sim], order)[0], min(HJD_inbounds),
+        rootlist.append(best_root(calc.poly.regr_polyfit(HJD_inbounds, all_sims[sim], order)[0], min(HJD_inbounds),
                                   max(HJD_inbounds), filter_files))
         # kweelist.append(KvW(HJD_inbounds,all_sims[sim])[0]) # uncomment to sim kwee
     rooterr = statistics.stdev(rootlist)
     # kweeerr=statistics.stdev(kweelist) # uncomment for siming kwee
     kweeerr = 0  # comment to sim kwee
     return rooterr, rootlist, kweeerr
 
@@ -239,25 +255,25 @@
     master_magnight = []
     master_fluxnight = []
     master_magerrnight = []
     master_fluxerrnight = []
     master_span = []
 
     for band in range(filters):
-        HJD_mag_magerr = vseq.io.importFile_pd(filter_files[band])
+        HJD_mag_magerr = io.importFile_pd(filter_files[band])
         HJD = HJD_mag_magerr[0]
         mag = HJD_mag_magerr[1]
         magerr = HJD_mag_magerr[2]
         HJD, mag, magerr = zip(*sorted(list(zip(HJD, mag, magerr))))
         master_HJD.append(HJD)
         master_mag.append(mag)
         master_magerr.append(magerr)
         master_dates.append([])
         for n in range(len(master_HJD[band])):
-            master_dates[band].append(vseq.calc.astro.convert.JD_to_Greg(np.floor(master_HJD[band][n]) + 0.75))
+            master_dates[band].append(calc.astro.convert.JD_to_Greg(np.floor(master_HJD[band][n]) + 0.75))
             # master_dates[band].append(np.floor(master_HJD[band][n]))
         count_nights = Counter(master_dates[band])
         count_uniques = np.unique(master_dates[band])
         master_unique_dates.append(list(count_uniques))
         master_ob_night.append([])
         master_HJDnight.append([])
         master_magnight.append([])
@@ -296,78 +312,78 @@
         all_fluxerr.append([])
         for band in range(filters):
             all_HJD[night] += list(master_HJDnight[band][night])
             all_flux[night] += list(master_fluxnight[band][night])
             all_fluxerr[night] += list(master_fluxerrnight[band][night])
 
     intday = int(all_HJD[day][0])
-    fracHJD = vseq.calc.frac(np.array(all_HJD[day]))
+    fracHJD = calc.frac(np.array(all_HJD[day]))
 
     global last_lb
     global last_rb
 
     if lb is not None and rb is not None:
         # Splot = plt.figure(1, figsize=(9,8), dpi=256)
         # MIN = Splot.subplots(len([1, 3]), sharex=False, sharey=False,
         #                   gridspec_kw={'hspace': 0, 'height_ratios': [1, 3]})
 
         parameters = {'axes.labelsize': fontsize}
         plt.rcParams.update(parameters)
 
-        [Splot, MIN], fig = vseq.plot.multiplot(figsize=(5, 4), height_ratios=[1, 4], sharex=False, sharey=False,
+        [Splot, MIN], fig = plot.multiplot(figsize=(5, 4), height_ratios=[1, 4], sharex=False, sharey=False,
                                                 hspace=0)
         MIN.errorbar(fracHJD, all_flux[day], all_fluxerr[day], fmt='ok', ms=3, capsize=3, elinewidth=0.6, ecolor='gray',
                      capthick=0.6)  # ,'ok',ms=3)
 
-        fig.canvas.mpl_connect('key_press_event', press)
-        fig.canvas.get_tk_widget().focus_force()
+        fig.canvas.mpl_connect('key_press_event', lambda event: press(event, Z))
+        # fig.canvas.get_tk_widget().focus_force()
 
         HJD_inbounds, flux_inbounds, fluxerr_inbounds = [], [], []
         for n in range(len(all_HJD[day])):
             if lb < fracHJD[n] < rb:
                 HJD_inbounds.append(fracHJD[n])
                 flux_inbounds.append(all_flux[day][n])
                 fluxerr_inbounds.append(all_fluxerr[day][n])
         try:
-            poly = vseq.calc.poly.regr_polyfit(HJD_inbounds, flux_inbounds, order)
+            poly = calc.poly.regr_polyfit(HJD_inbounds, flux_inbounds, order)
         except ValueError:
             print("\nThe boundary you last entered was incorrect, please try again. \n")
             plot_obs(filter_files, day=day, lb=last_lb, rb=last_rb, order=order, resolution=resolution, npairs=npairs,
                      para_range=None, norm_method="norm")
         try:
             coef, err, R2, results = poly[:4:]
         except UnboundLocalError:
             print("\nEntered in an incorrect boundary value. Please try again.\n")
             plot_obs(filter_files, day=day, lb=last_lb, rb=last_rb, order=order, resolution=resolution, npairs=npairs,
                      para_range=None, norm_method="norm")
-        print('R2 =', R2)
+        print('\n\nR2 =', R2)
         coef_deriv = []
 
         for n in range(1, len(coef)):
             coef_deriv.append(n * coef[n])
         HJD_band_in = []
         flux_band_in = []
         fluxerr_band_in = []
         for band in range(filters):
             HJD_band_in.append([])
             flux_band_in.append([])
             fluxerr_band_in.append([])
             for n in range(len(master_HJDnight[band][day])):
-                tempfrac = vseq.calc.frac(np.array(master_HJDnight[band][day]))
+                tempfrac = calc.frac(np.array(master_HJDnight[band][day]))
                 if lb < tempfrac[n] < rb:
                     HJD_band_in[band].append(tempfrac[n])
                     flux_band_in[band].append(master_fluxnight[band][day][n])
                     fluxerr_band_in[band].append(master_fluxerrnight[band][day][n])
 
         # red_chi = vseq.calc.error.red_X2(flux_inbounds, results, fluxerr_inbounds) / len(results)
         # root_error, kweeer = sim_min(HJD_band_in, flux_band_in, fluxerr_band_in, order, sims, filter_files)[0:3:2]
 
         # ===================================================================================================
         try:
-            t_kw, sigt_kw = KvW(HJD_inbounds, flux_inbounds, resolution=resolution, para_range=para_range, discard=discard,
+            t_kw, sigt_kw, Z = KvW(HJD_inbounds, flux_inbounds, resolution=resolution, para_range=para_range, discard=discard,
                                 need_error=True, ax=Splot, npairs=npairs, entire_S=entire_S)
         except IndexError:
             print("Please try entering in that last key board press you entered. An error ocurred.\n")
             plot_obs(filter_files, day=day, lb=last_lb, rb=last_rb, order=order, resolution=resolution, npairs=npairs,
                      para_range=None, norm_method="norm")
 
         # bestroot = best_root(coef, min(HJD_inbounds), max(HJD_inbounds), filter_files)
@@ -381,15 +397,15 @@
         MIN.set_ylim(None, 0.06 + MIN.get_ylim()[-1])
         MIN.margins(0.02, None)
         MIN.axvline(lb, color='limegreen', linestyle='--', alpha=1, linewidth=None)
         MIN.axvline(rb, color='limegreen', linestyle='--', alpha=1, linewidth=None)
         # MIN.axvline(bestroot, color='r',
         #            label=r'$T_{\rm LSQ^' + str(order) + '}=' + str(round(intday * 0 + bestroot, 6)) + '\pm' + str(
         #                round(idkerror, 6)) + '$')
-        poly_x, poly_y = vseq.calc.poly.polylist(coef, min(HJD_inbounds), max(HJD_inbounds), 100)
+        poly_x, poly_y = calc.poly.polylist(coef, min(HJD_inbounds), max(HJD_inbounds), 100)
         MIN.plot(poly_x, poly_y, 'r-', lw=1, zorder=10)
         Splot.xaxis.set_label_position("top")
         Splot.xaxis.tick_top()
 
         print('============================')
         print('T_KW:     ' + str(intday + t_kw))
         # totalerr = np.sqrt(sigt_kw ** 2 + kweeer ** 2)
@@ -405,28 +421,28 @@
         # print('err_form: ' + str(round(idkerror, 16)))
         # print('err_MC:   ' + str(round(root_error, 16)))
 
         MIN.legend(loc='upper right', framealpha=1, borderaxespad=0, shadow=False, fancybox=False, edgecolor='k', fontsize=5)
         MIN.annotate('' + filter_files[0] + '', xy=(MIN.get_xlim()[0] + 0.001, MIN.get_ylim()[1] - 0.005), va='top',
                      ha='left', fontsize=fontsize)
 
-        vseq.plot.sm_format(MIN, xtop=False, yright=False, ydirection='out', xdirection='out', X=Xtick, numbersize=6)
-        vseq.plot.sm_format(Splot, xbottom=False, yright=False, ydirection='out', xdirection='out', bottomspine=False,
+        plot.sm_format(MIN, xtop=False, yright=False, ydirection='out', xdirection='out', X=Xtick, numbersize=6)
+        plot.sm_format(Splot, xbottom=False, yright=False, ydirection='out', xdirection='out', bottomspine=False,
                             y=1000000, numbersize=6)
         plt.grid(alpha=0.35)
         plt.savefig('MIN-program_demo.pdf', bbox_inches='tight')
         # print(f"Backend: {plt.get_backend()}")
         f = zoom_factory(MIN, base_scale=2.)
         plt.show()
     else:
         ax = plt.figure(figsize=(9, 7), dpi=256).subplots()
-        vseq.plot.sm_format(ax, xformatter=False, numbersize=7, Xsize=0, xsize=0, tickwidth=1)
+        plot.sm_format(ax, xformatter=False, numbersize=7, Xsize=0, xsize=0, tickwidth=1)
         scaling = 1
         # fracHJD=vseq.calc.frac(np.array(all_HJD[day]))*scaling
-        fracHJD = vseq.calc.frac(np.array(all_HJD[day])) * scaling
+        fracHJD = calc.frac(np.array(all_HJD[day])) * scaling
 
         # plt.plot(fracHJD,all_flux[day],'ok',ms=3)
         plt.errorbar(fracHJD, all_flux[day], all_fluxerr[day], fmt='ok', ms=3, capsize=3, elinewidth=0.6, ecolor='gray',
                      capthick=0.6)  # ,'ok',ms=3)
         # plt.errorbar(fracHJD,-2.5*np.log10(np.array(all_flux[day])),all_fluxerr[day],fmt='ok',ms=3,capsize=3,elinewidth=0.6,ecolor='gray',capthick=0.6)#,'ok',ms=3)
         plt.xlabel('+' + str(intday) + ' [HJD]', fontsize=fontsize)
         plt.ylabel('Flux', fontsize=fontsize)
@@ -436,15 +452,29 @@
 
     last_lb = lb
     last_rb = rb
 
     return 'Done'
 
 
-def press(event):
+def press(event, Z):
+    """
+    Pressing a key will do something
+
+    Parameters
+    ----------
+    event : matplotlib event
+        The event that is triggered by pressing a key
+    Z : list
+        List of the data to be plotted
+
+    Returns
+    -------
+    None
+    """
     global rb
     global lb
     global day
     if event.key == "d":
         # right boundary line
         lb = lb
         rb = event.xdata
@@ -500,15 +530,15 @@
                      xdata + cur_xrange*scale_factor])
         ax.set_ylim([ydata - cur_yrange*scale_factor,
                      ydata + cur_yrange*scale_factor])
         plt.draw() # force re-draw
 
     fig = ax.get_figure() # get the figure of interest
     # attach the call back
-    fig.canvas.mpl_connect('scroll_event',zoom_fun)
+    fig.canvas.mpl_connect('scroll_event', zoom_fun)
 
     # return the function
     return zoom_fun
 
 
 def main():
     """
@@ -525,37 +555,40 @@
         while True:
             filter1 = input("Please enter a complete file pathway to your data file (i.e. C:\\folder1\\folder2\\data.txt: ")
             if path.exists(filter1):
                 break
             else:
                 print("\nOne of the files you have entered does not exist, please try all three again.\n")
                 continue
+        print("\nPress 'h' for help.\n")
         plot_obs([filter1], day=day, lb=lb, rb=rb, order=order, resolution=resolution, npairs=npairs,
                  para_range=None, norm_method='norm')
     elif num_filters == '2':
         while True:
             filter1 = input("Please enter a complete file pathway to data file 1 (i.e. C:\\folder1\\folder2\\data.txt: ")
             filter2 = input("Please enter a complete file pathway to data file 2 (i.e. C:\\folder1\\folder2\\data.txt: ")
             if path.exists(filter1) and path.exists(filter2):
                 break
             else:
                 print("\nOne of the files you have entered does not exist, please try all three again.\n")
                 continue
+        print("\nPress 'h' for help.\n")
         plot_obs([filter1, filter2], day=day, lb=lb, rb=rb, order=order, resolution=resolution, npairs=npairs,
                  para_range=None, norm_method='norm')
     elif num_filters == '3':
         while True:
             filter1 = input("Please enter a complete file pathway to data file 1 (i.e. C:\\folder1\\folder2\\data.txt: ")
             filter2 = input("Please enter a complete file pathway to data file 2 (i.e. C:\\folder1\\folder2\\data.txt: ")
             filter3 = input("Please enter a complete file pathway to data file 3 (i.e. C:\\folder1\\folder2\\data.txt: ")
             if path.exists(filter1) and path.exists(filter2) and path.exists(filter3):
                 break
             else:
                 print("\nOne of the files you have entered does not exist, please try all three again.\n")
                 continue
+        print("\nPress 'h' for help.\n")
         plot_obs([filter1, filter2, filter3], day=day, lb=lb, rb=rb, order=order, resolution=resolution, npairs=npairs,
                  para_range=None, norm_method='norm')
     elif num_filters.lower() == "close":
         exit()
     else:
         print("Please enter a number between 1-3 or the word 'Close'.\n")
         main()
```

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/gaia.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/menu.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/menu.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 The main program helps centralize all the other programs into one selection routine that can be run and call all
 other programs.
+
 Author: Kyle Koeller
 Created: 8/29/2022
-Last Updated: 05/14/2023
+Last Updated: 06/15/2023
 """
 
 import pandas as pd
 
 """
 # testing imports
 from tess_data_search import main as data_search
@@ -32,15 +33,15 @@
 
 
 def main():
     print("If you need a description of what each option does, please refer to the README for this packages GitHub page"
           " https://github.com/kjkoeller/EclipsingBinaries/")
     print("\nWhich program do you want to run?\n\n")
 
-    options = ["IRAF Reduction", "Find Minimum", "TESS Database Search/Download", "AIJ Comparison Star Selector",
+    options = ["IRAF Reduction", "Find Minimum (WIP)", "TESS Database Search/Download", "AIJ Comparison Star Selector",
                "BSUO or SARA/TESS Night Filters", "O-C Plotting", "Gaia Search", "O'Connel Effect", "Color Light Curve",
                "Close Program"]
     numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
 
     total = pd.DataFrame({"Options": options,
                           "Numbers": numbers})
```

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/multi_aperture_photometry.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/multi_aperture_photometry.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/tesscut.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/tests/test_OC_plot.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.4a9
+Version: 3.0.0a1
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/LICENSE` & `EclipsingBinaries-3.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/PKG-INFO` & `EclipsingBinaries-3.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.4a9
+Version: 3.0.0a1
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-2.8.4a9/README.md` & `EclipsingBinaries-3.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a9/setup.py` & `EclipsingBinaries-3.0.0a1/setup.py`

 * *Files identical despite different names*

