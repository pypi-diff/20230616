# Comparing `tmp/xflow-net-0.0.8.tar.gz` & `tmp/xflow-net-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xflow-net-0.0.8.tar", last modified: Thu Jun 15 03:53:39 2023, max compression
+gzip compressed data, was "xflow-net-0.0.9.tar", last modified: Fri Jun 16 03:29:19 2023, max compression
```

## Comparing `xflow-net-0.0.8.tar` & `xflow-net-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:53:39.139107 xflow-net-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-15 03:53:28.000000 xflow-net-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-06-15 03:53:39.139107 xflow-net-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-15 03:53:28.000000 xflow-net-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:53:39.139107 xflow-net-0.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:53:28.000000 xflow-net-0.0.8/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-15 03:53:28.000000 xflow-net-0.0.8/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 03:53:28.000000 xflow-net-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-15 03:53:39.143107 xflow-net-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-15 03:53:28.000000 xflow-net-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:53:39.139107 xflow-net-0.0.8/xflow/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 03:53:28.000000 xflow-net-0.0.8/xflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:53:39.139107 xflow-net-0.0.8/xflow/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 03:53:28.000000 xflow-net-0.0.8/xflow/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-15 03:53:28.000000 xflow-net-0.0.8/xflow/dataset/nx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-15 03:53:28.000000 xflow-net-0.0.8/xflow/dataset/pyg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:53:39.139107 xflow-net-0.0.8/xflow/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-15 03:53:28.000000 xflow-net-0.0.8/xflow/diffusion/IC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-15 03:53:28.000000 xflow-net-0.0.8/xflow/diffusion/LT.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-15 03:53:28.000000 xflow-net-0.0.8/xflow/diffusion/SI.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:53:28.000000 xflow-net-0.0.8/xflow/diffusion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:53:39.139107 xflow-net-0.0.8/xflow/method/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:53:28.000000 xflow-net-0.0.8/xflow/method/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-15 03:53:28.000000 xflow-net-0.0.8/xflow/method/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-06-15 03:53:28.000000 xflow-net-0.0.8/xflow/method/im.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-15 03:53:28.000000 xflow-net-0.0.8/xflow/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-15 03:53:28.000000 xflow-net-0.0.8/xflow/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:53:39.139107 xflow-net-0.0.8/xflow_net.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-06-15 03:53:39.000000 xflow-net-0.0.8/xflow_net.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-15 03:53:39.000000 xflow-net-0.0.8/xflow_net.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:53:39.000000 xflow-net-0.0.8/xflow_net.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 03:53:39.000000 xflow-net-0.0.8/xflow_net.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 03:53:39.000000 xflow-net-0.0.8/xflow_net.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.772961 xflow-net-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-16 03:29:05.000000 xflow-net-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-16 03:29:19.772961 xflow-net-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-16 03:29:05.000000 xflow-net-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.768961 xflow-net-0.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:29:05.000000 xflow-net-0.0.9/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-16 03:29:05.000000 xflow-net-0.0.9/examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-16 03:29:05.000000 xflow-net-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-16 03:29:19.772961 xflow-net-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-16 03:29:05.000000 xflow-net-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.768961 xflow-net-0.0.9/xflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.768961 xflow-net-0.0.9/xflow/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/dataset/nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/dataset/pyg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.768961 xflow-net-0.0.9/xflow/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/diffusion/IC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/diffusion/LT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/diffusion/SI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/diffusion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.768961 xflow-net-0.0.9/xflow/method/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/method/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/method/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/method/im.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-16 03:29:05.000000 xflow-net-0.0.9/xflow/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:29:19.772961 xflow-net-0.0.9/xflow_net.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-16 03:29:19.000000 xflow-net-0.0.9/xflow_net.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-16 03:29:19.000000 xflow-net-0.0.9/xflow_net.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:29:19.000000 xflow-net-0.0.9/xflow_net.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 03:29:19.000000 xflow-net-0.0.9/xflow_net.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 03:29:19.000000 xflow-net-0.0.9/xflow_net.egg-info/top_level.txt
```

### Comparing `xflow-net-0.0.8/LICENSE` & `xflow-net-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.8/setup.py` & `xflow-net-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # Package meta-data.
 NAME = 'xflow-net'
 DESCRIPTION = 'a python library for graph flow'
 URL = 'https://xflow.network/'
 EMAIL = 'zchen@cse.msstate.edu'
 AUTHOR = 'XGraphing'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-   'networkx', 'ndlib'
+   'networkx', 'ndlib', 'torch_geometric'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

### Comparing `xflow-net-0.0.8/xflow/dataset/nx.py` & `xflow-net-0.0.9/xflow/dataset/nx.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.8/xflow/dataset/pyg.py` & `xflow-net-0.0.9/xflow/dataset/pyg.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.8/xflow/diffusion/IC.py` & `xflow-net-0.0.9/xflow/diffusion/IC.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.8/xflow/diffusion/LT.py` & `xflow-net-0.0.9/xflow/diffusion/LT.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.8/xflow/diffusion/SI.py` & `xflow-net-0.0.9/xflow/diffusion/SI.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.8/xflow/method/ibm.py` & `xflow-net-0.0.9/xflow/method/ibm.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.8/xflow/method/im.py` & `xflow-net-0.0.9/xflow/method/im.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.8/xflow/visualization.py` & `xflow-net-0.0.9/xflow/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import plotly.graph_objects as go
 import random
 import dash
 import dash_core_components as dcc
 import dash_html_components as html
 from dash.dependencies import Input, Output
 
+# todo
 # Step 1: Randomly draw a 50-node graph using NetworkX
 G = nx.gnm_random_graph(50, 100)
 
 # Step 2: Create an initial plot using Plotly
 pos = nx.spring_layout(G)
 node_trace = go.Scatter(
     x=[pos[node][0] for node in G.nodes()],
```

### Comparing `xflow-net-0.0.8/xflow_net.egg-info/SOURCES.txt` & `xflow-net-0.0.9/xflow_net.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 examples/__init__.py
 examples/main.py
 xflow/__init__.py
 xflow/seed.py
+xflow/util.py
 xflow/visualization.py
 xflow/dataset/__init__.py
 xflow/dataset/nx.py
 xflow/dataset/pyg.py
 xflow/diffusion/IC.py
 xflow/diffusion/LT.py
 xflow/diffusion/SI.py
```

