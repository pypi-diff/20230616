# Comparing `tmp/redfish_protocol_validator-1.1.6.tar.gz` & `tmp/redfish_protocol_validator-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_protocol_validator-1.1.6.tar", last modified: Fri Feb 10 20:47:50 2023, max compression
+gzip compressed data, was "redfish_protocol_validator-1.1.7.tar", last modified: Fri Jun 16 20:11:41 2023, max compression
```

## Comparing `redfish_protocol_validator-1.1.6.tar` & `redfish_protocol_validator-1.1.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:47:50.439090 redfish_protocol_validator-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-02-10 20:47:50.439090 redfish_protocol_validator-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:47:50.439090 redfish_protocol_validator-1.1.6/redfish_protocol_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/console_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    32039 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/protocol_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    24904 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/redfish_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    21014 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    54308 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/security_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    48776 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/service_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    63807 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/service_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    28980 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/service_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/system_under_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:47:50.439090 redfish_protocol_validator-1.1.6/redfish_protocol_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-02-10 20:47:50.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-10 20:47:50.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 20:47:50.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-10 20:47:50.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-10 20:47:50.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-10 20:47:50.000000 redfish_protocol_validator-1.1.6/redfish_protocol_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 20:47:50.439090 redfish_protocol_validator-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-02-10 20:47:38.000000 redfish_protocol_validator-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:41.953263 redfish_protocol_validator-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-16 20:11:41.953263 redfish_protocol_validator-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:41.953263 redfish_protocol_validator-1.1.7/redfish_protocol_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/console_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32037 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14056 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/protocol_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24902 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/redfish_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21012 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54306 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/security_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48774 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/service_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65115 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/service_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28978 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/service_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/system_under_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13570 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:41.953263 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-16 20:11:41.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-16 20:11:41.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:11:41.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 20:11:41.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 20:11:41.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-16 20:11:41.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:11:41.953263 redfish_protocol_validator-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/setup.py
```

### Comparing `redfish_protocol_validator-1.1.6/LICENSE.md` & `redfish_protocol_validator-1.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.1.6/PKG-INFO` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: redfish_protocol_validator
-Version: 1.1.6
+Name: redfish-protocol-validator
+Version: 1.1.7
 Summary: Redfish Protocol Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_protocol_validator-1.1.6/README.md` & `redfish_protocol_validator-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/accounts.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 import logging
 import random
 import string
 from urllib.parse import urlparse
 
 import requests
@@ -85,16 +85,29 @@
     while True:
         user = 'rfpv%04x' % random.randrange(2 ** 16)  # ex: 'rfpvc91c'
         if user not in existing_users:
             break
     return user
 
 
-def new_password(sut: SystemUnderTest, length=10, upper=1, lower=1,
-                 digits=1, symbols=0):
+def new_password(sut: SystemUnderTest, length=16, upper=1, lower=1,
+                 digits=1, symbols=1):
+    # Get the min and max password length and override 'length' if needed
+    # Use either limit if one is specified
+    response = sut.get_response('GET', sut.account_service_uri)
+    try:
+        if response.ok:
+            data = response.json()
+            if 'MinPasswordLength' in data and length < data['MinPasswordLength']:
+                length = data['MinPasswordLength']
+            elif 'MaxPasswordLength' in data and length > data['MaxPasswordLength']:
+                length = data['MaxPasswordLength']
+    except:
+        pass
+
     ascii_symbols = '_-.'
     pwd = random.sample(string.ascii_uppercase, upper)
     pwd.extend(random.sample(string.ascii_lowercase, lower))
     pwd.extend(random.sample(string.digits, digits))
     pwd.extend(random.sample(ascii_symbols, symbols))
     pwd.extend(random.sample(string.ascii_letters,
                              length - upper - lower - digits - symbols))
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/console_scripts.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/console_scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 import argparse
 import logging
 import sys
 from datetime import datetime
 from pathlib import Path
 
@@ -21,15 +21,15 @@
 from redfish_protocol_validator import service_requests
 from redfish_protocol_validator import service_responses
 from redfish_protocol_validator import sessions
 from redfish_protocol_validator import utils
 from redfish_protocol_validator.constants import Result
 from redfish_protocol_validator.system_under_test import SystemUnderTest
 
-tool_version = '1.1.6'
+tool_version = '1.1.7'
 
 
 def perform_tests(sut: SystemUnderTest):
     """Perform the protocol validation tests on the resources."""
     protocol_details.test_protocol_details(sut)
     service_requests.test_service_requests(sut)
     service_responses.test_service_responses(sut)
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/constants.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 from aenum import Enum, auto
 
 
 SSDP_ALL = 'ssdp:all'
 SSDP_REDFISH = 'urn:dmtf-org:service:redfish-rest:1'
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/protocol_details.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/protocol_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 import re
 import xml.etree.ElementTree as ET
 from urllib.parse import urlparse
 
 import requests
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/redfish_logo.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/redfish_logo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 """
 Redfish Logo
 
 File : redfish_logo.py
 
 Brief : This file contains the Base64 encoded image data for the Redfish Logo
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/report.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 import html as html_mod
 import json
 from datetime import datetime
 
 from redfish_protocol_validator import redfish_logo
 from redfish_protocol_validator.constants import Result
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/resources.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 import logging
 import random
 
 import requests
 
 from redfish_protocol_validator import accounts as acct
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/security_details.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/security_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 from base64 import b64decode
 import socket
 import ssl
 from urllib.parse import urlparse
 
 import requests
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/service_details.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/service_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 import json
 import time
 from urllib.parse import urlparse
 
 import requests
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/service_requests.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/service_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 import logging
 from urllib.parse import urlparse
 
 import requests
 
 from redfish_protocol_validator import utils
@@ -1134,35 +1134,60 @@
                 msg)
 
 
 def test_post_create_not_supported(sut: SystemUnderTest):
     """Perform tests for Assertion.REQ_POST_CREATE_NOT_SUPPORTED."""
     response = sut.get_response('POST', sut.accounts_uri)
     if response is None:
-        msg = ('Not response found for POST to Accounts URI; unable to test '
+        msg = ('No response found for POST to Accounts URI; unable to test '
                'this assertion')
         sut.log(Result.NOT_TESTED, 'POST', '', sut.accounts_uri,
                 Assertion.REQ_POST_CREATE_NOT_SUPPORTED, msg)
     elif response.ok:
         sut.log(Result.PASS, 'POST', response.status_code, sut.accounts_uri,
                 Assertion.REQ_POST_CREATE_NOT_SUPPORTED,
                 'Service supports creation of resources')
     elif response.status_code == requests.codes.METHOD_NOT_ALLOWED:
         sut.log(Result.PASS, 'POST', response.status_code, sut.accounts_uri,
                 Assertion.REQ_POST_CREATE_NOT_SUPPORTED,
                 'Test passed')
     else:
-        msg = ('POST request to URI %s failed with %s; expected %s; extended '
-               'error: %s' % (sut.accounts_uri, response.status_code,
-                              requests.codes.METHOD_NOT_ALLOWED,
-                              utils.get_extended_error(response)))
-        sut.log(Result.FAIL, 'POST', response.status_code, sut.accounts_uri,
-                Assertion.REQ_POST_CREATE_NOT_SUPPORTED,
-                msg)
-
+        try:
+            allow = sut.get_response('GET', sut.accounts_uri).headers.get('Allow')
+        except:
+            allow = None
+        if allow:
+            if 'POST' in allow.upper():
+                msg = ('POST request to URI %s failed with %s; extended '
+                       'error: %s; GET response contains an Allow header '
+                       'with POST specified' %
+                       (sut.accounts_uri, response.status_code,
+                        utils.get_extended_error(response)))
+                sut.log(Result.WARN, 'POST', response.status_code,
+                        sut.accounts_uri,
+                        Assertion.REQ_POST_CREATE_NOT_SUPPORTED, msg)
+            else:
+                msg = ('POST request to URI %s failed with %s; expected %s; '
+                       'extended error: %s' %
+                       (sut.accounts_uri, response.status_code,
+                        requests.codes.METHOD_NOT_ALLOWED,
+                        utils.get_extended_error(response)))
+                sut.log(Result.FAIL, 'POST', response.status_code,
+                        sut.accounts_uri,
+                        Assertion.REQ_POST_CREATE_NOT_SUPPORTED, msg)
+        else:
+            msg = ('POST request to URI %s failed with %s; expected %s; '
+                   'extended error: %s; GET response does not contain an '
+                   'Allow header to verify' %
+                   (sut.accounts_uri, response.status_code,
+                    requests.codes.METHOD_NOT_ALLOWED,
+                    utils.get_extended_error(response)))
+            sut.log(Result.WARN, 'POST', response.status_code,
+                    sut.accounts_uri, Assertion.REQ_POST_CREATE_NOT_SUPPORTED,
+                    msg)
 
 def test_post_create_not_idempotent(sut: SystemUnderTest):
     """Perform tests for Assertion.REQ_POST_CREATE_NOT_IDEMPOTENT."""
     uri = sut.sessions_uri
     payload = {
         'UserName': sut.username,
         'Password': sut.password
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/service_responses.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/service_responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 import io
 import xml.etree.ElementTree as ET
 
 import requests
 
 from redfish_protocol_validator import utils
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/sessions.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 import logging
 from urllib.parse import urlparse
 
 import requests
 
 from redfish_protocol_validator import accounts
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/system_under_test.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/system_under_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 import logging
 from urllib.parse import urlparse
 
 import requests
 
 from redfish_protocol_validator.utils import redfish_version_to_tuple
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator/utils.py` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 import http.client
 import io
 import logging
 import math
 import re
 import socket
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator.egg-info/PKG-INFO` & `redfish_protocol_validator-1.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: redfish-protocol-validator
-Version: 1.1.6
+Name: redfish_protocol_validator
+Version: 1.1.7
 Summary: Redfish Protocol Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_protocol_validator-1.1.6/redfish_protocol_validator.egg-info/SOURCES.txt` & `redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.1.6/setup.py` & `redfish_protocol_validator-1.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Copyright Notice:
 # Copyright 2020-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/Redfish-Protocol-Validator/blob/master/LICENSE.md
+# https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 from setuptools import setup
 from codecs import open
 
 with open("README.md", "r", "utf-8") as f:
     long_description = f.read()
 
 setup(
     name="redfish_protocol_validator",
-    version="1.1.6",
+    version="1.1.7",
     description="Redfish Protocol Validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DMTF, https://www.dmtf.org/standards/feedback",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
@@ -26,9 +26,9 @@
     keywords="Redfish",
     url="https://github.com/DMTF/Redfish-Protocol-Validator",
     packages=["redfish_protocol_validator"],
     entry_points={
         'console_scripts': ['rf_protocol_validator=redfish_protocol_validator.console_scripts:main']
     },
     install_requires=["aenum", "colorama", "pyasn1", "pyasn1-modules",
-                      "requests>=2.23.0", "sseclient-py", "urllib3"]
+                      "requests>=2.23.0", "sseclient-py", "urllib3<2"]
 )
```

