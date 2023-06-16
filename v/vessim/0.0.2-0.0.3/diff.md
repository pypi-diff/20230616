# Comparing `tmp/vessim-0.0.2.tar.gz` & `tmp/vessim-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vessim-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vessim-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vessim-0.0.2.tar` & `vessim-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,51 @@
--rw-r--r--   0        0        0     1085 2023-06-04 18:37:57.805833 vessim-0.0.2/.github/workflows/vessim-ci.yml
--rw-r--r--   0        0        0     1142 2023-06-09 11:35:36.040425 vessim-0.0.2/.gitignore
--rw-r--r--   0        0        0     1089 2023-06-09 10:55:14.692611 vessim-0.0.2/LICENSE
--rw-r--r--   0        0        0      289 2023-06-09 11:36:26.384790 vessim-0.0.2/README.md
--rw-r--r--   0        0        0     4696 2023-06-05 11:14:10.461302 vessim-0.0.2/carbon-aware_control_unit/carbon_aware_control_unit.py
--rw-r--r--   0        0        0      931 2023-05-23 12:28:30.339243 vessim-0.0.2/carbon-aware_control_unit/main.py
--rw-r--r--   0        0        0   427933 2023-05-23 13:29:52.934217 vessim-0.0.2/evaluation.ipynb
--rw-r--r--   0        0        0     2097 2023-06-05 11:17:48.679082 vessim-0.0.2/example_node/README.md
--rw-r--r--   0        0        0     2037 2023-06-08 11:05:26.203311 vessim-0.0.2/example_node/node_api_server.py
--rw-r--r--   0        0        0      173 2023-06-05 11:14:10.462401 vessim-0.0.2/example_node/rpi/config/config.txt
--rw-r--r--   0        0        0      159 2023-06-05 11:14:10.462724 vessim-0.0.2/example_node/rpi/config/rc.local
--rw-r--r--   0        0        0     1405 2023-06-05 11:14:10.463000 vessim-0.0.2/example_node/rpi/init.sh
--rw-r--r--   0        0        0     2127 2023-06-05 11:14:10.463312 vessim-0.0.2/example_node/rpi/lib/pi_controller.py
--rw-r--r--   0        0        0       47 2023-06-05 11:14:10.463651 vessim-0.0.2/example_node/rpi/requirements.txt
--rw-r--r--   0        0        0     1415 2023-06-08 11:05:26.203642 vessim-0.0.2/example_node/rpi/rpi_api_server.py
--rw-r--r--   0        0        0      638 2023-06-05 11:14:10.464204 vessim-0.0.2/example_node/virtual_node/linear_power_model.py
--rw-r--r--   0        0        0       23 2023-06-05 11:17:48.679232 vessim-0.0.2/example_node/virtual_node/requirements.txt
--rw-r--r--   0        0        0     3671 2023-06-08 11:05:26.203868 vessim-0.0.2/example_node/virtual_node/v_node_api_server.py
--rw-r--r--   0        0        0     1379 2023-06-09 11:06:42.915265 vessim-0.0.2/experimental/pp_scenario.py
--rw-r--r--   0        0        0     2375 2023-06-08 11:04:22.045307 vessim-0.0.2/lib/http_client.py
--rw-r--r--   0        0        0     3783 2023-06-09 08:28:46.374666 vessim-0.0.2/main.py
--rw-r--r--   0        0        0     3533 2023-06-09 08:28:51.975101 vessim-0.0.2/main_new.py
--rw-r--r--   0        0        0     2956 2023-06-09 11:38:59.333992 vessim-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      415 2023-06-09 11:36:08.170605 vessim-0.0.2/requirements.txt
--rw-r--r--   0        0        0     1811 2023-06-09 08:20:55.357876 vessim-0.0.2/simulator/computing_system.py
--rw-r--r--   0        0        0     1753 2023-06-09 08:20:55.358152 vessim-0.0.2/simulator/power_meter.py
--rw-r--r--   0        0        0     4522 2023-06-08 11:04:22.046853 vessim-0.0.2/simulator/redis_docker.py
--rw-r--r--   0        0        0     1224 2023-06-08 11:04:22.047006 vessim-0.0.2/simulator/solar_controller.py
--rw-r--r--   0        0        0     9403 2023-06-09 11:36:26.385012 vessim-0.0.2/simulator/virtual_energy_system.py
--rw-r--r--   0        0        0     1438 2023-06-09 08:30:30.957245 vessim-0.0.2/tests/test_carbon_api.py
--rw-r--r--   0        0        0     1910 2023-06-08 11:05:26.204334 vessim-0.0.2/tests/test_storage.py
--rw-r--r--   0        0        0      897 2023-05-23 12:28:30.349242 vessim-0.0.2/tf_gcp_node/.gitignore
--rw-r--r--   0        0        0     2253 2023-05-23 12:28:30.349446 vessim-0.0.2/tf_gcp_node/README.md
--rw-r--r--   0        0        0     3194 2023-06-08 11:05:26.204615 vessim-0.0.2/tf_gcp_node/main.tf
--rw-r--r--   0        0        0      249 2023-05-23 12:28:30.349833 vessim-0.0.2/tf_gcp_node/outputs.tf
--rwxr-xr-x   0        0        0      262 2023-05-23 12:28:30.350118 vessim-0.0.2/tf_gcp_node/ssh_scripts/tfreceive
--rwxr-xr-x   0        0        0      248 2023-05-23 12:28:30.350465 vessim-0.0.2/tf_gcp_node/ssh_scripts/tfsend
--rwxr-xr-x   0        0        0      225 2023-05-23 12:28:30.350732 vessim-0.0.2/tf_gcp_node/ssh_scripts/tfssh
--rw-r--r--   0        0        0      667 2023-05-23 12:28:30.351270 vessim-0.0.2/tf_gcp_node/variables.tf
--rw-r--r--   0        0        0       83 2023-06-09 11:34:03.886216 vessim-0.0.2/vessim/__init__.py
--rw-r--r--   0        0        0      416 2023-06-08 15:37:09.254824 vessim-0.0.2/vessim/_util.py
--rw-r--r--   0        0        0     3661 2023-06-09 08:28:23.139799 vessim-0.0.2/vessim/carbon_api.py
--rw-r--r--   0        0        0     4166 2023-06-09 08:24:59.930007 vessim-0.0.2/vessim/core.py
--rw-r--r--   0        0        0     1500 2023-06-08 11:05:23.749112 vessim-0.0.2/vessim/microgrid.py
--rw-r--r--   0        0        0     1977 2023-06-08 22:58:27.902499 vessim-0.0.2/vessim/monitor.py
--rw-r--r--   0        0        0     4028 2023-06-08 14:26:16.529827 vessim-0.0.2/vessim/storage.py
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 vessim-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-16 14:57:30.270261 vessim-0.0.3/.github/workflows/vessim-ci.yml
+-rw-r--r--   0        0        0     1142 2023-06-09 14:00:54.375018 vessim-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1089 2023-06-09 14:00:54.375226 vessim-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1602 2023-06-16 15:08:04.614316 vessim-0.0.3/README.md
+-rw-r--r--   0        0        0     4778 2023-06-16 14:56:58.586950 vessim-0.0.3/examples/scenario_1.py
+-rw-r--r--   0        0        0     4730 2023-06-16 14:53:48.527891 vessim-0.0.3/examples/sil/carbon-aware_control_unit/carbon_aware_control_unit.py
+-rw-r--r--   0        0        0      931 2023-06-16 14:34:31.939597 vessim-0.0.3/examples/sil/carbon-aware_control_unit/main.py
+-rw-r--r--   0        0        0     2097 2023-06-16 14:34:31.939747 vessim-0.0.3/examples/sil/example_node/README.md
+-rw-r--r--   0        0        0     2262 2023-06-16 14:53:48.528050 vessim-0.0.3/examples/sil/example_node/node_api_server.py
+-rw-r--r--   0        0        0      173 2023-06-16 14:34:31.940065 vessim-0.0.3/examples/sil/example_node/rpi/config/config.txt
+-rw-r--r--   0        0        0      159 2023-06-16 14:34:31.940212 vessim-0.0.3/examples/sil/example_node/rpi/config/rc.local
+-rw-r--r--   0        0        0     1405 2023-06-16 14:34:31.940332 vessim-0.0.3/examples/sil/example_node/rpi/init.sh
+-rw-r--r--   0        0        0     2119 2023-06-16 14:34:31.940488 vessim-0.0.3/examples/sil/example_node/rpi/lib/pi_controller.py
+-rw-r--r--   0        0        0       47 2023-06-16 14:34:31.940579 vessim-0.0.3/examples/sil/example_node/rpi/requirements.txt
+-rw-r--r--   0        0        0     1294 2023-06-16 14:53:48.528254 vessim-0.0.3/examples/sil/example_node/rpi/rpi_api_server.py
+-rw-r--r--   0        0        0      638 2023-06-16 14:34:31.940829 vessim-0.0.3/examples/sil/example_node/virtual_node/linear_power_model.py
+-rw-r--r--   0        0        0       23 2023-06-16 14:34:31.940934 vessim-0.0.3/examples/sil/example_node/virtual_node/requirements.txt
+-rw-r--r--   0        0        0     3550 2023-06-16 14:53:48.528453 vessim-0.0.3/examples/sil/example_node/virtual_node/v_node_api_server.py
+-rw-r--r--   0        0        0      897 2023-06-16 14:34:31.941210 vessim-0.0.3/examples/sil/tf_gcp_node/.gitignore
+-rw-r--r--   0        0        0     2253 2023-06-16 14:34:31.941318 vessim-0.0.3/examples/sil/tf_gcp_node/README.md
+-rw-r--r--   0        0        0     3194 2023-06-16 14:34:31.941444 vessim-0.0.3/examples/sil/tf_gcp_node/main.tf
+-rw-r--r--   0        0        0      249 2023-06-16 14:34:31.941592 vessim-0.0.3/examples/sil/tf_gcp_node/outputs.tf
+-rwxr-xr-x   0        0        0      262 2023-06-16 14:34:31.941737 vessim-0.0.3/examples/sil/tf_gcp_node/ssh_scripts/tfreceive
+-rwxr-xr-x   0        0        0      248 2023-06-16 14:34:31.941842 vessim-0.0.3/examples/sil/tf_gcp_node/ssh_scripts/tfsend
+-rwxr-xr-x   0        0        0      225 2023-06-16 14:34:31.941938 vessim-0.0.3/examples/sil/tf_gcp_node/ssh_scripts/tfssh
+-rw-r--r--   0        0        0      667 2023-06-16 14:34:31.942037 vessim-0.0.3/examples/sil/tf_gcp_node/variables.tf
+-rw-r--r--   0        0        0    58362 2023-06-16 14:34:31.942294 vessim-0.0.3/experimental/custom.json
+-rw-r--r--   0        0        0   427169 2023-06-16 15:07:31.717850 vessim-0.0.3/experimental/evaluation.ipynb
+-rw-r--r--   0        0        0     1379 2023-06-09 14:00:54.382555 vessim-0.0.3/experimental/pp_scenario.py
+-rw-r--r--   0        0        0     2826 2023-06-16 15:09:38.958920 vessim-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      415 2023-06-09 14:00:54.384250 vessim-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     1442 2023-06-16 14:34:31.943217 vessim-0.0.3/tests/test_carbon_api.py
+-rw-r--r--   0        0        0     1915 2023-06-16 14:34:31.943608 vessim-0.0.3/tests/test_storage.py
+-rw-r--r--   0        0        0       83 2023-06-16 15:12:35.504704 vessim-0.0.3/vessim/__init__.py
+-rw-r--r--   0        0        0      188 2023-06-16 14:34:31.943833 vessim-0.0.3/vessim/core/__init__.py
+-rw-r--r--   0        0        0     2918 2023-06-16 14:34:31.944203 vessim-0.0.3/vessim/core/simulator.py
+-rw-r--r--   0        0        0     4030 2023-06-16 14:34:31.944716 vessim-0.0.3/vessim/core/storage.py
+-rw-r--r--   0        0        0      515 2023-06-16 14:34:31.944870 vessim-0.0.3/vessim/cosim/__init__.py
+-rw-r--r--   0        0        0     5162 2023-06-16 14:34:31.945160 vessim-0.0.3/vessim/cosim/_util.py
+-rw-r--r--   0        0        0     1625 2023-06-16 14:34:31.945661 vessim-0.0.3/vessim/cosim/carbon_api.py
+-rw-r--r--   0        0        0     1706 2023-06-16 14:34:31.945796 vessim-0.0.3/vessim/cosim/computing_system.py
+-rw-r--r--   0        0        0     9541 2023-06-16 14:56:58.587227 vessim-0.0.3/vessim/cosim/energy_system_interface.py
+-rw-r--r--   0        0        0     1469 2023-06-16 14:34:31.946070 vessim-0.0.3/vessim/cosim/generator.py
+-rw-r--r--   0        0        0     1425 2023-06-16 14:34:31.946197 vessim-0.0.3/vessim/cosim/microgrid.py
+-rw-r--r--   0        0        0     2036 2023-06-16 14:34:31.946331 vessim-0.0.3/vessim/cosim/monitor.py
+-rw-r--r--   0        0        0      131 2023-06-16 14:34:31.946456 vessim-0.0.3/vessim/sil/__init__.py
+-rw-r--r--   0        0        0     2105 2023-06-16 14:53:48.533390 vessim-0.0.3/vessim/sil/http_client.py
+-rw-r--r--   0        0        0      930 2023-06-16 14:34:31.946911 vessim-0.0.3/vessim/sil/node.py
+-rw-r--r--   0        0        0     2325 2023-06-16 14:34:31.947017 vessim-0.0.3/vessim/sil/power_meter.py
+-rw-r--r--   0        0        0     4522 2023-06-16 14:34:31.947351 vessim-0.0.3/vessim/sil/redis_docker.py
+-rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 vessim-0.0.3/PKG-INFO
```

### Comparing `vessim-0.0.2/.github/workflows/vessim-ci.yml` & `vessim-0.0.3/.github/workflows/vessim-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: vessim CI
+name: CI
 
 # event that triggers workflow
 # here when a "push" is made
 on: 
   push:
 
 jobs:
```

### Comparing `vessim-0.0.2/.gitignore` & `vessim-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `vessim-0.0.2/LICENSE` & `vessim-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vessim-0.0.2/carbon-aware_control_unit/carbon_aware_control_unit.py` & `vessim-0.0.3/examples/sil/carbon-aware_control_unit/carbon_aware_control_unit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from ..lib.http_client import HTTPClient
+from vessim.sil.http_client import HTTPClient
 import simpy
 from typing import Dict
 
 
 class RemoteBattery:
-    """Initializes a battery instance that holds some info of the remote battery.
+    """Initializes a battery instance that holds info of the remote battery.
 
     Args:
         soc: The initial state of the battery's state of charge in %.
         min_soc: The minimum state of charge threshold for the battery in %.
-        grid_charge: The power which the battery is charged with from the public grid in W.
+        grid_charge: The power which the battery is charged with from the
+            public grid in W.
     """
 
     def __init__(self, soc: float = 0.0, min_soc: float = 0.0, grid_charge: float = 0.0) -> None:
         self.soc = soc
         self.min_soc = min_soc
         self.grid_charge = grid_charge
 
 
 class CarbonAwareControlUnit:
-    """The Carbon Aware Control Unit uses the VESSIM API to execute real-time carbon-aware scenarios.
+    """The CACU uses the VESSIM API for real-time carbon-aware scenarios.
 
-    The Carbon Aware control unit uses an API server to communicate with the VES
-    simulation and retrieve real-time data about energy demand, solar power
+    The Carbon Aware control unit uses an API server to communicate with the
+    VES simulation and retrieve real-time data about energy demand, solar power
     production, and grid carbon intensity via GET requests. Under predefined
-    scenarios, the control unit sends SET requests to adjust the VES simulation and
-    computing system behavior. The Carbon Aware control unit's objective is to
-    optimize the use of renewable energy sources and minimize carbon emissions by
-    taking real-time decisions and actions based on these scenarios.
+    scenarios, the control unit sends SET requests to adjust the VES simulation
+    and computing system behavior. The Carbon Aware control unit's objective is
+    to optimize the use of renewable energy sources and minimize carbon
+    emissions by taking real-time decisions and actions based on these
+    scenarios.
 
     Args:
         server_address: The address of the server to connect to.
         nodes: A dictionary representing the nodes that the Control Unit
             manages, with node IDs as keys and node objects as values.
 
     Attributes:
@@ -64,17 +66,17 @@
         battery's minimum state of charge (SOC) based on the current time, and
         adjusts the power modes of the nodes based on the current carbon
         intensity and battery SOC.
 
         Yields:
             A SimPy timeout event that delays the process by one unit of time.
         """
-        battery = RemoteBattery(soc=self.client.get('/battery-soc'))
-        solar = self.client.get('/solar')
-        ci = self.client.get('/ci')
+        battery = RemoteBattery(soc=self.client.get('/battery-soc')['battery_soc'])
+        solar = self.client.get('/solar')['solar']
+        ci = self.client.get('/ci')['ci']
         nodes_power_mode = {}
 
         # Set the minimum SOC of the battery based on the current time
         if self.env.now < 60*36:
             battery.min_soc = 0.3
         else:
             battery.min_soc = 0.6
@@ -106,12 +108,13 @@
         self.client.put('/ves/battery', {'min_soc': battery.min_soc, 'grid_charge': battery.grid_charge})
 
 
     def send_nodes_power_mode(self, nodes_power_mode: Dict[int, str]) -> None:
         """Sends power mode data for nodes to the VES API.
 
         Args:
-            nodes_power_mode: A dictionary containing node IDs as keys and their respective power modes as values.
+            nodes_power_mode: A dictionary containing node IDs as keys and
+                their respective power modes as values.
 
         """
         for node_id, power_mode in nodes_power_mode.items():
             self.client.put(f'/ves/nodes/{node_id}', {'power_mode': power_mode})
```

### Comparing `vessim-0.0.2/carbon-aware_control_unit/main.py` & `vessim-0.0.3/examples/sil/carbon-aware_control_unit/main.py`

 * *Files identical despite different names*

### Comparing `vessim-0.0.2/evaluation.ipynb` & `vessim-0.0.3/experimental/evaluation.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9946875%*

 * *Differences: {"'cells'": "{1: {'metadata': {delete: ['pycharm']}}, 2: {'metadata': {delete: ['pycharm']}}, 4: "*

 * *            "{'metadata': {delete: ['pycharm']}}, 5: {'metadata': {delete: ['pycharm']}}, 6: "*

 * *            "{'metadata': {delete: ['pycharm']}}, 7: {'metadata': {delete: ['pycharm']}}, 8: "*

 * *            "{'metadata': {delete: ['pycharm']}}, 10: {'metadata': {delete: ['pycharm']}}, 11: "*

 * *            "{'metadata': {delete: ['pycharm']}}, 12: {'metadata': {delete: ['pycharm']}}, 13: "*

 * *            "{'metadata': {de […]*

```diff
@@ -21,18 +21,15 @@
                 "from datetime import timedelta"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "Time\n2020-06-01 00:00:00    170.319207\n2020-06-01 00:15:00    171.376437\n2020-06-01 00:30:00    173.543319\n2020-06-01 00:45:00    175.554316\n2020-06-01 01:00:00    175.636264\n                          ...    \n2021-01-09 22:00:00    521.153048\n2021-01-09 22:15:00    517.600964\n2021-01-09 22:30:00    514.656596\n2021-01-09 22:45:00    510.659998\n2021-01-09 23:00:00    508.090652\nName: Germany, Length: 21403, dtype: float64"
                     },
                     "execution_count": 2,
@@ -46,18 +43,15 @@
                 "ger['2020-06-01 00:00:00':]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "<AxesSubplot: xlabel='time', ylabel='power'>"
                     },
                     "execution_count": 3,
@@ -89,18 +83,15 @@
             },
             "source": []
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "frequency\n600.0     1453.779866\n700.0     1654.780903\n800.0     1781.070569\n900.0     1900.280368\n1000.0    2044.742742\n1100.0    2193.650167\n1200.0    2321.230602\n1300.0    2791.271773\n1400.0    2964.385886\nName: power, dtype: float64"
                     },
                     "execution_count": 4,
@@ -114,18 +105,15 @@
                 "p"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 23,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "600.0     1192.27\n700.0     1391.94\n800.0     1592.71\n900.0     1786.62\n1000.0    1992.70\n1100.0    2192.85\n1200.0    2392.55\n1300.0    2592.28\n1400.0    2793.28\nName: events, dtype: float64"
                     },
                     "execution_count": 23,
@@ -142,18 +130,15 @@
                 "events_per_second"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 24,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>power</th>\n      <th>events</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>600.0</th>\n      <td>1453.779866</td>\n      <td>1192.27</td>\n    </tr>\n    <tr>\n      <th>700.0</th>\n      <td>1654.780903</td>\n      <td>1391.94</td>\n    </tr>\n    <tr>\n      <th>800.0</th>\n      <td>1781.070569</td>\n      <td>1592.71</td>\n    </tr>\n    <tr>\n      <th>900.0</th>\n      <td>1900.280368</td>\n      <td>1786.62</td>\n    </tr>\n    <tr>\n      <th>1000.0</th>\n      <td>2044.742742</td>\n      <td>1992.70</td>\n    </tr>\n    <tr>\n      <th>1100.0</th>\n      <td>2193.650167</td>\n      <td>2192.85</td>\n    </tr>\n    <tr>\n      <th>1200.0</th>\n      <td>2321.230602</td>\n      <td>2392.55</td>\n    </tr>\n    <tr>\n      <th>1300.0</th>\n      <td>2791.271773</td>\n      <td>2592.28</td>\n    </tr>\n    <tr>\n      <th>1400.0</th>\n      <td>2964.385886</td>\n      <td>2793.28</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
                         "text/plain": "              power   events\n600.0   1453.779866  1192.27\n700.0   1654.780903  1391.94\n800.0   1781.070569  1592.71\n900.0   1900.280368  1786.62\n1000.0  2044.742742  1992.70\n1100.0  2193.650167  2192.85\n1200.0  2321.230602  2392.55\n1300.0  2791.271773  2592.28\n1400.0  2964.385886  2793.28"
                     },
@@ -167,18 +152,15 @@
                 "raspi"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 27,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "(0.0, 2800.0)"
                     },
                     "execution_count": 27,
@@ -203,18 +185,15 @@
                 "ax2.set_ylim(0,2800)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "with open(\"data/weather_berlin_2021-06.csv\", \"r\") as f:\n",
                 "    solar = pd.read_csv(f, index_col=0, parse_dates=True)[\"solar\"]\n",
                 "solar.index = solar.index - timedelta(days=365)"
             ]
@@ -228,18 +207,15 @@
                 "# Simulation"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "class Battery:\n",
                 "    \"\"\"(Way too) simple battery.\n",
                 "\n",
                 "    Args:\n",
@@ -303,18 +279,15 @@
                 "        return cons"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 19,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Baseline: Raspi processed 377.11 million events using 104.81 Wh\n",
@@ -418,18 +391,15 @@
                 "measurements_2 = run_simulation(carbon_aware=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Carbon Emissions: 41.72 gCO2; Grid energy: 171.15 Wh\n",
@@ -531,32 +501,26 @@
                 "fig.align_ylabels()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "fig.savefig(\"../../Latex/2023-wiley-specialissue/ama/figures/evaluation.pdf\", dpi=300, bbox_inches='tight')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "0.3619729561274676\n",
@@ -569,18 +533,15 @@
                 "print(1-(grid2.sum()/grid1.sum()))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "(35.92938967512796, 0.0)"
                     },
                     "execution_count": 15,
@@ -594,18 +555,15 @@
                 "grid1[second_night_start:second_night_end].sum() / 60, grid2[second_night_start:second_night_end].sum() / 60"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "1.0\n",
@@ -630,18 +588,15 @@
                 "print(EVENTS_PER_SECOND_LOW / BASE_LOAD_LOW)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "1.0\n",
@@ -658,18 +613,15 @@
                 "print(BASE_LOAD_LOW / EVENTS_PER_SECOND_LOW / \u00f6)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "1.0\n",
@@ -686,18 +638,15 @@
                 "print(BASE_LOAD_LOW_AWS / EVENTS_PER_SECOND_LOW_AWS / \u00f6)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `vessim-0.0.2/example_node/README.md` & `vessim-0.0.3/examples/sil/example_node/README.md`

 * *Files identical despite different names*

### Comparing `vessim-0.0.2/example_node/node_api_server.py` & `vessim-0.0.3/examples/sil/example_node/node_api_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from abc import ABC, abstractmethod
 from pydantic import BaseModel
 from fastapi import FastAPI, HTTPException
 import uvicorn
 
-class PowerMode(BaseModel):
-    power_mode: str
-
 class FastApiServer(ABC):
     """An abstract base class that represents a FastAPI server.
 
     Args:
         host: The host on which to run the FastAPI application.
         port: The port on which to run the FastAPI application.
     """
@@ -19,35 +16,40 @@
         self.host = host
         self.port = port
         self.power_mode = "high performance"
         self.setup_routes()
 
     def setup_routes(self) -> None:
         """Setup the routes for the FastAPI application. """
-        @self.app.put("/power_mode")
-        async def set_power_mode(power_mode: PowerMode) -> str:
-            return self.set_power_mode(power_mode.power_mode)
-
-        @self.app.get("/power_mode")
-        async def get_power_mode() -> str:
-            return self.power_mode
-
-        @self.app.get("/power")
-        async def get_power() -> float:
-            return self.get_power()
+
+        class PowerModeModel(BaseModel):
+            power_mode: str
+
+        @self.app.put("/power_mode", response_model=PowerModeModel)
+        async def set_power_mode(power_mode: PowerModeModel) -> PowerModeModel:
+            self.set_power_mode(power_mode.power_mode)
+            return power_mode
+
+        @self.app.get("/power_mode", response_model=PowerModeModel)
+        async def get_power_mode() -> PowerModeModel:
+            return PowerModeModel(power_mode=self.power_mode)
+
+        class PowerModel(BaseModel):
+            power: float
+
+        @self.app.get("/power", response_model=PowerModel)
+        async def get_power() -> PowerModel:
+            return PowerModel(power=self.get_power())
 
     @abstractmethod
-    def set_power_mode(self, power_mode: str) -> str:
+    def set_power_mode(self, power_mode: str) -> None:
         """Set the power mode for the server.
 
         Args:
             power_mode: The power mode to set.
-
-        Returns:
-            The new power mode.
         """
         power_modes = ["power-saving", "normal", "high performance"]
         if power_mode not in power_modes:
             raise HTTPException(
                 status_code=400,
                 detail=f"{power_mode} is not a valid power mode. "
                        f"Available power modes: {power_modes}"
```

### Comparing `vessim-0.0.2/example_node/rpi/init.sh` & `vessim-0.0.3/examples/sil/example_node/rpi/init.sh`

 * *Files identical despite different names*

### Comparing `vessim-0.0.2/example_node/rpi/lib/pi_controller.py` & `vessim-0.0.3/examples/sil/example_node/rpi/lib/pi_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
         Returns:
             The current frequency of the CPU.
         """
         return self.cpu.get_frequencies()[0]
 
     def frequency_index(self) -> int:
-        """Get the index of the current CPU frequency in list of available frequencies.
+        """Get the index of the current CPU frequency of available frequencies.
 
         Returns:
             The index of the current CPU frequency.
         """
         return self.available_frequencies.index(self.frequency())
 
     def set_max_frequency(self, frequency) -> None:
```

### Comparing `vessim-0.0.2/example_node/rpi/rpi_api_server.py` & `vessim-0.0.3/examples/sil/example_node/rpi/rpi_api_server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import sys
 sys.path.append("../")
 from node_api_server import FastApiServer
 from lib.pi_controller import PiController
-from fastapi import HTTPException
 
 class RpiNodeApiServer(FastApiServer):
     """A Raspberry Pi node API server, extending the base FastApiServer class.
 
     Args:
         host: The host on which to run the FastAPI application.
         port: The port on which to run the FastAPI application.
@@ -18,26 +17,22 @@
         self.power_config = {
             "power-saving": 800 * 1000,
             "normal": 1100 * 1000,
             "high performance": 1400 * 1000,
         }
         self.start()
 
-    def set_power_mode(self, power_mode: str) -> str:
-        """Sets power mode for server and adjusts the max frequency of Pi accordingly.
+    def set_power_mode(self, power_mode: str) -> None:
+        """Sets power mode for server and adjusts the max frequency of Pi.
 
         Args:
             power_mode: The power mode to set.
-
-        Returns:
-            The new power mode.
         """
         super().set_power_mode(power_mode)
         self.pi_controller.set_max_frequency(self.power_config[power_mode])
-        return power_mode
 
     def get_power(self) -> float:
         """Get the power usage of the Raspberry Pi.
 
         Returns:
             The current power usage.
         """
```

### Comparing `vessim-0.0.2/example_node/virtual_node/linear_power_model.py` & `vessim-0.0.3/examples/sil/example_node/virtual_node/linear_power_model.py`

 * *Files identical despite different names*

### Comparing `vessim-0.0.2/example_node/virtual_node/v_node_api_server.py` & `vessim-0.0.3/examples/sil/example_node/virtual_node/v_node_api_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from node_api_server import FastApiServer
 import subprocess
 import multiprocessing
 import psutil
 import re
 
 class VirtualNodeApiServer(FastApiServer):
-    """This class represents a virtual node API server, extending the base
-    FastApiServer class.
+    """This class is a virtual node API server, extending FastApiServer.
 
     The server continuosely runs a sysbench instance that puts load on the CPU.
     Depending on the `power_mode`, the sysbench instance claims different CPU
     utilisation.
 
     Args:
         host: The host on which to run the FastAPI application.
@@ -25,27 +24,23 @@
         self.power_model = LinearPowerModel(p_static=30, p_max=150)
         self.power_config = None
         self.sysbench = None
         self._run_benchmark()
         self._restart_sysbench(run_forever=True)
         self.start()
 
-    def set_power_mode(self, power_mode: str) -> str:
+    def set_power_mode(self, power_mode: str) -> None:
         """Set the power mode for the server.
 
         Args:
             power_mode: The desired power mode. Can be "high performance",
                 "normal" or "power-saving".
-
-        Returns:
-            str: The power mode that has been set.
         """
         super().set_power_mode(power_mode)
         self._restart_sysbench(run_forever=True)
-        return power_mode
 
     def get_power(self) -> float:
         """Get the power usage of the virtual node.
 
         Returns:
             The current power usage.
         """
```

### Comparing `vessim-0.0.2/experimental/pp_scenario.py` & `vessim-0.0.3/experimental/pp_scenario.py`

 * *Files identical despite different names*

### Comparing `vessim-0.0.2/lib/http_client.py` & `vessim-0.0.3/vessim/sil/http_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,39 +17,34 @@
         server_address: The address of the server to connect to.
             e.g. http://localhost
     """
 
     def __init__(self, server_address: str) -> None:
         self.server_address = server_address
 
-    def get(self, route: str) -> Any:
+    def get(self, route: str) -> dict:
         """Sends a GET request to the server and retrieves data.
 
         Args:
             route: The path of the endpoint to send the request to.
 
         Raises:
             HTTPClientError if the data could not be retrieved from route
 
         Returns:
-            The data retrieved from the server. Can be a dictionary, float,
-            int, string, or None if request fails.
+            A dictionary containing the response.
         """
         response = requests.get(self.server_address + route)
         if response.status_code == 200:
-            try:
-                data = response.json() # assuming the response data is in JSON format
-            except ValueError:
-                data = response.content.decode('utf-8') # fallback to string if not JSON
-            return data
-        else:
-            raise HTTPClientError(
-                response.status_code,
-                f'Failed to retrieve data from {route}'
-            )
+            return response.json() # assuming the response data is in JSON format
+
+        raise HTTPClientError(
+            response.status_code,
+            f'Failed to retrieve data from {route}'
+        )
 
     def put(self, route: str, data: Dict[str, Any]) -> None:
         """Sends a PUT request to the server to update data.
 
         Raises:
             HTTPClientError if the data could not be updated at route
```

### Comparing `vessim-0.0.2/pyproject.toml` & `vessim-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -11,20 +11,17 @@
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Topic :: Scientific/Engineering",
   "Topic :: Software Development :: Testing",
   "Topic :: Education",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [ # Optional
   "pandas",
   "mosaik",
   "mosaik-api",
```

### Comparing `vessim-0.0.2/simulator/computing_system.py` & `vessim-0.0.3/vessim/cosim/computing_system.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,56 @@
-from vessim.core import VessimSimulator, VessimModel
-from simulator.power_meter import PowerMeter
 from typing import List
 
+from vessim.cosim._util import VessimSimulator, VessimModel
+from vessim.sil.power_meter import PowerMeter
+
 
 class ComputingSystemSim(VessimSimulator):
     """Computing System simulator that executes its model."""
 
     META = {
         "type": "time-based",
         "models": {
-            "ComputingSystemModel": {
+            "ComputingSystem": {
                 "public": True,
                 "params": ["power_meters", "pue"],
-                "attrs": ["p_cons"],
+                "attrs": ["p"],
             },
         },
     }
 
     def __init__(self):
         self.step_size = None
-        super().__init__(self.META, ComputingSystemModel)
+        super().__init__(self.META, _ComputingSystemModel)
 
     def init(self, sid, time_resolution, step_size, eid_prefix=None):
         self.step_size = step_size
         return super().init(sid, time_resolution, eid_prefix=eid_prefix)
 
     def next_step(self, time):
         return time + self.step_size
 
 
-class ComputingSystemModel(VessimModel):
+class _ComputingSystemModel(VessimModel):
     """Model of the computing system.
 
     This model considers the power usage effectiveness (PUE) and power
     consumption of a list of power meters.
 
-    Attributes:
+    Args:
         power_meters: A list of PowerMeter objects
             representing power meters in the system.
         pue: The power usage effectiveness of the system.
-        p_cons: The power consumption of the system, computed in the step
-            method.
     """
 
-    def __init__(self, power_meters: List[PowerMeter], pue: float):
+    def __init__(self, power_meters: List[PowerMeter], pue: float = 1):
         self.power_meters = power_meters
         self.pue = pue
-        self.p_cons = 0.0
+        self.p = 0.0
 
     def step(self, time: int, inputs: dict) -> None:
         """Updates the power consumption of the system.
 
         The power consumption is calculated as the product of the PUE and the
         sum of the node power of all power meters.
         """
-        self.p_cons = self.pue * sum(pm.measure() for pm in self.power_meters)
+        self.p = self.pue * sum(pm.measure() for pm in self.power_meters)
```

### Comparing `vessim-0.0.2/simulator/redis_docker.py` & `vessim-0.0.3/vessim/sil/redis_docker.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import docker
+import threading
 from time import sleep
 
+import docker
 import redis
+import uvicorn
 from fastapi import FastAPI
 from redis import Redis
-import threading
-import uvicorn
 
 
 class RedisDocker:
     """Class for connection to a Docker container with Redis.
 
     Attributes:
         redis: The redis db that can be used to get and set key, value pairs.
```

### Comparing `vessim-0.0.2/simulator/virtual_energy_system.py` & `vessim-0.0.3/vessim/cosim/energy_system_interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,235 +1,240 @@
-import mosaik_api
-from vessim.core import VessimSimulator, VessimModel
-from vessim.storage import SimpleBattery
-from simulator.redis_docker import RedisDocker
-from fastapi import FastAPI, HTTPException
-from typing import Dict, List, Any
+from threading import Thread
+from typing import Dict, List, Any, Optional
 
+from fastapi import FastAPI
+from fastapi import HTTPException
+from pydantic import BaseModel
 
-META = {
-    "type": "time-based",
-    "models": {
-        "VirtualEnergySystemModel": {
-            "public": True,
-            "params": ["battery", "db_host", "api_host"],
-            "attrs": ["consumption", "battery", "solar", "ci", "grid_power"],
-        },
-    },
-}
+from vessim.core.storage import SimpleBattery, DefaultStoragePolicy
+from vessim.cosim._util import VessimSimulator, VessimModel
+from vessim.sil.http_client import HTTPClient, HTTPClientError
+from vessim.sil.node import Node
+from vessim.sil.redis_docker import RedisDocker
 
 
-class VirtualEnergySystem(VessimSimulator):
+class EnergySystemInterfaceSim(VessimSimulator):
     """Virtual Energy System (VES) simulator that executes the VES model."""
 
+    META = {
+        "type": "time-based",
+        "models": {
+            "EnergySystemInterface": {
+                "public": True,
+                "params": ["battery", "policy", "db_host", "api_host", "nodes"],
+                "attrs": ["battery", "p_cons", "p_gen", "p_grid", "ci"],
+            },
+        },
+    }
+
     def __init__(self) -> None:
         self.step_size = None
-        super().__init__(META, VirtualEnergySystemModel)
+        super().__init__(self.META, _EnergySystemInterfaceModel)
 
     def init(self, sid, time_resolution, step_size, eid_prefix=None):
         self.step_size = step_size
-        super().init(sid, time_resolution, eid_prefix=eid_prefix)
+        return super().init(sid, time_resolution, eid_prefix=eid_prefix)
 
     def finalize(self) -> None:
         """Stops the uvicorn server after the simulation has finished."""
         super().finalize()
         for model_instance in self.entities.values():
             model_instance.redis_docker.stop()
 
     def next_step(self, time):
         return time + self.step_size
 
-# TODO in the future we have to differentiate between the energy system
-#   and the virtualization layers.
 
+class _EnergySystemInterfaceModel(VessimModel):
+    """Software-in-the-Loop interface to the energy system simulation.
 
-class VirtualEnergySystemModel(VessimModel):
-    """A virtual energy system model.
+    TODO this class is still very specific to our paper use case and does not generalize
+        well to other scenarios.
 
     Args:
         battery: SimpleBatteryModel used by the system.
+        policy: The (dis)charging policy used to control the battery.
+        nodes: List of physical or virtual computing nodes.
         db_host (optional): The host address for the database, defaults to '127.0.0.1'.
         api_host (optional): The host address for the API, defaults to '127.0.0.1'.
-
-    Attributes:
-        step_size: The time step in seconds for the model.
-        battery: The battery model used by the system.
-        battery_grid_charge: The amount of energy charged to the battery from the grid.
-        nodes_power_mode: The power mode of individual nodes.
-        consumption: The current total energy consumption of the system.
-        solar: The current energy generated by solar panels.
-        ci: The current public grid carbon intensity.
-        grid_power: The total power drawn from or fed back into the grid.
-        redis_docker: The Redis Docker instance used by the system.
-
     """
 
     def __init__(
         self,
+        nodes: list[Node],
         battery: SimpleBattery,
+        policy: DefaultStoragePolicy,
         db_host: str = "127.0.0.1",
         api_host: str = "127.0.0.1",
     ):
-        # ves attributes
+        self.nodes = nodes
         self.battery = battery
-        self.battery_grid_charge = 0.0
-        self.nodes_power_mode: Dict[str, str] = {}
-        self.consumption = 0
-        self.solar = 0
+        self.policy = policy
+        self.p_cons = 0
+        self.p_gen = 0
+        self.p_grid = 0
         self.ci = 0
-        self.grid_power = 0
 
         # db & api
         self.redis_docker = RedisDocker(host=db_host)
         f_api = self.init_fastapi()
         self.redis_docker.run(f_api, host=api_host)
 
     def step(self, time: int, inputs: dict) -> None:
-        """Step the virtual energy system model.
-
-        Executes a single time step of the energy system model, calculating
-        energy consumption and generation and determining how much power to
-        draw from or feed back into the grid. If there is not enough solar
-        power available, the method tries to use the battery. If there is
-        excess solar power, the method will charge the battery or feed back
-        into the grid.
-        """
-        # update input
-        self.consumption = inputs["consumption"]
-        self.solar = inputs["solar"]
+        self.p_cons = inputs["p_cons"]
+        self.p_gen = inputs["p_gen"]
         self.ci = inputs["ci"]
+        self.p_grid = inputs["p_grid"]
 
-        # If delta is positive there is excess power,
-        # if negative there is a power deficit.
-        delta = self.battery_grid_charge + self.solar - self.consumption
-
-        # battery charge is the value the battery is (dis)charged with
-        battery_charge = min(
-            self.battery.max_charge_power, max(delta, -self.battery.max_charge_power)
-        )
-
-        delta -= battery_charge
-        # (dis)charge the battery
-        battery_excess = self.battery.update(
-            power=battery_charge, duration=self.step_size
-        )
-
-        # battery_excess contains the excess energy after an update:
-        #   - positive if the battery is fully charged
-        #   - negative if the battery is empty
-        #   - else 0
-        delta -= battery_excess + self.battery_grid_charge
-        # draw or feed back into the grid
-        self.grid_power = delta
+        # update redis
+        self.redis_docker.redis.set("solar", self.p_gen)
+        self.redis_docker.redis.set("ci", self.ci)
+
+        # get redis update
+        self.battery.min_soc = float(self.redis_get("battery.min_soc"))
+        self.policy.grid_power = float(self.redis_get("battery_grid_charge"))
+        # update power mode for the node remotely
+        for node in self.nodes:
+            updated_power_mode = self.redis_get("node.power_mode", str(node.id))
+            if node.power_mode == updated_power_mode:
+                continue
+            node.power_mode = updated_power_mode
+            http_client = HTTPClient(f"{node.address}:{node.port}")
+
+            def update_power_model():
+                try:
+                    http_client.put("/power_mode", {"power_mode": node.power_mode})
+                except HTTPClientError as e:
+                    print(e)
+            # use thread to not slow down simulation
+            update_thread = Thread(target=update_power_model)
+            update_thread.start()
 
     def init_fastapi(self) -> FastAPI:
         """Initializes the FastAPI application.
 
         Returns:
             FastAPI: The initialized FastAPI application.
         """
         app = FastAPI()
-
         self.init_get_routes(app)
         self.init_put_routes(app)
-
         return app
 
-    def redis_get(self, entry: str) -> Any:
+    def redis_get(self, entry: str, field: Optional[str] = None) -> Any:
         """Method for getting data from Redis database.
 
         Args:
             entry: The name of the key to retrieve from Redis.
+            field: The field (or item_id in your case) to retrieve from the
+                hash at the specified key.
 
         Returns:
             any: The value retrieved from Redis.
 
         Raises:
-            ValueError: If the key does not exist in Redis.
+            ValueError: If the key or the field does not exist in Redis.
         """
-        value = self.redis_docker.redis.get(entry)
+        if self.redis_docker.redis.type(entry) == b'hash' and field is not None:
+            value = self.redis_docker.redis.hget(entry, field)
+        else:
+            value = self.redis_docker.redis.get(entry)
+
         if value is None:
-            raise ValueError(f"entry {entry} does not exist")
+            if field:
+                raise ValueError(f"field {field} does not exist in the hash {entry}")
+            else:
+                raise ValueError(f"entry {entry} does not exist")
         return value
 
     def init_get_routes(self, app: FastAPI) -> None:
         """Initializes GET routes for a FastAPI.
 
         With the given route attributes, the initial values of the attributes
         are stored in Redis key-value store.
 
         Args:
-            app (FastAPI): The FastAPI app to add the GET routes to.
+            app: The FastAPI app to add the GET routes to.
         """
         # store attributes and its initial values in Redis key-value store
         redis_init_content = {
-            "solar": self.solar,
+            "p_cons": self.p_cons,
+            "solar": self.p_gen,
+            "p_grid": self.p_grid,
             "ci": self.ci,
             "battery.soc": self.battery.soc(),
+            "battery.min_soc": self.battery.min_soc,
+            "battery_grid_charge": self.policy.grid_power
             # TODO implement forecasts:
             #'ci_forecast': self.ci_forecast,
             #'solar_forecast': self.solar_forecast
         }
         self.redis_docker.redis.mset(redis_init_content)
+        for node in self.nodes:
+            self.redis_docker.redis.hset("node.power_mode", str(node.id), node.power_mode)
 
-        @app.get("/solar")
-        async def get_solar() -> float:
-            return float(self.redis_get("solar"))
-
-        @app.get("/ci")
-        async def get_ci() -> float:
-            return float(self.redis_get("ci"))
-
-        @app.get("/battery-soc")
-        async def get_battery_soc() -> float:
-            return float(self.redis_get("battery.soc"))
+        class SolarModel(BaseModel):
+            solar: float
+
+        @app.get("/solar", response_model=SolarModel)
+        async def get_solar() -> SolarModel:
+            return SolarModel(solar=self.p_gen)
+
+        class CiModel(BaseModel):
+            ci: float
+
+        @app.get("/ci", response_model=CiModel)
+        async def get_ci() -> CiModel:
+            return CiModel(ci=self.ci)
+
+        class BatterySocModel(BaseModel):
+            battery_soc: float
+
+        @app.get("/battery-soc", response_model=BatterySocModel)
+        async def get_battery_soc() -> BatterySocModel:
+            return BatterySocModel(battery_soc=self.battery.soc())
 
     def init_put_routes(self, app: FastAPI) -> None:
         """Initialize PUT routes for the FastAPI application.
 
         Two PUT routes are set up: '/ves/battery' to update the battery
         settings, and '/cs/nodes/{item_id}' to update the power mode of a
         specific node. This method handles data validation and updates the
         corresponding attributes in the application instance and Redis
         datastore.
 
         Args:
-            app (FastAPI): FastAPI application instance to which PUT routes are added.
+            app: FastAPI application instance to which PUT routes are added.
         """
 
-        def validate_keys(data: Dict[str, Any], expected_keys: List[str]):
-            missing_keys = set(expected_keys) - set(data.keys())
-            if missing_keys:
-                raise HTTPException(
-                    status_code=422, detail=f"Missing keys: {', '.join(missing_keys)}"
-                )
+        class BatteryModel(BaseModel):
+            min_soc: float
+            grid_charge: float
+
+        @app.put("/ves/battery", response_model=BatteryModel)
+        async def put_battery(battery: BatteryModel) -> BatteryModel:
+            self.redis_docker.redis.set("battery.min_soc", battery.min_soc)
+            self.redis_docker.redis.set("battery_grid_charge", battery.grid_charge)
+            return battery
+
+        class NodeModel(BaseModel):
+            power_mode: str
 
-        @app.put("/ves/battery")
-        async def put_battery(data: Dict[str, float]):
-            validate_keys(data, ["min_soc", "grid_charge"])
-            self.battery.min_soc = data["min_soc"]
-            self.redis_docker.redis.set("battery.min_soc", data["min_soc"])
-            self.battery_grid_charge = data["grid_charge"]
-            self.redis_docker.redis.set("battery_grid_charge", data["grid_charge"])
-            return data
-
-        @app.put("/cs/nodes/{item_id}")
-        async def put_nodes(data: Dict[str, str], item_id: int):
-            validate_keys(data, ["power_mode"])
+        @app.put("/cs/nodes/{item_id}", response_model=NodeModel)
+        async def put_nodes(node: Node, item_id: int) -> Node:
             power_modes = ["power-saving", "normal", "high performance"]
-            value = data["power_mode"]
-            if value not in power_modes:
+            power_mode = node.power_mode
+            if power_mode not in power_modes:
                 raise HTTPException(
-                status_code=400,
-                detail=f"{value} is not a valid power mode. "
-                f"Available power modes: {power_modes}",
+                    status_code=400,
+                    detail=f"{power_mode} is not a valid power mode. "
+                           f"Available power modes: {power_modes}"
             )
-            self.nodes_power_mode[item_id] = value
-            self.redis_docker.redis.hset("nodes_power_mode", str(item_id), value)
-            return data
+            self.redis_docker.redis.hset("node.power_mode", str(item_id), power_mode)
+            return node
 
     def print_redis(self):
         """Debugging function that simply prints all entries of the redis db."""
         r = self.redis_docker.redis
         # Start the SCAN iterator
         cursor = 0
         while True:
@@ -252,12 +257,7 @@
                 else:
                     value = None
 
                 print(f"Key: {key}, Type: {key_type}, Value: {value}")
 
             if cursor == 0:
                 break
-
-
-def main():
-    """Start the mosaik simulation."""
-    return mosaik_api.start_simulation(VirtualEnergySystem())
```

### Comparing `vessim-0.0.2/tests/test_carbon_api.py` & `vessim-0.0.3/tests/test_carbon_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import pytest
 
-from vessim.carbon_api import CarbonApi
+from vessim.core.simulator import CarbonApi
 
 
 class TestCarbonApi:
 
     @pytest.fixture
     def ci_api(self) -> CarbonApi:
         index = [pd.to_datetime("2023-01-01T00:00:00"),
```

### Comparing `vessim-0.0.2/tests/test_storage.py` & `vessim-0.0.3/tests/test_storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from vessim.storage import SimpleBattery
+from vessim.core.storage import SimpleBattery
 
 
 class TestSimpleBattery:
 
     @pytest.fixture
     def battery(self) -> SimpleBattery:
         return SimpleBattery(capacity=100, charge_level=80, min_soc=0.1)
```

### Comparing `vessim-0.0.2/tf_gcp_node/.gitignore` & `vessim-0.0.3/examples/sil/tf_gcp_node/.gitignore`

 * *Files identical despite different names*

### Comparing `vessim-0.0.2/tf_gcp_node/README.md` & `vessim-0.0.3/examples/sil/tf_gcp_node/README.md`

 * *Files identical despite different names*

### Comparing `vessim-0.0.2/tf_gcp_node/main.tf` & `vessim-0.0.3/examples/sil/tf_gcp_node/main.tf`

 * *Files identical despite different names*

### Comparing `vessim-0.0.2/tf_gcp_node/variables.tf` & `vessim-0.0.3/examples/sil/tf_gcp_node/variables.tf`

 * *Files identical despite different names*

### Comparing `vessim-0.0.2/vessim/microgrid.py` & `vessim-0.0.3/vessim/cosim/microgrid.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,45 @@
-from abc import ABC, abstractmethod
-from typing import Optional, Callable
+from typing import Optional, Union
 
-from vessim.core import VessimSimulator, VessimModel
-from vessim.storage import Storage, StoragePolicy, DefaultStoragePolicy
+from vessim.core.storage import Storage, StoragePolicy, DefaultStoragePolicy
+from vessim.cosim._util import VessimSimulator, VessimModel
 
 
 class MicrogridSim(VessimSimulator):
 
     META = {
         "type": "event-based",
         "models": {
-            "MicrogridModel": {
+            "Microgrid": {
                 "public": True,
                 "params": ["storage", "policy"],
-                "attrs": ["p_gen", "p_cons", "p_grid"],
+                "attrs": ["p", "p_delta"],
             },
         },
     }
 
     def __init__(self) -> None:
         self.step_size = None
-        super().__init__(self.META, MicrogridModel)
+        super().__init__(self.META, _MicrogridModel)
 
     def next_step(self, time):
         return None
 
 
-class MicrogridModel(VessimModel):
+class _MicrogridModel(VessimModel):  # TODO abstract away
     def __init__(self,
                  storage: Optional[Storage] = None,
                  policy: Optional[StoragePolicy] = None):
         self.storage = storage
         self.policy = policy if policy is not None else DefaultStoragePolicy()
-        self.p_gen = 0.0
-        self.p_cons = 0.0
-        self.p_grid = 0.0
+        self.p_delta = 0.0
         self._last_step_time = 0
 
     def step(self, time: int, inputs: dict) -> None:
-        self.p_gen = inputs["p_gen"]
-        self.p_cons = inputs["p_cons"]
-        p_delta = self.p_gen - self.p_cons
+        p: Union[float, list[float]] = inputs["p"]
+        p_delta = p if type(p) == float else sum(inputs["p"])
         time_since_last_step = time - self._last_step_time
         if self.storage is None:
-            self.p_grid = p_delta
+            self.p_delta = p_delta
         else:
-            self.p_grid = self.policy.apply(self.storage, p_delta, time_since_last_step)
+            self.p_delta = self.policy.apply(self.storage, p_delta, time_since_last_step)
         self._last_step_time = time
```

### Comparing `vessim-0.0.2/vessim/monitor.py` & `vessim-0.0.3/vessim/cosim/monitor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 from collections import defaultdict
-from datetime import datetime, timedelta
+from datetime import datetime
 from typing import Dict, Callable, Any
 
+import mosaik_api
 import pandas as pd
-import csv
 from loguru import logger
 
-import mosaik_api
-
-from vessim._util import Clock
+from vessim.cosim._util import Clock
 
-META = {
-    "type": "event-based",
-    "models": {
-        "Monitor": {
-            "public": True,
-            "any_inputs": True,
-            "params": ["fn", "sim_start"],
-            "attrs": [],
-        },
-    },
-}
 
-
-class Monitor(mosaik_api.Simulator):
+class MonitorSim(mosaik_api.Simulator):  # TODO Make time based
     """Simple data collector for printing data at the end of simulation.
 
     Attributes:
         eid: Identifier of Simulator Instance
         data: Dictionary for holding the necessary simulation data
     """
 
+    META = {
+        "type": "event-based",
+        "models": {
+            "Monitor": {
+                "public": True,
+                "any_inputs": True,
+                "params": ["fn", "sim_start"],
+                "attrs": [],
+            },
+        },
+    }
+
     def __init__(self):
-        super().__init__(META)
+        super().__init__(self.META)
         self.eid = None
         self.data = defaultdict(dict)
         self.fn = None
         self._clock = None
 
     def init(self, sid, time_resolution):
         return self.meta
```

### Comparing `vessim-0.0.2/vessim/storage.py` & `vessim-0.0.3/vessim/core/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def update(self, power: float, duration: int) -> float:
         max_charge_p_delta, p_delta = 0, 0
 
         if self.c_rate is not None:
             max_rate = self.c_rate * self.capacity / 3600
             if power >= max_rate:
                 logger.info(f"Trying to charge storage '{__class__.__name__}' with "
-                            f"{power}W but only {max_rate} are supported.")
+                            f"{power} W but only {max_rate} W are supported.")
                 max_charge_p_delta = power - max_rate
                 power = max_rate
 
             if power <= -max_rate:
                 logger.info(f"Trying to discharge storage '{__class__.__name__}' with "
                             f"{power} W but only {max_rate} W are supported.")
                 max_charge_p_delta = power + max_rate
@@ -76,15 +76,14 @@
 
         return p_delta + max_charge_p_delta
 
     def soc(self):
         return self.charge_level / self.capacity
 
 
-
 class StoragePolicy(ABC):
 
     @abstractmethod
     def apply(self, storage: Storage, p_delta: float, time_since_last_step: int) -> float:
         """(Dis)charge the storage according to the policy."""
```

