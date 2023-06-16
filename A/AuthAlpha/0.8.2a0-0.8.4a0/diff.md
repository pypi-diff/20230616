# Comparing `tmp/AuthAlpha-0.8.2-alpha.tar.gz` & `tmp/AuthAlpha-0.8.4-alpha.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AuthAlpha-0.8.2-alpha.tar", last modified: Sun Oct 30 07:20:31 2022, max compression
+gzip compressed data, was "AuthAlpha-0.8.4-alpha.tar", last modified: Fri Jun 16 17:55:45 2023, max compression
```

## Comparing `AuthAlpha-0.8.2-alpha.tar` & `AuthAlpha-0.8.4-alpha.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2022-10-30 07:20:31.239436 AuthAlpha-0.8.2-alpha/
-drwxrwxrwx   0        0        0        0 2022-10-30 07:20:31.239436 AuthAlpha-0.8.2-alpha/AuthAlpha/
--rw-rw-rw-   0        0        0     2166 2022-10-30 06:57:53.948627 AuthAlpha-0.8.2-alpha/AuthAlpha/Non_Password_Hashing.py
--rw-rw-rw-   0        0        0     3759 2022-10-30 06:57:53.948627 AuthAlpha-0.8.2-alpha/AuthAlpha/OTPMethods.py
--rw-rw-rw-   0        0        0     9192 2022-10-30 06:57:53.948627 AuthAlpha-0.8.2-alpha/AuthAlpha/Password_Hashing.py
--rw-rw-rw-   0        0        0     1045 2022-10-30 06:57:53.948627 AuthAlpha-0.8.2-alpha/AuthAlpha/__init__.py
--rw-rw-rw-   0        0        0     1053 2022-10-30 07:20:31.239436 AuthAlpha-0.8.2-alpha/PKG-INFO
--rw-rw-rw-   0        0        0       65 2022-10-30 07:00:24.931018 AuthAlpha-0.8.2-alpha/setup.cfg
--rw-rw-rw-   0        0        0     1340 2022-10-30 07:19:45.409331 AuthAlpha-0.8.2-alpha/setup.py
+drwxrwxr-x   0 theorist  (1000) theorist  (1000)        0 2023-06-16 17:55:45.063714 AuthAlpha-0.8.4-alpha/
+drwxrwxr-x   0 theorist  (1000) theorist  (1000)        0 2023-06-16 17:55:45.063714 AuthAlpha-0.8.4-alpha/AuthAlpha/
+-rw-rw-r--   0 theorist  (1000) theorist  (1000)     2346 2023-06-16 17:49:41.983036 AuthAlpha-0.8.4-alpha/AuthAlpha/Non_Password_Hashing.py
+-rw-rw-r--   0 theorist  (1000) theorist  (1000)     3831 2023-06-16 17:49:41.991036 AuthAlpha-0.8.4-alpha/AuthAlpha/OTPMethods.py
+-rw-rw-r--   0 theorist  (1000) theorist  (1000)     9786 2023-06-16 17:49:41.995036 AuthAlpha-0.8.4-alpha/AuthAlpha/Password_Hashing.py
+-rw-rw-r--   0 theorist  (1000) theorist  (1000)     1018 2023-06-16 17:49:41.979036 AuthAlpha-0.8.4-alpha/AuthAlpha/__init__.py
+-rw-rw-r--   0 theorist  (1000) theorist  (1000)     1032 2023-06-16 17:55:45.063714 AuthAlpha-0.8.4-alpha/PKG-INFO
+-rw-rw-r--   0 theorist  (1000) theorist  (1000)       65 2023-06-11 18:56:46.304261 AuthAlpha-0.8.4-alpha/setup.cfg
+-rw-rw-r--   0 theorist  (1000) theorist  (1000)     1365 2023-06-16 17:55:32.123536 AuthAlpha-0.8.4-alpha/setup.py
```

### Comparing `AuthAlpha-0.8.2-alpha/AuthAlpha/OTPMethods.py` & `AuthAlpha-0.8.4-alpha/AuthAlpha/OTPMethods.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,95 @@
-"""
-Copyright (C) 2021-2022 Mayank Vats
-See license.txt
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License v3
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-__author__ = "Mayank Vats"
-__email__ = "dev-theorist.e5xna@simplelogin.com"
-__Description__ = "AuthAlpha: A package to manage Hashing and OTP generation."
-__version__ = "0.8.2alpha"
-
-"""
-
-
-class TwoFactorAuth:
-
-    @staticmethod
-    def static_otp(otp_len: int = 6) -> str:
-        """
-        Used to generate Random ONE-TIME-PASSWORDS which are
-        utilized in the app for user verification and authentication.
-        Gets SystemRandom class instance out of secrets module and
-        generates a random integer in range [a, b].
-        :param: otp_len=6: length of the otp
-        :return: str(random integer in range [10^n, (10^n) - 1])
-        """
-        # secure random integer numbers
-        from secrets import SystemRandom
-
-        secrets_generator = SystemRandom()
-        l_range = (10 ** (otp_len - 1))
-        h_range = (l_range * 10) - 1
-        otp = secrets_generator.randint(l_range, h_range)
-        return str(otp)
-
-    @staticmethod
-    def totp(name, issuer_name: str, secret_len: int = 64) -> tuple:
-        from pyotp import random_base32, TOTP
-        token = random_base32(secret_len)
-        URL = TOTP(token).provisioning_uri(name=name, issuer_name=issuer_name)
-
-        return token, URL
-
-    @staticmethod
-    def verify(token: str, otp) -> bool:
-        from pyotp import TOTP
-
-        return TOTP(token).verify(str(otp))
-
-    @staticmethod
-    def encrypt(key: bytes, source: bytes, encode=True) -> str:
-        import base64
-        from Crypto.Cipher import AES
-        from Crypto.Hash import SHA256
-        from Crypto import Random
-        key = SHA256.new(key).digest()  # use SHA-256 over our key to get a proper-sized AES key
-        IV = Random.new().read(AES.block_size)  # generate IV
-        encryptor = AES.new(key, AES.MODE_CBC, IV)
-        padding = AES.block_size - len(source) % AES.block_size  # calculate needed padding
-        source += bytes([padding]) * padding  # Python 2.x: source += chr(padding) * padding
-        data = IV + encryptor.encrypt(source)  # store the IV at the beginning and encrypt
-        return base64.b64encode(data).decode("latin-1") if encode else data
-
-    @staticmethod
-    def decrypt(key: bytes, source, decode=True) -> str:
-        import base64
-        from Crypto.Cipher import AES
-        from Crypto.Hash import SHA256
-        if decode:
-            source = base64.b64decode(source.encode("latin-1"))
-        key = SHA256.new(key).digest()  # use SHA-256 over our key to get a proper-sized AES key
-        IV = source[:AES.block_size]  # extract the IV from the beginning
-        decryptor = AES.new(key, AES.MODE_CBC, IV)
-        data = decryptor.decrypt(source[AES.block_size:])  # decrypt
-        padding = data[-1]  # pick the padding value from the end; Python 2.x: ord(data[-1])
-        if data[-padding:] != bytes([padding]) * padding:  # Python 2.x: chr(padding) * padding
-            raise ValueError("Invalid padding...")
-        return data[:-padding].decode('utf-8')  # remove the padding
+"""
+Copyright (C) 2021-2023 Mayank Vats
+See license.txt
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License v3
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+__author__ = "Mayank Vats"
+__email__ = "dev-theorist.e5xna@simplelogin.com"
+__Description__ = "AuthAlpha: A package to manage Hashing and OTP generation."
+__version__ = "0.8.4alpha"
+
+"""
+
+
+class TwoFactorAuth:
+
+    def __repr__(self):
+        return "TwoFactorAuth()"
+
+    def __str__(self):
+        return "\033[1mTwo Factor Authentication Class[TwoFactorAuth]\033[0m."
+
+    @staticmethod
+    def static_otp(otp_len: int = 6) -> str:
+        """
+        Used to generate Random ONE-TIME-PASSWORDS which are
+        utilized in the app for user verification and authentication.
+        Gets SystemRandom class instance out of secrets module and
+        generates a random integer in range [a, b].
+        :param: otp_len=6: length of the otp
+        :return: str(random integer in range [10^n, (10^n) - 1])
+        """
+        # secure random integer numbers
+        from secrets import SystemRandom
+
+        secrets_generator = SystemRandom()
+        l_range = (10 ** (otp_len - 1))
+        h_range = (l_range * 10) - 1
+        otp = secrets_generator.randint(l_range, h_range)
+        return str(otp)
+
+    @staticmethod
+    def totp(name, issuer_name: str, secret_len: int = 64) -> tuple:
+        from pyotp import random_base32, TOTP
+        token = random_base32(secret_len)
+        URL = TOTP(token).provisioning_uri(name=name, issuer_name=issuer_name)
+
+        return token, URL
+
+    @staticmethod
+    def verify(token: str, otp) -> bool:
+        from pyotp import TOTP
+
+        return TOTP(token).verify(str(otp))
+
+    @staticmethod
+    def encrypt(key: bytes, source: bytes, encode=True) -> str:
+        import base64
+        from Crypto.Cipher import AES
+        from Crypto.Hash import SHA256
+        from Crypto import Random
+        key = SHA256.new(key).digest()  # use SHA-256 over our key to get a proper-sized AES key
+        IV = Random.new().read(AES.block_size)  # generate IV
+        encryptor = AES.new(key, AES.MODE_CBC, IV)
+        padding = AES.block_size - len(source) % AES.block_size  # calculate needed padding
+        source += bytes([padding]) * padding  # Python 2.x: source += chr(padding) * padding
+        data = IV + encryptor.encrypt(source)  # store the IV at the beginning and encrypt
+        return base64.b64encode(data).decode("latin-1") if encode else data
+
+    @staticmethod
+    def decrypt(key: bytes, source, decode=True) -> str:
+        import base64
+        from Crypto.Cipher import AES
+        from Crypto.Hash import SHA256
+        if decode:
+            source = base64.b64decode(source.encode("latin-1"))
+        key = SHA256.new(key).digest()  # use SHA-256 over our key to get a proper-sized AES key
+        IV = source[:AES.block_size]  # extract the IV from the beginning
+        decryptor = AES.new(key, AES.MODE_CBC, IV)
+        data = decryptor.decrypt(source[AES.block_size:])  # decrypt
+        padding = data[-1]  # pick the padding value from the end; Python 2.x: ord(data[-1])
+        if data[-padding:] != bytes([padding]) * padding:  # Python 2.x: chr(padding) * padding
+            raise ValueError("Invalid padding...")
+        return data[:-padding].decode('utf-8')  # remove the padding
```

### Comparing `AuthAlpha-0.8.2-alpha/AuthAlpha/Password_Hashing.py` & `AuthAlpha-0.8.4-alpha/AuthAlpha/Password_Hashing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,208 +1,223 @@
-"""
-Copyright (C) 2021-2022 Mayank Vats
-See license.txt
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License v3
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-__author__ = "Mayank Vats"
-__email__ = "dev-theorist.e5xna@simplelogin.com"
-__Description__ = "AuthAlpha: A package to manage Hashing and OTP generation."
-__version__ = "0.8.2alpha"
-
-"""
-
-
-class PassHashing:
-
-    def __init__(self, algorithm):
-        self.algorithm = algorithm
-        self.supported_hash_methods = [
-            "argon2id",
-            "pbkdf2:sha1",
-            "pbkdf2:sha224",
-            "pbkdf2:sha256",
-            "pbkdf2:sha384",
-            "pbkdf2:sha512",
-            "bcrypt",
-            "scrypt"
-        ]
-
-    def generate_password_hash(self, password: str, cost: int = None, prov_salt: bytes = None):
-        """
-        :param cost: Specify number of iterations for a certain algorithm,
-        default values are chosen sensibly, but you can still change them.
-        (NOT APPLICABLE FOR ARGON2ID(TBD))
-        :param password: type(password) is str
-        :param prov_salt: (optional) provide a bytes-like salt for hashing
-        only applicable for pbkdf2 hashes.
-        :return: str(hash)
-        This method generates a hash pertaining to a specified algorithm,
-        see supported_hash_algorithms.
-        """
-
-        if self.algorithm == "argon2id":
-            from argon2 import PasswordHasher
-            crypt_er = PasswordHasher()
-            return crypt_er.hash(password)
-
-        elif self.algorithm.startswith("pbkdf2:"):
-            from secrets import choice
-            from hashlib import pbkdf2_hmac
-            SALT_CHARS = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
-            DEFAULT_ITERATIONS = 300000
-
-            if not prov_salt:
-                # Generating a random salt and encoding it to bytes
-                salt = "".join(choice(SALT_CHARS) for _ in range(16)).encode("utf-8")
-                # Type-casting the inputted password to string and then encoding it to bytes.
-                byte_password = password.encode("utf-8")
-                # self.algorithm[7:].split(":") returns a list like this: ['pbkdf2', 'sha256']
-                args = self.algorithm.split(":")[1]
-
-                # Default rounds of pbkdf2
-                if not cost:
-                    h = pbkdf2_hmac(args, byte_password, salt, DEFAULT_ITERATIONS).hex()
-                    actual_method = f"$pbkdf2:{args}:{DEFAULT_ITERATIONS}"
-                    return f"{actual_method}${salt.decode('utf-8')}${h}"
-
-                # Custom rounds of pbkdf2
-                else:
-                    h = pbkdf2_hmac(args, byte_password, salt, cost).hex()  # specified number of rounds
-                    actual_method = f"$pbkdf2:{args}:{cost}"
-                    return f"{actual_method}${salt.decode('utf-8')}${h}"
-
-            else:
-                # In-case the user provides a salt, hashing is done using it. type(salt) is bytes
-                byte_password = password.encode("utf-8")
-                args = self.algorithm.split(":")[1]
-
-                if not cost:
-                    h = pbkdf2_hmac(args, byte_password, prov_salt, DEFAULT_ITERATIONS).hex()
-                    actual_method = f"$pbkdf2:{args}:{DEFAULT_ITERATIONS}"
-                    return f"{actual_method}${prov_salt.decode('utf-8')}${h}"
-                else:
-                    h = pbkdf2_hmac(args, byte_password, prov_salt, cost).hex()  # specified number of rounds
-                    actual_method = f"$pbkdf2:{args}:{cost}"
-                    return f"{actual_method}${prov_salt.decode('utf-8')}${h}"
-
-        elif self.algorithm == "bcrypt":
-            from bcrypt import hashpw, gensalt
-            DEFAULT_ITERATIONS = 13  # 2^13
-            if not cost:
-                return f"$bcrypt{hashpw(password.encode('utf-8'), gensalt(DEFAULT_ITERATIONS)).decode('utf-8')}"
-            else:
-                return f"$bcrypt{hashpw(password.encode('utf-8'), gensalt(cost)).decode('utf-8')}"
-
-        elif self.algorithm == "scrypt":
-            from scrypt import hash
-            from secrets import choice
-            SALT_CHARS = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
-            DEFAULT_ITERATIONS = 14  # 2^14
-            if not prov_salt:
-                # Generating a random salt and encoding it to bytes
-                salt = "".join(choice(SALT_CHARS) for _ in range(16)).encode("utf-8")
-                byte_password = password.encode("utf-8")
-
-                if not cost:
-                    hashed = hash(byte_password, salt).hex()
-                    return f"$scrypt$N={DEFAULT_ITERATIONS}$r=8$p=1${salt.decode('utf-8')}${hashed}"
-                else:
-                    hashed = hash(byte_password, salt, N=1 << cost).hex()
-                    return f"$scrypt$N={cost}$r=8$p=1${salt.decode('utf-8')}${hashed}"
-
-            else:
-                byte_password = password.encode("utf-8")
-                if not cost:
-                    hashed = hash(byte_password, prov_salt).hex()
-                    return f"$scrypt$N={DEFAULT_ITERATIONS}$r=8$p=1${prov_salt.decode('utf-8')}${hashed}"
-                else:
-                    hashed = hash(byte_password, prov_salt, N=1 << cost).hex()
-                    return f"$scrypt$N={cost}$r=8$p=1${prov_salt.decode('utf-8')}${hashed}"
-
-        else:
-            return f"We don't support '{self.algorithm}' method yet. \n" \
-                   f"Here are the supported methods : {self.supported_hash_methods}"
-
-    def check_password_hash(self, secret: str, password: str):
-        """
-        Checks a plain text password against a provides hash of a supported algorithm
-        see supported_hash_types.
-        :param secret: hash digest of a certain algorithm
-        :param password: Plain-text password
-        :return: True or False (password is correct or not)
-        """
-        if "$argon" in secret:
-            from argon2 import PasswordHasher, exceptions
-            crypt_er = PasswordHasher()
-            try:
-                return crypt_er.verify(secret, password)
-            except exceptions.VerifyMismatchError:
-                return False
-
-        elif "$pbkdf2" in secret:
-            method, prov_salt, hashval = secret[1:].split("$", 2)
-            import hmac
-            return hmac.compare_digest(
-                self.generate_password_hash(password,
-                                            cost=int(method.split(":")[2]),
-                                            prov_salt=prov_salt.encode("utf-8"))[1:].split("$", 2)[2],
-                hashval
-            )
-
-        elif "$bcrypt" in secret:
-            from bcrypt import hashpw
-            salt = f"$2b${secret[11:13]}${secret[14:]}".encode("utf-8")
-            hashed = f'$bcrypt{hashpw(password.encode("utf-8"), salt).decode("utf-8")}'
-            return secret == hashed
-
-        elif "$scrypt" in secret:
-            from scrypt import hash
-            secret_data = secret[1:].split("$")
-            hashed, prov_salt = secret_data[5], secret_data[4].encode('utf-8')
-            return hashed == self.generate_password_hash(password,
-                                                         cost=int(secret_data[1][2:]),
-                                                         prov_salt=prov_salt)[1:].split("$")[5]
-
-        else:
-            raise TypeError("Unsupported Hash-Type\nTry using the following\n"
-                            f"{self.supported_hash_methods}")
-
-
-if __name__ == '__main__':
-
-    hashes_to_hashes = PassHashing("argon2id")
-    # This section illustrates common errors and their work-around
-    # If you provide a hash digest which is not recognized Type error will be raised
-    # check_hash("NOTRECOGNIZED", 1234567890)
-
-    """
-    Traceback (most recent call last):
-        raise TypeError("Unsupported Hash-Type\nTry using the following\n"
-    TypeError: Unsupported Hash-Type
-    Try using the following
-    ['argon2id', 'pbkdf2:sha1', 'pbkdf2:sha224', 'pbkdf2:sha256', 'pbkdf2:sha384', 'pbkdf2:sha512', 'bcrypt', 'scrypt']
-    """
-
-    # You can catch the above exception like so:
-
-    try:
-        hashes_to_hashes.check_password_hash("NOTRECOGNIZED", 1234567890)
-    except TypeError as e:
-        print(e, "\n")
-
-    # You can print Supported list on demand like so:
-
-    print("Supported Hash Methods: \n", hashes_to_hashes.supported_hash_methods)
-
-    # See <https://github.com/Theorist-Git/AuthAlpha> for tutorials.
+"""
+Copyright (C) 2021-2023 Mayank Vats
+See license.txt
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License v3
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+__author__ = "Mayank Vats"
+__email__ = "dev-theorist.e5xna@simplelogin.com"
+__Description__ = "AuthAlpha: A package to manage Hashing and OTP generation."
+__version__ = "0.8.4alpha"
+
+"""
+
+
+class PassHashing:
+
+    def __init__(self, algorithm):
+        self.algorithm = algorithm
+        self.supported_hash_methods = [
+            "argon2id",
+            "pbkdf2:sha1",
+            "pbkdf2:sha224",
+            "pbkdf2:sha256",
+            "pbkdf2:sha384",
+            "pbkdf2:sha512",
+            "bcrypt",
+            "scrypt"
+        ]
+
+    def __repr__(self):
+        return "PassHashing('{}')".format(self.algorithm)
+
+    def __str__(self):
+        return f"\033[1mPassword Hashing Class [PassHashing]\033[0m. \033[92mAlgorithm:\033[0m \033[1m{self.algorithm}\033[0m "
+
+    def generate_password_hash(self, password: str, cost: int = None, prov_salt: bytes = None):
+        """
+        :param cost: Specify number of iterations for a certain algorithm,
+        default values are chosen sensibly, but you can still change them.
+        (NOT APPLICABLE FOR ARGON2ID(TBD))
+        :param password: type(password) is str
+        :param prov_salt: (optional) provide a bytes-like salt for hashing
+        only applicable for pbkdf2 hashes.
+        :return: str(hash)
+        This method generates a hash pertaining to a specified algorithm,
+        see supported_hash_algorithms.
+        """
+
+        if self.algorithm == "argon2id":
+            from argon2 import PasswordHasher
+            crypt_er = PasswordHasher()
+            return crypt_er.hash(password)
+
+        elif self.algorithm.startswith("pbkdf2:"):
+            from secrets import choice
+            from hashlib import pbkdf2_hmac
+            SALT_CHARS = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
+            DEFAULT_ITERATIONS = 300000
+
+            if not prov_salt:
+                # Generating a random salt and encoding it to bytes
+                salt = "".join(choice(SALT_CHARS) for _ in range(16)).encode("utf-8")
+                # Type-casting the inputted password to string and then encoding it to bytes.
+                byte_password = password.encode("utf-8")
+                args = self.algorithm.split(":")[1]
+
+                # Default rounds of pbkdf2
+                if not cost:
+                    h = pbkdf2_hmac(args, byte_password, salt, DEFAULT_ITERATIONS).hex()
+                    actual_method = f"$pbkdf2:{args}:{DEFAULT_ITERATIONS}"
+                    return f"{actual_method}${salt.decode('utf-8')}${h}"
+
+                # Custom rounds of pbkdf2
+                else:
+                    h = pbkdf2_hmac(args, byte_password, salt, cost).hex()  # specified number of rounds
+                    actual_method = f"$pbkdf2:{args}:{cost}"
+                    return f"{actual_method}${salt.decode('utf-8')}${h}"
+
+            else:
+                # In-case the user provides a salt, hashing is done using it. type(salt) is bytes
+                byte_password = password.encode("utf-8")
+                args = self.algorithm.split(":")[1]
+
+                if not cost:
+                    h = pbkdf2_hmac(args, byte_password, prov_salt, DEFAULT_ITERATIONS).hex()
+                    actual_method = f"$pbkdf2:{args}:{DEFAULT_ITERATIONS}"
+                    return f"{actual_method}${prov_salt.decode('utf-8')}${h}"
+                else:
+                    h = pbkdf2_hmac(args, byte_password, prov_salt, cost).hex()  # specified number of rounds
+                    actual_method = f"$pbkdf2:{args}:{cost}"
+                    return f"{actual_method}${prov_salt.decode('utf-8')}${h}"
+
+        elif self.algorithm == "bcrypt":
+            from bcrypt import hashpw, gensalt
+            DEFAULT_ITERATIONS = 13  # 2^13
+
+            if not prov_salt:
+                if not cost:
+                    return f"$bcrypt{hashpw(password.encode('utf-8'), gensalt(DEFAULT_ITERATIONS)).decode('utf-8')}"
+                else:
+                    return f"$bcrypt{hashpw(password.encode('utf-8'), gensalt(cost)).decode('utf-8')}"
+            elif prov_salt:
+                if prov_salt.endswith(b".") or prov_salt.endswith(b"O") or prov_salt.endswith(b"e") or prov_salt.endswith(b"u"):
+                    return f"$bcrypt{hashpw(password.encode('utf-8'), prov_salt).decode('utf-8')}"
+                else:
+                    raise(TypeError("Invalid Salt\n(AuthAlpha): The salt must end with '.', 'O', "
+                                    "'e' or 'u' in bcrypt. See https://github.com/Theorist-Git/AuthAlpha/commit/b00b7ce1b33c64d61da85ea2b657617008f16abe"))
+
+        elif self.algorithm == "scrypt":
+            from scrypt import hash
+            from secrets import choice
+            SALT_CHARS = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
+            DEFAULT_ITERATIONS = 14  # 2^14
+            if not prov_salt:
+                # Generating a random salt and encoding it to bytes
+                salt = "".join(choice(SALT_CHARS) for _ in range(16)).encode("utf-8")
+                byte_password = password.encode("utf-8")
+
+                if not cost:
+                    hashed = hash(byte_password, salt).hex()
+                    return f"$scrypt$N={DEFAULT_ITERATIONS}$r=8$p=1${salt.decode('utf-8')}${hashed}"
+                else:
+                    hashed = hash(byte_password, salt, N=1 << cost).hex()
+                    return f"$scrypt$N={cost}$r=8$p=1${salt.decode('utf-8')}${hashed}"
+
+            else:
+                byte_password = password.encode("utf-8")
+                if not cost:
+                    hashed = hash(byte_password, prov_salt).hex()
+                    return f"$scrypt$N={DEFAULT_ITERATIONS}$r=8$p=1${prov_salt.decode('utf-8')}${hashed}"
+                else:
+                    hashed = hash(byte_password, prov_salt, N=1 << cost).hex()
+                    return f"$scrypt$N={cost}$r=8$p=1${prov_salt.decode('utf-8')}${hashed}"
+
+        else:
+            return f"We don't support '{self.algorithm}' method yet. \n" \
+                   f"Here are the supported methods : {self.supported_hash_methods}"
+
+    def check_password_hash(self, secret: str, password: str):
+        """
+        Checks a plain text password against a provides hash of a supported algorithm
+        see supported_hash_types
+        :param secret: hash digest of a certain algorithm
+        :param password: Plain-text password
+        :return: True or False (password is correct or not)
+        """
+        if "$argon" in secret:
+            from argon2 import PasswordHasher, exceptions
+            crypt_er = PasswordHasher()
+            try:
+                return crypt_er.verify(secret, password)
+            except exceptions.VerifyMismatchError:
+                return False
+
+        elif "$pbkdf2" in secret:
+            method, prov_salt, hashval = secret[1:].split("$", 2)
+            import hmac
+            return hmac.compare_digest(
+                self.generate_password_hash(password,
+                                            cost=int(method.split(":")[2]),
+                                            prov_salt=prov_salt.encode("utf-8"))[1:].split("$", 2)[2],
+                hashval
+            )
+
+        elif "$bcrypt" in secret:
+            from bcrypt import hashpw
+            hash_data = secret[1:].split("$")
+            salt = f"${hash_data[1]}${hash_data[2]}${hash_data[3][:22]}".encode("utf-8")
+            hashed = self.generate_password_hash(password, prov_salt=salt)
+            return secret == hashed
+
+        elif "$scrypt" in secret:
+            from scrypt import hash
+            secret_data = secret[1:].split("$")
+            hashed, prov_salt = secret_data[5], secret_data[4].encode('utf-8')
+            return hashed == self.generate_password_hash(password,
+                                                         cost=int(secret_data[1][2:]),
+                                                         prov_salt=prov_salt)[1:].split("$")[5]
+
+        else:
+            raise TypeError("Unsupported Hash-Type\nTry using the following\n"
+                            f"{self.supported_hash_methods}")
+
+
+if __name__ == '__main__':
+
+    hashes_to_hashes = PassHashing("argon2id")
+    # This section illustrates common errors and their work-around
+    # If you provide a hash digest which is not recognized Type error will be raised
+    # check_hash("NOTRECOGNIZED", 1234567890)
+    print(hashes_to_hashes)
+
+    """
+    Traceback (most recent call last):
+        raise TypeError("Unsupported Hash-Type\nTry using the following\n"
+    TypeError: Unsupported Hash-Type
+    Try using the following
+    ['argon2id', 'pbkdf2:sha1', 'pbkdf2:sha224', 'pbkdf2:sha256', 'pbkdf2:sha384', 'pbkdf2:sha512', 'bcrypt', 'scrypt']
+    """
+
+    # You can catch the above exception like so:
+
+    try:
+        hashes_to_hashes.check_password_hash("NOTRECOGNIZED", str(1234567890))
+    except TypeError as e:
+        print(e, "\n")
+
+    # You can print Supported list on demand like so:
+
+    print("Supported Hash Methods: \n", hashes_to_hashes.supported_hash_methods)
+
+    # See <https://github.com/Theorist-Git/AuthAlpha> for tutorials.
```

### Comparing `AuthAlpha-0.8.2-alpha/AuthAlpha/__init__.py` & `AuthAlpha-0.8.4-alpha/AuthAlpha/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-"""
-Copyright (C) 2021-2022 Mayank Vats
-See license.txt
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License v3
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-__author__ = "Mayank Vats"
-__email__ = "dev-theorist.e5xna@simplelogin.com"
-__Description__ = "AuthAlpha: A package to manage Hashing and OTP generation."
-__version__ = "0.8.2alpha"
-
-"""
-
-from AuthAlpha.Password_Hashing import PassHashing
-from AuthAlpha.Non_Password_Hashing import NonPassHashing
-from AuthAlpha.OTPMethods import TwoFactorAuth
+"""
+Copyright (C) 2021-2023 Mayank Vats
+See license.txt
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License v3
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+__author__ = "Mayank Vats"
+__email__ = "dev-theorist.e5xna@simplelogin.com"
+__Description__ = "AuthAlpha: A package to manage Hashing and OTP generation."
+__version__ = "0.8.4alpha"
+
+"""
+
+from AuthAlpha.Password_Hashing import PassHashing
+from AuthAlpha.Non_Password_Hashing import NonPassHashing
+from AuthAlpha.OTPMethods import TwoFactorAuth
```

### Comparing `AuthAlpha-0.8.2-alpha/PKG-INFO` & `AuthAlpha-0.8.4-alpha/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 1.1
-Name: AuthAlpha
-Version: 0.8.2-alpha
-Summary: A python abstraction to generate and authenticate hashes of passwords and files of any type. The package can also be used to implement classic and Time Based OTPs.
-Home-page: https://github.com/Theorist-Git/AuthAlpha
-Author: Mayank Vats
-Author-email: dev-theorist.e5xna@simplelogin.com
-License: GNU GPLv3
-Download-URL: https://github.com/Theorist-Git/AuthAlpha/archive/refs/tags/v0.8.2-alpha.tar.gz
-Description: UNKNOWN
-Keywords: AUTHENTICATION,CRYPTOGRAPHY,HASHING
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.9
+Metadata-Version: 1.1
+Name: AuthAlpha
+Version: 0.8.4-alpha
+Summary: A python abstraction to generate and authenticate hashes of passwords and files of any type. The package can also be used to implement classic and Time Based OTPs.
+Home-page: https://github.com/Theorist-Git/AuthAlpha
+Author: Mayank Vats
+Author-email: dev-theorist.e5xna@simplelogin.com
+License: GNU GPLv3
+Download-URL: https://github.com/Theorist-Git/AuthAlpha/archive/refs/tags/v0.8.4-alpha.tar.gz
+Description: UNKNOWN
+Keywords: AUTHENTICATION,CRYPTOGRAPHY,HASHING
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
```

### Comparing `AuthAlpha-0.8.2-alpha/setup.py` & `AuthAlpha-0.8.4-alpha/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from distutils.core import setup
 
 setup(
     name='AuthAlpha',
     packages=['AuthAlpha'],
-    version='0.8.2-alpha',
+    version='0.8.4-alpha',
     license='GNU GPLv3',
     description='A python abstraction to generate and authenticate hashes of passwords and files of any type. The '
                 'package can also be used to implement classic and Time Based OTPs.',
     author='Mayank Vats',
     author_email='dev-theorist.e5xna@simplelogin.com',
     url='https://github.com/Theorist-Git/AuthAlpha',
-    download_url='https://github.com/Theorist-Git/AuthAlpha/archive/refs/tags/v0.8.2-alpha.tar.gz',
+    download_url='https://github.com/Theorist-Git/AuthAlpha/archive/refs/tags/v0.8.4-alpha.tar.gz',
     keywords=['AUTHENTICATION', 'CRYPTOGRAPHY', 'HASHING'],
     install_requires=[
         'argon2-cffi',
         'bcrypt',
         'scrypt',
-        'pyotp'
+        'pyotp',
+        'pycryptodome',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         # "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
```

