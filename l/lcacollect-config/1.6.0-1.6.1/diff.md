# Comparing `tmp/lcacollect_config-1.6.0.tar.gz` & `tmp/lcacollect_config-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcacollect_config-1.6.0.tar", max compression
+gzip compressed data, was "lcacollect_config-1.6.1.tar", max compression
```

## Comparing `lcacollect_config-1.6.0.tar` & `lcacollect_config-1.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    10173 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/LICENSE
--rw-r--r--   0        0        0     1462 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/README.md
--rw-r--r--   0        0        0     2520 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/__init__.py
--rw-r--r--   0        0        0     2831 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/config.py
--rw-r--r--   0        0        0     1507 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/connection.py
--rw-r--r--   0        0        0      372 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/context.py
--rw-r--r--   0        0        0     2835 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/email.py
--rw-r--r--   0        0        0      263 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/exceptions.py
--rw-r--r--   0        0        0      637 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/fastapi.py
--rw-r--r--   0        0        0      597 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/formatting.py
--rw-r--r--   0        0        0        0 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/graphql/__init__.py
--rw-r--r--   0        0        0     2772 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/graphql/input_filters.py
--rw-r--r--   0        0        0     1270 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/graphql/pagination.py
--rw-r--r--   0        0        0      400 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/permissions.py
--rw-r--r--   0        0        0     1043 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/router.py
--rw-r--r--   0        0        0      535 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/security.py
--rw-r--r--   0        0        0     5079 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/user.py
--rw-r--r--   0        0        0     2634 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/validate.py
--rw-r--r--   0        0        0     2537 1970-01-01 00:00:00.000000 lcacollect_config-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/LICENSE
+-rw-r--r--   0        0        0     1462 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/README.md
+-rw-r--r--   0        0        0     2521 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/__init__.py
+-rw-r--r--   0        0        0     2831 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/config.py
+-rw-r--r--   0        0        0     1507 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/connection.py
+-rw-r--r--   0        0        0      372 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/context.py
+-rw-r--r--   0        0        0     2835 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/email.py
+-rw-r--r--   0        0        0      263 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/exceptions.py
+-rw-r--r--   0        0        0      637 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/fastapi.py
+-rw-r--r--   0        0        0      597 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/formatting.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/graphql/__init__.py
+-rw-r--r--   0        0        0     2772 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/graphql/input_filters.py
+-rw-r--r--   0        0        0     1270 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/graphql/pagination.py
+-rw-r--r--   0        0        0      400 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/permissions.py
+-rw-r--r--   0        0        0     1043 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/router.py
+-rw-r--r--   0        0        0      535 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/security.py
+-rw-r--r--   0        0        0     5079 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/user.py
+-rw-r--r--   0        0        0     2634 2023-06-16 11:32:19.190830 lcacollect_config-1.6.1/src/lcacollect_config/validate.py
+-rw-r--r--   0        0        0     2537 1970-01-01 00:00:00.000000 lcacollect_config-1.6.1/PKG-INFO
```

### Comparing `lcacollect_config-1.6.0/LICENSE` & `lcacollect_config-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.6.0/README.md` & `lcacollect_config-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.6.0/pyproject.toml` & `lcacollect_config-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lcacollect-config"
-version = "1.6.0"
+version = "1.6.1"
 description = "This package contains shared config and utils to be used across LCAcollect backends."
 authors = ["Christian Kongsgaard <chrk@arkitema.com>"]
 repository = "https://github.com/lcacollect/shared-config-backend"
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -83,8 +83,8 @@
     "DEFAULT_AD_FQDN=PLACEHOLDER",
     "SENDGRID_SECRET=c2VjcmV0",
     "EMAIL_NOTIFICATION_FROM=no-reply@arkitema.com",  # no-reply@molio.com
     "INTERNAL_EMAIL_DOMAINS_LIST=arkitema,cowi,cowicloud",
 ]
 
 [tool.coverage.run]
-omit=["src/exceptions/*.py"]
+omit=["src/exceptions/*.py"]
```

### Comparing `lcacollect_config-1.6.0/src/lcacollect_config/config.py` & `lcacollect_config-1.6.1/src/lcacollect_config/config.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.6.0/src/lcacollect_config/connection.py` & `lcacollect_config-1.6.1/src/lcacollect_config/connection.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.6.0/src/lcacollect_config/email.py` & `lcacollect_config-1.6.1/src/lcacollect_config/email.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.6.0/src/lcacollect_config/fastapi.py` & `lcacollect_config-1.6.1/src/lcacollect_config/fastapi.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.6.0/src/lcacollect_config/formatting.py` & `lcacollect_config-1.6.1/src/lcacollect_config/formatting.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.6.0/src/lcacollect_config/graphql/input_filters.py` & `lcacollect_config-1.6.1/src/lcacollect_config/graphql/input_filters.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.6.0/src/lcacollect_config/graphql/pagination.py` & `lcacollect_config-1.6.1/src/lcacollect_config/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.6.0/src/lcacollect_config/router.py` & `lcacollect_config-1.6.1/src/lcacollect_config/router.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.6.0/src/lcacollect_config/security.py` & `lcacollect_config-1.6.1/src/lcacollect_config/security.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.6.0/src/lcacollect_config/user.py` & `lcacollect_config-1.6.1/src/lcacollect_config/user.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.6.0/src/lcacollect_config/validate.py` & `lcacollect_config-1.6.1/src/lcacollect_config/validate.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.6.0/PKG-INFO` & `lcacollect_config-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcacollect-config
-Version: 1.6.0
+Version: 1.6.1
 Summary: This package contains shared config and utils to be used across LCAcollect backends.
 Home-page: https://github.com/lcacollect/shared-config-backend
 License: Apache-2.0
 Author: Christian Kongsgaard
 Author-email: chrk@arkitema.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

