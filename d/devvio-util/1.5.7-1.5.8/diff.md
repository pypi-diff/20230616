# Comparing `tmp/devvio_util-1.5.7.tar.gz` & `tmp/devvio_util-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvio_util-1.5.7.tar", last modified: Fri Jun 16 01:42:27 2023, max compression
+gzip compressed data, was "devvio_util-1.5.8.tar", last modified: Fri Jun 16 03:39:17 2023, max compression
```

## Comparing `devvio_util-1.5.7.tar` & `devvio_util-1.5.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:27.307435 devvio_util-1.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-16 01:42:27.307435 devvio_util-1.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:19.000000 devvio_util-1.5.7/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:27.303435 devvio_util-1.5.7/devvio_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/lib_creds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:27.307435 devvio_util-1.5.7/devvio_util/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/address.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/atomic_transaction_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/chainstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/devv_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/devv_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/final_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/smart_coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/psql_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:27.303435 devvio_util-1.5.7/devvio_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-16 01:42:27.000000 devvio_util-1.5.7/devvio_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-16 01:42:27.000000 devvio_util-1.5.7/devvio_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:42:27.000000 devvio_util-1.5.7/devvio_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:42:27.000000 devvio_util-1.5.7/devvio_util.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 01:42:27.000000 devvio_util-1.5.7/devvio_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 01:42:27.000000 devvio_util-1.5.7/devvio_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 01:42:27.307435 devvio_util-1.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-16 01:42:19.000000 devvio_util-1.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:17.008532 devvio_util-1.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-16 03:39:17.008532 devvio_util-1.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:09.000000 devvio_util-1.5.8/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:17.000532 devvio_util-1.5.8/devvio_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/lib_creds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:17.008532 devvio_util-1.5.8/devvio_util/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/atomic_transaction_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/chainstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/devv_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/devv_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/final_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/smart_coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/psql_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:17.004532 devvio_util-1.5.8/devvio_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-16 03:39:16.000000 devvio_util-1.5.8/devvio_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-16 03:39:16.000000 devvio_util-1.5.8/devvio_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:39:16.000000 devvio_util-1.5.8/devvio_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:39:16.000000 devvio_util-1.5.8/devvio_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 03:39:16.000000 devvio_util-1.5.8/devvio_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 03:39:16.000000 devvio_util-1.5.8/devvio_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 03:39:17.008532 devvio_util-1.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-16 03:39:09.000000 devvio_util-1.5.8/setup.py
```

### Comparing `devvio_util-1.5.7/devvio_util/config.py` & `devvio_util-1.5.8/devvio_util/config.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util/lib_creds.py` & `devvio_util-1.5.8/devvio_util/lib_creds.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util/primitives/address.py` & `devvio_util-1.5.8/devvio_util/primitives/address.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util/primitives/chainstate.py` & `devvio_util-1.5.8/devvio_util/primitives/chainstate.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util/primitives/devv_constants.py` & `devvio_util-1.5.8/devvio_util/primitives/devv_constants.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util/primitives/devv_sign.py` & `devvio_util-1.5.8/devvio_util/primitives/devv_sign.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util/primitives/final_block.py` & `devvio_util-1.5.8/devvio_util/primitives/final_block.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util/primitives/signature.py` & `devvio_util-1.5.8/devvio_util/primitives/signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             return self._canonical[1:]
         return self._canonical
 
     # return hex representation (without prefix)
     def get_hex_str(self) -> str:
         if not self._canonical:
             raise Exception('Signature is not initialized!')
-        return self._canonical.hex()[2:].upper()
+        return self._canonical.hex().upper()
 
     def is_wallet_sig(self) -> bool:
         if not self.__bool__():
             return False
         return self._size == kWALLET_SIG_SIZE
 
     def is_node_sig(self) -> bool:
```

### Comparing `devvio_util-1.5.7/devvio_util/primitives/smart_coin.py` & `devvio_util-1.5.8/devvio_util/primitives/smart_coin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util/primitives/summary.py` & `devvio_util-1.5.8/devvio_util/primitives/summary.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util/primitives/transaction.py` & `devvio_util-1.5.8/devvio_util/primitives/transaction.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util/primitives/transfer.py` & `devvio_util-1.5.8/devvio_util/primitives/transfer.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util/primitives/utils.py` & `devvio_util-1.5.8/devvio_util/primitives/utils.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util/primitives/validation.py` & `devvio_util-1.5.8/devvio_util/primitives/validation.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util/psql_mixin.py` & `devvio_util-1.5.8/devvio_util/psql_mixin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/devvio_util.egg-info/SOURCES.txt` & `devvio_util-1.5.8/devvio_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.7/setup.py` & `devvio_util-1.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='devvio_util',
-      version='1.5.7',
+      version='1.5.8',
       long_description=open('README.txt').read(),
       long_description_content_type='text/markdown',
       description='Utility to be used inside Devvio projects',
       author='Devvio Team',
       author_email='support@devv.io',
       license='Devvio',
       packages=['devvio_util', 'devvio_util/primitives'],
```

