# Comparing `tmp/funga-eth-0.7.2.tar.gz` & `tmp/funga-eth-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funga-eth-0.7.2.tar", last modified: Sat Jun 10 08:13:57 2023, max compression
+gzip compressed data, was "funga-eth-0.7.3.tar", last modified: Fri Jun 16 14:40:05 2023, max compression
```

## Comparing `funga-eth-0.7.2.tar` & `funga-eth-0.7.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-10 08:13:57.479992 funga-eth-0.7.2/
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:49:56.000000 funga-eth-0.7.2/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       82 2023-06-03 12:07:27.000000 funga-eth-0.7.2/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)     2008 2023-06-10 08:13:57.479992 funga-eth-0.7.2/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1322 2023-06-03 12:11:27.000000 funga-eth-0.7.2/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 07:51:12.000000 funga-eth-0.7.2/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1630 2022-11-14 07:51:25.000000 funga-eth-0.7.2/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-10 08:13:57.469992 funga-eth-0.7.2/funga/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-10 08:13:57.473325 funga-eth-0.7.2/funga/eth/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:17:05.000000 funga-eth-0.7.2/funga/eth/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-10 08:13:57.473325 funga-eth-0.7.2/funga/eth/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:17:05.000000 funga-eth-0.7.2/funga/eth/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3564 2021-10-10 10:17:05.000000 funga-eth-0.7.2/funga/eth/cli/handle.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2298 2021-10-15 20:57:44.000000 funga-eth-0.7.2/funga/eth/cli/http.py
--rw-r--r--   0 lash      (1000) lash      (1000)      556 2021-10-10 10:17:05.000000 funga-eth-0.7.2/funga/eth/cli/jsonrpc.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1546 2021-10-15 20:39:41.000000 funga-eth-0.7.2/funga/eth/cli/socket.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-10 08:13:57.469992 funga-eth-0.7.2/funga/eth/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-10 08:13:57.473325 funga-eth-0.7.2/funga/eth/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)       76 2021-10-10 10:17:05.000000 funga-eth-0.7.2/funga/eth/data/config/database.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       82 2021-10-10 10:17:05.000000 funga-eth-0.7.2/funga/eth/data/config/signer.ini
--rw-r--r--   0 lash      (1000) lash      (1000)     2479 2022-10-13 07:37:03.000000 funga-eth-0.7.2/funga/eth/encoding.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-10 08:13:57.476658 funga-eth-0.7.2/funga/eth/keystore/
--rw-r--r--   0 lash      (1000) lash      (1000)      209 2021-10-10 10:17:05.000000 funga-eth-0.7.2/funga/eth/keystore/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1143 2021-10-10 11:04:50.000000 funga-eth-0.7.2/funga/eth/keystore/dict.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1560 2022-01-24 11:37:10.000000 funga-eth-0.7.2/funga/eth/keystore/interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5335 2022-01-25 09:02:00.000000 funga-eth-0.7.2/funga/eth/keystore/keyfile.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3659 2021-10-30 06:00:33.000000 funga-eth-0.7.2/funga/eth/keystore/sql.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1107 2023-03-29 14:12:40.000000 funga-eth-0.7.2/funga/eth/message.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-10 08:13:57.476658 funga-eth-0.7.2/funga/eth/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     2978 2022-12-16 11:44:47.000000 funga-eth-0.7.2/funga/eth/runnable/keyfile.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2104 2023-03-27 13:56:19.000000 funga-eth-0.7.2/funga/eth/runnable/msg.py
--rwxr-xr-x   0 lash      (1000) lash      (1000)     4308 2023-06-03 12:25:41.000000 funga-eth-0.7.2/funga/eth/runnable/signer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-10 08:13:57.476658 funga-eth-0.7.2/funga/eth/signer/
--rw-r--r--   0 lash      (1000) lash      (1000)       56 2023-03-13 16:41:32.000000 funga-eth-0.7.2/funga/eth/signer/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3210 2023-03-28 15:47:47.000000 funga-eth-0.7.2/funga/eth/signer/defaultsigner.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4693 2021-10-15 20:59:28.000000 funga-eth-0.7.2/funga/eth/transaction.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-10 08:13:57.476658 funga-eth-0.7.2/funga_eth.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)     2008 2023-06-10 08:13:57.000000 funga-eth-0.7.2/funga_eth.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1006 2023-06-10 08:13:57.000000 funga-eth-0.7.2/funga_eth.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-10 08:13:57.000000 funga-eth-0.7.2/funga_eth.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      151 2023-06-10 08:13:57.000000 funga-eth-0.7.2/funga_eth.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      192 2023-06-10 08:13:57.000000 funga-eth-0.7.2/funga_eth.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        6 2023-06-10 08:13:57.000000 funga-eth-0.7.2/funga_eth.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      162 2023-06-10 08:12:46.000000 funga-eth-0.7.2/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      399 2023-06-10 08:13:57.479992 funga-eth-0.7.2/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)     1625 2023-06-10 08:13:15.000000 funga-eth-0.7.2/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       35 2021-10-10 16:05:05.000000 funga-eth-0.7.2/sql_requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 16:05:05.000000 funga-eth-0.7.2/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-10 08:13:57.479992 funga-eth-0.7.2/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     3477 2022-01-25 09:02:00.000000 funga-eth-0.7.2/tests/test_cli.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1519 2021-10-10 10:17:05.000000 funga-eth-0.7.2/tests/test_keystore_dict.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1537 2022-01-25 09:02:00.000000 funga-eth-0.7.2/tests/test_pbkdf2.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2855 2021-10-10 10:17:05.000000 funga-eth-0.7.2/tests/test_sign.py
--rw-r--r--   0 lash      (1000) lash      (1000)      268 2021-10-10 10:17:05.000000 funga-eth-0.7.2/tests/test_socket.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-16 14:40:05.303294 funga-eth-0.7.3/
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:49:56.000000 funga-eth-0.7.3/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       82 2023-06-03 12:07:27.000000 funga-eth-0.7.3/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)     2008 2023-06-16 14:40:05.303294 funga-eth-0.7.3/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1322 2023-06-03 12:11:27.000000 funga-eth-0.7.3/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 07:51:12.000000 funga-eth-0.7.3/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1630 2022-11-14 07:51:25.000000 funga-eth-0.7.3/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-16 14:40:05.296627 funga-eth-0.7.3/funga/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-16 14:40:05.299960 funga-eth-0.7.3/funga/eth/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:17:05.000000 funga-eth-0.7.3/funga/eth/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-16 14:40:05.299960 funga-eth-0.7.3/funga/eth/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:17:05.000000 funga-eth-0.7.3/funga/eth/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3564 2021-10-10 10:17:05.000000 funga-eth-0.7.3/funga/eth/cli/handle.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2298 2021-10-15 20:57:44.000000 funga-eth-0.7.3/funga/eth/cli/http.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      556 2021-10-10 10:17:05.000000 funga-eth-0.7.3/funga/eth/cli/jsonrpc.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1546 2021-10-15 20:39:41.000000 funga-eth-0.7.3/funga/eth/cli/socket.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-16 14:40:05.296627 funga-eth-0.7.3/funga/eth/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-16 14:40:05.299960 funga-eth-0.7.3/funga/eth/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)       76 2021-10-10 10:17:05.000000 funga-eth-0.7.3/funga/eth/data/config/database.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       82 2021-10-10 10:17:05.000000 funga-eth-0.7.3/funga/eth/data/config/signer.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)     2691 2023-06-16 14:38:42.000000 funga-eth-0.7.3/funga/eth/encoding.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-16 14:40:05.299960 funga-eth-0.7.3/funga/eth/keystore/
+-rw-r--r--   0 lash      (1000) lash      (1000)      209 2021-10-10 10:17:05.000000 funga-eth-0.7.3/funga/eth/keystore/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1143 2021-10-10 11:04:50.000000 funga-eth-0.7.3/funga/eth/keystore/dict.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1560 2022-01-24 11:37:10.000000 funga-eth-0.7.3/funga/eth/keystore/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5335 2022-01-25 09:02:00.000000 funga-eth-0.7.3/funga/eth/keystore/keyfile.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3659 2021-10-30 06:00:33.000000 funga-eth-0.7.3/funga/eth/keystore/sql.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1313 2023-06-16 14:12:48.000000 funga-eth-0.7.3/funga/eth/message.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-16 14:40:05.299960 funga-eth-0.7.3/funga/eth/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3258 2023-06-16 14:36:05.000000 funga-eth-0.7.3/funga/eth/runnable/keyfile.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2104 2023-03-27 13:56:19.000000 funga-eth-0.7.3/funga/eth/runnable/msg.py
+-rwxr-xr-x   0 lash      (1000) lash      (1000)     4308 2023-06-03 12:25:41.000000 funga-eth-0.7.3/funga/eth/runnable/signer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-16 14:40:05.303294 funga-eth-0.7.3/funga/eth/signer/
+-rw-r--r--   0 lash      (1000) lash      (1000)       56 2023-03-13 16:41:32.000000 funga-eth-0.7.3/funga/eth/signer/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3210 2023-03-28 15:47:47.000000 funga-eth-0.7.3/funga/eth/signer/defaultsigner.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4693 2021-10-15 20:59:28.000000 funga-eth-0.7.3/funga/eth/transaction.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-16 14:40:05.303294 funga-eth-0.7.3/funga_eth.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2008 2023-06-16 14:40:05.000000 funga-eth-0.7.3/funga_eth.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1006 2023-06-16 14:40:05.000000 funga-eth-0.7.3/funga_eth.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-16 14:40:05.000000 funga-eth-0.7.3/funga_eth.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      151 2023-06-16 14:40:05.000000 funga-eth-0.7.3/funga_eth.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      192 2023-06-16 14:40:05.000000 funga-eth-0.7.3/funga_eth.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        6 2023-06-16 14:40:05.000000 funga-eth-0.7.3/funga_eth.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      162 2023-06-10 08:12:46.000000 funga-eth-0.7.3/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      399 2023-06-16 14:40:05.303294 funga-eth-0.7.3/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)     1625 2023-06-16 14:36:37.000000 funga-eth-0.7.3/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       35 2021-10-10 16:05:05.000000 funga-eth-0.7.3/sql_requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 16:05:05.000000 funga-eth-0.7.3/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-16 14:40:05.303294 funga-eth-0.7.3/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3477 2022-01-25 09:02:00.000000 funga-eth-0.7.3/tests/test_cli.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1519 2021-10-10 10:17:05.000000 funga-eth-0.7.3/tests/test_keystore_dict.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1537 2022-01-25 09:02:00.000000 funga-eth-0.7.3/tests/test_pbkdf2.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2855 2021-10-10 10:17:05.000000 funga-eth-0.7.3/tests/test_sign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      268 2021-10-10 10:17:05.000000 funga-eth-0.7.3/tests/test_socket.py
```

### Comparing `funga-eth-0.7.2/LICENSE` & `funga-eth-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/PKG-INFO` & `funga-eth-0.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funga-eth
-Version: 0.7.2
+Version: 0.7.3
 Summary: Ethereum implementation of the funga keystore and signer
 Home-page: https://git.defalsify.org/funga-eth
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `funga-eth-0.7.2/README.md` & `funga-eth-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/WAIVER` & `funga-eth-0.7.3/WAIVER`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/WAIVER.asc` & `funga-eth-0.7.3/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/funga/eth/cli/handle.py` & `funga-eth-0.7.3/funga/eth/cli/handle.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/funga/eth/cli/http.py` & `funga-eth-0.7.3/funga/eth/cli/http.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/funga/eth/cli/jsonrpc.py` & `funga-eth-0.7.3/funga/eth/cli/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/funga/eth/cli/socket.py` & `funga-eth-0.7.3/funga/eth/cli/socket.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/funga/eth/encoding.py` & `funga-eth-0.7.3/funga/eth/encoding.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,22 @@
 
 def private_key_to_address(pk, result_format='hex'):
     pubk = coincurve.PublicKey.from_secret(pk.secret)
     #logg.debug('secret {} '.format(pk.secret.hex()))
     return public_key_to_address(pubk, result_format)
 
 
+def private_key_to_public_key(pk, result_format='hex'):
+    pubk = coincurve.PublicKey.from_secret(pk.secret)
+    r = pubk.format(compressed=False)
+    if result_format=='hex':
+        r = r.hex()
+    return r
+
+
 def is_address(address_hex):
     try:
         address_hex = strip_0x(address_hex, pad=False)
     except ValueError:
         return False
     return len(address_hex) == 40
```

### Comparing `funga-eth-0.7.2/funga/eth/keystore/dict.py` & `funga-eth-0.7.3/funga/eth/keystore/dict.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/funga/eth/keystore/interface.py` & `funga-eth-0.7.3/funga/eth/keystore/interface.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/funga/eth/keystore/keyfile.py` & `funga-eth-0.7.3/funga/eth/keystore/keyfile.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/funga/eth/keystore/sql.py` & `funga-eth-0.7.3/funga/eth/keystore/sql.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/funga/eth/runnable/keyfile.py` & `funga-eth-0.7.3/funga/eth/runnable/keyfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,28 +17,30 @@
         from_file,
         to_dict,
         )
 
 
 from funga.eth.encoding import (
         private_key_to_address,
+        private_key_to_public_key,
         private_key_from_bytes,
         )
 
 
 logging.basicConfig(level=logging.WARNING)
 logg = logging.getLogger()
 
 argparser = argparse.ArgumentParser()
 argparser.add_argument('-d', '--decrypt', dest='d', type=str, help='decrypt file')
 argparser.add_argument('--private-key', dest='private_key', action='store_true', help='output private key instead of address')
 argparser.add_argument('--passphrase-file', dest='passphrase_file', type=str, help='Keystore file to use for signing or address')
 argparser.add_argument('-0', dest='nonl', action='store_true', help='no newline at end of output')
 argparser.add_argument('-z', action='store_true', help='zero-length password')
-argparser.add_argument('-k', type=str, help='load key from file')
+argparser.add_argument('-k', type=str, help='load private key from file')
+argparser.add_argument('-p', '--public-key', dest='p', action='store_true', help='return public key instead of address')
 argparser.add_argument('-v', action='store_true', help='be verbose')
 args = argparser.parse_args()
 
 if args.v:
     logg.setLevel(logging.DEBUG)
 
 mode = 'create'
@@ -78,15 +80,19 @@
         try:
             r = from_file(args.d, passphrase).hex()
         except DecryptError:
             sys.stderr.write('Invalid passphrase\n')
             sys.exit(1)
         if not secret:
             pk = private_key_from_bytes(bytes.fromhex(r))
-            r = private_key_to_address(pk)
+            r = None
+            if args.p:
+                r = private_key_to_public_key(pk)
+            else:
+                r = private_key_to_address(pk)
     elif mode == 'create':
         if passphrase == None:
             passphrase = getpass.getpass('encryption phrase: ')
         pk_bytes = None
         if pk_hex != None:
             pk_hex = strip_0x(pk_hex)
             pk_bytes = bytes.fromhex(pk_hex)
```

### Comparing `funga-eth-0.7.2/funga/eth/runnable/msg.py` & `funga-eth-0.7.3/funga/eth/runnable/msg.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/funga/eth/runnable/signer.py` & `funga-eth-0.7.3/funga/eth/runnable/signer.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/funga/eth/signer/defaultsigner.py` & `funga-eth-0.7.3/funga/eth/signer/defaultsigner.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/funga/eth/transaction.py` & `funga-eth-0.7.3/funga/eth/transaction.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/funga_eth.egg-info/PKG-INFO` & `funga-eth-0.7.3/funga_eth.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funga-eth
-Version: 0.7.2
+Version: 0.7.3
 Summary: Ethereum implementation of the funga keystore and signer
 Home-page: https://git.defalsify.org/funga-eth
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `funga-eth-0.7.2/funga_eth.egg-info/SOURCES.txt` & `funga-eth-0.7.3/funga_eth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/setup.py` & `funga-eth-0.7.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 f = open('README.md', 'r')
 description = f.read()
 f.close()
 
 setup(
         name="funga-eth",
-        version="0.7.2",
+        version="0.7.3",
         description="Ethereum implementation of the funga keystore and signer",
         author="Louis Holbrook",
         author_email="dev@holbrook.no",
         packages=[
             'funga.eth.signer',
             'funga.eth',
             'funga.eth.cli',
```

### Comparing `funga-eth-0.7.2/tests/test_cli.py` & `funga-eth-0.7.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/tests/test_keystore_dict.py` & `funga-eth-0.7.3/tests/test_keystore_dict.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/tests/test_pbkdf2.py` & `funga-eth-0.7.3/tests/test_pbkdf2.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.7.2/tests/test_sign.py` & `funga-eth-0.7.3/tests/test_sign.py`

 * *Files identical despite different names*

