# Comparing `tmp/micropython_wifi_communication-0.0.1.tar.gz` & `tmp/micropython_wifi_communication-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_wifi_communication-0.0.1.tar", last modified: Fri Jun 16 00:40:34 2023, max compression
+gzip compressed data, was "micropython_wifi_communication-0.0.2.tar", last modified: Fri Jun 16 17:08:48 2023, max compression
```

## Comparing `micropython_wifi_communication-0.0.1.tar` & `micropython_wifi_communication-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 00:40:34.670646 micropython_wifi_communication-0.0.1/
--rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      409 2023-06-16 00:40:34.653025 micropython_wifi_communication-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-16 00:29:04.000000 micropython_wifi_communication-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 00:40:34.589942 micropython_wifi_communication-0.0.1/comu/
--rw-rw-rw-   0        0        0       36 2023-06-15 19:49:52.000000 micropython_wifi_communication-0.0.1/comu/__init__.py
--rw-rw-rw-   0        0        0     1329 2023-06-16 00:39:40.000000 micropython_wifi_communication-0.0.1/comu/ci.py
--rw-rw-rw-   0        0        0     2633 2023-06-16 00:38:52.000000 micropython_wifi_communication-0.0.1/comu/se.py
--rw-rw-rw-   0        0        0      386 2023-06-15 18:40:47.000000 micropython_wifi_communication-0.0.1/comu/util.py
-drwxrwxrwx   0        0        0        0 2023-06-16 00:40:34.647513 micropython_wifi_communication-0.0.1/micropython_wifi_communication.egg-info/
--rw-rw-rw-   0        0        0      409 2023-06-16 00:40:34.000000 micropython_wifi_communication-0.0.1/micropython_wifi_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-06-16 00:40:34.000000 micropython_wifi_communication-0.0.1/micropython_wifi_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 00:40:34.000000 micropython_wifi_communication-0.0.1/micropython_wifi_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-16 00:40:34.000000 micropython_wifi_communication-0.0.1/micropython_wifi_communication.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 00:40:34.670646 micropython_wifi_communication-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      510 2023-06-16 00:32:18.000000 micropython_wifi_communication-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:08:48.654636 micropython_wifi_communication-0.0.2/
+-rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0      409 2023-06-16 17:08:48.654636 micropython_wifi_communication-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-06-16 00:29:04.000000 micropython_wifi_communication-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 17:08:48.575785 micropython_wifi_communication-0.0.2/comu/
+-rw-rw-rw-   0        0        0       36 2023-06-15 19:49:52.000000 micropython_wifi_communication-0.0.2/comu/__init__.py
+-rw-rw-rw-   0        0        0     2236 2023-06-16 17:07:02.000000 micropython_wifi_communication-0.0.2/comu/ci.py
+-rw-rw-rw-   0        0        0     2713 2023-06-16 17:07:02.000000 micropython_wifi_communication-0.0.2/comu/se.py
+-rw-rw-rw-   0        0        0      386 2023-06-15 18:40:47.000000 micropython_wifi_communication-0.0.2/comu/util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:08:48.653594 micropython_wifi_communication-0.0.2/micropython_wifi_communication.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-06-16 17:08:47.000000 micropython_wifi_communication-0.0.2/micropython_wifi_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-06-16 17:08:47.000000 micropython_wifi_communication-0.0.2/micropython_wifi_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 17:08:47.000000 micropython_wifi_communication-0.0.2/micropython_wifi_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-16 17:08:47.000000 micropython_wifi_communication-0.0.2/micropython_wifi_communication.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 17:08:48.654636 micropython_wifi_communication-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      510 2023-06-16 17:07:34.000000 micropython_wifi_communication-0.0.2/setup.py
```

### Comparing `micropython_wifi_communication-0.0.1/LICENCE` & `micropython_wifi_communication-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `micropython_wifi_communication-0.0.1/comu/se.py` & `micropython_wifi_communication-0.0.2/comu/se.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,13 +63,16 @@
             va, me = validator(message)
             if not va:
                 return me['inf']
         except:
             self.ence()
 
     def ence(self):
-        # self.client_socket.close()
-        self.server_socket.listen(1)
-        # Aceita uma nova conexão
-        self.client_socket, self.client_address = self.server_socket.accept()
-        self.client_socket.settimeout(300)
-        print("cliente aceito")
+        try:
+            # self.client_socket.close()
+            self.server_socket.listen(1)
+            # Aceita uma nova conexão
+            self.client_socket, self.client_address = self.server_socket.accept()
+            self.client_socket.settimeout(300)
+            print("cliente aceito")
+        except:
+            self.ence()
```

