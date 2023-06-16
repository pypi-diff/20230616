# Comparing `tmp/sixth-sense-0.0.4.tar.gz` & `tmp/sixth-sense-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sixth-sense-0.0.4.tar", last modified: Wed Jun 14 23:28:02 2023, max compression
+gzip compressed data, was "dist/sixth-sense-0.0.5.tar", last modified: Fri Jun 16 03:36:02 2023, max compression
```

## Comparing `sixth-sense-0.0.4.tar` & `sixth-sense-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/
--rw-r--r--   0 mac        (501) staff       (20)      759 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)       20 2023-06-09 19:50:05.000000 sixth-sense-0.0.4/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     2014 2023-06-14 23:08:33.000000 sixth-sense-0.0.4/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense/
--rw-r--r--   0 mac        (501) staff       (20)       46 2023-06-12 01:09:39.000000 sixth-sense-0.0.4/sixth_sense/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense/middlewares/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-sense-0.0.4/sixth_sense/middlewares/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3715 2023-06-12 02:56:19.000000 sixth-sense-0.0.4/sixth_sense/middlewares/encryption_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-sense-0.0.4/sixth_sense/middlewares/six_base_http_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     3930 2023-06-12 02:55:48.000000 sixth-sense-0.0.4/sixth_sense/middlewares/six_independent_rate_limiter.py
--rw-r--r--   0 mac        (501) staff       (20)     4204 2023-06-14 03:49:11.000000 sixth-sense-0.0.4/sixth_sense/middlewares/six_rate_limiter_middleware.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense/pen_test/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-sense-0.0.4/sixth_sense/pen_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-sense-0.0.4/sixth_sense/pen_test/auto_pen_test.py
--rw-r--r--   0 mac        (501) staff       (20)      624 2023-06-10 23:02:11.000000 sixth-sense-0.0.4/sixth_sense/schemas.py
--rw-r--r--   0 mac        (501) staff       (20)     4191 2023-06-14 20:44:16.000000 sixth-sense-0.0.4/sixth_sense/sixth_sense.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-sense-0.0.4/sixth_sense/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-sense-0.0.4/sixth_sense/utils/encryption_utils.py
--rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-sense-0.0.4/sixth_sense/utils/time_utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      759 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      685 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       12 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 03:36:02.000000 sixth-sense-0.0.5/
+-rw-r--r--   0 mac        (501) staff       (20)     3127 2023-06-16 03:36:02.000000 sixth-sense-0.0.5/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1923 2023-06-16 03:29:15.000000 sixth-sense-0.0.5/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-16 03:36:02.000000 sixth-sense-0.0.5/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     3786 2023-06-16 03:35:41.000000 sixth-sense-0.0.5/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 03:36:02.000000 sixth-sense-0.0.5/sixth_sense/
+-rw-r--r--   0 mac        (501) staff       (20)       46 2023-06-12 01:09:39.000000 sixth-sense-0.0.5/sixth_sense/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 03:36:02.000000 sixth-sense-0.0.5/sixth_sense/middlewares/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-sense-0.0.5/sixth_sense/middlewares/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3715 2023-06-12 02:56:19.000000 sixth-sense-0.0.5/sixth_sense/middlewares/encryption_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-sense-0.0.5/sixth_sense/middlewares/six_base_http_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     3930 2023-06-12 02:55:48.000000 sixth-sense-0.0.5/sixth_sense/middlewares/six_independent_rate_limiter.py
+-rw-r--r--   0 mac        (501) staff       (20)     4215 2023-06-15 05:27:52.000000 sixth-sense-0.0.5/sixth_sense/middlewares/six_rate_limiter_middleware.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 03:36:02.000000 sixth-sense-0.0.5/sixth_sense/pen_test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-sense-0.0.5/sixth_sense/pen_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-sense-0.0.5/sixth_sense/pen_test/auto_pen_test.py
+-rw-r--r--   0 mac        (501) staff       (20)      624 2023-06-10 23:02:11.000000 sixth-sense-0.0.5/sixth_sense/schemas.py
+-rw-r--r--   0 mac        (501) staff       (20)     4195 2023-06-15 02:55:23.000000 sixth-sense-0.0.5/sixth_sense/sixth_sense.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 03:36:02.000000 sixth-sense-0.0.5/sixth_sense/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-sense-0.0.5/sixth_sense/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-sense-0.0.5/sixth_sense/utils/encryption_utils.py
+-rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-sense-0.0.5/sixth_sense/utils/time_utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 03:36:02.000000 sixth-sense-0.0.5/sixth_sense.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     3127 2023-06-16 03:36:02.000000 sixth-sense-0.0.5/sixth_sense.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      685 2023-06-16 03:36:02.000000 sixth-sense-0.0.5/sixth_sense.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-16 03:36:02.000000 sixth-sense-0.0.5/sixth_sense.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-16 03:36:02.000000 sixth-sense-0.0.5/sixth_sense.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       12 2023-06-16 03:36:02.000000 sixth-sense-0.0.5/sixth_sense.egg-info/top_level.txt
```

### Comparing `sixth-sense-0.0.4/sixth_sense/middlewares/encryption_middleware.py` & `sixth-sense-0.0.5/sixth_sense/middlewares/encryption_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.4/sixth_sense/middlewares/six_base_http_middleware.py` & `sixth-sense-0.0.5/sixth_sense/middlewares/six_base_http_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.4/sixth_sense/middlewares/six_independent_rate_limiter.py` & `sixth-sense-0.0.5/sixth_sense/middlewares/six_independent_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.4/sixth_sense/middlewares/six_rate_limiter_middleware.py` & `sixth-sense-0.0.5/sixth_sense/middlewares/six_rate_limiter_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
                 for new_route in route.app.routes:
                     path = "/v"+str(route.app.version)+new_route.path
                     edited_route = re.sub(r'\W+', '~', path)
                     self._log_dict[str(edited_route)] = {}
             else:
                 edited_route = re.sub(r'\W+', '~', route.path)
                 self._log_dict[str(edited_route)] = {}
+                
 
     async def set_body(self, request: Request, body: bytes):
         async def receive() -> Message:
             return {'type': 'http.request', 'body': body}
         request._receive = receive
         
     def _is_rate_limit_reached(self, uid, route):
@@ -73,15 +74,15 @@
         route = request.scope["path"]
         route = re.sub(r'\W+', '~', route)
         rate_limit_resp = requests.get("https://backend.withsix.co/project-config/config/get-route-rate-limit/"+self._apikey+"/"+route)
         
         if rate_limit_resp.status_code == 200:
             rate_limit = schemas.RateLimiter.parse_obj(rate_limit_resp.json())
             self._config.rate_limiter[route] = rate_limit
-            preferred_id = host if self._config.rate_limiter[route].unique_id == "" or self._config.rate_limiter[route].unique_id == "host" else body[self._config.rate_limiter[route].unique_id]
+            preferred_id = host if self._config.rate_limiter[route].unique_id == "" or self._config.rate_limiter[route].unique_id == "host" else self._config.rate_limiter[route].unique_id
             _response = await call_next(request)
             if self._is_rate_limit_reached(preferred_id, route): 
                 return _response
             else:
                 output={
                     "message": "max request reached"
                 }
```

### Comparing `sixth-sense-0.0.4/sixth_sense/schemas.py` & `sixth-sense-0.0.5/sixth_sense/schemas.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.4/sixth_sense/sixth_sense.py` & `sixth-sense-0.0.5/sixth_sense/sixth_sense.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,17 +68,17 @@
             user_id = self._apikey, 
             rate_limiter = _rl_configs, 
             encryption = schemas.Encryption(public_key="dummy",private_key="dummy", use_count=0, last_updated=0,created_at=0), 
             base_url = "op",
             last_updated=get_time_now(), 
             created_at=get_time_now(), 
             encryption_enabled=config.encryption_enabled if config != None else False, 
-            rate_limiter_enabled=config.rate_limiter_enabled if config != None else False
+            rate_limiter_enabled=config.rate_limiter_enabled if config != None else True
         )
         _base_url = "https://backend.withsix.co"
         _project_config_resp = requests.post(_base_url+"/project-config/config/sync-user-config", json=_config.dict())
         if _project_config_resp.status_code == status.HTTP_200_OK:
-            return True
+            return _config
         else: 
-            return False
+            return _config
```

### Comparing `sixth-sense-0.0.4/sixth_sense/utils/encryption_utils.py` & `sixth-sense-0.0.5/sixth_sense/utils/encryption_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.4/sixth_sense/utils/time_utils.py` & `sixth-sense-0.0.5/sixth_sense/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.4/sixth_sense.egg-info/SOURCES.txt` & `sixth-sense-0.0.5/sixth_sense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.4/sixth_sense.egg-info/requires.txt` & `sixth-sense-0.0.5/sixth_sense.egg-info/requires.txt`

 * *Files identical despite different names*

