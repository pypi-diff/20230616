# Comparing `tmp/flask_signing-0.4.1.tar.gz` & `tmp/flask_signing-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_signing-0.4.1.tar", last modified: Thu Jun 15 19:13:16 2023, max compression
+gzip compressed data, was "flask_signing-0.5.0.tar", last modified: Fri Jun 16 04:29:25 2023, max compression
```

## Comparing `flask_signing-0.4.1.tar` & `flask_signing-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 19:13:16.805594 flask_signing-0.4.1/
--rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.4.1/LICENSE
--rw-rw-r--   0 sig       (1000) sig       (1000)       81 2023-06-14 04:02:03.000000 flask_signing-0.4.1/MANIFEST.in
--rw-rw-r--   0 sig       (1000) sig       (1000)     3890 2023-06-15 19:13:16.805594 flask_signing-0.4.1/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)     3158 2023-06-14 12:49:49.000000 flask_signing-0.4.1/README.md
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 19:13:16.805594 flask_signing-0.4.1/docs/
--rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.4.1/docs/combined.png
--rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.4.1/docs/logo.png
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 19:13:16.805594 flask_signing-0.4.1/flask_signing/
--rw-rw-r--   0 sig       (1000) sig       (1000)    15435 2023-06-15 19:12:13.000000 flask_signing-0.4.1/flask_signing/__init__.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 19:13:16.805594 flask_signing-0.4.1/flask_signing.egg-info/
--rw-rw-r--   0 sig       (1000) sig       (1000)     3890 2023-06-15 19:13:16.000000 flask_signing-0.4.1/flask_signing.egg-info/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)      298 2023-06-15 19:13:16.000000 flask_signing-0.4.1/flask_signing.egg-info/SOURCES.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-15 19:13:16.000000 flask_signing-0.4.1/flask_signing.egg-info/dependency_links.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-15 19:13:16.000000 flask_signing-0.4.1/flask_signing.egg-info/requires.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       20 2023-06-15 19:13:16.000000 flask_signing-0.4.1/flask_signing.egg-info/top_level.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-15 19:13:16.805594 flask_signing-0.4.1/setup.cfg
--rw-rw-r--   0 sig       (1000) sig       (1000)     1237 2023-06-15 19:12:13.000000 flask_signing-0.4.1/setup.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 19:13:16.805594 flask_signing-0.4.1/tests/
--rw-rw-r--   0 sig       (1000) sig       (1000)     9760 2023-06-15 18:29:02.000000 flask_signing-0.4.1/tests/__init__.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-16 04:29:25.418191 flask_signing-0.5.0/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.5.0/LICENSE
+-rw-rw-r--   0 sig       (1000) sig       (1000)       43 2023-06-15 20:25:19.000000 flask_signing-0.5.0/MANIFEST.in
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3890 2023-06-16 04:29:25.418191 flask_signing-0.5.0/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3158 2023-06-16 04:19:42.000000 flask_signing-0.5.0/README.md
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-16 04:29:25.414191 flask_signing-0.5.0/docs/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.5.0/docs/combined.png
+-rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.5.0/docs/logo.png
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-16 04:29:25.414191 flask_signing-0.5.0/flask_signing/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    20631 2023-06-16 04:28:00.000000 flask_signing-0.5.0/flask_signing/__init__.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)      213 2023-06-16 04:19:36.000000 flask_signing-0.5.0/flask_signing/__metadata__.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-16 04:29:25.418191 flask_signing-0.5.0/flask_signing.egg-info/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3890 2023-06-16 04:29:25.000000 flask_signing-0.5.0/flask_signing.egg-info/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)      345 2023-06-16 04:29:25.000000 flask_signing-0.5.0/flask_signing.egg-info/SOURCES.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-16 04:29:25.000000 flask_signing-0.5.0/flask_signing.egg-info/dependency_links.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-16 04:29:25.000000 flask_signing-0.5.0/flask_signing.egg-info/requires.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       20 2023-06-16 04:29:25.000000 flask_signing-0.5.0/flask_signing.egg-info/top_level.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-11 20:04:40.000000 flask_signing-0.5.0/requirements.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-16 04:29:25.418191 flask_signing-0.5.0/setup.cfg
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1587 2023-06-15 20:26:56.000000 flask_signing-0.5.0/setup.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-16 04:29:25.418191 flask_signing-0.5.0/tests/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    11035 2023-06-16 04:16:19.000000 flask_signing-0.5.0/tests/__init__.py
```

### Comparing `flask_signing-0.4.1/LICENSE` & `flask_signing-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_signing-0.4.1/PKG-INFO` & `flask_signing-0.5.0/flask_signing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flask_signing
-Version: 0.4.1
+Name: flask-signing
+Version: 0.5.0
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -61,15 +61,15 @@
 @app.route('/sign')
 def sign():
     key = signatures.write_key_to_database(scope='test', expiration=1, active=True, email='test@example.com')
     return f'Key generated: {key}'
 
 @app.route('/verify/<key>')
 def verify(key):
-    valid = signatures.verify_signature(signature=key, scope='example')
+    valid = signatures.validate_request(signature=key, scope='example')
     return f'Key valid: {valid}'
 
 @app.route('/expire/<key>')
 def expire(key):
     expired = signatures.expire_key(key)
     return f'Key expired: {expired}'
```

### Comparing `flask_signing-0.4.1/README.md` & `flask_signing-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 @app.route('/sign')
 def sign():
     key = signatures.write_key_to_database(scope='test', expiration=1, active=True, email='test@example.com')
     return f'Key generated: {key}'
 
 @app.route('/verify/<key>')
 def verify(key):
-    valid = signatures.verify_signature(signature=key, scope='example')
+    valid = signatures.validate_request(signature=key, scope='example')
     return f'Key valid: {valid}'
 
 @app.route('/expire/<key>')
 def expire(key):
     expired = signatures.expire_key(key)
     return f'Key expired: {expired}'
```

### Comparing `flask_signing-0.4.1/docs/combined.png` & `flask_signing-0.5.0/docs/combined.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.4.1/docs/logo.png` & `flask_signing-0.5.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.4.1/flask_signing/__init__.py` & `flask_signing-0.5.0/flask_signing/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,153 @@
-__name__ = "flask_signing"
-__author__ = "Sig Janoska-Bedi"
-__credits__ = ["Sig Janoska-Bedi",]
-__version__ = "0.4.1"
-__license__ = "BSD-3-Clause"
-__maintainer__ = "Sig Janoska-Bedi"
-__email__ = "signe@atreeus.com"
-
+from .__metadata__ import (__name__, __author__, __credits__, __version__, 
+                       __license__, __maintainer__, __email__)
 import datetime, secrets
+from functools import wraps
 from sqlalchemy import func, literal
 from sqlalchemy.exc import SQLAlchemyError
 from flask_sqlalchemy import SQLAlchemy
 from typing import Union, List, Dict, Any
 
+class RateLimitExceeded(Exception):
+    """
+    An exception that is raised when the request count for a specific signature 
+    exceeds the maximum allowed requests within a specified time period in the 
+    Signatures class.
+
+    This exception is used to signal that the rate limit has been exceeded, so the 
+    calling code can catch this exception and handle it appropriately - for example,
+    by sending an HTTP 429 Too Many Requests response to a client.
+    """
+    pass
+
 class Signatures:
     """
     The Signatures class handles operations related to the creation, management, and validation 
     of signing keys in the database.
     """
     
-    def __init__(self, app, safe_mode:bool=True, byte_len:int=24):
+    def __init__(self, app, safe_mode:bool=True, byte_len:int=24, rate_limiting=False, rate_limiting_max_requests=10, rate_limiting_period=datetime.timedelta(minutes=1)):
         """
         Initializes a new instance of the Signatures class.
 
         Args:
             app (Flask): A flask object to contain the context for database interactions. 
             safe_mode (bool, optional): If safe_mode is enabled, we will prevent rotation of disabled or rotated keys. Defaults to True.
             byte_len (int, optional): The length of the generated signing keys. Defaults to 24.
+            rate_limiting (bool, optional): If rate_limiting is enabled, we will impose key-by-key rate limits. Defaults to False.
+            rate_limiting_max_requests (int, optional): Maximum allowed requests per time period.
+            rate_limiting_period (datetime.timedelta, optional): Time period for rate limiting. Defaults to 1 hour.
         """
 
         self.db = SQLAlchemy(app)
         self.Signing = self.get_model()
         self.db.create_all()  # this will create all necessary tables
 
-        # self.db = database
         self.byte_len = byte_len
+
+        # Set safe mode to prevent disabled/rotated keys from being rotated
         self.safe_mode = safe_mode
 
+        # Set rate limiting attributes
+        self.rate_limiting = rate_limiting
+        self.rate_limiting_max_requests = rate_limiting_max_requests
+        self.rate_limiting_period = rate_limiting_period
+
+    class request_limiter:
+        """
+        A descriptor class that wraps a function with rate limiting logic. This descriptor is meant to 
+        be used as a decorator for methods in the Signatures class.
+
+        If rate limiting is enabled in the Signatures instance, this decorator checks the request count 
+        for the provided signature and raises a `RateLimitExceeded` exception if the count exceeds 
+        the max requests allowed in a set time period. 
+
+        If the time period has passed since the last request, it resets the request count. If the request 
+        count is within limits, it increments the request count and updates the time of the last request.
+
+        If rate limiting is not enabled, the descriptor simply calls the original function.
+
+        Args:
+            func (Callable): The function to wrap with rate limiting logic.
+
+        Returns:
+            wrapper (Callable): The wrapped function which now includes rate limiting logic.
+        """
+
+        def __init__(self, func):
+            self.func = func
+
+        def __get__(self, instance, owner):
+            @wraps(self.func)
+            def wrapper(signature, *args, **kwargs):
+
+                # If rate limiting has not been enabled, then we always return True
+                if not instance.rate_limiting:
+                    return True
+
+                Signing = instance.get_model()
+
+                signing_key = Signing.query.filter_by(signature=signature).first()
+
+                # If the key does not exist
+                if not signing_key:
+                    return False
+
+                # Reset request_count if period has passed since last_request_time
+                if datetime.datetime.utcnow() - signing_key.last_request_time >= instance.rate_limiting_period:
+                    signing_key.request_count = 0
+                    signing_key.last_request_time = datetime.datetime.utcnow()
+
+                # Check if request_count exceeds max_requests
+                if signing_key.request_count >= instance.rate_limiting_max_requests:
+                    raise RateLimitExceeded("Too many requests. Please try again later.")
+
+                # If limit not exceeded, increment request_count and update last_request_time
+                signing_key.request_count += 1
+                signing_key.last_request_time = datetime.datetime.utcnow()
+
+                instance.db.session.commit()
+
+                return self.func(instance, signature, *args, **kwargs)
+            return wrapper
+
+    @request_limiter
+    def validate_request(self, signature, scope):
+        """
+        Validates a request by verifying the given signing key against a specific scope.
+        
+        This function wraps the `verify_signature` function with rate limiting support. 
+        If rate limiting is enabled, it checks whether the request count for the signature 
+        has exceeded the maximum allowed requests within the specified time period.
+        
+        If the rate limit is exceeded, it raises a `RateLimitExceeded` exception and returns False.
+        If the rate limit is not exceeded, it calls the `verify_signature` function to verify the key.
+        
+        Args:
+            signature (str): The signing key to be verified.
+            scope (str): The scope against which the signing key will be validated.
+
+        Returns:
+            bool: True if the signing key is valid and hasn't exceeded rate limit, False otherwise.
+
+        Raises:
+            RateLimitExceeded: If the number of requests with this signing key exceeds 
+            the maximum allowed within the specified time period.
+        """
+
+        try:
+            valid = self.verify_signature(signature, scope)
+        except RateLimitExceeded as e:
+            print(e)  # Or handle the exception in some other way
+            return False
+
+        return valid
+
+
+
     def generate_key(self, length:int=None) -> str:
         """
         Generates a signing key with the specified byte length. 
         Note: byte length generally translates to about 1.3 times as many chars,
         see https://docs.python.org/3/library/secrets.html.
 
         Args:
@@ -200,14 +308,16 @@
                 email = self.db.Column(self.db.String(100)) 
                 # scope = self.db.Column(self.db.String(100))
                 # scope = self.db.Column(self.db.MutableList.as_mutable(self.db.String(100)), default=[]),
                 scope = self.db.Column(self.db.JSON())
                 active = self.db.Column(self.db.Boolean)
                 timestamp = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
                 expiration = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
+                request_count = self.db.Column(self.db.Integer, default=0)
+                last_request_time = self.db.Column(self.db.DateTime, default=datetime.datetime.utcnow)
                 # previous_key = self.db.Column(self.db.String(1000), db.ForeignKey('signing.signature'))
                 previous_key = self.db.Column(self.db.String(1000), self.db.ForeignKey('signing.signature'), nullable=True)
                 rotated = self.db.Column(self.db.Boolean)
                 # parent = db.relationship("Signing", remote_side=[signature]) # self referential relationship
                 children = self.db.relationship('Signing', backref=self.db.backref('parent', remote_side=[signature])) # self referential relationship
 
             self._model = Signing
```

### Comparing `flask_signing-0.4.1/flask_signing.egg-info/PKG-INFO` & `flask_signing-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flask-signing
-Version: 0.4.1
+Name: flask_signing
+Version: 0.5.0
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -61,15 +61,15 @@
 @app.route('/sign')
 def sign():
     key = signatures.write_key_to_database(scope='test', expiration=1, active=True, email='test@example.com')
     return f'Key generated: {key}'
 
 @app.route('/verify/<key>')
 def verify(key):
-    valid = signatures.verify_signature(signature=key, scope='example')
+    valid = signatures.validate_request(signature=key, scope='example')
     return f'Key valid: {valid}'
 
 @app.route('/expire/<key>')
 def expire(key):
     expired = signatures.expire_key(key)
     return f'Key expired: {expired}'
```

### Comparing `flask_signing-0.4.1/tests/__init__.py` & `flask_signing-0.5.0/tests/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import os, datetime, unittest
+import os, datetime, unittest, time
 from flask import Flask
 from flask_sqlalchemy import SQLAlchemy
-from flask_signing import Signatures
+from flask_signing import Signatures, RateLimitExceeded
 
 class TestFlaskSigning(unittest.TestCase):
 
     def setUp(self):
         """
         Set up testing environment.
         """
@@ -210,9 +210,41 @@
 
             # Get the new key that replaced the late_expire_key
             new_late_expire_key = Signing.query.filter_by(previous_key=late_expire_key).first()
             # Check that the new key's previous_key is the old key
             self.assertEqual(new_late_expire_key.previous_key, late_expire_key)
 
 
+    def test_rate_limiting(self):
+        """
+        Test rate limiting functionality
+        """
+
+        with self.app.app_context():
+            # Enable rate limiting
+            self.signatures.rate_limiting = True
+            self.signatures.rate_limiting_max_requests = 2
+            self.signatures.rate_limiting_period = datetime.timedelta(seconds=2)
+
+            # Generate a signature
+            scope = ['example']
+            signature = self.signatures.write_key_to_database(scope=scope, active=True)
+
+            # Validate the key once, should return True
+            self.assertTrue(self.signatures.validate_request(signature, scope))
+
+            # Validate the key twice, should return True
+            self.assertTrue(self.signatures.validate_request(signature, scope))
+
+            # Now we expect a RateLimitExceeded exception because we are exceeding the rate limit
+            with self.assertRaises(RateLimitExceeded):
+                self.assertTrue(self.signatures.validate_request(signature, scope))
+
+            # Wait for the rate limit period to pass
+            time.sleep(2)
+
+            # Validate the key again, should return True
+            self.assertTrue(self.signatures.validate_request(signature, scope))
+
+
 if __name__ == '__main__':
     unittest.main()
```

