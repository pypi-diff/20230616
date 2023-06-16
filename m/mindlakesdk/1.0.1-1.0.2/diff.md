# Comparing `tmp/mindlakesdk-1.0.1.tar.gz` & `tmp/mindlakesdk-1.0.2.tar.gz`

## Comparing `mindlakesdk-1.0.1.tar` & `mindlakesdk-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,16 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/requirements.txt
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/examples/env_template.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/examples/quickstart.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/examples/use_case_1.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/examples/use_case_2.py
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/examples/use_case_3.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/README.md
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/__init__.py
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/cryptor.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/datalake.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/keyhelper.py
--rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/message.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/permission.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/settings.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/mindlakesdk/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/env_template.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_all.py
--rw-r--r--   0        0        0    12613 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_base.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_create.py
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_delete.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_drop.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_encryption.py
--rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_insert.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_link.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_sharing.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/tests/test_update.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/LICENSE
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/README.md
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 mindlakesdk-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/requirements.txt
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/mindlakesdk/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/mindlakesdk/README.md
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/mindlakesdk/__init__.py
+-rw-r--r--   0        0        0     9614 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/mindlakesdk/cryptor.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/mindlakesdk/datalake.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/mindlakesdk/keyhelper.py
+-rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/mindlakesdk/message.py
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/mindlakesdk/permission.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/mindlakesdk/settings.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/mindlakesdk/utils.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 mindlakesdk-1.0.2/PKG-INFO
```

### Comparing `mindlakesdk-1.0.1/mindlakesdk/LICENSE` & `mindlakesdk-1.0.2/mindlakesdk/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.1/mindlakesdk/__init__.py` & `mindlakesdk-1.0.2/mindlakesdk/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 name = "mindlakesdk"
 
 from eth_account.messages import encode_defunct
 from web3 import Web3
+import requests
 
 import mindlakesdk.settings as settings
 import mindlakesdk.utils
 from mindlakesdk.utils import ResultType, Session, DataType
 import mindlakesdk.keyhelper
 from mindlakesdk.datalake import DataLake
 from mindlakesdk.cryptor import Cryptor
@@ -18,14 +19,15 @@
 
     DataType = DataType
 
     def __init__(self, walletPrivateKey: str, appKey: str, gateway: str = None):
         logging.debug(__name__)
         self.__session = mindlakesdk.utils.Session()
         session = self.__session
+        session.requstSession = requests.Session()
         self.datalake = DataLake(session)
         self.cryptor = Cryptor(session)
         self.permission = Permission(session)
         
         web3 = Web3(Web3.HTTPProvider(settings.WEB3API))
         walletAccount = web3.eth.account.from_key(walletPrivateKey)
```

### Comparing `mindlakesdk-1.0.1/mindlakesdk/cryptor.py` & `mindlakesdk-1.0.2/mindlakesdk/cryptor.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,44 +17,23 @@
         enc_float8 = 4
         enc_decimal = 6
         enc_text = 7
         enc_timestamp = 8
 
     def __init__(self, session: Session):
         self.__session = session
+        self.cryptParamsByColumn = {}
+        self.cryptParamsByID = {}
     
-    def encrypt(self, data, columnOrType: str|DataType) -> ResultType:
-        if isinstance(columnOrType, DataType):
-            dataType = columnOrType
-            result = mindlakesdk.message.getDKbyName(self.__session)
-            if not result:
-                return result
-        else:
-            tableName, columnName = columnOrType.split('.')
-            result = mindlakesdk.message.getDataTypeByName(self.__session, tableName, columnName)
-            if not result:
-                return result
-            dataType = DataType(result.data)
-            result = mindlakesdk.message.getDKbyName(self.__session, self.__session.walletAddress, tableName, columnName)
-            # Temporary solution for MS not returning Error Code
-            if result.code == 40010:
-                # DK not found, create one
-                result = mindlakesdk.keyhelper.genDK(self.__session, tableName, columnName)
-                if not result:
-                    return result
-            elif not result:
-                return result
-            else:
-                pass
-        encTypeNum = Cryptor.EncType['enc_' + dataType.name].value
+    def encrypt(self, data, columnOrType) -> ResultType:
+        result = self.__getEncryptParams(columnOrType)
+        if not result:
+            return result
+        ctxid, encTypeNum, dk, alg, dataType = result.data
         data = Cryptor.__encodeByDataType(data, dataType)
-        ctxid = result.data['ctxId']
-        dkCipher = result.data['encryptedDek']
-        dkID, dk = mindlakesdk.keyhelper.decryptDKb64(self.__session.mk, dkCipher)
-        alg = result.data['algorithm']
         header = Cryptor.__genCryptoHeader(ctxid, encTypeNum)
         checkCode = Cryptor.__genCheckCode(data, 1)
         data_to_enc = data + checkCode
         if alg == 3:
             iv = get_random_bytes(16)
             encrypted_data = mindlakesdk.utils.aesEncrypt(dk, iv, data_to_enc)
         elif alg == 0:
@@ -63,14 +42,50 @@
         buf = header + iv + encrypted_data
         tmp = buf[1:]
         checkCode2 = Cryptor.__genCheckCode(tmp, 1)
         result = checkCode2 + tmp
         resultHex = '\\x' + result.hex()
         return ResultType(0, None, resultHex)
 
+    def __getEncryptParams(self, columnOrType):
+        result = self.cryptParamsByColumn.get(columnOrType)
+        if not result:
+            if isinstance(columnOrType, DataType):
+                dataType = columnOrType
+                result = mindlakesdk.message.getDKbyName(self.__session)
+                if not result:
+                    return result
+            else:
+                tableName, columnName = columnOrType.split('.')
+                result = mindlakesdk.message.getDataTypeByName(self.__session, tableName, columnName)
+                if not result:
+                    return result
+                dataType = DataType(result.data)
+                result = mindlakesdk.message.getDKbyName(self.__session, self.__session.walletAddress, tableName, columnName)
+                # Temporary solution for MS not returning Error Code
+                if result.code == 40010:
+                    # DK not found, create one
+                    result = mindlakesdk.keyhelper.genDK(self.__session, tableName, columnName)
+                    if not result:
+                        return result
+                elif not result:
+                    return result
+                else:
+                    pass
+            encTypeNum = Cryptor.EncType['enc_' + dataType.name].value
+            ctxid = result.data['ctxId']
+            dkCipher = result.data['encryptedDek']
+            dkID, dk = mindlakesdk.keyhelper.decryptDKb64(self.__session.mk, dkCipher)
+            alg = result.data['algorithm']
+            result = (ctxid, encTypeNum, dk, alg, dataType)
+            self.cryptParamsByColumn[columnOrType] = result
+            self.cryptParamsByID[ctxid] = (dk, alg)
+        return ResultType(0, None, result)
+
+
     def __encodeByDataType(data, dataType: DataType) -> bytes:
         if dataType == DataType.int4:
             result = struct.pack("<i", data)
         elif dataType == DataType.int8:
             result = struct.pack("<q", data)
         elif dataType == DataType.float4:
             result = struct.pack("<f", data)
@@ -87,56 +102,69 @@
             u_sec -= 946684800000000
             u_sec += int(datetime.datetime.now().astimezone().utcoffset().total_seconds() * 1000000)
             result = struct.pack('<q', u_sec)
         else:
             raise Exception("Unsupported encryption type")
         return result
 
-    def decrypt(self, cipher: bytes|str) -> ResultType:
+    def decrypt(self, cipher) -> ResultType:
         if isinstance(cipher, str):
             data = bytes.fromhex(cipher[2:])
         else:
             data = cipher
         header = Cryptor.__extractCryptoHeader(data)
         encTypeNum = Cryptor.__extractEncType(header)
         ctxId = Cryptor.__extractCtxId(header)
-        result = mindlakesdk.message.getDKbyCid(self.__session, ctxId)
+        result = self.__getDecryptParams(ctxId)
         if not result:
             return result
-        dkCipher = result.data['encryptedDek']
-        # TODO: catch decryption error
-        try:
-            dkID, dk = mindlakesdk.keyhelper.decryptDKb64(self.__session.mk, dkCipher)
-        except:
-            return ResultType(60003, "Can't handle DK")
-        alg = result.data['algorithm']
-        if alg is None:
-            raise Exception("Cannot find data key by ctxId")
+        dk, alg = result.data
+        idx = (header[1] & 0x7) + 2
+        if alg == 3:
+            iv = data[idx:idx+16]
+            cipherBlob = data[idx+16:]
+            plainBlob = mindlakesdk.utils.aesDecrypt(dk, iv, cipherBlob)
+        elif alg == 0:
+            iv = data[idx:idx+12]
+            idx += 12
+            mac = data[idx:idx+16]
+            idx += 16
+            cipherBlob = data[idx:]
+            plainBlob = mindlakesdk.utils.aesGCMDecrypt(dk, iv, cipherBlob, mac)
         else:
-            idx = (header[1] & 0x7) + 2
-            if alg == 3:
-                iv = data[idx:idx+16]
-                cipherBlob = data[idx+16:]
-                plainBlob = mindlakesdk.utils.aesDecrypt(dk, iv, cipherBlob)
-            elif alg == 0:
-                iv = data[idx:idx+12]
-                idx += 12
-                mac = data[idx:idx+16]
-                idx += 16
-                cipherBlob = data[idx:]
-                plainBlob = mindlakesdk.utils.aesGCMDecrypt(dk, iv, cipherBlob, mac)
-            else:
-                raise Exception("Unsupported algorithm to decrypt")
-            result = plainBlob[:-1]
-            checkCode = plainBlob[-1:]
-            checkCode2 = Cryptor.__genCheckCode(result, 1)
-            if checkCode != checkCode2:
-                raise Exception("Check code is not correct")
-            result = Cryptor.__decodeByEncType(result, Cryptor.EncType(encTypeNum))
-            return ResultType(0, None, result)
+            return ResultType(60004, "Unsupported algorithm to decrypt")
+        result = plainBlob[:-1]
+        checkCode = plainBlob[-1:]
+        checkCode2 = Cryptor.__genCheckCode(result, 1)
+        if checkCode != checkCode2:
+            return ResultType(60005, "Check code of cipher is not correct")
+        result = Cryptor.__decodeByEncType(result, Cryptor.EncType(encTypeNum))
+        return ResultType(0, None, result)
+
+    def __getDecryptParams(self, ctxId: int):
+        params = self.cryptParamsByID.get(ctxId)
+        if not params:
+            result = mindlakesdk.message.getDKbyCid(self.__session, ctxId)
+            if not result:
+                return result
+            if not result.data:
+                return ResultType(60002, "Can't get data key")
+            dkCipher = result.data['encryptedDek']
+            if not dkCipher:
+                return ResultType(60002, "Can't get data key")
+            try:
+                dkID, dk = mindlakesdk.keyhelper.decryptDKb64(self.__session.mk, dkCipher)
+            except:
+                return ResultType(60003, "Can't handle data key")
+            alg = result.data['algorithm']
+            if alg is None:
+                return ResultType(60002, "Can't get data key")
+            params = (dk, alg)
+            self.cryptParamsByID[ctxId] = params
+        return ResultType(0, None, params)
 
     def __decodeByEncType(data, encType: EncType):
         if encType == Cryptor.EncType.enc_int4:
             size = struct.calcsize('<i')
             buf = data[:size]
             result = struct.unpack('<i', buf)[0]
         elif encType == Cryptor.EncType.enc_int8:
@@ -183,15 +211,15 @@
         return header
     
     def __extractEncType(header):
         tmp_value = header[1]
         type_value = (tmp_value & 0xF8) >> 3
         return type_value
     
-    def __extractCtxId(header):
+    def __extractCtxId(header) -> int:
         ctxIdLen = header[1] & 0x7
         assert len(header) == ctxIdLen + 2
         ctxId = 0
         for i in range(ctxIdLen):
             index = len(header) - 1 - i
             ctxId = ctxId << 8 | (header[index] & 0xFF)
         return ctxId
@@ -212,14 +240,14 @@
         ctxLen = len(head) - 2
 
         tmp_val = head[1]
         tmp_val = (tmp_val & 0xFFFFFFF8) | (ctxLen & 0x7)
         head[1] = tmp_val
         return bytes(head)
 
-    def __genCheckCode(data, resultSize):
+    def __genCheckCode(data: bytes, resultSize):
         tmpCode = bytearray(resultSize)
         for i in range(len(data)):
             n = i % resultSize
             tmpCode[n] ^= data[i]
         return bytes(tmpCode)
```

### Comparing `mindlakesdk-1.0.1/mindlakesdk/datalake.py` & `mindlakesdk-1.0.2/mindlakesdk/datalake.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.1/mindlakesdk/keyhelper.py` & `mindlakesdk-1.0.2/mindlakesdk/keyhelper.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.1/mindlakesdk/message.py` & `mindlakesdk-1.0.2/mindlakesdk/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,16 +139,24 @@
     data = {"bizType":128, 'tableName': tableName}
     return __requestCommon(session, data)
 
 def sendListGrantee(session: Session) -> ResultType:
     data = {"bizType":126}
     return __requestCommon(session, data)
 
-def sendListGrantedColumn(session: Session, walletAddress: str) -> ResultType:
-    data = {"bizType":127, 'targetWalletAddress': walletAddress}
+def sendListGrantedColumn(session: Session, targetWalletAddress: str) -> ResultType:
+    data = {"bizType":127, 'targetWalletAddress': targetWalletAddress}
+    return __requestCommon(session, data)
+
+def sendListOwner(session: Session) -> ResultType:
+    data = {"bizType":130}
+    return __requestCommon(session, data)
+
+def sendListOwnerColumn(session: Session, targetWalletAddress: str) -> ResultType:
+    data = {"bizType":131, 'targetWalletAddress': targetWalletAddress}
     return __requestCommon(session, data)
 
 def __requestCommon(session: Session, data: str) -> ResultType:
     if session.isLogin:
         result = request(data, session)
         if result:
             return ResultType(result["code"], result["message"], result["data"])
```

### Comparing `mindlakesdk-1.0.1/mindlakesdk/permission.py` & `mindlakesdk-1.0.2/mindlakesdk/permission.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,8 +135,14 @@
         return b'\x01' + signature
     
     def listGrantee(self) -> ResultType:
         return mindlakesdk.message.sendListGrantee(self.__session)  
     
     def listGrantedColumn(self, walletAddress: str) -> ResultType:
         return mindlakesdk.message.sendListGrantedColumn(self.__session, walletAddress) 
+    
+    def listOwner(self) -> ResultType:
+        return mindlakesdk.message.sendListOwner(self.__session)
+    
+    def listOwnerColumn(self, walletAddress: str) -> ResultType:
+        return mindlakesdk.message.sendListOwnerColumn(self.__session, walletAddress)
```

### Comparing `mindlakesdk-1.0.1/mindlakesdk/settings.py` & `mindlakesdk-1.0.2/mindlakesdk/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-GATEWAY = 'http://sdk.mindnetwork.xyz/node'
+GATEWAY = 'https://sdk.mindnetwork.xyz/node'
 WEB3API = 'https://goerli.infura.io/v3/744c0ade89464e4b867ca1b002a10231'
 CONTRACT_ADDRESS = '0xF5932e67e84F08965DC6D62C2B67f47a6826E5a7'
 CONTRACT_ABI = [
         {
                 "anonymous": False,
                 "inputs": [
                         {
@@ -66,8 +66,8 @@
                                 "type": "bytes"
                         }
                 ],
                 "stateMutability": "view",
                 "type": "function"
         }
 ]
-VERSION = 'v1.0.0'
+VERSION = 'v1.0.2'
```

### Comparing `mindlakesdk-1.0.1/mindlakesdk/utils.py` & `mindlakesdk-1.0.2/mindlakesdk/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from Crypto.Cipher import AES, PKCS1_OAEP
 from Crypto.Util.Padding import pad, unpad
 from Crypto.Signature import pss
 from Crypto.PublicKey import RSA
 from Crypto.Hash import SHA256, HMAC
 from Crypto.Random import get_random_bytes
 from enum import Enum
-import requests
 import json
 import mindlakesdk.settings as settings
 import logging
 
 class ResultType:
     def __init__(self, code: int, message: str = None, data = None):
         self.code = code
@@ -37,14 +36,15 @@
         self.isLogin = False
         self.token = None
         self.accountID = None
         self.nodePK = None
         self.pkID = None
         self.appKey = None
         self.gateway = None
+        self.requstSession = None
         
 def genRSAKey():
     rsaKey = RSA.generate(2048)
     return rsaKey
 
 def genAESKey():
     aesKey = get_random_bytes(16)
@@ -113,15 +113,15 @@
     headers = {}
     headers['Content-Type'] = 'application/json'
     headers['wa'] = session.walletAddress
     headers['ver'] = settings.VERSION
     headers['app'] = session.appKey
     if session.token:
         headers['token'] = session.token
-    response = requests.post(session.gateway, json=data, headers=headers)
+    response = session.requstSession.post(session.gateway, json=data, headers=headers)
     logging.debug("============== Mind SDK request ==============")
     logging.debug('MindSDKHeaders: %s'%headers)
     logging.debug("MindSDKData: %s"%data)
     logging.debug('MindSDKRequest: %s'%response.request.body.decode('utf-8'))
     logging.debug('MindSDKResponse: %s'%response.text)
     if response and response.status_code == 200:
         return json.loads(response.text)
```

### Comparing `mindlakesdk-1.0.1/LICENSE` & `mindlakesdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.1/README.md` & `mindlakesdk-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,35 +19,39 @@
 * web3
 * pynacl
 
 ### Installing
 
 * pip install mindlakesdk
 
-### Executing program
-
-* [quick starts](https://mind-network.gitbook.io/mind-lake-sdk/get-started)
-* [more examples](https://mind-network.gitbook.io/mind-lake-sdk/use-cases)
-* Step-by-step bullets
+### Import
 ```
 import mindlakesdk
 ...
 ```
 
+### More examples
+* [step-by-step tutorial](/tutorial/README.md)
+* [quick starts](https://mind-network.gitbook.io/mind-lake-sdk/get-started)
+* [more examples](https://mind-network.gitbook.io/mind-lake-sdk/use-cases)
+
+
+
 ## code
 ```
 mind-lake-sdk-python
 |-- mindlakesdk # source code
 |   |-- __init__.py
 |   |-- datalake.py
 |   |-- permission.py
 |   |-- cryptor.py
 |   └-- utils.py
 |-- tests # unit test code
 |-- examples # use case examples
+|-- tutorial # step-by-step tutorial
 |-- README.md
 └--- LICENSE
 
 ```
 
 ## Help
```

### Comparing `mindlakesdk-1.0.1/pyproject.toml` & `mindlakesdk-1.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mindlakesdk"
-version = "v1.0.1"
+version = "v1.0.2"
 authors = [
   { name="Mind Labs", email="biz@mindnetwork.xyz" },
 ]
 description = "A Python SDK to connect to Mind Lake"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -22,7 +22,10 @@
     "web3",
     "pynacl"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/mind-network/mind-lake-sdk-python"
 "Bug Tracker" = "https://github.com/mind-network/mind-lake-sdk-python/issues"
+
+[tool.hatch.build]
+exclude = ["/examples", "/tests", "/tutorial"]
```

### Comparing `mindlakesdk-1.0.1/PKG-INFO` & `mindlakesdk-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindlakesdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python SDK to connect to Mind Lake
 Project-URL: Homepage, https://github.com/mind-network/mind-lake-sdk-python
 Project-URL: Bug Tracker, https://github.com/mind-network/mind-lake-sdk-python/issues
 Author-email: Mind Labs <biz@mindnetwork.xyz>
 License-File: LICENSE
 Keywords: datalake,encryption,web3
 Classifier: License :: OSI Approved :: MIT License
@@ -37,35 +37,39 @@
 * web3
 * pynacl
 
 ### Installing
 
 * pip install mindlakesdk
 
-### Executing program
-
-* [quick starts](https://mind-network.gitbook.io/mind-lake-sdk/get-started)
-* [more examples](https://mind-network.gitbook.io/mind-lake-sdk/use-cases)
-* Step-by-step bullets
+### Import
 ```
 import mindlakesdk
 ...
 ```
 
+### More examples
+* [step-by-step tutorial](/tutorial/README.md)
+* [quick starts](https://mind-network.gitbook.io/mind-lake-sdk/get-started)
+* [more examples](https://mind-network.gitbook.io/mind-lake-sdk/use-cases)
+
+
+
 ## code
 ```
 mind-lake-sdk-python
 |-- mindlakesdk # source code
 |   |-- __init__.py
 |   |-- datalake.py
 |   |-- permission.py
 |   |-- cryptor.py
 |   └-- utils.py
 |-- tests # unit test code
 |-- examples # use case examples
+|-- tutorial # step-by-step tutorial
 |-- README.md
 └--- LICENSE
 
 ```
 
 ## Help
```

