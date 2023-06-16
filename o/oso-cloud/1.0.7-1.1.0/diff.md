# Comparing `tmp/oso_cloud-1.0.7-py3-none-any.whl.zip` & `tmp/oso_cloud-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7233 bytes, number of entries: 9
--rw-r--r--  2.0 unx       34 b- defN 23-Apr-27 16:03 oso_cloud/__init__.py
--rw-r--r--  2.0 unx    10113 b- defN 23-Apr-27 16:03 oso_cloud/api.py
--rw-r--r--  2.0 unx     1619 b- defN 23-Apr-27 16:03 oso_cloud/helpers.py
--rw-r--r--  2.0 unx     6222 b- defN 23-Apr-27 16:03 oso_cloud/oso.py
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-27 16:03 oso_cloud/version.py
--rw-r--r--  2.0 unx     3468 b- defN 23-Apr-27 16:03 oso_cloud-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 16:03 oso_cloud-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-27 16:03 oso_cloud-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      681 b- defN 23-Apr-27 16:03 oso_cloud-1.0.7.dist-info/RECORD
-9 files, 22261 bytes uncompressed, 6069 bytes compressed:  72.7%
+Zip file size: 7242 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       34 b- defN 23-Jun-16 16:11 oso_cloud/__init__.py
+-rw-r--r--  2.0 unx    10361 b- defN 23-Jun-16 16:11 oso_cloud/api.py
+-rw-r--r--  2.0 unx     1619 b- defN 23-Jun-16 16:11 oso_cloud/helpers.py
+-rw-r--r--  2.0 unx     6177 b- defN 23-Jun-16 16:11 oso_cloud/oso.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-16 16:11 oso_cloud/version.py
+-rw-r--r--  2.0 unx     3468 b- defN 23-Jun-16 16:11 oso_cloud-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 16:11 oso_cloud-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-16 16:11 oso_cloud-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      681 b- defN 23-Jun-16 16:11 oso_cloud-1.1.0.dist-info/RECORD
+9 files, 22464 bytes uncompressed, 6078 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: oso_cloud/oso.py
 Comment: 
 
 Filename: oso_cloud/version.py
 Comment: 
 
-Filename: oso_cloud-1.0.7.dist-info/METADATA
+Filename: oso_cloud-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: oso_cloud-1.0.7.dist-info/WHEEL
+Filename: oso_cloud-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: oso_cloud-1.0.7.dist-info/top_level.txt
+Filename: oso_cloud-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: oso_cloud-1.0.7.dist-info/RECORD
+Filename: oso_cloud-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oso_cloud/api.py

```diff
@@ -137,46 +137,51 @@
             return False
         return 400 <= exc.response.status_code < 500
     else:
         return False
 
 
 class API:
-    def __init__(self, url="https://cloud.osohq.com", api_key=None, user_agent=None):
+    def __init__(self, url="https://api.osohq.com", api_key=None):
         self.url = url
         self.api_base = "api"
         self.user_agent = (
             f"Oso Cloud (python {platform.python_version()}; rv:{__version__})"
         )
-        if user_agent:
-            self.user_agent = f"{self.user_agent} {user_agent}"
         if api_key:
             self.token = api_key
         else:
             raise ValueError("Must set an api_key")
         self.session = requests.Session()
         self.session.headers.update(self._default_headers())
 
-    def _handle_result(self, result):
+    def _handle_result(self, result, is_mutation=False):
         if not result.ok:
             code, text = result.status_code, result.text
             msg = f"Got unexpected error from Oso Service: {code}\n{text}"
             raise Exception(msg)
         try:
+            if is_mutation:
+                self._set_last_offset(result)
             return result.json()
         except json.decoder.JSONDecodeError:
-            return result.text
+            raise Exception("failed to deserialize results: ", result.text)
 
     def _default_headers(self):
         return {
             "Authorization": f"Bearer {self.token}",
             "User-Agent": self.user_agent,
             "X-OsoApiVersion": "0",
         }
 
+    def _set_last_offset(self, result):
+        last_offset = result.headers.get("OsoOffset")
+        if last_offset:
+            self.session.headers.update({"OsoOffset": last_offset})
+
     @backoff.on_exception(
         backoff.expo,
         (requests.exceptions.ConnectionError, requests.exceptions.Timeout),
         max_time=NETWORK_ERROR_MAX_TIME,
         max_tries=NETWORK_ERROR_MAX_RETRIES,
     )
     @backoff.on_exception(
@@ -247,60 +252,60 @@
 
     def post_policy(self, data):
         params = None
         json = asdict(data)
         result = self._do_post(
             f"{self.url}/{self.api_base}/policy", params=params, json=json
         )
-        response = self._handle_result(result)
+        response = self._handle_result(result, True)
         return ApiResult(**response)
 
     def post_facts(self, data):
         params = None
         json = asdict(data)
         result = self._do_post(
             f"{self.url}/{self.api_base}/facts", params=params, json=json
         )
-        response = self._handle_result(result)
+        response = self._handle_result(result, True)
         return Fact(**response)
 
     def delete_facts(self, data):
         params = None
         json = asdict(data)
         result = self._do_delete(
             f"{self.url}/{self.api_base}/facts", params=params, json=json
         )
-        response = self._handle_result(result)
+        response = self._handle_result(result, True)
         return ApiResult(**response)
 
     def post_bulk_load(self, data):
         params = None
         json = list(map(asdict, data))
         result = self._do_post(
             f"{self.url}/{self.api_base}/bulk_load", params=params, json=json
         )
-        response = self._handle_result(result)
+        response = self._handle_result(result, True)
         return ApiResult(**response)
 
     def post_bulk_delete(self, data):
         params = None
         json = list(map(asdict, data))
         result = self._do_post(
             f"{self.url}/{self.api_base}/bulk_delete", params=params, json=json
         )
-        response = self._handle_result(result)
+        response = self._handle_result(result, True)
         return ApiResult(**response)
 
     def post_bulk(self, data):
         params = None
         json = asdict(data)
         result = self._do_post(
             f"{self.url}/{self.api_base}/bulk", params=params, json=json
         )
-        response = self._handle_result(result)
+        response = self._handle_result(result, True)
         return ApiResult(**response)
 
     def post_authorize(self, data):
         params = None
         json = asdict(data)
         result = self._do_post(
             f"{self.url}/{self.api_base}/authorize", params=params, json=json
@@ -346,19 +351,17 @@
 
     def clear_data(self):
         params = None
         json = None
         result = self._do_post(
             f"{self.url}/{self.api_base}/clear_data", params=params, json=json
         )
-        response = self._handle_result(result)
+        response = self._handle_result(result, True)
         return ApiResult(**response)
 
-    # NOTE: the args stuff here doesn not show up in the openapi spec
-    # so we don't codegen this correctly
     def get_facts(self, predicate, *args):
         params = {}
         params["predicate"] = predicate
         for i, arg in enumerate(args):
             if arg.type is not None:
                 params[f"args.{i}.type"] = arg.type
             if arg.id is not None:
@@ -376,14 +379,18 @@
     def post_query(self, data):
         params = None
         json = asdict(data)
         result = self._do_post(
             f"{self.url}/{self.api_base}/query", params=params, json=json
         )
         response = self._handle_result(result)
-        # this doesn't get codegen'd properly either
         return QueryResult(
-            [
-                Fact(fact["predicate"], [Value(**arg) for arg in fact["args"]])
-                for fact in response["results"]
-            ]
+            list(
+                map(
+                    lambda fact: Fact(
+                        predicate=fact["predicate"],
+                        args=list(map(lambda arg: Value(**arg), fact["args"])),
+                    ),
+                    response["results"],
+                )
+            )
         )
```

## oso_cloud/oso.py

```diff
@@ -15,18 +15,16 @@
 class Oso:
     """Oso Cloud client
 
     For more detailed documentation, see
     https://www.osohq.com/docs/reference/client-apis/python
     """
 
-    def __init__(
-        self, url: str = "https://cloud.osohq.com", api_key=None, user_agent=None
-    ):
-        self.api = api.API(url, api_key, user_agent)
+    def __init__(self, url: str = "https://api.osohq.com", api_key=None):
+        self.api = api.API(url, api_key)
 
     def authorize(
         self,
         actor: Value,
         action: str,
         resource: Value,
         context_facts: List[Fact] = [],
```

## oso_cloud/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.7"
+__version__ = "1.1.0"
```

## Comparing `oso_cloud-1.0.7.dist-info/METADATA` & `oso_cloud-1.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oso-cloud
-Version: 1.0.7
+Version: 1.1.0
 Summary: Oso Cloud Python client
 Home-page: https://www.osohq.com
 Author: Oso Security
 Author-email: support@osohq.com
 License: Apache-2.0
 Project-URL: Documentation, https://www.osohq.com/docs
 Keywords: authorization,rbac,oso,oso cloud,authorization as a service,microservice authorization
```

## Comparing `oso_cloud-1.0.7.dist-info/RECORD` & `oso_cloud-1.1.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 oso_cloud/__init__.py,sha256=YxeVgapgfhYulcVgIBJcjHovx_SQ0ChyyA3dKzCgGVo,34
-oso_cloud/api.py,sha256=tq_kA6cYSFQzkgPY6kJ49j1l7Wuo4Nh_DfBTu4dL8J8,10113
+oso_cloud/api.py,sha256=_gRQnfnDPBq6tfD36AYRCo3J8I9eHGPFMRqrLannFnM,10361
 oso_cloud/helpers.py,sha256=UjUP1oCQihjnzDbXR_erulFHsOA5LmnojuNTAa7BGX4,1619
-oso_cloud/oso.py,sha256=t_TtpMbC8JpZ9s5PFlobBUB_6SkOxqgemKK66eVBQAA,6222
-oso_cloud/version.py,sha256=BW7SWRpHoxuOQZ67pS20yog2LWYl-nK7-BEFBNrHGgA,22
-oso_cloud-1.0.7.dist-info/METADATA,sha256=t8GTXPFqIA1nRDHCXVswxG2Pdqx2p4Zzfr-9mfbXySo,3468
-oso_cloud-1.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-oso_cloud-1.0.7.dist-info/top_level.txt,sha256=pzOq04dOQpqHFKR4eDR1MMZ23BacelJsh7LKlSdFnmw,10
-oso_cloud-1.0.7.dist-info/RECORD,,
+oso_cloud/oso.py,sha256=ry8mgooqy2wmrqmlh5ltfgf9eTdDOjsGOQ1Skorgiic,6177
+oso_cloud/version.py,sha256=LGVQyDsWifdACo7qztwb8RWWHds1E7uQ-ZqD8SAjyw4,22
+oso_cloud-1.1.0.dist-info/METADATA,sha256=jnY46fmiam1McpRCxCxD8_aeroUfQTuzaIc3mfQ4TME,3468
+oso_cloud-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+oso_cloud-1.1.0.dist-info/top_level.txt,sha256=pzOq04dOQpqHFKR4eDR1MMZ23BacelJsh7LKlSdFnmw,10
+oso_cloud-1.1.0.dist-info/RECORD,,
```

