# Comparing `tmp/devvio_util-1.5.6.tar.gz` & `tmp/devvio_util-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvio_util-1.5.6.tar", last modified: Wed Jun 14 03:10:43 2023, max compression
+gzip compressed data, was "devvio_util-1.5.7.tar", last modified: Fri Jun 16 01:42:27 2023, max compression
```

## Comparing `devvio_util-1.5.6.tar` & `devvio_util-1.5.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:43.391799 devvio_util-1.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 03:10:43.391799 devvio_util-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:35.000000 devvio_util-1.5.6/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:43.391799 devvio_util-1.5.6/devvio_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/lib_creds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:43.391799 devvio_util-1.5.6/devvio_util/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/address.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/atomic_transaction_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/chainstate.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/devv_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/devv_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/final_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/smart_coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/psql_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:43.391799 devvio_util-1.5.6/devvio_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 03:10:43.000000 devvio_util-1.5.6/devvio_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-14 03:10:43.000000 devvio_util-1.5.6/devvio_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:10:43.000000 devvio_util-1.5.6/devvio_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:10:43.000000 devvio_util-1.5.6/devvio_util.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 03:10:43.000000 devvio_util-1.5.6/devvio_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 03:10:43.000000 devvio_util-1.5.6/devvio_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 03:10:43.395799 devvio_util-1.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-14 03:10:35.000000 devvio_util-1.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:27.307435 devvio_util-1.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-16 01:42:27.307435 devvio_util-1.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:19.000000 devvio_util-1.5.7/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:27.303435 devvio_util-1.5.7/devvio_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/lib_creds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:27.307435 devvio_util-1.5.7/devvio_util/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/atomic_transaction_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/chainstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/devv_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/devv_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/final_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/smart_coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/primitives/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-16 01:42:19.000000 devvio_util-1.5.7/devvio_util/psql_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:42:27.303435 devvio_util-1.5.7/devvio_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-16 01:42:27.000000 devvio_util-1.5.7/devvio_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-16 01:42:27.000000 devvio_util-1.5.7/devvio_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:42:27.000000 devvio_util-1.5.7/devvio_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:42:27.000000 devvio_util-1.5.7/devvio_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 01:42:27.000000 devvio_util-1.5.7/devvio_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 01:42:27.000000 devvio_util-1.5.7/devvio_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 01:42:27.307435 devvio_util-1.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-16 01:42:19.000000 devvio_util-1.5.7/setup.py
```

### Comparing `devvio_util-1.5.6/devvio_util/config.py` & `devvio_util-1.5.7/devvio_util/config.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.6/devvio_util/lib_creds.py` & `devvio_util-1.5.7/devvio_util/lib_creds.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.6/devvio_util/primitives/address.py` & `devvio_util-1.5.7/devvio_util/primitives/address.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.6/devvio_util/primitives/chainstate.py` & `devvio_util-1.5.7/devvio_util/primitives/chainstate.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.6/devvio_util/primitives/devv_constants.py` & `devvio_util-1.5.7/devvio_util/primitives/devv_constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 kENVELOPE_SIZE = 34
 kLEGACY_ENVELOPE_SIZE = 17
 kSIGNER_LENGTH_OFFSET = 34
 kMIN_PAYLOAD_SIZE = 8
 kFLAGS_OFFSET = 24
 kOPERATION_OFFSET = 25
 kLEGACY_OPERATION_OFFSET = 16
+kTIMESTAMP_OFFSET = 26
 
 kTRANSFER_NONADDR_DATA_SIZE = kUINT64_SIZE*3
 kMERKLE_SIZE = 32
 kPREV_HASH_SIZE = 32
 
 kPEM_PREFIX = '-----BEGIN ENCRYPTED PRIVATE KEY-----\n'
 kPEM_SUFFIX = '\n-----END ENCRYPTED PRIVATE KEY-----'
@@ -40,7 +41,13 @@
     SEND = 2
     DELETE = 3
     REVERT = 4
     CONFIRM = 5
     SUMMARIZE = 6
     RECOVER = 7
     NUM_OPS = 8
+
+    def get(self, op: str) -> int:
+        try:
+            return self.__getattribute__(op)
+        except Exception as e:
+            raise Exception(f"Invalid op string {op}")
```

### Comparing `devvio_util-1.5.6/devvio_util/primitives/devv_sign.py` & `devvio_util-1.5.7/devvio_util/primitives/devv_sign.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,26 @@
 from devvio_util.primitives.signature import Signature
 from devvio_util.primitives.address import Address
 from devvio_util.primitives.devv_constants import \
     kWALLET_ADDR_SIZE, kNODE_ADDR_SIZE, kNODE_SIG_SIZE, kWALLET_SIG_SIZE, \
     kPEM_PREFIX, kPEM_SUFFIX, kPEM_PREFIX_SIZE, kPEM_SUFFIX_SIZE
 from devvio_util.primitives.utils import set_uint8
 
-from hashlib import sha256
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.backends.openssl import backend
 from cryptography.hazmat.primitives import serialization as sz
 from cryptography.hazmat.primitives.hashes import SHA256
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.exceptions import InvalidSignature
 import pkg_resources
 
 kWALLET_CURVE = ec.SECP256K1()
 kNODE_CURVE = ec.SECP384R1()
 
 
-class DevvHash:
-    """ Holds a sha256 hash of the given binary data"""
-    def __init__(self, raw_bin: bytes):
-        """ Initialize DevvHash with the sha256 hash of the given data
-        :param raw_bin: binary data to hash
-        :type raw_bin: bytes
-        """
-        self._hash = None
-        if not isinstance(raw_bin, bytes):
-            raise Exception(f'Failed to hash {type(raw_bin)} (expected bytes)')
-        if raw_bin:
-            self._hash = sha256(raw_bin).digest()
-
-    def get_bin(self) -> bytes:
-        """ Return the sha256 hash as a bytes object
-        :return: hashed data binary
-        :rtype: bytes
-        """
-        return self._hash if self._hash else b''
-
-    def get_hex(self) -> str:
-        """ Return the sha256 hash as a hex string
-        :return: hexdigest of the hashed data
-        :rtype: str
-        """
-        return self._hash.hex() if self._hash else ''
-
-
 def crypto_sanity_check(pkey: str = None, pub: str or Address = None, aes_pass: str = None) -> tuple:
     """ Tests the cryptographic methods in this devv_sign module. Can be used to validate a given keypair and aes key,
     otherwise will generate a test key
 
     :param pkey: str of private key, without PEM prefix/suffix or newlines
     :type pkey: str
     :param pub: public key as a hex string or devvio-util Address object
@@ -62,61 +33,60 @@
     """
     if not aes_pass:
         aes_pass = 'password'
     if not pkey:
         ec_key = EcSigner(aes_pass=aes_pass)
         pub = ec_key.get_signer_addr()
         pkey = ec_key.get_pkey()
-    msg = DevvHash(b'Testing')
+    msg = b'Testing'
     sign_binary(pkey, pub, msg, aes_pass)
     crypto_version = str(pkg_resources.get_distribution('cryptography'))
     openssl_version = backend.openssl_version_text()
     return openssl_version, crypto_version
 
 
-def sign_binary(pkey: str, pub: str or Address, msg: DevvHash, aes_pass: str) -> Signature:
-    """ Signs the given DevvHash using the given keypair and aes key, and validates the signature
+def format_pkey(pkey: str) -> bytes:
+    return bytes(kPEM_PREFIX + pkey + kPEM_SUFFIX, 'utf-8')
+
+
+def sign_binary(pkey: str, pub: str or Address, msg: bytes, aes_pass: str) -> Signature:
+    """ Signs the given msg binary using the given keypair and aes key, and validates the signature
 
     :param pkey: str of private key, without PEM prefix/suffix or newlines
     :type pkey: str
     :param pub: public key as a hex string or devvio-util Address object
     :type pub: str
     :param msg: contains the hashed binary to be signed
-    :type msg: DevvHash
+    :type msg: bytes
     :param aes_pass: aes key to decrypt/encrypt the pkey with; this is required
     :type aes_pass: str
-    :return: a new signature for the given DevvHash object
+    :return: a new signature for the given bytes object
     :rtype: Signature
     """
     try:
-        temp = msg.get_bin()
-
-        pkey_bin = bytes(kPEM_PREFIX + pkey + kPEM_SUFFIX, 'utf-8')
+        pkey_bin = format_pkey(pkey)
         signer = EcSigner(pkey=pkey_bin,
                           pub=pub, aes_pass=aes_pass)
 
-        sig = signer.sign(temp)
+        sig = signer.sign(msg)
         sig_size = len(sig)
 
         if sig_size < 80:
             pad_len = kWALLET_SIG_SIZE
         else:
             pad_len = kNODE_SIG_SIZE
 
         if sig_size < pad_len:
             padding = b''
             for i in range(pad_len - sig_size):
                 padding += set_uint8(0)
             sig += padding
         elif sig_size > pad_len:
             sig = sig[:pad_len]
-        sig_size = pad_len
 
-        if not Signature.is_valid_sig_size(sig_size):
-            raise ValueError(f"Invalid signature size ({sig_size})")
         sig = Signature(sig)
 
         return sig
     except Exception as e:
         raise RuntimeError(f"Signature procedure failed ({e})")
```

### Comparing `devvio_util-1.5.6/devvio_util/primitives/final_block.py` & `devvio_util-1.5.7/devvio_util/primitives/final_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,22 +42,22 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self._canonical:
             self._canonical.__exit__()
 
     def get_indexes(self, buffer: InputBuffer):
         version_ = buffer.get_next_uint8()
         if not version_:
-            raise Exception("Invalid serialized FinalBlock, buffer empty!")
+            raise Exception("Invalid FinalBlock: buffer empty!")
 
         if version_ > 1:
-            raise Exception(f"Invalid FinalBlock.version: {version_}")
+            raise Exception(f"Invalid FinalBlock: bad {version_}")
 
         num_bytes_ = buffer.get_next_uint64()
         if not num_bytes_:
-            raise Exception("Invalid serialized FinalBlock, wrong size!")
+            raise Exception("Invalid FinalBlock: wrong size!")
 
         if not self._is_legacy:
             self._shard_index = buffer.get_next_uint64()
             self._block_height = buffer.get_next_uint64()
 
         self._block_time = buffer.get_next_uint64()
         self._prev_hash = buffer.get_next_prev_hash()
```

### Comparing `devvio_util-1.5.6/devvio_util/primitives/signature.py` & `devvio_util-1.5.7/devvio_util/primitives/signature.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.6/devvio_util/primitives/smart_coin.py` & `devvio_util-1.5.7/devvio_util/primitives/smart_coin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.6/devvio_util/primitives/summary.py` & `devvio_util-1.5.7/devvio_util/primitives/summary.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.6/devvio_util/primitives/transaction.py` & `devvio_util-1.5.7/devvio_util/primitives/transaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from devvio_util.primitives.address import Address
 from devvio_util.primitives.signature import Signature
-from devvio_util.primitives.utils import InputBuffer, set_uint64, set_uint8
-from devvio_util.primitives.devv_sign import sign_binary, DevvHash
+from devvio_util.primitives.utils import InputBuffer, set_uint64, set_uint8, get_int
+from devvio_util.primitives.devv_sign import sign_binary
 from devvio_util.primitives.transfer import Transfer
 from devvio_util.primitives.devv_constants import kLEGACY_ENVELOPE_SIZE, kNODE_SIG_BUF_SIZE, kNODE_ADDR_BUF_SIZE, \
     kSIGNER_LENGTH_OFFSET, kUINT_SIZE, kMIN_PAYLOAD_SIZE, kFLAGS_OFFSET, kOPERATION_OFFSET, kLEGACY_OPERATION_OFFSET, \
-    kENVELOPE_SIZE, OpType
+    kENVELOPE_SIZE, kTIMESTAMP_OFFSET, OpType
 
 
 class Transaction:
     """
     Holds a collection of Transfers and their corresponding signature.
 
     Note: serialization of legacy blocks not currently implemented
@@ -93,21 +93,36 @@
         else:
             offset = kENVELOPE_SIZE + self._payload_size + self._xfer_size + self._signer_size
         raw_sig = self._canonical[offset:]
         if not raw_sig:
             return None
         return Signature(raw_sig)
 
+    def get_op(self) -> int:
+        return self._canonical[kOPERATION_OFFSET] if not self._is_legacy else self._canonical[kLEGACY_OPERATION_OFFSET]
+
+    def get_flags(self) -> int:
+        return self._canonical[kFLAGS_OFFSET] if not self._is_legacy else None
+
+    def get_timestamp(self) -> int:
+        return get_int(self._canonical[kTIMESTAMP_OFFSET:kTIMESTAMP_OFFSET + 8], False)
+
     def get_payload(self) -> str:
         if self._is_legacy:
             offset = kNODE_ADDR_BUF_SIZE + self._xfer_size + self._signer_size
         else:
             offset = kENVELOPE_SIZE + self._xfer_size + self._signer_size
         return self.get_canonical()[offset:offset + self._payload_size].decode('utf-8')
 
+    def __len__(self):
+        return self.get_size()
+
+    def get_size(self) -> int:
+        return self._tx_size
+
     def get_canonical(self) -> bytes:
         return self._canonical
 
     def get_hex_str(self) -> str or None:
         if not self._canonical:
             return None
         return self._canonical.hex()
@@ -156,58 +171,69 @@
 
         if self._payload_size < kMIN_PAYLOAD_SIZE:
             raise ValueError(f"Failed to serialize transaction, payload too small ({self._payload_size})")
 
         self._canonical = bytes()
         self._canonical += set_uint64(self._payload_size)
 
-        if oper >= OpType.NUM_OPS:
-            raise ValueError(f"Invalid Transaction: bad OpType ({oper} >= {OpType.NUM_OPS})")
-        self._canonical += set_uint8(oper)
         if flags != 0:
             raise ValueError("Invalid Transaction: unknown flags")
         self._canonical += set_uint8(flags)
+        if oper >= OpType.NUM_OPS:
+            raise ValueError(f"Invalid Transaction: bad OpType ({oper} >= {OpType.NUM_OPS})")
+        self._canonical += set_uint8(oper)
         self._canonical += set_uint64(timestamp)
         self._canonical += signer.get_canonical()
 
         self._xfer_size = 0
         for xfer in xfers:
-            self._xfer_size += xfer.get_size()
+            self._xfer_size += xfer.get_size() + 1
             self._canonical += xfer.get_canonical()
 
-        self._signer_size = signer.get_size()
+        self._signer_size = signer.get_size() + 1
         self._tx_size = kENVELOPE_SIZE + self._signer_size + self._xfer_size + self._payload_size \
                         + signer.get_corresponding_sig_size()
 
         self._canonical = set_uint64(self._tx_size) + set_uint64(self._xfer_size) + self._canonical
 
-    def serialize(self, oper: int, xfers: list, payload: str, flags: int,
+    def serialize(self, oper: int, xfers: list, payload: bytes, flags: int,
                   timestamp: int, sig: Signature = None, is_legacy: bool = False):
         """
         Initialize Transaction attributes and generate canonical form.
 
         :param oper: operation type, as denoted in devv_constants.OpType
         :type oper: int
         :param xfers: list of Transfer objects
         :type xfers: list
-        :param payload: Transaction payload
-        :type payload: str
+        :param payload: Transaction payload binary
+        :type payload: bytes
         :param flags: tx flags, to be stored as an uint8, typically zero
         :type flags: int
         :param timestamp: time of tx to be stored as an uint64
         :type timestamp: int
         :param sig: signature to assign to this transaction
         :type sig: Signature or str
         :param is_legacy: if True, will follow canonical patterns for legacy blocks
         :type is_legacy: bool
         :return: the initialized Transaction object
         :rtype: Transaction
         """
+        self._signer = None
+        for xfer in xfers:
+            if xfer.get_amount() < 0:
+                self._signer = xfer.get_addr()
+                break
+        if not self._signer:
+            raise Exception('Invalid Transaction: one Transfer must have amount < 0')
+
         self._is_legacy = is_legacy
         self._pre_signature_init(oper, self._signer, xfers, payload, flags, timestamp)
+        self._canonical += payload
+        if (size := len(self._canonical)) != (exp_size := self._tx_size - self._signer.get_corresponding_sig_size()):
+            raise Exception(f"Invalid Transaction: unexpected canonical length ({size} != {exp_size})")
         if sig:
             self.set_sig(sig)
         return self
 
     def set_sig(self, sig: Signature or str):
         """
         Add the given signature to the Transaction's current canonical form.
@@ -229,15 +255,15 @@
         :type pkey: str
         :param aes_pass: aes key to decrypt/encrypt the pkey with; this is required
         :type aes_pass: str
         :return: the new signature for the tx
         :rtype: Signature
         """
         digest = self.get_message_digest()
-        self._sig = sign_binary(pkey=pkey, pub=self._signer, msg=DevvHash(digest), aes_pass=aes_pass)
+        self._sig = sign_binary(pkey=pkey, pub=self._signer, msg=digest, aes_pass=aes_pass)
         self._canonical = digest + self._sig.get_canonical(self._is_legacy)
         return self._sig
 
     def from_dict(self, props: dict):
         """
         Initializes a Transaction object from a dictionary. Expects the below keys:
 
@@ -259,31 +285,21 @@
         :rtype: Transaction
         """
         try:
             # construct xfers
             xfers = [Transfer(xfer) for xfer in props['xfers']]
             if not xfers:
                 raise Exception('Invalid Transaction: failed to parse any xfers')
-            self._signer = None
-            for xfer in xfers:
-                if xfer.get_amount() < 0:
-                    self._signer = xfer.get_addr()
-                    break
-            if not self._signer:
-                raise Exception('Invalid Transaction: one Transfer must have amount < 0')
 
             # get payload binary
             payload = bytes(props['payload'], 'utf-8')
 
             # check operation type
             if isinstance(props['op'], str):
-                try:
-                    op = OpType().__getattribute__(props['op'])
-                except Exception as e:
-                    raise Exception(f"Invalid Transaction: bad op string {props['op']}")
+                op = OpType().get(props['op'])
             elif props['op'] >= OpType.NUM_OPS:
                 raise Exception(f"Invalid Transaction: bad op int {props['op']}")
             else:
                 op = props['op']
 
             # initialize attributes and construct canonical
             return self.serialize(op, xfers, payload, props['flags'], props['timestamp'],
```

### Comparing `devvio_util-1.5.6/devvio_util/primitives/transfer.py` & `devvio_util-1.5.7/devvio_util/primitives/transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from devvio_util.primitives.devv_constants import kTRANSFER_NONADDR_DATA_SIZE
 from devvio_util.primitives.address import Address
-from devvio_util.primitives.utils import InputBuffer, set_int64, set_uint64
+from devvio_util.primitives.utils import InputBuffer, set_int64, set_uint64, set_uint8
 
 
 class Transfer:
     def __init__(self, xfer: dict or bytes or InputBuffer or None = None):
         self._addr = None
         self._delay = None
         self._amount = None
@@ -55,15 +55,15 @@
         self._canonical = bytes()
         self._size = self._addr.get_size() + kTRANSFER_NONADDR_DATA_SIZE
         self._canonical += self._addr.get_canonical()
         self._canonical += set_uint64(self._coin_id)
         self._canonical += set_int64(self._amount)
         self._canonical += set_uint64(self._delay)
         if len(self._canonical) != self._size + 1:
-            raise Exception(f"Invalid Transfer: canonical size invalid ({self._size} != {len(self._canonical)})")
+            raise Exception(f"Invalid Transfer: canonical size invalid ({len(self._canonical)} != {self._size + 1})")
 
     def __bool__(self):
         return self._canonical is not None
 
     def __str__(self):
         return str(self.get_dict())
```

### Comparing `devvio_util-1.5.6/devvio_util/primitives/utils.py` & `devvio_util-1.5.7/devvio_util/primitives/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         return self.get_next_hex(kPREV_HASH_SIZE, increment)
 
     def get_next_hex(self, num_bytes: int, increment: bool = True) -> str:
         result = self.get_next_bytes(num_bytes, increment).hex()
         return result
 
     def get_next_int(self, num_bytes: int, increment: bool = True, signed: bool = False, ) -> int:
-        result = int.from_bytes(self.get_next_bytes(num_bytes, increment), 'little', signed=signed)
+        result = get_int(self.get_next_bytes(num_bytes, increment), signed)
         return result
 
     def get_next_prefixed_obj(self, increment: bool = True):
         offset = self.tell()
         size = self.get_next_uint8()
         res = self.get_next_bytes(size)
         if not res or not increment:
@@ -90,14 +90,17 @@
     def seek(self, offset: int):
         self._reader.seek(offset)
 
     def tell(self) -> int:
         return self._reader.tell()
 
 
+def get_int(x: bytes, signed: bool) -> int:
+    return int.from_bytes(x, 'little', signed=signed)
+
 def set_uint64(x: int) -> bytes:
     return set_int(x, kUINT64_SIZE, False)
 
 
 def set_uint32(x: int) -> bytes:
     return set_int(x, kUINT32_SIZE, False)
```

### Comparing `devvio_util-1.5.6/devvio_util/primitives/validation.py` & `devvio_util-1.5.7/devvio_util/primitives/validation.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.6/devvio_util/psql_mixin.py` & `devvio_util-1.5.7/devvio_util/psql_mixin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.6/devvio_util.egg-info/SOURCES.txt` & `devvio_util-1.5.7/devvio_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

