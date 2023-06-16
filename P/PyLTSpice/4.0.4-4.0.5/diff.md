# Comparing `tmp/PyLTSpice-4.0.4.tar.gz` & `tmp/PyLTSpice-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\sandbox\PySpice\dist\.tmp-ydkee3cw\PyLTSpice-4.0.4.tar", last modified: Tue Jun  6 07:12:14 2023, max compression
+gzip compressed data, was "C:\sandbox\PySpice\dist\.tmp-84jaqpyk\PyLTSpice-4.0.5.tar", last modified: Fri Jun 16 14:16:18 2023, max compression
```

## Comparing `PyLTSpice-4.0.4.tar` & `PyLTSpice-4.0.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.262939 PyLTSpice-4.0.4/
--rw-rw-rw-   0        0        0    35823 2022-12-04 12:18:59.000000 PyLTSpice-4.0.4/LICENSE
--rw-rw-rw-   0        0        0    58218 2023-06-06 07:12:14.261743 PyLTSpice-4.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.146625 PyLTSpice-4.0.4/PyLTSpice/
--rw-rw-rw-   0        0        0     9679 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/Histogram.py
--rw-rw-rw-   0        0        0      362 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/LTSpiceBatch.py
--rw-rw-rw-   0        0        0      333 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/LTSpice_RawRead.py
--rw-rw-rw-   0        0        0      332 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/LTSpice_RawWrite.py
--rw-rw-rw-   0        0        0     6743 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/LTSteps.py
--rw-rw-rw-   0        0        0     1692 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.180377 PyLTSpice-4.0.4/PyLTSpice/client_server/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/client_server/__init__.py
--rw-rw-rw-   0        0        0     8488 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/client_server/sim_client.py
--rw-rw-rw-   0        0        0     5570 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/client_server/sim_server.py
--rw-rw-rw-   0        0        0     4865 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/client_server/srv_sim_runner.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.189063 PyLTSpice-4.0.4/PyLTSpice/log/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/log/__init__.py
--rw-rw-rw-   0        0        0    29997 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/log/ltsteps.py
--rw-rw-rw-   0        0        0     6047 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/log/semi_dev_op_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.203701 PyLTSpice-4.0.4/PyLTSpice/raw/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/raw/__init__.py
--rw-rw-rw-   0        0        0    14667 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/raw/raw_classes.py
--rw-rw-rw-   0        0        0     5609 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/raw/raw_convert.py
--rw-rw-rw-   0        0        0    36151 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/raw/raw_read.py
--rw-rw-rw-   0        0        0    16752 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/raw/raw_write.py
--rw-rw-rw-   0        0        0     4014 2023-05-14 19:17:53.000000 PyLTSpice-4.0.4/PyLTSpice/rawplot.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.240743 PyLTSpice-4.0.4/PyLTSpice/sim/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/sim/__init__.py
--rw-rw-rw-   0        0        0     8683 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/ltspice_simulator.py
--rw-rw-rw-   0        0        0     4738 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/ngspice_simulator.py
--rw-rw-rw-   0        0        0     1505 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/sim/process_callback.py
--rw-rw-rw-   0        0        0     7179 2023-06-04 10:41:26.000000 PyLTSpice-4.0.4/PyLTSpice/sim/run_task.py
--rw-rw-rw-   0        0        0     4809 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/sim/sim_analysis.py
--rw-rw-rw-   0        0        0    10823 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/sim_batch.py
--rw-rw-rw-   0        0        0    23309 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/sim_runner.py
--rw-rw-rw-   0        0        0     9298 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/sim_stepping.py
--rw-rw-rw-   0        0        0     4652 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/sim/simulator.py
--rw-rw-rw-   0        0        0    46624 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/spice_editor.py
--rw-rw-rw-   0        0        0     7456 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/xyce_simulator.py
--rw-rw-rw-   0        0        0    21638 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim_batch.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.246771 PyLTSpice-4.0.4/PyLTSpice/utils/
--rw-rw-rw-   0        0        0     2935 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/utils/detect_encoding.py
--rw-rw-rw-   0        0        0    11563 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/utils/sweep_iterators.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.167871 PyLTSpice-4.0.4/PyLTSpice.egg-info/
--rw-rw-rw-   0        0        0    58218 2023-06-06 07:12:13.000000 PyLTSpice-4.0.4/PyLTSpice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1361 2023-06-06 07:12:13.000000 PyLTSpice-4.0.4/PyLTSpice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 07:12:13.000000 PyLTSpice-4.0.4/PyLTSpice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      165 2023-06-06 07:12:13.000000 PyLTSpice-4.0.4/PyLTSpice.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-06-06 07:12:13.000000 PyLTSpice-4.0.4/PyLTSpice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-06 07:12:13.000000 PyLTSpice-4.0.4/PyLTSpice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    16437 2023-06-04 10:54:08.000000 PyLTSpice-4.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.249446 PyLTSpice-4.0.4/doc/
--rw-rw-rw-   0        0        0     2448 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/doc/conf.py
--rw-rw-rw-   0        0        0     1193 2023-06-04 10:50:02.000000 PyLTSpice-4.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 07:12:14.262939 PyLTSpice-4.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.252633 PyLTSpice-4.0.4/tests/
--rw-rw-rw-   0        0        0      801 2023-05-14 19:17:08.000000 PyLTSpice-4.0.4/tests/test_ltsteps.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.255247 PyLTSpice-4.0.4/tests/unittest/
-drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.257843 PyLTSpice-4.0.4/tests/unittest/sweep_iterators/
--rw-rw-rw-   0        0        0     6014 2023-05-14 19:17:08.000000 PyLTSpice-4.0.4/tests/unittest/sweep_iterators/sweep_iterators_unittest.py
--rw-rw-rw-   0        0        0    19227 2023-05-14 19:17:08.000000 PyLTSpice-4.0.4/tests/unittest/test_pyltspice.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.026907 PyLTSpice-4.0.5/
+-rw-rw-rw-   0        0        0    35823 2022-12-04 12:18:59.000000 PyLTSpice-4.0.5/LICENSE
+-rw-rw-rw-   0        0        0    58334 2023-06-16 14:16:18.025910 PyLTSpice-4.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 14:16:17.915878 PyLTSpice-4.0.5/PyLTSpice/
+-rw-rw-rw-   0        0        0     9679 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/Histogram.py
+-rw-rw-rw-   0        0        0      362 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/LTSpiceBatch.py
+-rw-rw-rw-   0        0        0      333 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/LTSpice_RawRead.py
+-rw-rw-rw-   0        0        0      332 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/LTSpice_RawWrite.py
+-rw-rw-rw-   0        0        0     6743 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/LTSteps.py
+-rw-rw-rw-   0        0        0     1692 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:16:17.944826 PyLTSpice-4.0.5/PyLTSpice/client_server/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/client_server/__init__.py
+-rw-rw-rw-   0        0        0     8488 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/client_server/sim_client.py
+-rw-rw-rw-   0        0        0     5570 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/client_server/sim_server.py
+-rw-rw-rw-   0        0        0     4865 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/client_server/srv_sim_runner.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:16:17.953334 PyLTSpice-4.0.5/PyLTSpice/log/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/log/__init__.py
+-rw-rw-rw-   0        0        0    29997 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/log/ltsteps.py
+-rw-rw-rw-   0        0        0     6047 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/log/semi_dev_op_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:16:17.966506 PyLTSpice-4.0.5/PyLTSpice/raw/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/raw/__init__.py
+-rw-rw-rw-   0        0        0    14667 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/raw/raw_classes.py
+-rw-rw-rw-   0        0        0     5609 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/raw/raw_convert.py
+-rw-rw-rw-   0        0        0    36151 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/raw/raw_read.py
+-rw-rw-rw-   0        0        0    16752 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/raw/raw_write.py
+-rw-rw-rw-   0        0        0     4014 2023-05-14 19:17:53.000000 PyLTSpice-4.0.5/PyLTSpice/rawplot.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.000035 PyLTSpice-4.0.5/PyLTSpice/sim/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/sim/__init__.py
+-rw-rw-rw-   0        0        0     9342 2023-06-16 12:17:42.000000 PyLTSpice-4.0.5/PyLTSpice/sim/ltspice_simulator.py
+-rw-rw-rw-   0        0        0     4738 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim/ngspice_simulator.py
+-rw-rw-rw-   0        0        0     1505 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/sim/process_callback.py
+-rw-rw-rw-   0        0        0     7179 2023-06-04 10:41:26.000000 PyLTSpice-4.0.5/PyLTSpice/sim/run_task.py
+-rw-rw-rw-   0        0        0     4809 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/sim/sim_analysis.py
+-rw-rw-rw-   0        0        0    10823 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim/sim_batch.py
+-rw-rw-rw-   0        0        0    23309 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim/sim_runner.py
+-rw-rw-rw-   0        0        0     9298 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim/sim_stepping.py
+-rw-rw-rw-   0        0        0     4652 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/sim/simulator.py
+-rw-rw-rw-   0        0        0    46624 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim/spice_editor.py
+-rw-rw-rw-   0        0        0     7456 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim/xyce_simulator.py
+-rw-rw-rw-   0        0        0    21638 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim_batch.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.006939 PyLTSpice-4.0.5/PyLTSpice/utils/
+-rw-rw-rw-   0        0        0     2935 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/utils/detect_encoding.py
+-rw-rw-rw-   0        0        0    11563 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/utils/sweep_iterators.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:16:17.933827 PyLTSpice-4.0.5/PyLTSpice.egg-info/
+-rw-rw-rw-   0        0        0    58334 2023-06-16 14:16:17.000000 PyLTSpice-4.0.5/PyLTSpice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1361 2023-06-16 14:16:17.000000 PyLTSpice-4.0.5/PyLTSpice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 14:16:17.000000 PyLTSpice-4.0.5/PyLTSpice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      165 2023-06-16 14:16:17.000000 PyLTSpice-4.0.5/PyLTSpice.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-06-16 14:16:17.000000 PyLTSpice-4.0.5/PyLTSpice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-16 14:16:17.000000 PyLTSpice-4.0.5/PyLTSpice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    16553 2023-06-16 12:20:56.000000 PyLTSpice-4.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.009950 PyLTSpice-4.0.5/doc/
+-rw-rw-rw-   0        0        0     2448 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/doc/conf.py
+-rw-rw-rw-   0        0        0     1193 2023-06-16 12:20:56.000000 PyLTSpice-4.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 14:16:18.027904 PyLTSpice-4.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.012944 PyLTSpice-4.0.5/tests/
+-rw-rw-rw-   0        0        0      801 2023-05-14 19:17:08.000000 PyLTSpice-4.0.5/tests/test_ltsteps.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.017931 PyLTSpice-4.0.5/tests/unittest/
+drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.020923 PyLTSpice-4.0.5/tests/unittest/sweep_iterators/
+-rw-rw-rw-   0        0        0     6014 2023-05-14 19:17:08.000000 PyLTSpice-4.0.5/tests/unittest/sweep_iterators/sweep_iterators_unittest.py
+-rw-rw-rw-   0        0        0    19227 2023-05-14 19:17:08.000000 PyLTSpice-4.0.5/tests/unittest/test_pyltspice.py
```

### Comparing `PyLTSpice-4.0.4/LICENSE` & `PyLTSpice-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PKG-INFO` & `PyLTSpice-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLTSpice
-Version: 4.0.4
+Version: 4.0.5
 Summary: A set of tools to Automate LTSpice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -975,14 +975,17 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 4.0.5\
+  Accepting fixes from aanas-sayed@GitHub that fixes issues with running the LTSpice in Linux.
+
 * Version 4.0.4\
   Improved usage of the logging library. (Thanks TSprech@GitHub)\
   Included RunTask number in the log messages.\ 
   Included milliseconds in the time elapsed calculation.
 
 * Version 4.0.3\
   Fixing issue in elapsed time calculation.\
```

### Comparing `PyLTSpice-4.0.4/PyLTSpice/Histogram.py` & `PyLTSpice-4.0.5/PyLTSpice/Histogram.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/LTSteps.py` & `PyLTSpice-4.0.5/PyLTSpice/LTSteps.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/__init__.py` & `PyLTSpice-4.0.5/PyLTSpice/__init__.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/client_server/sim_client.py` & `PyLTSpice-4.0.5/PyLTSpice/client_server/sim_client.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/client_server/sim_server.py` & `PyLTSpice-4.0.5/PyLTSpice/client_server/sim_server.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/client_server/srv_sim_runner.py` & `PyLTSpice-4.0.5/PyLTSpice/client_server/srv_sim_runner.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/log/ltsteps.py` & `PyLTSpice-4.0.5/PyLTSpice/log/ltsteps.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/log/semi_dev_op_reader.py` & `PyLTSpice-4.0.5/PyLTSpice/log/semi_dev_op_reader.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/raw/raw_classes.py` & `PyLTSpice-4.0.5/PyLTSpice/raw/raw_classes.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/raw/raw_convert.py` & `PyLTSpice-4.0.5/PyLTSpice/raw/raw_convert.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/raw/raw_read.py` & `PyLTSpice-4.0.5/PyLTSpice/raw/raw_read.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/raw/raw_write.py` & `PyLTSpice-4.0.5/PyLTSpice/raw/raw_write.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/rawplot.py` & `PyLTSpice-4.0.5/PyLTSpice/rawplot.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/sim/ltspice_simulator.py` & `PyLTSpice-4.0.5/PyLTSpice/sim/ltspice_simulator.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,20 +30,35 @@
 
 class LTspice(Simulator):
     """Stores the simulator location and command line options and is responsible for generating netlists and running
     simulations."""
 
     """Searches on the any usual locations for a simulator"""
     if sys.platform == "linux":
-        if os.environ.get('LTSPICEFOLDER') is not None:
-            spice_exe = ["wine", os.environ['LTSPICEFOLDER'] + "/XVIIx64.exe"]
+        spice_folder = os.environ.get("LTSPICEFOLDER")
+        spice_executable = os.environ.get("LTSPICEEXECUTABLE")
+
+        if spice_folder and spice_executable:
+            spice_exe = ["wine", os.path.join(spice_folder, spice_executable)]
+            process_name = spice_executable
+        elif spice_folder:
+            spice_exe = ["wine", os.path.join(spice_folder, "/XVIIx64.exe")]
+            process_name = "XVIIx64.exe"
+        elif spice_executable:
+            default_folder = os.path.expanduser(
+                "~/.wine/drive_c/Program Files/LTC/LTspiceXVII"
+            )
+            spice_exe = ["wine", os.path.join(default_folder, spice_executable)]
+            process_name = spice_executable
         else:
-            spice_exe = ["wine",
-                           os.path.expanduser("~") + "/.wine/drive_c/Program Files/LTC/LTspiceXVII/XVIIx64.exe"]
-        process_name = "XVIIx64.exe"
+            default_folder = os.path.expanduser(
+                "~/.wine/drive_c/Program Files/LTC/LTspiceXVII"
+            )
+            spice_exe = ["wine", os.path.join(default_folder, "XVIIx64.exe")]
+            process_name = "XVIIx64.exe"
     elif sys.platform == "darwin":
         spice_exe = ['/Applications/LTspice.app/Contents/MacOS/LTspice']
         process_name = "XVIIx64"
     else:  # Windows
         for exe in (  # Placed in order of preference. The first to be found will be used.
                 os.path.expanduser(r"~\AppData\Local\Programs\ADI\LTspice\LTspice.exe"),
                 r"C:\Program Files\ADI\LTspice\LTspice.exe",
```

### Comparing `PyLTSpice-4.0.4/PyLTSpice/sim/ngspice_simulator.py` & `PyLTSpice-4.0.5/PyLTSpice/sim/ngspice_simulator.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/sim/process_callback.py` & `PyLTSpice-4.0.5/PyLTSpice/sim/process_callback.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/sim/run_task.py` & `PyLTSpice-4.0.5/PyLTSpice/sim/run_task.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/sim/sim_analysis.py` & `PyLTSpice-4.0.5/PyLTSpice/sim/sim_analysis.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/sim/sim_batch.py` & `PyLTSpice-4.0.5/PyLTSpice/sim/sim_batch.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/sim/sim_runner.py` & `PyLTSpice-4.0.5/PyLTSpice/sim/sim_runner.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/sim/sim_stepping.py` & `PyLTSpice-4.0.5/PyLTSpice/sim/sim_stepping.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/sim/simulator.py` & `PyLTSpice-4.0.5/PyLTSpice/sim/simulator.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/sim/spice_editor.py` & `PyLTSpice-4.0.5/PyLTSpice/sim/spice_editor.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/sim/xyce_simulator.py` & `PyLTSpice-4.0.5/PyLTSpice/sim/xyce_simulator.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/sim_batch.py` & `PyLTSpice-4.0.5/PyLTSpice/sim_batch.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/utils/detect_encoding.py` & `PyLTSpice-4.0.5/PyLTSpice/utils/detect_encoding.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice/utils/sweep_iterators.py` & `PyLTSpice-4.0.5/PyLTSpice/utils/sweep_iterators.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/PyLTSpice.egg-info/PKG-INFO` & `PyLTSpice-4.0.5/PyLTSpice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLTSpice
-Version: 4.0.4
+Version: 4.0.5
 Summary: A set of tools to Automate LTSpice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -975,14 +975,17 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 4.0.5\
+  Accepting fixes from aanas-sayed@GitHub that fixes issues with running the LTSpice in Linux.
+
 * Version 4.0.4\
   Improved usage of the logging library. (Thanks TSprech@GitHub)\
   Included RunTask number in the log messages.\ 
   Included milliseconds in the time elapsed calculation.
 
 * Version 4.0.3\
   Fixing issue in elapsed time calculation.\
```

### Comparing `PyLTSpice-4.0.4/PyLTSpice.egg-info/SOURCES.txt` & `PyLTSpice-4.0.5/PyLTSpice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/README.md` & `PyLTSpice-4.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -286,14 +286,17 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 4.0.5\
+  Accepting fixes from aanas-sayed@GitHub that fixes issues with running the LTSpice in Linux.
+
 * Version 4.0.4\
   Improved usage of the logging library. (Thanks TSprech@GitHub)\
   Included RunTask number in the log messages.\ 
   Included milliseconds in the time elapsed calculation.
 
 * Version 4.0.3\
   Fixing issue in elapsed time calculation.\
```

### Comparing `PyLTSpice-4.0.4/doc/conf.py` & `PyLTSpice-4.0.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/pyproject.toml` & `PyLTSpice-4.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "PyLTSpice"
-version = "4.0.4"
+version = "4.0.5"
 authors = [
   { name="Nuno Brum", email="me@nunobrum.com" },
 ]
 description = "A set of tools to Automate LTSpice simulations"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `PyLTSpice-4.0.4/tests/test_ltsteps.py` & `PyLTSpice-4.0.5/tests/test_ltsteps.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/tests/unittest/sweep_iterators/sweep_iterators_unittest.py` & `PyLTSpice-4.0.5/tests/unittest/sweep_iterators/sweep_iterators_unittest.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.4/tests/unittest/test_pyltspice.py` & `PyLTSpice-4.0.5/tests/unittest/test_pyltspice.py`

 * *Files identical despite different names*

