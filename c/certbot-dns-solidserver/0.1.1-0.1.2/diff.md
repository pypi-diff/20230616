# Comparing `tmp/certbot-dns-solidserver-0.1.1.tar.gz` & `tmp/certbot-dns-solidserver-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-solidserver-0.1.1.tar", last modified: Tue Jun  6 12:46:46 2023, max compression
+gzip compressed data, was "certbot-dns-solidserver-0.1.2.tar", last modified: Fri Jun 16 09:25:42 2023, max compression
```

## Comparing `certbot-dns-solidserver-0.1.1.tar` & `certbot-dns-solidserver-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-06 12:46:46.151028 certbot-dns-solidserver-0.1.1/
--rw-r--r--   0 charles   (1000) charles   (1000)    10786 2023-06-06 10:03:36.000000 certbot-dns-solidserver-0.1.1/LICENSE.txt
--rw-r--r--   0 charles   (1000) charles   (1000)     4427 2023-06-06 12:46:46.151028 certbot-dns-solidserver-0.1.1/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)     3282 2023-06-06 10:03:38.000000 certbot-dns-solidserver-0.1.1/README.md
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-06 12:46:46.147694 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver/
--rw-r--r--   0 charles   (1000) charles   (1000)     2558 2023-06-06 10:04:42.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver/__init__.py
--rw-r--r--   0 charles   (1000) charles   (1000)     5273 2023-06-06 10:04:42.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver/dns_solidserver.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-06 12:46:46.151028 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/
--rw-r--r--   0 charles   (1000) charles   (1000)     4427 2023-06-06 12:46:46.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)      403 2023-06-06 12:46:46.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/SOURCES.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        1 2023-06-06 12:46:46.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/dependency_links.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       90 2023-06-06 12:46:46.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/entry_points.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       48 2023-06-06 12:46:46.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/requires.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       24 2023-06-06 12:46:46.000000 certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/top_level.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       67 2023-06-06 12:46:46.151028 certbot-dns-solidserver-0.1.1/setup.cfg
--rw-r--r--   0 charles   (1000) charles   (1000)     1770 2023-06-06 12:14:10.000000 certbot-dns-solidserver-0.1.1/setup.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-16 09:25:42.191441 certbot-dns-solidserver-0.1.2/
+-rw-r--r--   0 charles   (1000) charles   (1000)    10786 2023-06-06 10:03:36.000000 certbot-dns-solidserver-0.1.2/LICENSE.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)     4493 2023-06-16 09:25:42.191441 certbot-dns-solidserver-0.1.2/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)     3348 2023-06-16 09:19:49.000000 certbot-dns-solidserver-0.1.2/README.md
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-16 09:25:42.191441 certbot-dns-solidserver-0.1.2/certbot_dns_solidserver/
+-rw-r--r--   0 charles   (1000) charles   (1000)     2558 2023-06-06 10:04:42.000000 certbot-dns-solidserver-0.1.2/certbot_dns_solidserver/__init__.py
+-rw-r--r--   0 charles   (1000) charles   (1000)     5623 2023-06-16 09:12:12.000000 certbot-dns-solidserver-0.1.2/certbot_dns_solidserver/dns_solidserver.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-16 09:25:42.191441 certbot-dns-solidserver-0.1.2/certbot_dns_solidserver.egg-info/
+-rw-r--r--   0 charles   (1000) charles   (1000)     4493 2023-06-16 09:25:42.000000 certbot-dns-solidserver-0.1.2/certbot_dns_solidserver.egg-info/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)      403 2023-06-16 09:25:42.000000 certbot-dns-solidserver-0.1.2/certbot_dns_solidserver.egg-info/SOURCES.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)        1 2023-06-16 09:25:42.000000 certbot-dns-solidserver-0.1.2/certbot_dns_solidserver.egg-info/dependency_links.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       90 2023-06-16 09:25:42.000000 certbot-dns-solidserver-0.1.2/certbot_dns_solidserver.egg-info/entry_points.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       48 2023-06-16 09:25:42.000000 certbot-dns-solidserver-0.1.2/certbot_dns_solidserver.egg-info/requires.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       24 2023-06-16 09:25:42.000000 certbot-dns-solidserver-0.1.2/certbot_dns_solidserver.egg-info/top_level.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       67 2023-06-16 09:25:42.191441 certbot-dns-solidserver-0.1.2/setup.cfg
+-rw-r--r--   0 charles   (1000) charles   (1000)     1770 2023-06-16 09:13:39.000000 certbot-dns-solidserver-0.1.2/setup.py
```

### Comparing `certbot-dns-solidserver-0.1.1/LICENSE.txt` & `certbot-dns-solidserver-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-solidserver-0.1.1/PKG-INFO` & `certbot-dns-solidserver-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-solidserver
-Version: 0.1.1
+Version: 0.1.2
 Summary: SOLIDserver DNS Authenticator plugin for Certbot
 Home-page: https://gitlab.com/charlyhong/certbot-dns-solidserver
 Author: Charles Hong
 Author-email: ch@efficientip.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
@@ -71,15 +71,17 @@
     # Sample SOLIDserver INI file
     # Default location /etc/letsencrypt/solidserver.ini
     #
     dns_solidserver_hostname="your.solidserver.host"
     dns_solidserver_username="myremoteuser"
     dns_solidserver_password="verysecureremoteuserpassword"
     dns_solidserver_dnsname="my.dns.server"
-    dns_solidserver_viewname="external"
+    #
+    # Optional: uncomment this line if dnsview must be used
+    #dns_solidserver_viewname="external"
 
 The path to this file can be provided interactively or using the
 ``--dns-solidserver-credentials`` command-line argument. Certbot
 records the path to this file for use during renewal, but does not store the
 file's contents.
 
 **CAUTION:** You should protect these API credentials as you would the
@@ -102,15 +104,15 @@
 
 To acquire a single certificate for both ``example.com`` and
 ``*.example.com``, waiting 900 seconds for DNS propagation:
 
     certbot certonly \
      --authenticator dns-solidserver \
      --dns-solidserver-credentials /etc/letsencrypt/.secrets/domain.tld.ini \
-     --dns-solidserver-propagation-seconds 900 \
+     --dns-solidserver-propagation-seconds 60 \
      --server https://acme-v02.api.letsencrypt.org/directory \
      --agree-tos \
      --rsa-key-size 4096 \
      -d 'example.com' \
      -d '*.example.com'
```

### Comparing `certbot-dns-solidserver-0.1.1/README.md` & `certbot-dns-solidserver-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,17 @@
     # Sample SOLIDserver INI file
     # Default location /etc/letsencrypt/solidserver.ini
     #
     dns_solidserver_hostname="your.solidserver.host"
     dns_solidserver_username="myremoteuser"
     dns_solidserver_password="verysecureremoteuserpassword"
     dns_solidserver_dnsname="my.dns.server"
-    dns_solidserver_viewname="external"
+    #
+    # Optional: uncomment this line if dnsview must be used
+    #dns_solidserver_viewname="external"
 
 The path to this file can be provided interactively or using the
 ``--dns-solidserver-credentials`` command-line argument. Certbot
 records the path to this file for use during renewal, but does not store the
 file's contents.
 
 **CAUTION:** You should protect these API credentials as you would the
@@ -73,15 +75,15 @@
 
 To acquire a single certificate for both ``example.com`` and
 ``*.example.com``, waiting 900 seconds for DNS propagation:
 
     certbot certonly \
      --authenticator dns-solidserver \
      --dns-solidserver-credentials /etc/letsencrypt/.secrets/domain.tld.ini \
-     --dns-solidserver-propagation-seconds 900 \
+     --dns-solidserver-propagation-seconds 60 \
      --server https://acme-v02.api.letsencrypt.org/directory \
      --agree-tos \
      --rsa-key-size 4096 \
      -d 'example.com' \
      -d '*.example.com'
```

### Comparing `certbot-dns-solidserver-0.1.1/certbot_dns_solidserver/__init__.py` & `certbot-dns-solidserver-0.1.2/certbot_dns_solidserver/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-solidserver-0.1.1/certbot_dns_solidserver/dns_solidserver.py` & `certbot-dns-solidserver-0.1.2/certbot_dns_solidserver/dns_solidserver.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,14 @@
             "credentials",
             "SOLIDserver credentials INI file",
             {
                 "hostname": "Hostname for SOLIDserver REST API.",
                 "username": "Username for SOLIDserver REST API.",
                 "password": "Password for SOLIDserver REST API.",
                 "dnsname": "DNS server name.",
-                "viewname": "View to use for TXT entries (leave blank if not used)"
             },
         )
 
     def _perform(self, domain, validation_name, validation):
         self._get_eiprest_client().add_txt_record(domain, validation_name, validation, self.ttl)
 
     def _cleanup(self, domain, validation_name, validation):
@@ -72,15 +71,15 @@
         logger.debug("creating eiprest client")
         self.dnsname = dnsname
         self.viewname = viewname
         self.eiprest = EipRest(host=hostname, user=username, password=password)
 
     def add_txt_record(self, domain, record_name, record_content, ttl):
         record = self.get_rr_txt(record_name)
-        if record is not None:
+        if record:
             if record[0]["value1"] == record_content:
                 logger.info(f"already there, id {record[0]['rr_id']}")
                 return
             else:
                 logger.info(f"update record {record[0]['rr_id']}")
                 self.update_rr_txt(record[0]['rr_id'], record_content, ttl)    
         else:
@@ -88,29 +87,37 @@
             self.add_rr_txt(record_name, record_content, ttl)
 
     def del_txt_record(self, domain, record_name, record_content, ttl):
         params = {
             'WHERE': f"rr_full_name='{record_name}' AND rr_type='TXT' AND value1='{record_content}' AND vdns_parent_id=0 AND dnszone_type='master'",
         }
         self.eiprest.query('GET', 'dns_rr_list', params)
-        resp = self.eiprest.getData()
-        if resp:
-            for rr in resp:
-                logger.info(f"delete record TXT {rr['rr_full_name']}")
-                self.eiprest.query('DELETE', 'dns_rr_delete', {'rr_id': rr['rr_id']})
+        if self.eiprest.resp.status_code == 200:
+            resp = self.eiprest.getData()
+            if resp:
+                for rr in resp:
+                    logger.info(f"delete record TXT {rr['rr_full_name']}")
+                    self.eiprest.query('DELETE', 'dns_rr_delete', {'rr_id': rr['rr_id']})
 
     def get_rr_txt(self, rr_name):
         params = {
             'WHERE': f"dns_name='{self.dnsname}' AND rr_full_name='{rr_name}' AND rr_type='TXT'",
             'limit': 1,
         }
         if self.viewname:
             params['WHERE'] += f" AND dnsview_name='{self.viewname}'"
         self.eiprest.query('GET', 'dns_rr_list', params)
-        return self.eiprest.getData()
+        if self.eiprest.resp is not None:
+            status_code = self.eiprest.resp.status_code
+            if status_code == 200 or status_code == 204:
+                return self.eiprest.getData()
+            else:
+                raise errors.PluginError(f"Error while searching record TXT: return code {status_code}")
+        else:
+            raise errors.PluginError(f"Failed to query {self.eiprest.host}")
 
     def update_rr_txt(self, rr_id, value1, ttl):
         params = {
             'rr_id': rr_id,
             'value1': value1,
             'rr_ttl': ttl,
             'add_flag': 'edit_only',
```

### Comparing `certbot-dns-solidserver-0.1.1/certbot_dns_solidserver.egg-info/PKG-INFO` & `certbot-dns-solidserver-0.1.2/certbot_dns_solidserver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-solidserver
-Version: 0.1.1
+Version: 0.1.2
 Summary: SOLIDserver DNS Authenticator plugin for Certbot
 Home-page: https://gitlab.com/charlyhong/certbot-dns-solidserver
 Author: Charles Hong
 Author-email: ch@efficientip.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
@@ -71,15 +71,17 @@
     # Sample SOLIDserver INI file
     # Default location /etc/letsencrypt/solidserver.ini
     #
     dns_solidserver_hostname="your.solidserver.host"
     dns_solidserver_username="myremoteuser"
     dns_solidserver_password="verysecureremoteuserpassword"
     dns_solidserver_dnsname="my.dns.server"
-    dns_solidserver_viewname="external"
+    #
+    # Optional: uncomment this line if dnsview must be used
+    #dns_solidserver_viewname="external"
 
 The path to this file can be provided interactively or using the
 ``--dns-solidserver-credentials`` command-line argument. Certbot
 records the path to this file for use during renewal, but does not store the
 file's contents.
 
 **CAUTION:** You should protect these API credentials as you would the
@@ -102,15 +104,15 @@
 
 To acquire a single certificate for both ``example.com`` and
 ``*.example.com``, waiting 900 seconds for DNS propagation:
 
     certbot certonly \
      --authenticator dns-solidserver \
      --dns-solidserver-credentials /etc/letsencrypt/.secrets/domain.tld.ini \
-     --dns-solidserver-propagation-seconds 900 \
+     --dns-solidserver-propagation-seconds 60 \
      --server https://acme-v02.api.letsencrypt.org/directory \
      --agree-tos \
      --rsa-key-size 4096 \
      -d 'example.com' \
      -d '*.example.com'
```

### Comparing `certbot-dns-solidserver-0.1.1/setup.py` & `certbot-dns-solidserver-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "0.1.1"
+version = "0.1.2"
 
 install_requires = [
     "acme>=0.29.0",
     "certbot>=0.34.0",
     "eiprest",
     "setuptools",
 ]
```

