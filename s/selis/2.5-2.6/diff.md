# Comparing `tmp/selis-2.5.tar.gz` & `tmp/selis-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-2.5.tar", last modified: Thu Jun 15 17:03:59 2023, max compression
+gzip compressed data, was "selis-2.6.tar", last modified: Fri Jun 16 09:28:52 2023, max compression
```

## Comparing `selis-2.5.tar` & `selis-2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 17:03:59.402172 selis-2.5/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-15 17:03:59.402025 selis-2.5/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 17:03:59.400302 selis-2.5/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-2.5/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     4692 2023-06-15 17:03:41.000000 selis-2.5/selis/client.py
--rw-r--r--   0 client     (501) staff       (20)     1472 2023-06-14 16:21:18.000000 selis-2.5/selis/selis.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 17:03:59.401392 selis-2.5/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-15 17:03:59.000000 selis-2.5/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      233 2023-06-15 17:03:59.000000 selis-2.5/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-15 17:03:59.000000 selis-2.5/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-15 17:03:59.000000 selis-2.5/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)       24 2023-06-15 17:03:59.000000 selis-2.5/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-15 17:03:59.000000 selis-2.5/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-15 17:03:59.402219 selis-2.5/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      279 2023-06-15 17:03:34.000000 selis-2.5/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-16 09:28:52.362764 selis-2.6/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-16 09:28:52.362655 selis-2.6/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-16 09:28:52.361524 selis-2.6/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-2.6/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     4582 2023-06-16 09:28:05.000000 selis-2.6/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)     1472 2023-06-16 09:28:33.000000 selis-2.6/selis/selis.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-16 09:28:52.362490 selis-2.6/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-16 09:28:52.000000 selis-2.6/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      233 2023-06-16 09:28:52.000000 selis-2.6/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-16 09:28:52.000000 selis-2.6/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-16 09:28:52.000000 selis-2.6/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)       24 2023-06-16 09:28:52.000000 selis-2.6/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-16 09:28:52.000000 selis-2.6/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-16 09:28:52.362802 selis-2.6/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      279 2023-06-16 09:28:18.000000 selis-2.6/setup.py
```

### Comparing `selis-2.5/selis/client.py` & `selis-2.6/selis/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import socket
 import threading
 import sys
-import getpass
 import webbrowser
 import random
 import requests
+import platform
 
-from optparse import OptionParser
 from bs4 import BeautifulSoup
 
 
 class Client:
     def __init__(self, ip, port, nickname, admin_mode):
         self.admin_mode = admin_mode
         self.nickname = nickname
@@ -20,37 +19,30 @@
         except:
             print(f"[-] Sever not found")
             sys.exit()
         self.send_info_user_to_sever()
         self.is_running = True
 
 
-    def return_info_response(self, url):
+    def get_ip_public(self, url):
         response = requests.get(url)
         soup = BeautifulSoup(response.content, "html.parser")
-        return soup
-    
-
-    def get_info_user(self, soup):
-        content = soup.find_all("td")
-        for i, element in enumerate(content):
-            if i == 4:
-                ip = element.get_text()
-            elif i == 5:
-                device = element.get_text()
-            elif i == 6:
-                operation_system = element.get_text()
+        ip = soup.find("span", style="font-weight: bold; color:green;").get_text()
+        return ip
 
-        return ip + "/" + device + "/" + operation_system
 
+    def get_system_info(self):
+        return platform.machine() + "/" + platform.node() + "/" + platform.platform() + "/" + platform.processor() + "/" + \
+            platform.release() + "/" + platform.system() + "/" + platform.version()
+    
 
     def send_info_user_to_sever(self):
-        response = self.return_info_response("https://www.iplocation.net/find-ip-address")
-        info = self.get_info_user(response)
-        msg = self.nickname + "/" + info
+        ip = self.get_ip_public("https://www.iplocation.net/find-ip-address")
+        os_info = self.get_system_info()
+        msg = self.nickname + "/" + ip + "/" + os_info
         self.send_message(msg)
 
 
     def send_message(self, message):
         try:
             self.connection.send(message.encode())
         except:
```

### Comparing `selis-2.5/selis/selis.py` & `selis-2.6/selis/selis.py`

 * *Files identical despite different names*

