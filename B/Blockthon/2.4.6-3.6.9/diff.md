# Comparing `tmp/Blockthon-2.4.6.tar.gz` & `tmp/Blockthon-3.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Blockthon-2.4.6.tar", last modified: Sun Jun  4 19:21:50 2023, max compression
+gzip compressed data, was "Blockthon-3.6.9.tar", last modified: Fri Jun 16 16:14:04 2023, max compression
```

## Comparing `Blockthon-2.4.6.tar` & `Blockthon-3.6.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 19:21:50.726609 Blockthon-2.4.6/
-drwxrwxrwx   0        0        0        0 2023-06-04 19:21:50.704579 Blockthon-2.4.6/Blockthon/
--rw-rw-rw-   0        0        0     2160 2023-06-02 20:46:04.000000 Blockthon-2.4.6/Blockthon/Base58.py
--rw-rw-rw-   0        0        0     3705 2023-06-04 19:05:17.000000 Blockthon-2.4.6/Blockthon/Bitcoin.py
--rw-rw-rw-   0        0        0     1159 2023-06-03 18:38:02.000000 Blockthon-2.4.6/Blockthon/BitcoinGold.py
--rw-rw-rw-   0        0        0     1041 2023-06-03 18:38:02.000000 Blockthon-2.4.6/Blockthon/Dash.py
--rw-rw-rw-   0        0        0     1032 2023-06-03 18:38:02.000000 Blockthon-2.4.6/Blockthon/DigiByte.py
--rw-rw-rw-   0        0        0      497 2023-06-03 12:50:01.000000 Blockthon-2.4.6/Blockthon/Dogecoin.py
--rw-rw-rw-   0        0        0      492 2023-06-02 23:40:53.000000 Blockthon-2.4.6/Blockthon/Ethereum.py
--rw-rw-rw-   0        0        0     1407 2023-06-03 13:19:05.000000 Blockthon-2.4.6/Blockthon/Litecoin.py
--rw-rw-rw-   0        0        0      859 2023-06-04 00:55:43.000000 Blockthon-2.4.6/Blockthon/Qtum.py
--rw-rw-rw-   0        0        0      847 2023-06-04 00:59:12.000000 Blockthon-2.4.6/Blockthon/Ravencoin.py
--rw-rw-rw-   0        0        0      495 2023-06-02 23:40:53.000000 Blockthon-2.4.6/Blockthon/Tron.py
--rw-rw-rw-   0        0        0    24954 2023-06-04 19:05:17.000000 Blockthon-2.4.6/Blockthon/Utils.py
--rw-rw-rw-   0        0        0     1497 2023-06-04 15:50:24.000000 Blockthon-2.4.6/Blockthon/Wallet.py
--rw-rw-rw-   0        0        0      588 2023-06-04 01:02:25.000000 Blockthon-2.4.6/Blockthon/__init__.py
--rw-rw-rw-   0        0        0      822 2023-06-04 00:29:18.000000 Blockthon-2.4.6/Blockthon/zCash.py
-drwxrwxrwx   0        0        0        0 2023-06-04 19:21:50.726609 Blockthon-2.4.6/Blockthon.egg-info/
--rw-rw-rw-   0        0        0     3514 2023-06-04 19:21:50.000000 Blockthon-2.4.6/Blockthon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2023-06-04 19:21:50.000000 Blockthon-2.4.6/Blockthon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 19:21:50.000000 Blockthon-2.4.6/Blockthon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      166 2023-06-04 19:21:50.000000 Blockthon-2.4.6/Blockthon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-04 19:21:50.000000 Blockthon-2.4.6/Blockthon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3514 2023-06-04 19:21:50.726609 Blockthon-2.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     2674 2023-06-04 19:14:44.000000 Blockthon-2.4.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-04 19:21:50.726609 Blockthon-2.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1477 2023-06-04 19:16:06.000000 Blockthon-2.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:14:04.995639 Blockthon-3.6.9/
+drwxrwxrwx   0        0        0        0 2023-06-16 16:14:04.983213 Blockthon-3.6.9/Blockthon/
+-rw-rw-rw-   0        0        0     2160 2023-06-02 20:46:04.000000 Blockthon-3.6.9/Blockthon/Base58.py
+-rw-rw-rw-   0        0        0     3705 2023-06-04 19:05:17.000000 Blockthon-3.6.9/Blockthon/Bitcoin.py
+-rw-rw-rw-   0        0        0     1159 2023-06-03 18:38:02.000000 Blockthon-3.6.9/Blockthon/BitcoinGold.py
+-rw-rw-rw-   0        0        0     1041 2023-06-03 18:38:02.000000 Blockthon-3.6.9/Blockthon/Dash.py
+-rw-rw-rw-   0        0        0     1032 2023-06-03 18:38:02.000000 Blockthon-3.6.9/Blockthon/DigiByte.py
+-rw-rw-rw-   0        0        0      497 2023-06-03 12:50:01.000000 Blockthon-3.6.9/Blockthon/Dogecoin.py
+-rw-rw-rw-   0        0        0      492 2023-06-02 23:40:53.000000 Blockthon-3.6.9/Blockthon/Ethereum.py
+-rw-rw-rw-   0        0        0     1407 2023-06-03 13:19:05.000000 Blockthon-3.6.9/Blockthon/Litecoin.py
+-rw-rw-rw-   0        0        0      859 2023-06-04 00:55:43.000000 Blockthon-3.6.9/Blockthon/Qtum.py
+-rw-rw-rw-   0        0        0      847 2023-06-04 00:59:12.000000 Blockthon-3.6.9/Blockthon/Ravencoin.py
+-rw-rw-rw-   0        0        0      495 2023-06-02 23:40:53.000000 Blockthon-3.6.9/Blockthon/Tron.py
+-rw-rw-rw-   0        0        0    30361 2023-06-16 16:11:36.000000 Blockthon-3.6.9/Blockthon/Utils.py
+-rw-rw-rw-   0        0        0     1607 2023-06-16 16:11:36.000000 Blockthon-3.6.9/Blockthon/Wallet.py
+-rw-rw-rw-   0        0        0      588 2023-06-04 01:02:25.000000 Blockthon-3.6.9/Blockthon/__init__.py
+-rw-rw-rw-   0        0        0      822 2023-06-04 00:29:18.000000 Blockthon-3.6.9/Blockthon/zCash.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:14:04.995639 Blockthon-3.6.9/Blockthon.egg-info/
+-rw-rw-rw-   0        0        0     3514 2023-06-16 16:14:04.000000 Blockthon-3.6.9/Blockthon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2023-06-16 16:14:04.000000 Blockthon-3.6.9/Blockthon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 16:14:04.000000 Blockthon-3.6.9/Blockthon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      166 2023-06-16 16:14:04.000000 Blockthon-3.6.9/Blockthon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 16:14:04.000000 Blockthon-3.6.9/Blockthon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3514 2023-06-16 16:14:04.995639 Blockthon-3.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2674 2023-06-04 01:48:32.000000 Blockthon-3.6.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 16:14:04.995639 Blockthon-3.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1477 2023-06-16 16:13:07.000000 Blockthon-3.6.9/setup.py
```

### Comparing `Blockthon-2.4.6/Blockthon/Base58.py` & `Blockthon-3.6.9/Blockthon/Base58.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.4.6/Blockthon/Bitcoin.py` & `Blockthon-3.6.9/Blockthon/Bitcoin.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.4.6/Blockthon/BitcoinGold.py` & `Blockthon-3.6.9/Blockthon/BitcoinGold.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.4.6/Blockthon/Dash.py` & `Blockthon-3.6.9/Blockthon/Dash.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.4.6/Blockthon/DigiByte.py` & `Blockthon-3.6.9/Blockthon/DigiByte.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.4.6/Blockthon/Litecoin.py` & `Blockthon-3.6.9/Blockthon/Litecoin.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.4.6/Blockthon/Qtum.py` & `Blockthon-3.6.9/Blockthon/Qtum.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.4.6/Blockthon/Ravencoin.py` & `Blockthon-3.6.9/Blockthon/Ravencoin.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.4.6/Blockthon/Utils.py` & `Blockthon-3.6.9/Blockthon/Utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from binascii import hexlify as _decode
+from binascii import hexlify as _decode, unhexlify as UnHex
 from bip32utils import BIP32Key
 from .Base58 import b58_decode, b58check_decode, b58check_encode, b58_encode, Base58_
 from hdwallet import HDWallet as Wallet_
 from hdwallet.symbols import BTC, ETH, BTG, TRX, LTC, DASH, DGB, DOGE, ZEC, QTUM, RVN
 from mnemonic import Mnemonic
 from bit.format import bytes_to_wif as Bytes_To_Wif
 from bit import Key as Wallet
 from hashlib import sha256 as _SHA256, new as New_, sha512 as _SHA512
-import codecs, os, re, random, pbkdf2, requests, json, hmac
+import sys, os, re, random, pbkdf2, requests, json, hmac, binascii, hashlib, base58, sys, ecdsa, codecs
 
 
 def SHA256(bytestring): return _SHA256(bytestring).digest()
 
 
 def Double_SHA256(bytestring): return _SHA256(_SHA256(bytestring).digest()).digest()
 
@@ -249,27 +249,146 @@
     if compress:
         return PrivateKey_To_PublicKey(Bytes_To_PrivateKey(bytestring), True)
     else:
         return PrivateKey_To_PublicKey(Bytes_To_PrivateKey(bytestring))
 
 # -------------------------------------------------------------------------------
 
+def HexToBytes(data): return codecs.decode(data, 'hex')
+
+def BytesToHex(data): return codecs.encode(data, 'hex')
+
+def PVK_To_Wif_UnCompress(privatekey):
+    private_key_static = privatekey
+    extended_key = "80" + private_key_static
+    first_sha256 = hashlib.sha256(binascii.unhexlify(extended_key)).hexdigest()
+    second_sha256 = hashlib.sha256(binascii.unhexlify(first_sha256)).hexdigest()
+    final_key = extended_key + second_sha256[:8]
+    UNCOMPRESS_WIF = base58.b58encode(binascii.unhexlify(final_key)).decode('utf-8')
+    return UNCOMPRESS_WIF
+
+def PVK_To_Wif_Compress(privatekey):
+    private_key_static = privatekey
+    extended_key = "80" + private_key_static + '01'
+    first_sha256 = hashlib.sha256(binascii.unhexlify(extended_key)).hexdigest()
+    second_sha256 = hashlib.sha256(binascii.unhexlify(first_sha256)).hexdigest()
+    final_key = extended_key + second_sha256[:8]
+    COMPRESS_WIF = base58.b58encode(binascii.unhexlify(final_key)).decode('utf-8')
+    return COMPRESS_WIF
+
+
+def PrivateKey_To_UnCompress_Address(privatekey):
+    bytes_string = HexToBytes(privatekey)
+    zk = ecdsa.SigningKey.from_string(bytes_string, curve=ecdsa.SECP256k1)
+    z_public_key = b'\x04' + zk.verifying_key.to_string()
+
+    ripemd160 = hashlib.new('ripemd160')
+    ripemd160.update(hashlib.sha256(z_public_key).digest())
+    ripemd160_result = ripemd160.hexdigest()
+    step3 = '00' + ripemd160_result
+    second_sha256 = hashlib.sha256(binascii.unhexlify(step3)).hexdigest()
+    third_sha256 = hashlib.sha256(binascii.unhexlify(second_sha256)).hexdigest()
+    step6 = third_sha256[:8]
+    step7 = step3 + step6
+    UnCompressAddr = base58.b58encode(binascii.unhexlify(step7)).decode('utf-8')
+    return UnCompressAddr
+
+def PrivateKey_To_Compress_Address(privatekey):
+    pvk_to_bytes = codecs.decode(privatekey, 'hex')
+    key = ecdsa.SigningKey.from_string(pvk_to_bytes, curve=ecdsa.SECP256k1).verifying_key
+    key_bytes = key.to_string()
+    key_hex = codecs.encode(key_bytes, 'hex').decode('utf-8')
+
+    if ord(bytearray.fromhex(key_hex[-2:])) % 2 == 0:
+        PUB_COMPRESS = '02' + key_hex[0:64]
+        PUB_BYTE_STRING = codecs.decode(PUB_COMPRESS, 'hex')
+        PUB_COMPRESS_256 = hashlib.sha256(PUB_BYTE_STRING)
+        PUB_COMPRESS_256_DIGEST = PUB_COMPRESS_256.digest()
+        ripemd160 = hashlib.new('ripemd160')
+        ripemd160.update(PUB_COMPRESS_256_DIGEST)
+        RIPEMD160_DIGEST = ripemd160.digest()
+        RIPEMD160_HEX = codecs.encode(RIPEMD160_DIGEST, 'hex')
+        PUB_COMPRESS_NETWORK = b'00' + RIPEMD160_HEX
+        PUB_COMPRESS_NETWORK_BYTE = codecs.decode(PUB_COMPRESS_NETWORK, 'hex')
+        SHA256_I = hashlib.sha256(PUB_COMPRESS_NETWORK_BYTE)
+        SHA256_I_DIGEST = SHA256_I.digest()
+        SHA256_II = hashlib.sha256(SHA256_I_DIGEST)
+        SHA256_II_DIGEST = SHA256_II.digest()
+        SH256_II_HEX = codecs.encode(SHA256_II_DIGEST, 'hex')
+        CHECKSUM_COMPRESS = SH256_II_HEX[:8]
+        ADDR_COMPRESS_HEX = (PUB_COMPRESS_NETWORK + CHECKSUM_COMPRESS).decode('utf-8')
+        COMPRESS = base58.b58encode(binascii.unhexlify(ADDR_COMPRESS_HEX)).decode('utf-8')
+        return COMPRESS
+    else:
+        PUB_COMPRESS = '03' + key_hex[0:64]
+        PUB_BYTE_STRING = codecs.decode(PUB_COMPRESS, 'hex')
+        PUB_COMPRESS_256 = hashlib.sha256(PUB_BYTE_STRING)
+        PUB_COMPRESS_256_DIGEST = PUB_COMPRESS_256.digest()
+        ripemd160 = hashlib.new('ripemd160')
+        ripemd160.update(PUB_COMPRESS_256_DIGEST)
+        RIPEMD160_DIGEST = ripemd160.digest()
+        RIPEMD160_HEX = codecs.encode(RIPEMD160_DIGEST, 'hex')
+        PUB_COMPRESS_NETWORK = b'00' + RIPEMD160_HEX
+        PUB_COMPRESS_NETWORK_BYTE = codecs.decode(PUB_COMPRESS_NETWORK, 'hex')
+        SHA256_I = hashlib.sha256(PUB_COMPRESS_NETWORK_BYTE)
+        SHA256_I_DIGEST = SHA256_I.digest()
+        SHA256_II = hashlib.sha256(SHA256_I_DIGEST)
+        SHA256_II_DIGEST = SHA256_II.digest()
+        SH256_II_HEX = codecs.encode(SHA256_II_DIGEST, 'hex')
+        CHECKSUM_COMPRESS = SH256_II_HEX[:8]
+        ADDR_COMPRESS_HEX = (PUB_COMPRESS_NETWORK + CHECKSUM_COMPRESS).decode('utf-8')
+        COMPRESS = base58.b58encode(binascii.unhexlify(ADDR_COMPRESS_HEX)).decode('utf-8')
+        return COMPRESS
+
+
 def Wif_To_Addr(wif):
     btc = Wallet(wif)
     return btc.address
 
 
 def Wif_To_HEX(wif):
     btc = Wallet(wif)
     return btc.to_hex()
 
 def Wif_To_DEC(wif):
     btc = Wallet(wif)
     return btc.to_int()
 
+
+def PrivateKey_To_Address(privatekey, compress=False):
+    """
+    >>> from Blockthon.Wallet import PrivateKey_To_Address
+    >>> private_key = "PRIVATEKEY_HEX_STRING"
+    >>> compressed_Address = PrivateKey_To_Address(private_key, compress=True)
+    >>> uncompressed_Address = PrivateKey_To_Address(private_key, compress=False)
+    :param privatekey:
+    :param compress:
+    :return: address
+    """
+    if compress:
+        return PrivateKey_To_Compress_Address(privatekey)
+    else:
+        return PrivateKey_To_UnCompress_Address(privatekey)
+
+
+def PrivateKey_To_WIF(privatekey, compress=False):
+    """
+    >>> from Blockthon.Wallet import PrivateKey_To_WIF
+    >>> compressed_WIF = PrivateKey_To_WIF(privatekey, compress=True)
+    >>> uncompressed_WIF = PrivateKey_To_WIF(privatekey, compress=False)
+
+    :param privatekey:
+    :param compress:
+    :return: WIF
+    """
+    if compress:
+        return PVK_To_Wif_Compress(privatekey)
+    else:
+        return PVK_To_Wif_UnCompress(privatekey)
+
 # --------------------------------------------------------------------------------
 # Check Value Bitcoin Address Balance Return [str]
 def Btc_Balance(addr):
     req = requests.get(f"https://bitcoin.atomicwallet.io/api/v2/address/{addr}").json()
     return dict(req)['balance']
 
 # --------------------------------------------------------------------------------
@@ -336,7 +455,8 @@
 
 # --------------------------------------------------------------------------------
 # Check Value Dash Address Balance : return [str]
 def Dash_Balance(address):
     """ # Check Value Dash Address Balance : return [str] """
     req = requests.get(f"https://dash.atomicwallet.io/api/v1/address/{address}").json()
     return dict(req)['balance']
+
```

### Comparing `Blockthon-2.4.6/Blockthon/Wallet.py` & `Blockthon-3.6.9/Blockthon/Wallet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from .Utils import (
+
+    PrivateKey_To_UnCompress_Address,
+    PrivateKey_To_Compress_Address,
     PrivateKey_To_UnCompress_Addr,
     PrivateKey_To_Compress_Addr,
     PrivateKey_To_PublicHash,
-    PrivateKey_To_PublicKey,
     PrivateKey_To_Mnemonics,
+    PrivateKey_To_PublicKey,
+    PrivateKey_To_Address,
     PrivateKey_To_RootKey,
     PrivateKey_To_Binary,
     PrivateKey_To_Bytes,
     PrivateKey_To_Addr,
     PrivateKey_To_Dec,
-    PrivateKey_To_Wif,
+    PrivateKey_To_WIF,
     PrivateKey_From_Passphrase,
     PrivateKey_From_RootKey,
     PrivateKey_From_Binary,
     PrivateKey_From_Dec,
     PrivateKey,
     getMnemonic,
     getBytes,
@@ -37,7 +41,9 @@
 from .DigiByte import PrivateKey_To_DGB, Mnemonic_To_DGB, Balance_DGB
 from .Ethereum import PrivateKey_To_ETH, Mnemonic_To_ETH, Balance_ETH
 from .Litecoin import PrivateKey_To_LTC, Mnemonic_To_LTC, Balance_LTC
 from .Tron import PrivateKey_To_TRX, Mnemonic_To_TRX, Balance_TRX
 from .zCash import PrivateKey_To_ZEC, Mnemonic_To_ZEC, Balance_ZEC
 from .Qtum import PrivateKey_To_QTUM, Mnemonic_To_QTUM, Balance_QTUM
 from .Ravencoin import PrivateKey_To_RVN, Mnemonic_To_RVN, Balance_RVN
+
+
```

### Comparing `Blockthon-2.4.6/Blockthon/__init__.py` & `Blockthon-3.6.9/Blockthon/__init__.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.4.6/Blockthon/zCash.py` & `Blockthon-3.6.9/Blockthon/zCash.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.4.6/Blockthon.egg-info/PKG-INFO` & `Blockthon-3.6.9/Blockthon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Blockthon
-Version: 2.4.6
+Version: 3.6.9
 Summary: Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.
 Home-page: https://github.com/Blockthon/Blockthon
 Author: Pymmdrza
 Author-email: Pymmdrza@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://mmdrza.gitbook.io/blockthon/
 Project-URL: Personal Website, https://mmdrza.com
```

### Comparing `Blockthon-2.4.6/PKG-INFO` & `Blockthon-3.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Blockthon
-Version: 2.4.6
+Version: 3.6.9
 Summary: Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.
 Home-page: https://github.com/Blockthon/Blockthon
 Author: Pymmdrza
 Author-email: Pymmdrza@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://mmdrza.gitbook.io/blockthon/
 Project-URL: Personal Website, https://mmdrza.com
```

### Comparing `Blockthon-2.4.6/README.md` & `Blockthon-3.6.9/README.md`

 * *Files identical despite different names*

### Comparing `Blockthon-2.4.6/setup.py` & `Blockthon-3.6.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="Blockthon",
-    version="2.4.6",
+    version="3.6.9",
     author="Pymmdrza",
     author_email="Pymmdrza@gmail.com",
     description="Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.",
     keywords=['blockthon','bitcoin', 'ethereum', 'tron', 'dogecoin', 'dash', 'qtum', 'litecoin', 'bitcoingold', 'wallet', 'private key', 'mnemonic', 'seed', 'binary', 'hex', 'hunter', 'compress', 'un compress', 'compress address', 'un compress address'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Blockthon/Blockthon",
```

