# Comparing `tmp/guardpost-1.0.1.tar.gz` & `tmp/guardpost-1.0.2.tar.gz`

## Comparing `guardpost-1.0.1.tar` & `guardpost-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,20 @@
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 guardpost-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 guardpost-1.0.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 guardpost-1.0.1/.pytest_cache/README.md
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 guardpost-1.0.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 guardpost-1.0.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/__about__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/__init__.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/abc.py
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/authentication.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/authorization.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/common.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/py.typed
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/utils.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/jwks/__init__.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/jwks/caching.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/jwks/openid.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/jwks/urls.py
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 guardpost-1.0.1/guardpost/jwts/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 guardpost-1.0.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 guardpost-1.0.1/LICENSE
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 guardpost-1.0.1/README.md
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 guardpost-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 guardpost-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 guardpost-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/__about__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/__init__.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/abc.py
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/authentication.py
+-rw-r--r--   0        0        0     9232 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/authorization.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/common.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/py.typed
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/utils.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/jwks/__init__.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/jwks/caching.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/jwks/openid.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/jwks/urls.py
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 guardpost-1.0.2/guardpost/jwts/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 guardpost-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 guardpost-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 guardpost-1.0.2/README.md
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 guardpost-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 guardpost-1.0.2/PKG-INFO
```

### Comparing `guardpost-1.0.1/CHANGELOG.md` & `guardpost-1.0.2/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.0.2] - 2023-06-16 :corn:
+- Raises a more specific exception `ForbiddenError` when the user of an
+  operation is authenticated properly, but authorization fails.
+  This enables better handling of authorization error, differentiating when the
+  user context is missing or invalid, and when the context is valid but the
+  user has no rights to do a certain operation. See [#371](https://github.com/Neoteroi/BlackSheep/issues/371).
+
 ## [1.0.1] - 2023-03-20 :sun_with_face:
 - Improves the automatic rotation of `JWKS`: when validating `JWTs`, `JWKS` are
   refreshed automatically if an unknown `kid` is encountered, and `JWKS` were
   last fetched more than `refresh_time` seconds ago (by default 120 seconds).
 - Corrects an inconsistency in how `claims` are read in the `User` class.
 
 ## [1.0.0] - 2023-01-07 :star:
```

### Comparing `guardpost-1.0.1/guardpost/__init__.py` & `guardpost-1.0.2/guardpost/__init__.py`

 * *Files identical despite different names*

### Comparing `guardpost-1.0.1/guardpost/abc.py` & `guardpost-1.0.2/guardpost/abc.py`

 * *Files identical despite different names*

### Comparing `guardpost-1.0.1/guardpost/authentication.py` & `guardpost-1.0.2/guardpost/authentication.py`

 * *Files identical despite different names*

### Comparing `guardpost-1.0.1/guardpost/authorization.py` & `guardpost-1.0.2/guardpost/authorization.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,19 @@
 def _is_async_handler(handler_type: Type[Requirement]) -> bool:
     # Faster alternative to using inspect.iscoroutinefunction without caching
     # Note: this must be used on Types - not instances!
     return inspect.iscoroutinefunction(handler_type.handle)
 
 
 class UnauthorizedError(AuthorizationError):
+    """
+    Error class used for all situations in which a user initiating an operation is not
+    authorized to complete the operation.
+    """
+
     def __init__(
         self,
         forced_failure: Optional[str],
         failed_requirements: Sequence[Requirement],
         scheme: Optional[str] = None,
         error: Optional[str] = None,
         error_description: Optional[str] = None,
@@ -81,14 +86,22 @@
             return (
                 f"The user is not authorized to perform the selected action. "
                 f"Failed requirements: {errors}."
             )
         return "Unauthorized"
 
 
+class ForbiddenError(UnauthorizedError):
+    """
+    A specific kind of authorization error, used to indicate that the application
+    understands a request but refuses to authorize it. In other words, the user context
+    is valid but the user is not authorized to perform a certain operation.
+    """
+
+
 class AuthorizationContext:
     __slots__ = ("identity", "requirements", "_succeeded", "_failed_forced")
 
     def __init__(self, identity: Identity, requirements: Sequence[Requirement]):
         self.identity = identity
         self.requirements = requirements
         self._succeeded: Set[Requirement] = set()
@@ -224,14 +237,18 @@
             for requirement in context.requirements:
                 if _is_async_handler(type(requirement)):  # type: ignore
                     await requirement.handle(context)
                 else:
                     requirement.handle(context)  # type: ignore
 
             if not context.has_succeeded:
+                if identity and identity.is_authenticated():
+                    raise ForbiddenError(
+                        context.forced_failure, context.pending_requirements
+                    )
                 raise UnauthorizedError(
                     context.forced_failure, context.pending_requirements
                 )
 
     async def _handle_with_identity_getter(
         self, policy_name: Optional[str], *args, **kwargs
     ):
```

### Comparing `guardpost-1.0.1/guardpost/common.py` & `guardpost-1.0.2/guardpost/common.py`

 * *Files identical despite different names*

### Comparing `guardpost-1.0.1/guardpost/jwks/__init__.py` & `guardpost-1.0.2/guardpost/jwks/__init__.py`

 * *Files identical despite different names*

### Comparing `guardpost-1.0.1/guardpost/jwks/caching.py` & `guardpost-1.0.2/guardpost/jwks/caching.py`

 * *Files identical despite different names*

### Comparing `guardpost-1.0.1/guardpost/jwks/openid.py` & `guardpost-1.0.2/guardpost/jwks/openid.py`

 * *Files identical despite different names*

### Comparing `guardpost-1.0.1/guardpost/jwks/urls.py` & `guardpost-1.0.2/guardpost/jwks/urls.py`

 * *Files identical despite different names*

### Comparing `guardpost-1.0.1/guardpost/jwts/__init__.py` & `guardpost-1.0.2/guardpost/jwts/__init__.py`

 * *Files identical despite different names*

### Comparing `guardpost-1.0.1/LICENSE` & `guardpost-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `guardpost-1.0.1/README.md` & `guardpost-1.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -32,14 +32,64 @@
 pip install guardpost[jwt]
 ```
 
 ### Examples
 
 For examples, refer to the [examples folder](./examples).
 
+## Functions to validate JWTs
+
+GuardPost includes functions to validate JSON Web Tokens (JWTs) and handle
+JSON Web Keys Sets (JWKS).
+
+The built-in validator class can retrieve automatically JWKS from identity providers
+and handle automatically caching and keys rotation. Caching is useful to not incur in
+useless performance fees (e.g. downloading JWKS at each web request), and keys rotation
+is important because identity providers can periodically change the keys they use to
+sign JWTs.
+
+To use these features, install to include additional dependencies:
+
+```bash
+pip install guardpost[jwt]
+```
+
+The following example shows how to use guardpost to validate tokens:
+
+```python
+import asyncio
+from guardpost.jwts import JWTValidator
+
+
+async def main():
+    validator = JWTValidator(
+        authority="YOUR_AUTHORITY",
+        valid_issuers=["YOUR_ISSUER_VALUE"],
+        valid_audiences=["YOUR_AUDIENCE"],
+    )
+
+    # keys are fetched when necessary
+    data = await validator.validate_jwt("YOUR_TOKEN")
+
+    print(data)
+
+
+asyncio.run(main())
+```
+
+An example value for `authority`, to validate access tokens issued by
+Azure Active Directory could be: `https://sts.windows.net/YOUR_TENANT_ID/`.
+
+GuardPost is used in BlackSheep and has been tested with:
+
+- Auth0
+- Azure Active Directory
+- Azure Active Directory B2C
+- Okta
+
 ## If you have doubts about authentication vs authorization...
 `Authentication` answers the question: _Who is the user who is initiating the
 action?_, or more in general: _Who is the user, or what is the service, that is
 initiating the action?_.
 
 `Authorization` answers the question: _Is the user, or service, authorized to
 do something?_.
```

### Comparing `guardpost-1.0.1/pyproject.toml` & `guardpost-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `guardpost-1.0.1/PKG-INFO` & `guardpost-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guardpost
-Version: 1.0.1
+Version: 1.0.2
 Summary: Framework to handle authentication and authorization.
 Project-URL: Homepage, https://github.com/Neoteroi/GuardPost
 Project-URL: Bug Tracker, https://github.com/Neoteroi/GuardPost/issues
 Author-email: Roberto Prevato <roberto.prevato@gmail.com>
 License-File: LICENSE
 Keywords: authentication,authorization,claims,identity,strategy
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,14 +58,64 @@
 pip install guardpost[jwt]
 ```
 
 ### Examples
 
 For examples, refer to the [examples folder](./examples).
 
+## Functions to validate JWTs
+
+GuardPost includes functions to validate JSON Web Tokens (JWTs) and handle
+JSON Web Keys Sets (JWKS).
+
+The built-in validator class can retrieve automatically JWKS from identity providers
+and handle automatically caching and keys rotation. Caching is useful to not incur in
+useless performance fees (e.g. downloading JWKS at each web request), and keys rotation
+is important because identity providers can periodically change the keys they use to
+sign JWTs.
+
+To use these features, install to include additional dependencies:
+
+```bash
+pip install guardpost[jwt]
+```
+
+The following example shows how to use guardpost to validate tokens:
+
+```python
+import asyncio
+from guardpost.jwts import JWTValidator
+
+
+async def main():
+    validator = JWTValidator(
+        authority="YOUR_AUTHORITY",
+        valid_issuers=["YOUR_ISSUER_VALUE"],
+        valid_audiences=["YOUR_AUDIENCE"],
+    )
+
+    # keys are fetched when necessary
+    data = await validator.validate_jwt("YOUR_TOKEN")
+
+    print(data)
+
+
+asyncio.run(main())
+```
+
+An example value for `authority`, to validate access tokens issued by
+Azure Active Directory could be: `https://sts.windows.net/YOUR_TENANT_ID/`.
+
+GuardPost is used in BlackSheep and has been tested with:
+
+- Auth0
+- Azure Active Directory
+- Azure Active Directory B2C
+- Okta
+
 ## If you have doubts about authentication vs authorization...
 `Authentication` answers the question: _Who is the user who is initiating the
 action?_, or more in general: _Who is the user, or what is the service, that is
 initiating the action?_.
 
 `Authorization` answers the question: _Is the user, or service, authorized to
 do something?_.
```

