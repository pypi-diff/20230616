# Comparing `tmp/carto-auth-0.1.0b5.tar.gz` & `tmp/carto-auth-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carto-auth-0.1.0b5.tar", last modified: Thu Nov  3 13:33:58 2022, max compression
+gzip compressed data, was "carto-auth-0.2.0.tar", last modified: Fri Jun 16 07:43:40 2023, max compression
```

## Comparing `carto-auth-0.1.0b5.tar` & `carto-auth-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jesus     (1000) jesus     (1000)        0 2022-11-03 13:33:58.853163 carto-auth-0.1.0b5/
--rw-rw-r--   0 jesus     (1000) jesus     (1000)     2871 2022-11-03 13:33:58.853163 carto-auth-0.1.0b5/PKG-INFO
--rw-rw-r--   0 jesus     (1000) jesus     (1000)     1586 2022-11-03 13:32:09.000000 carto-auth-0.1.0b5/README.md
-drwxrwxr-x   0 jesus     (1000) jesus     (1000)        0 2022-11-03 13:33:58.853163 carto-auth-0.1.0b5/carto_auth/
--rw-rw-r--   0 jesus     (1000) jesus     (1000)      204 2022-09-16 13:13:51.000000 carto-auth-0.1.0b5/carto_auth/__init__.py
--rw-rw-r--   0 jesus     (1000) jesus     (1000)       24 2022-11-03 13:32:09.000000 carto-auth-0.1.0b5/carto_auth/_version.py
--rw-rw-r--   0 jesus     (1000) jesus     (1000)     9170 2022-11-03 13:32:09.000000 carto-auth-0.1.0b5/carto_auth/auth.py
--rw-rw-r--   0 jesus     (1000) jesus     (1000)       44 2022-11-03 13:32:09.000000 carto-auth-0.1.0b5/carto_auth/errors.py
--rw-rw-r--   0 jesus     (1000) jesus     (1000)     8737 2022-11-03 13:32:09.000000 carto-auth-0.1.0b5/carto_auth/pkce.py
--rw-rw-r--   0 jesus     (1000) jesus     (1000)     3542 2022-11-03 13:32:09.000000 carto-auth-0.1.0b5/carto_auth/utils.py
-drwxrwxr-x   0 jesus     (1000) jesus     (1000)        0 2022-11-03 13:33:58.853163 carto-auth-0.1.0b5/carto_auth.egg-info/
--rw-rw-r--   0 jesus     (1000) jesus     (1000)     2871 2022-11-03 13:33:58.000000 carto-auth-0.1.0b5/carto_auth.egg-info/PKG-INFO
--rw-rw-r--   0 jesus     (1000) jesus     (1000)      355 2022-11-03 13:33:58.000000 carto-auth-0.1.0b5/carto_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 jesus     (1000) jesus     (1000)        1 2022-11-03 13:33:58.000000 carto-auth-0.1.0b5/carto_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 jesus     (1000) jesus     (1000)        1 2022-11-03 13:33:58.000000 carto-auth-0.1.0b5/carto_auth.egg-info/not-zip-safe
--rw-rw-r--   0 jesus     (1000) jesus     (1000)       70 2022-11-03 13:33:58.000000 carto-auth-0.1.0b5/carto_auth.egg-info/requires.txt
--rw-rw-r--   0 jesus     (1000) jesus     (1000)       11 2022-11-03 13:33:58.000000 carto-auth-0.1.0b5/carto_auth.egg-info/top_level.txt
--rw-rw-r--   0 jesus     (1000) jesus     (1000)       69 2022-11-03 13:33:58.853163 carto-auth-0.1.0b5/setup.cfg
--rw-rw-r--   0 jesus     (1000) jesus     (1000)     1232 2022-11-03 13:32:09.000000 carto-auth-0.1.0b5/setup.py
+drwxrwxr-x   0 jesus     (1000) jesus     (1000)        0 2023-06-16 07:43:40.314641 carto-auth-0.2.0/
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)     2971 2023-06-16 07:43:40.314641 carto-auth-0.2.0/PKG-INFO
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)     1651 2022-11-07 15:46:47.000000 carto-auth-0.2.0/README.md
+drwxrwxr-x   0 jesus     (1000) jesus     (1000)        0 2023-06-16 07:43:40.314641 carto-auth-0.2.0/carto_auth/
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)      204 2022-11-07 15:46:47.000000 carto-auth-0.2.0/carto_auth/__init__.py
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)       22 2023-06-16 07:10:58.000000 carto-auth-0.2.0/carto_auth/_version.py
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)     9628 2023-06-16 07:15:35.000000 carto-auth-0.2.0/carto_auth/auth.py
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)       44 2022-11-07 15:46:47.000000 carto-auth-0.2.0/carto_auth/errors.py
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)     8935 2023-06-16 07:16:22.000000 carto-auth-0.2.0/carto_auth/pkce.py
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)     3561 2023-06-16 07:10:58.000000 carto-auth-0.2.0/carto_auth/utils.py
+drwxrwxr-x   0 jesus     (1000) jesus     (1000)        0 2023-06-16 07:43:40.314641 carto-auth-0.2.0/carto_auth.egg-info/
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)     2971 2023-06-16 07:43:40.000000 carto-auth-0.2.0/carto_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)      355 2023-06-16 07:43:40.000000 carto-auth-0.2.0/carto_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)        1 2023-06-16 07:43:40.000000 carto-auth-0.2.0/carto_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)        1 2023-06-16 07:43:40.000000 carto-auth-0.2.0/carto_auth.egg-info/not-zip-safe
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)       70 2023-06-16 07:43:40.000000 carto-auth-0.2.0/carto_auth.egg-info/requires.txt
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)       11 2023-06-16 07:43:40.000000 carto-auth-0.2.0/carto_auth.egg-info/top_level.txt
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)       69 2023-06-16 07:43:40.314641 carto-auth-0.2.0/setup.cfg
+-rw-rw-r--   0 jesus     (1000) jesus     (1000)     1245 2022-11-07 15:46:47.000000 carto-auth-0.2.0/setup.py
```

### Comparing `carto-auth-0.1.0b5/PKG-INFO` & `carto-auth-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carto-auth
-Version: 0.1.0b5
+Version: 0.2.0
 Summary: Python library to authenticate with CARTO
 Home-page: https://github.com/cartodb/carto-auth
 Author: CARTO
 Author-email: jarroyo@carto.com
 License: BSD 3-Clause
 Description: # carto-auth
         
@@ -39,14 +39,17 @@
         ```py
         from carto_auth import CartoAuth
         
         # Authentication
         carto_auth = CartoAuth.from_oauth()
         # carto_auth = CartoAuth.from_m2m("./carto_credentials.json")
         
+        # Get api base url
+        api_base_url = carto_auth.get_api_base_url()
+        
         # Get access token
         access_token = carto_auth.get_access_token()
         
         # CARTO Data Warehouse
         carto_dw_project, carto_dw_token = carto_auth.get_carto_dw_credentials()
         carto_dw_client = carto_auth.get_carto_dw_client()
         ```
@@ -70,15 +73,15 @@
         ## Contributors
         
         - [Jesús Arroyo](https://github.com/jesus89)
         - [Óscar Ramírez](https://github.com/tuxskar)
         
 Keywords: carto,auth,oauth,carto-dw,bigquery
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `carto-auth-0.1.0b5/README.md` & `carto-auth-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 ```py
 from carto_auth import CartoAuth
 
 # Authentication
 carto_auth = CartoAuth.from_oauth()
 # carto_auth = CartoAuth.from_m2m("./carto_credentials.json")
 
+# Get api base url
+api_base_url = carto_auth.get_api_base_url()
+
 # Get access token
 access_token = carto_auth.get_access_token()
 
 # CARTO Data Warehouse
 carto_dw_project, carto_dw_token = carto_auth.get_carto_dw_credentials()
 carto_dw_client = carto_auth.get_carto_dw_client()
 ```
```

### Comparing `carto-auth-0.1.0b5/carto_auth/auth.py` & `carto-auth-0.2.0/carto_auth/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,32 +29,35 @@
             provided by CARTO.
         cache_filepath (str, optional): File path where the token is stored.
             Default "home()/.carto-auth/token.json".
         use_cache (bool, optional): Whether the stored cached token should be used.
             Default True.
         open_browser (bool, optional): Whether the web browser should be opened
             to authorize a user. Default True.
+        org (str, optional): Single Sign-On (SSO) organization in CARTO.
     """
 
     def __init__(
         self,
         mode,
         api_base_url=None,
         access_token=None,
         expiration=None,
         client_id=None,
         client_secret=None,
         cache_filepath=None,
         use_cache=True,
         open_browser=True,
+        org=None,
     ):
         self._mode = mode
         self._api_base_url = api_base_url
         self._cache_filepath = cache_filepath
         self._use_cache = use_cache
+        self._org = org
 
         if mode == "oauth":
             self._access_token = access_token
             self._expiration = expiration
             self._open_browser = open_browser
         elif mode == "m2m":
             self._access_token = access_token
@@ -68,24 +71,28 @@
 
     @classmethod
     def from_oauth(
         cls,
         cache_filepath=None,
         use_cache=True,
         open_browser=True,
+        api_base_url=None,
+        org=None,
     ):
         """Create a CartoAuth object using OAuth with CARTO.
 
         Args:
             cache_filepath (str, optional): File path where the token is stored.
                 Default "home()/.carto-auth/token_oauth.json".
             use_cache (bool, optional): Whether the stored cached token should be used.
                 Default True.
             open_browser (bool, optional): Whether the web browser should be opened
                 to authorize a user. Default True.
+            api_base_url (str, optional): Base URL for a CARTO account.
+            org (str, optional): Single Sign-On (SSO) organization in CARTO.
         """
         mode = "oauth"
 
         if cache_filepath is None:
             cache_filepath = get_cache_filepath(mode)
 
         if use_cache:
@@ -99,25 +106,27 @@
                     mode=mode,
                     api_base_url=data.get("api_base_url"),
                     access_token=data.get("access_token"),
                     expiration=data.get("expiration"),
                     cache_filepath=cache_filepath,
                     use_cache=use_cache,
                     open_browser=open_browser,
+                    org=org,
                 )
 
-        data = get_oauth_token_info(open_browser)
+        data = get_oauth_token_info(open_browser, org)
         return cls(
             mode=mode,
-            api_base_url=get_api_base_url(data.get("access_token")),
+            api_base_url=api_base_url or get_api_base_url(data.get("access_token")),
             access_token=data.get("access_token"),
             expiration=data.get("expiration"),
             cache_filepath=cache_filepath,
             use_cache=use_cache,
             open_browser=open_browser,
+            org=org,
         )
 
     @classmethod
     def from_m2m(cls, filepath, cache_filepath=None, use_cache=True):
         """Create a CartoAuth object using CARTO credentials file.
 
         Args:
@@ -176,21 +185,24 @@
             expiration=data.get("expiration"),
             client_id=client_id,
             client_secret=client_secret,
             cache_filepath=cache_filepath,
             use_cache=use_cache,
         )
 
+    def get_api_base_url(self):
+        return self._api_base_url
+
     def get_access_token(self):
         if self._access_token and not is_token_expired(self._expiration):
             return self._access_token
 
         # Token expired
         if self._mode == "oauth":
-            data = get_oauth_token_info(self._open_browser)
+            data = get_oauth_token_info(self._open_browser, self._org)
         elif self._mode == "m2m":
             data = get_m2m_token_info(self._client_id, self._client_secret)
 
         self._access_token = data.get("access_token")
         self._expiration = data.get("expiration")
         self._save_cache_file()
```

### Comparing `carto-auth-0.1.0b5/carto_auth/pkce.py` & `carto-auth-0.2.0/carto_auth/pkce.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,27 +25,30 @@
 
 class CartoPKCE:
     """Implements PKCE Authorization Flow for client apps."""
 
     def __init__(
         self,
         open_browser=True,
+        org=None,
     ):
         """Creates PKCE Auth flow.
 
         Args:
             open_browser (bool, optional): Whether the web browser should be opened
                 to authorize a user. Default True, except when using Google Colab
                 or Databricks.
+            org (str, optional): Single Sign-On (SSO) organization in CARTO.
         """
         using_google_colab = "google.colab" in sys.modules
         using_databricks = "DATABRICKS_RUNTIME_VERSION" in os.environ
         self.open_browser = (
             False if (using_google_colab or using_databricks) else open_browser
         )
+        self.org = org
 
         self.redirect_uri = REDIRECT_URI if self.open_browser else REDIRECT_URI_CLI
 
         self._session = requests.Session()
         self._code_challenge_method = "S256"
         self._code_verifier = None
         self._code_challenge = None
@@ -82,14 +85,16 @@
             "audience": AUDIENCE,
             "redirect_uri": self.redirect_uri,
             "code_challenge_method": self._code_challenge_method,
             "code_challenge": self._code_challenge,
         }
         if state is not None:
             payload["state"] = state
+        if self.org is not None:
+            payload["organization"] = self.org
         urlparams = urlencode(payload)
         return "%s?%s" % (OAUTH_AUTHORIZE_URL, urlparams)
 
     def get_auth_response(self, open_browser=None):
         logger.info(
             "User authentication requires interaction with your "
             "web browser. Once you enter your credentials and "
```

### Comparing `carto-auth-0.1.0b5/carto_auth/utils.py` & `carto-auth-0.2.0/carto_auth/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 def api_headers(access_token):
     return {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {access_token}",
     }
 
 
-def get_oauth_token_info(open_browser=True):
-    carto_pkce = CartoPKCE(open_browser=open_browser)
+def get_oauth_token_info(open_browser=True, org=None):
+    carto_pkce = CartoPKCE(open_browser=open_browser, org=org)
     code = carto_pkce.get_auth_response()
     return carto_pkce.get_token_info(code)
 
 
 def get_m2m_token_info(client_id, client_secret):
     url = "https://auth.carto.com/oauth/token"
     headers = {"Content-Type": "application/x-www-form-urlencoded"}
```

### Comparing `carto-auth-0.1.0b5/carto_auth.egg-info/PKG-INFO` & `carto-auth-0.2.0/carto_auth.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carto-auth
-Version: 0.1.0b5
+Version: 0.2.0
 Summary: Python library to authenticate with CARTO
 Home-page: https://github.com/cartodb/carto-auth
 Author: CARTO
 Author-email: jarroyo@carto.com
 License: BSD 3-Clause
 Description: # carto-auth
         
@@ -39,14 +39,17 @@
         ```py
         from carto_auth import CartoAuth
         
         # Authentication
         carto_auth = CartoAuth.from_oauth()
         # carto_auth = CartoAuth.from_m2m("./carto_credentials.json")
         
+        # Get api base url
+        api_base_url = carto_auth.get_api_base_url()
+        
         # Get access token
         access_token = carto_auth.get_access_token()
         
         # CARTO Data Warehouse
         carto_dw_project, carto_dw_token = carto_auth.get_carto_dw_credentials()
         carto_dw_client = carto_auth.get_carto_dw_client()
         ```
@@ -70,15 +73,15 @@
         ## Contributors
         
         - [Jesús Arroyo](https://github.com/jesus89)
         - [Óscar Ramírez](https://github.com/tuxskar)
         
 Keywords: carto,auth,oauth,carto-dw,bigquery
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `carto-auth-0.1.0b5/setup.py` & `carto-auth-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     url="https://github.com/cartodb/carto-auth",
     license="BSD 3-Clause",
     packages=find_packages(exclude=["examples", "tests"]),
     python_requires=">=3.7",
     install_requires=["requests", "pyyaml"],
     extras_require={"carto-dw": ["google-auth", "google-cloud-bigquery>=2.34.4"]},
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

