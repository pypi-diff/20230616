# Comparing `tmp/redfish_utilities-3.1.3.tar.gz` & `tmp/redfish_utilities-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_utilities-3.1.3.tar", last modified: Tue Apr 25 14:51:11 2023, max compression
+gzip compressed data, was "redfish_utilities-3.1.4.tar", last modified: Fri Jun 16 20:13:54 2023, max compression
```

## Comparing `redfish_utilities-3.1.3.tar` & `redfish_utilities-3.1.4.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:51:11.717513 redfish_utilities-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-04-25 14:51:11.717513 redfish_utilities-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36943 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:51:11.713513 redfish_utilities-3.1.3/redfish_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/event_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17523 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/resets.py
--rw-r--r--   0 runner    (1001) docker     (123)    22014 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25851 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/redfish_utilities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:51:11.713513 redfish_utilities-3.1.3/redfish_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-04-25 14:51:11.000000 redfish_utilities-3.1.3/redfish_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-25 14:51:11.000000 redfish_utilities-3.1.3/redfish_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:51:11.000000 redfish_utilities-3.1.3/redfish_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 14:51:11.000000 redfish_utilities-3.1.3/redfish_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 14:51:11.000000 redfish_utilities-3.1.3/redfish_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:51:11.717513 redfish_utilities-3.1.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_bios_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_boot_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_diagnostic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_event_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_power_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_raw_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_sensor_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_sys_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/scripts/rf_virtual_media.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:51:11.717513 redfish_utilities-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-25 14:50:50.000000 redfish_utilities-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:13:54.407136 redfish_utilities-3.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-06-16 20:13:54.407136 redfish_utilities-3.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36943 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:13:54.403136 redfish_utilities-3.1.4/redfish_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/resets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25527 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/redfish_utilities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:13:54.403136 redfish_utilities-3.1.4/redfish_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-06-16 20:13:54.000000 redfish_utilities-3.1.4/redfish_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-16 20:13:54.000000 redfish_utilities-3.1.4/redfish_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:13:54.000000 redfish_utilities-3.1.4/redfish_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 20:13:54.000000 redfish_utilities-3.1.4/redfish_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 20:13:54.000000 redfish_utilities-3.1.4/redfish_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:13:54.407136 redfish_utilities-3.1.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_bios_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_boot_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_diagnostic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_event_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_power_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_sensor_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_sys_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/scripts/rf_virtual_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:13:54.407136 redfish_utilities-3.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-16 20:13:42.000000 redfish_utilities-3.1.4/setup.py
```

### Comparing `redfish_utilities-3.1.3/LICENSE.md` & `redfish_utilities-3.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.3/PKG-INFO` & `redfish_utilities-3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_utilities
-Version: 3.1.3
+Version: 3.1.4
 Summary: Redfish Utilities
 Home-page: https://github.com/DMTF/Redfish-Tacklebox
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_utilities-3.1.3/README.md` & `redfish_utilities-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.3/redfish_utilities/__init__.py` & `redfish_utilities-3.1.4/redfish_utilities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2022 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 from .accounts import get_users
 from .accounts import print_users
 from .accounts import add_user
 from .accounts import delete_user
 from .accounts import modify_user
 from .event_service import get_event_service
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities/accounts.py` & `redfish_utilities-3.1.4/redfish_utilities/accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Accounts Module
 
 File : accounts.py
 
 Brief : This file contains the definitions and functionalities for managing
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities/config.py` & `redfish_utilities-3.1.4/redfish_utilities/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2022 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Configuration Settings
 
 File : config.py
 
 Brief : This file contains configuration settings for the module; useful for
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities/event_service.py` & `redfish_utilities-3.1.4/redfish_utilities/event_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Event Service Module
 
 File : event_service.py
 
 Brief : This file contains the definitions and functionalities for managing
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities/inventory.py` & `redfish_utilities-3.1.4/redfish_utilities/inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Inventory Module
 
 File : inventory.py
 
 Brief : This file contains the definitions and functionalities for scanning a
         Redfish service for an inventory of components
 """
 
 import warnings
 import xlsxwriter
+from .collections import get_collection_ids
 from .messages import verify_response
 from . import config
 
 class RedfishChassisNotFoundError( Exception ):
     """
     Raised when a matching chassis cannot be found
     """
@@ -402,20 +403,12 @@
     Returns:
         A list of identifiers of the members of the chassis collection
     """
 
     # Get the service root to find the chassis collection
     service_root = context.get( "/redfish/v1/" )
     if "Chassis" not in service_root.dict:
-        # No system collection
+        # No chassis collection
         raise RedfishChassisNotFoundError( "Service does not contain a chassis collection" )
 
     # Get the chassis collection and iterate through its collection
-    avail_chassis = []
-    chassis_col = context.get( service_root.dict["Chassis"]["@odata.id"] )
-    while True:
-        for chassis_member in chassis_col.dict["Members"]:
-            avail_chassis.append( chassis_member["@odata.id"].strip( "/" ).split( "/" )[-1] )
-        if "Members@odata.nextLink" not in chassis_col.dict:
-            break
-        chassis_col = context.get( chassis_col.dict["Members@odata.nextLink"] )
-    return avail_chassis
+    return get_collection_ids( context, service_root.dict["Chassis"]["@odata.id"] )
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities/logs.py` & `redfish_utilities-3.1.4/redfish_utilities/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2022 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Logs Module
 
 File : logs.py
 
 Brief : This file contains the definitions and functionalities for interacting
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities/managers.py` & `redfish_utilities-3.1.4/redfish_utilities/managers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2021 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Managers Module
 
 File : managers.py
 
 Brief : This file contains the definitions and functionalities for interacting
         with the managers collection for a given Redfish service
 """
 
+from .collections import get_collection_ids
 from .messages import verify_response
 from .resets import reset_types
 
 class RedfishManagerNotFoundError( Exception ):
     """
     Raised when a matching manager cannot be found
     """
@@ -47,23 +48,15 @@
     # Get the service root to find the manager collection
     service_root = context.get( "/redfish/v1/" )
     if "Managers" not in service_root.dict:
         # No manager collection
         raise RedfishManagerNotFoundError( "Service does not contain a manager collection" )
 
     # Get the manager collection and iterate through its collection
-    avail_managers = []
-    manager_col = context.get( service_root.dict["Managers"]["@odata.id"] )
-    while True:
-        for manager_member in manager_col.dict["Members"]:
-            avail_managers.append( manager_member["@odata.id"].strip( "/" ).split( "/" )[-1] )
-        if "Members@odata.nextLink" not in manager_col.dict:
-            break
-        manager_col = context.get( manager_col.dict["Members@odata.nextLink"] )
-    return avail_managers
+    return get_collection_ids( context, service_root.dict["Managers"]["@odata.id"] )
 
 def get_manager( context, manager_id = None ):
     """
     Finds a manager matching the given identifier and returns its resource
 
     Args:
         context: The Redfish client object with an open session
@@ -84,20 +77,19 @@
         avail_managers = get_manager_ids( context )
         if len( avail_managers ) == 1:
             manager = context.get( manager_uri_pattern.format( avail_managers[0] ) )
         else:
             raise RedfishManagerNotFoundError( "Service does not contain exactly one manager; a target manager needs to be specified: {}".format( ", ".join( avail_managers ) ) )
 
     # Check the response and return the manager if the response is good
-    try:
-        verify_response( manager )
-    except:
+    if manager.status == 404:
         if avail_managers is None:
             avail_managers = get_manager_ids( context )
-        raise RedfishManagerNotFoundError( "Service does not contain a manager called {}; valid managers: {}".format( manager_id, ", ".join( avail_managers ) ) ) from None
+        raise RedfishManagerNotFoundError( "Service does not contain a manager called {}; valid managers: {}".format( manager_id, ", ".join( avail_managers ) ) )
+    verify_response( manager )
     return manager
 
 def print_manager( manager ):
     """
     Prints the manager info
 
     Args:
@@ -226,23 +218,15 @@
     # Get the manager to find its Ethernet interface collection
     manager = get_manager( context, manager_id )
     if "EthernetInterfaces" not in manager.dict:
         # No Ethernet interface collection
         raise RedfishManagerEthIntNotFoundError( "Manager {} does not contain an Ethernet interface collection".format( manager.dict["Id"] ) )
 
     # Get the Ethernet interface collection and iterate through its collection
-    avail_interfaces = []
-    interface_col = context.get( manager.dict["EthernetInterfaces"]["@odata.id"] )
-    while True:
-        for interface_member in interface_col.dict["Members"]:
-            avail_interfaces.append( interface_member["@odata.id"].strip( "/" ).split( "/" )[-1] )
-        if "Members@odata.nextLink" not in interface_col.dict:
-            break
-        interface_col = context.get( interface_col.dict["Members@odata.nextLink"] )
-    return avail_interfaces
+    return get_collection_ids( context, manager.dict["EthernetInterfaces"]["@odata.id"] )
 
 def get_manager_ethernet_interface( context, manager_id = None, interface_id = None ):
     """
     Finds an Ethernet interface for a manager matching the given identifiers and returns its resource
 
     Args:
         context: The Redfish client object with an open session
@@ -269,20 +253,19 @@
         avail_interfaces = get_manager_ethernet_interface_ids( context, manager_id )
         if len( avail_interfaces ) == 1:
             interface = context.get( interface_uri_pattern.format( manager_id, avail_interfaces[0] ) )
         else:
             raise RedfishManagerEthIntNotFoundError( "Manager {} does not contain exactly one Ethernet interface; a target Ethernet interface needs to be specified: {}".format( manager_id, ", ".join( avail_interfaces ) ) )
 
     # Check the response and return the Ethernet interface if the response is good
-    try:
-        verify_response( interface )
-    except:
+    if interface.status == 404:
         if avail_interfaces is None:
             avail_interfaces = get_manager_ethernet_interface_ids( context, manager_id )
-        raise RedfishManagerEthIntNotFoundError( "Manager {} does not contain an Ethernet interface called {}; valid Ethernet interfaces: {}".format( manager_id, interface_id, ", ".join( avail_interfaces ) ) ) from None
+        raise RedfishManagerEthIntNotFoundError( "Manager {} does not contain an Ethernet interface called {}; valid Ethernet interfaces: {}".format( manager_id, interface_id, ", ".join( avail_interfaces ) ) )
+    verify_response( interface )
     return interface
 
 def set_manager_ethernet_interface( context, manager_id = None, interface_id = None, vlan = None, ipv4_addresses = None, dhcpv4 = None, ipv6_addresses = None, ipv6_gateways = None, dhcpv6 = None ):
     """
     Finds an Ethernet interface matching the given ID and updates specified properties
 
     Args:
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities/messages.py` & `redfish_utilities-3.1.4/redfish_utilities/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Messages Module
 
 File : messages.py
 
 Brief : This file contains the definitions and functionalities for interacting
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities/resets.py` & `redfish_utilities-3.1.4/redfish_utilities/resets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Resets Module
 
 File : resets.py
 
 Brief : This file contains the common definitions and functionalities for
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities/sensors.py` & `redfish_utilities-3.1.4/redfish_utilities/sensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Sensors Module
 
 File : sensors.py
 
 Brief : This file contains the definitions and functionalities for scanning a
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities/systems.py` & `redfish_utilities-3.1.4/redfish_utilities/systems.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2021 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Systems Module
 
 File : systems.py
 
 Brief : This file contains the definitions and functionalities for interacting
         with the systems collection for a given Redfish service
 """
 
 import warnings
 import sys
+from .collections import get_collection_ids
 from .messages import verify_response
 from .resets import reset_types
 from . import config
 
 class RedfishSystemNotFoundError( Exception ):
     """
     Raised when a matching system cannot be found
@@ -73,23 +74,15 @@
     # Get the service root to find the system collection
     service_root = context.get( "/redfish/v1/" )
     if "Systems" not in service_root.dict:
         # No system collection
         raise RedfishSystemNotFoundError( "Service does not contain a system collection" )
 
     # Get the system collection and iterate through its collection
-    avail_systems = []
-    system_col = context.get( service_root.dict["Systems"]["@odata.id"] )
-    while True:
-        for system_member in system_col.dict["Members"]:
-            avail_systems.append( system_member["@odata.id"].strip( "/" ).split( "/" )[-1] )
-        if "Members@odata.nextLink" not in system_col.dict:
-            break
-        system_col = context.get( system_col.dict["Members@odata.nextLink"] )
-    return avail_systems
+    return get_collection_ids( context, service_root.dict["Systems"]["@odata.id"] )
 
 def get_system( context, system_id = None ):
     """
     Finds a system matching the given identifier and returns its resource
 
     Args:
         context: The Redfish client object with an open session
@@ -110,20 +103,19 @@
         avail_systems = get_system_ids( context )
         if len( avail_systems ) == 1:
             system = context.get( system_uri_pattern.format( avail_systems[0] ) )
         else:
             raise RedfishSystemNotFoundError( "Service does not contain exactly one system; a target system needs to be specified: {}".format( ", ".join( avail_systems ) ) )
 
     # Check the response and return the system if the response is good
-    try:
-        verify_response( system )
-    except:
+    if system.status == 404:
         if avail_systems is None:
             avail_systems = get_system_ids( context )
-        raise RedfishSystemNotFoundError( "Service does not contain a system called {}; valid systems: {}".format( system_id, ", ".join( avail_systems ) ) ) from None
+        raise RedfishSystemNotFoundError( "Service does not contain a system called {}; valid systems: {}".format( system_id, ", ".join( avail_systems ) ) )
+    verify_response( system )
     return system
 
 def get_system_boot( context, system_id = None ):
     """
     Finds a system matching the given ID and returns its Boot object
 
     Args:
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities/tasks.py` & `redfish_utilities-3.1.4/redfish_utilities/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Tasks Module
 
 File : tasks.py
 
 Brief : This file contains the definitions and functionalities for interacting
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities/update.py` & `redfish_utilities-3.1.4/redfish_utilities/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Update Module
 
 File : update.py
 
 Brief : This file contains the definitions and functionalities for interacting
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities.egg-info/PKG-INFO` & `redfish_utilities-3.1.4/redfish_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish-utilities
-Version: 3.1.3
+Version: 3.1.4
 Summary: Redfish Utilities
 Home-page: https://github.com/DMTF/Redfish-Tacklebox
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_utilities-3.1.3/redfish_utilities.egg-info/SOURCES.txt` & `redfish_utilities-3.1.4/redfish_utilities.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 AUTHORS.md
 LICENSE.md
 README.md
 setup.py
 redfish_utilities/__init__.py
 redfish_utilities/accounts.py
+redfish_utilities/collections.py
 redfish_utilities/config.py
 redfish_utilities/event_service.py
 redfish_utilities/inventory.py
 redfish_utilities/logs.py
 redfish_utilities/managers.py
 redfish_utilities/messages.py
 redfish_utilities/resets.py
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_accounts.py` & `redfish_utilities-3.1.4/scripts/rf_accounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish Accounts
 
 File : rf_accounts.py
 
 Brief : This script uses the redfish_utilities module to manage user accounts
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_bios_settings.py` & `redfish_utilities-3.1.4/scripts/rf_bios_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish BIOS Settings
 
 File : rf_bios_settings.py
 
 Brief : This script uses the redfish_utilities module to manager BIOS settings of a system
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_boot_override.py` & `redfish_utilities-3.1.4/scripts/rf_boot_override.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish Boot Override
 
 File : rf_boot_override.py
 
 Brief : This script uses the redfish_utilities module to manage a one time boot
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_diagnostic_data.py` & `redfish_utilities-3.1.4/scripts/rf_diagnostic_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2022 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish Diagnostic Data
 
 File : rf_diagnostic_data.py
 
 Brief : This script uses the redfish_utilities module to collect diagnostic data from a log service
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_discover.py` & `redfish_utilities-3.1.4/scripts/rf_discover.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish Discover
 
 File : rf_discover.py
 
 Brief : This script uses the redfish module to discover Redfish services
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_event_service.py` & `redfish_utilities-3.1.4/scripts/rf_event_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish Event Service
 
 File : rf_event_service.py
 
 Brief : This script uses the redfish_utilities module to manage the event service and event subscriptions
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_logs.py` & `redfish_utilities-3.1.4/scripts/rf_logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish Logs
 
 File : rf_logs.py
 
 Brief : This script uses the redfish_utilities module to manage logs
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_manager_config.py` & `redfish_utilities-3.1.4/scripts/rf_manager_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2021 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish Manager Configuration
 
 File : rf_manager_config.py
 
 Brief : This script uses the redfish_utilities module to manage managers
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_power_reset.py` & `redfish_utilities-3.1.4/scripts/rf_power_reset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish Power Reset
 
 File : rf_power_reset.py
 
 Brief : This script uses the redfish_utilities module to perform a reset of the system
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_raw_request.py` & `redfish_utilities-3.1.4/scripts/rf_raw_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2022 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish Raw Request
 
 File : rf_raw_request.py
 
 Brief : This script performs a raw request specified by the user
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_sensor_list.py` & `redfish_utilities-3.1.4/scripts/rf_sensor_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish Sensor List
 
 File : rf_sensor_list.py
 
 Brief : This script uses the redfish_utilities module to dump sensor info
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_sys_inventory.py` & `redfish_utilities-3.1.4/scripts/rf_sys_inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish System Inventory
 
 File : rf_sys_inventory.py
 
 Brief : This script uses the redfish_utilities module to dump system inventory
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_update.py` & `redfish_utilities-3.1.4/scripts/rf_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish Update
 
 File : rf_update.py
 
 Brief : This script uses the redfish_utilities module to perform updates
```

### Comparing `redfish_utilities-3.1.3/scripts/rf_virtual_media.py` & `redfish_utilities-3.1.4/scripts/rf_virtual_media.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2021 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 """
 Redfish Virtual Media
 
 File : rf_virtual_media.py
 
 Brief : This script uses the redfish_utilities module to manage virtual media
```

### Comparing `redfish_utilities-3.1.3/setup.py` & `redfish_utilities-3.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #! /usr/bin/python
 # Copyright Notice:
 # Copyright 2019-2022 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 from setuptools import setup
 from codecs import open
 
 with open( "README.md", "r", "utf-8" ) as f:
     long_description = f.read()
 
 setup(
     name = "redfish_utilities",
-    version = "3.1.3",
+    version = "3.1.4",
     description = "Redfish Utilities",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     author = "DMTF, https://www.dmtf.org/standards/feedback",
     license = "BSD 3-clause \"New\" or \"Revised License\"",
     classifiers = [
         "Development Status :: 5 - Production/Stable",
```

