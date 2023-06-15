# Comparing `tmp/hubspot3-3.2.8.tar.gz` & `tmp/hubspot3-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hubspot3-3.2.8.tar", last modified: Fri May 17 16:16:02 2019, max compression
+gzip compressed data, was "dist/hubspot3-3.2.9.tar", last modified: Fri May 24 01:29:27 2019, max compression
```

## Comparing `hubspot3-3.2.8.tar` & `hubspot3-3.2.9.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-17 16:16:02.000000 hubspot3-3.2.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8085 2019-05-17 16:16:02.000000 hubspot3-3.2.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     5845 2019-05-17 16:15:38.000000 hubspot3-3.2.8/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-17 16:16:02.000000 hubspot3-3.2.8/hubspot3/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8051 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11786 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4706 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/blog.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6361 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/broadcast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6109 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/companies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1833 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/contact_lists.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7024 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/contacts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4544 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/crm_associations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1621 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/crm_pipelines.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6611 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/deals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2720 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/engagements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3584 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/error.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      796 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/forms.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       96 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/globals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1476 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/keywords.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4934 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/leads.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      239 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/logging_helper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1333 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/owners.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2776 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/prospects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2019-05-17 16:15:38.000000 hubspot3-3.2.8/hubspot3/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-17 16:16:02.000000 hubspot3-3.2.8/hubspot3.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8085 2019-05-17 16:16:02.000000 hubspot3-3.2.8/hubspot3.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      633 2019-05-17 16:16:02.000000 hubspot3-3.2.8/hubspot3.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-17 16:16:02.000000 hubspot3-3.2.8/hubspot3.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-17 16:16:02.000000 hubspot3-3.2.8/hubspot3.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-05-17 16:16:02.000000 hubspot3-3.2.8/hubspot3.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      203 2019-05-17 16:16:02.000000 hubspot3-3.2.8/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)      963 2019-05-17 16:15:38.000000 hubspot3-3.2.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 01:29:27.000000 hubspot3-3.2.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6587 2019-05-24 01:29:27.000000 hubspot3-3.2.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4603 2019-05-24 01:29:03.000000 hubspot3-3.2.9/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 01:29:27.000000 hubspot3-3.2.9/hubspot3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8603 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11504 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4706 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/blog.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6361 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/broadcast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6109 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/companies.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1833 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/contact_lists.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7024 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/contacts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4544 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/crm_associations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1621 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/crm_pipelines.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6611 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/deals.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2720 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/engagements.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3584 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/error.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3334 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/forms.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       96 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/globals.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1476 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/keywords.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4934 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/leads.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      239 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/logging_helper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1333 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/owners.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2776 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/prospects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2657 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/tickets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2019-05-24 01:29:03.000000 hubspot3-3.2.9/hubspot3/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 01:29:27.000000 hubspot3-3.2.9/hubspot3.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6587 2019-05-24 01:29:26.000000 hubspot3-3.2.9/hubspot3.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      653 2019-05-24 01:29:27.000000 hubspot3-3.2.9/hubspot3.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-24 01:29:26.000000 hubspot3-3.2.9/hubspot3.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-24 01:29:26.000000 hubspot3-3.2.9/hubspot3.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-05-24 01:29:26.000000 hubspot3-3.2.9/hubspot3.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      203 2019-05-24 01:29:27.000000 hubspot3-3.2.9/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      963 2019-05-24 01:29:03.000000 hubspot3-3.2.9/setup.py
```

### Comparing `hubspot3-3.2.8/hubspot3/__init__.py` & `hubspot3-3.2.9/hubspot3/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,17 +49,15 @@
     def until_reset(self) -> int:
         """returns the number of seconds until limit reset"""
         return int((self.resets_at - datetime.now()).total_seconds())
 
     @property
     def until_cache_expire(self):
         """returns the number of seconds until the cache expires, and we need an update"""
-        return int(
-            (self.collected_at + timedelta(minutes=5) - datetime.now()).total_seconds()
-        )
+        return int((self.collected_at + timedelta(minutes=5) - datetime.now()).total_seconds())
 
     @property
     def calls_remaining(self) -> int:
         """returns the number of calls remaining in your usage limits for the day"""
         return self.usage_limit - self.current_usage
 
     @property
@@ -88,32 +86,39 @@
         api_key: str = None,
         access_token: str = None,
         refresh_token: str = None,
         client_id: str = None,
         timeout: int = 10,
         api_base: str = "api.hubapi.com",
         debug: bool = False,
+        disable_auth: bool = False,
         **extra_options: Any
     ) -> None:
         """full client constructor"""
         self.api_key = api_key or extra_options.get("api_key")
         self.access_token = access_token or extra_options.get("access_token")
         self.refresh_token = refresh_token or extra_options.get("refresh_token")
         self.client_id = client_id or extra_options.get("client_id")
-        if self.api_key and self.access_token:
-            raise HubspotBadConfig("Cannot use both api_key and access_token.")
-        if not (self.api_key or self.access_token or self.refresh_token):
-            raise HubspotNoConfig("Missing required credentials.")
+        if not disable_auth:
+            if self.api_key and self.access_token:
+                raise HubspotBadConfig("Cannot use both api_key and access_token.")
+            if not (self.api_key or self.access_token or self.refresh_token):
+                raise HubspotNoConfig("Missing required credentials.")
         self.auth = {
             "access_token": self.access_token,
             "api_key": self.api_key,
             "client_id": self.client_id,
             "refresh_token": self.refresh_token,
         }
-        self.options = {"api_base": api_base, "debug": debug, "timeout": timeout}
+        self.options = {
+            "api_base": api_base,
+            "debug": debug,
+            "disable_auth": disable_auth,
+            "timeout": timeout,
+        }
         self.options.update(extra_options)
 
         # rate limiting related stuff
         self._usage_limits = Hubspot3UsageLimits()
 
     @property
     def _base(self):
@@ -182,21 +187,28 @@
     def engagements(self):
         """returns a hubspot3 engagements client"""
         from hubspot3.engagements import EngagementsClient
 
         return EngagementsClient(**self.auth, **self.options)
 
     @property
-    def forms(self):
-        """returns a hubspot3 forms client"""
+    def form_submissions(self):
+        """returns a hubspot3 form submissions client"""
         from hubspot3.forms import FormSubmissionClient
 
         return FormSubmissionClient(**self.auth, **self.options)
 
     @property
+    def forms(self):
+        """returns a hubspot3 forms client"""
+        from hubspot3.forms import FormsClient
+
+        return FormsClient(**self.auth, **self.options)
+
+    @property
     def keywords(self):
         """returns a hubspot3 keywords client"""
         from hubspot3.keywords import KeywordsClient
 
         return KeywordsClient(**self.auth, **self.options)
 
     @property
@@ -224,14 +236,21 @@
     def settings(self):
         """returns a hubspot3 settings client"""
         from hubspot3.settings import SettingsClient
 
         return SettingsClient(**self.auth, **self.options)
 
     @property
+    def tickets(self):
+        """returns a hubspot3 tickets client"""
+        from hubspot3.tickets import TicketsClient
+
+        return TicketsClient(**self.auth, **self.options)
+
+    @property
     def usage_limits(self):
         """fetches and returns a nice usage liimitation object"""
         if self._usage_limits.need_update:
             limits = self._base._call("integrations/v1/limit/daily")[0]
             self._usage_limits = Hubspot3UsageLimits(
                 collected_at=datetime.fromtimestamp(int(limits["collectedAt"]) / 1000),
                 current_usage=int(limits["currentUsage"]),
```

### Comparing `hubspot3-3.2.8/hubspot3/base.py` & `hubspot3-3.2.9/hubspot3/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     HubspotNoConfig,
     HubspotNotFound,
     HubspotRateLimited,
     HubspotServerError,
     HubspotTimeout,
     HubspotUnauthorized,
 )
+from typing import Union
 
 
 class BaseClient(object):
     """Base abstract object for interacting with the HubSpot APIs"""
 
     # Controls how long we sleep for during retries, overridden by unittests
     # so tests run faster
@@ -39,14 +40,15 @@
         access_token=None,
         refresh_token=None,
         client_id=None,
         timeout=10,
         mixins=None,
         api_base="api.hubapi.com",
         debug=False,
+        disable_auth=False,
         **extra_options
     ):
         super(BaseClient, self).__init__()
         # reverse so that the first one in the list because the first parent
         if not mixins:
             mixins = []
         mixins.reverse()
@@ -55,19 +57,25 @@
                 self.__class__.__bases__ = (mixin_class,) + self.__class__.__bases__
 
         self.api_key = api_key or extra_options.get("api_key")
         self.access_token = access_token or extra_options.get("access_token")
         self.refresh_token = refresh_token or extra_options.get("refresh_token")
         self.client_id = client_id or extra_options.get("client_id")
         self.log = utils.get_log("hubspot3")
-        if self.api_key and self.access_token:
-            raise HubspotBadConfig("Cannot use both api_key and access_token.")
-        if not (self.api_key or self.access_token or self.refresh_token):
-            raise HubspotNoConfig("Missing required credentials.")
-        self.options = {"api_base": api_base, "debug": debug, "timeout": timeout}
+        if not disable_auth:
+            if self.api_key and self.access_token:
+                raise HubspotBadConfig("Cannot use both api_key and access_token.")
+            if not (self.api_key or self.access_token or self.refresh_token):
+                raise HubspotNoConfig("Missing required credentials.")
+        self.options = {
+            "api_base": api_base,
+            "debug": debug,
+            "disable_auth": disable_auth,
+            "timeout": timeout,
+        }
         self.options.update(extra_options)
         self._prepare_connection_type()
 
     def _prepare_connection_type(self):
         connection_types = {
             "http": http.client.HTTPConnection,
             "https": http.client.HTTPSConnection,
@@ -114,21 +122,15 @@
         if data and headers["Content-Type"] == "application/json":
             data = json.dumps(data)
 
         return url, headers, data
 
     def _create_request(self, conn, method, url, headers, data):
         conn.request(method, url, data, headers)
-        params = {
-            "method": method,
-            "url": url,
-            "data": data,
-            "headers": headers,
-            "host": conn.host,
-        }
+        params = {"method": method, "url": url, "data": data, "headers": headers, "host": conn.host}
         params["timeout"] = conn.timeout
         return params
 
     def _gunzip_body(self, body):
         return zlib.decompress(body)
 
     def _process_body(self, data, gzipped):
@@ -144,17 +146,15 @@
 
         encoding = [i[1] for i in result.getheaders() if i[0] == "content-encoding"]
         possibly_encoded = result.read()
         try:
             possibly_encoded = zlib.decompress(possibly_encoded, 16 + zlib.MAX_WBITS)
         except Exception:
             pass
-        result.body = self._process_body(
-            possibly_encoded, len(encoding) and encoding[0] == "gzip"
-        )
+        result.body = self._process_body(possibly_encoded, len(encoding) and encoding[0] == "gzip")
 
         conn.close()
         if result.status in (404, 410):
             raise HubspotNotFound(result, request)
         elif result.status == 401:
             raise HubspotUnauthorized(result, request)
         elif result.status == 409:
@@ -205,19 +205,15 @@
 
         url, headers, data = self._prepare_request(
             subpath, params, data, opts, doseq=doseq, query=query
         )
 
         if debug:
             print(
-                json.dumps(
-                    {"url": url, "headers": headers, "data": data},
-                    sort_keys=True,
-                    indent=2,
-                )
+                json.dumps({"url": url, "headers": headers, "data": data}, sort_keys=True, indent=2)
             )
 
         kwargs = {}
         kwargs["timeout"] = opts["timeout"]
 
         num_retries = opts.get("number_retries", 2)
 
@@ -233,59 +229,43 @@
             emergency_brake -= 1
             # avoid getting burned by any mistakes in While loop logic
             if emergency_brake < 1:
                 break
             try:
                 try_count += 1
                 connection = opts["connection_type"](opts["api_base"], **kwargs)
-                request_info = self._create_request(
-                    connection, method, url, headers, data
-                )
+                request_info = self._create_request(connection, method, url, headers, data)
                 result = self._execute_request_raw(connection, request_info)
                 break
             except HubspotUnauthorized:
                 self.log.warning("401 Unauthorized response to API request.")
-                if (
-                    self.access_token
-                    and self.refresh_token
-                    and self.client_id
-                    and not retried
-                ):
+                if self.access_token and self.refresh_token and self.client_id and not retried:
                     self.log.info("Refreshing access token")
                     try:
                         token_response = utils.refresh_access_token(
                             self.refresh_token, self.client_id
                         )
                         decoded = json.loads(token_response)
                         self.access_token = decoded["access_token"]
-                        self.log.info(
-                            "Retrying with new token {}".format(self.access_token)
-                        )
+                        self.log.info("Retrying with new token {}".format(self.access_token))
                     except Exception as exception:
-                        self.log.error(
-                            "Unable to refresh access_token: {}".format(exception)
-                        )
+                        self.log.error("Unable to refresh access_token: {}".format(exception))
                         raise
                     return self._call_raw(
                         subpath,
                         params=params,
                         method=method,
                         data=data,
                         doseq=doseq,
                         query=query,
                         retried=True,
                         **options
                     )
                 else:
-                    if (
-                        self.access_token
-                        and self.refresh_token
-                        and self.client_id
-                        and retried
-                    ):
+                    if self.access_token and self.refresh_token and self.client_id and retried:
                         self.log.error(
                             "Refreshed token, but request still was not authorized. "
                             " You may need to grant additional permissions."
                         )
                     elif self.access_token and not self.refresh_token:
                         self.log.error(
                             "In order to enable automated refreshing of your access "
@@ -305,36 +285,35 @@
                 if (
                     exception.result
                     and exception.result.status >= 300
                     and exception.result.status < 500
                 ):
                     raise
                 self._prepare_request_retry(method, url, headers, data)
-                self.log.warning(
-                    "HubspotError {} calling {}, retrying".format(exception, url)
-                )
+                self.log.warning("HubspotError {} calling {}, retrying".format(exception, url))
             # exponential back off
             # wait 0 seconds, 1 second, 3 seconds, 7 seconds, 15 seconds, etc
             time.sleep((pow(2, try_count - 1) - 1) * self.sleep_multiplier)
         return result
 
     def _call(
         self,
-        subpath,
-        params=None,
-        method="GET",
-        data=None,
-        doseq=False,
-        query="",
+        subpath: str,
+        params: dict = None,
+        method: str = "GET",
+        data: Union[str, dict, list] = None,
+        doseq: bool = False,
+        query: str = "",
+        raw: bool = False,
         **options
     ):
         result = self._call_raw(
             subpath,
             params=params,
             method=method,
             data=data,
             doseq=doseq,
             query=query,
             retried=False,
             **options
         )
-        return self._digest_result(result.body)
+        return result if raw else self._digest_result(result.body)
```

### Comparing `hubspot3-3.2.8/hubspot3/blog.py` & `hubspot3-3.2.9/hubspot3/blog.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/broadcast.py` & `hubspot3-3.2.9/hubspot3/broadcast.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/companies.py` & `hubspot3-3.2.9/hubspot3/companies.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/contact_lists.py` & `hubspot3-3.2.9/hubspot3/contact_lists.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/contacts.py` & `hubspot3-3.2.9/hubspot3/contacts.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/crm_associations.py` & `hubspot3-3.2.9/hubspot3/crm_associations.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/crm_pipelines.py` & `hubspot3-3.2.9/hubspot3/crm_pipelines.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/deals.py` & `hubspot3-3.2.9/hubspot3/deals.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/engagements.py` & `hubspot3-3.2.9/hubspot3/engagements.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/error.py` & `hubspot3-3.2.9/hubspot3/error.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/keywords.py` & `hubspot3-3.2.9/hubspot3/keywords.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/leads.py` & `hubspot3-3.2.9/hubspot3/leads.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/owners.py` & `hubspot3-3.2.9/hubspot3/owners.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/prospects.py` & `hubspot3-3.2.9/hubspot3/prospects.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/settings.py` & `hubspot3-3.2.9/hubspot3/settings.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3/utils.py` & `hubspot3-3.2.9/hubspot3/utils.py`

 * *Files identical despite different names*

### Comparing `hubspot3-3.2.8/hubspot3.egg-info/SOURCES.txt` & `hubspot3-3.2.9/hubspot3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,13 +17,14 @@
 hubspot3/globals.py
 hubspot3/keywords.py
 hubspot3/leads.py
 hubspot3/logging_helper.py
 hubspot3/owners.py
 hubspot3/prospects.py
 hubspot3/settings.py
+hubspot3/tickets.py
 hubspot3/utils.py
 hubspot3.egg-info/PKG-INFO
 hubspot3.egg-info/SOURCES.txt
 hubspot3.egg-info/dependency_links.txt
 hubspot3.egg-info/not-zip-safe
 hubspot3.egg-info/top_level.txt
```

### Comparing `hubspot3-3.2.8/setup.py` & `hubspot3-3.2.9/setup.py`

 * *Files identical despite different names*

