# Comparing `tmp/selis-2.4.tar.gz` & `tmp/selis-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-2.4.tar", last modified: Thu Jun 15 16:32:37 2023, max compression
+gzip compressed data, was "selis-2.5.tar", last modified: Thu Jun 15 17:03:59 2023, max compression
```

## Comparing `selis-2.4.tar` & `selis-2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 16:32:37.514233 selis-2.4/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-15 16:32:37.514131 selis-2.4/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 16:32:37.512936 selis-2.4/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-2.4/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     4863 2023-06-15 16:17:22.000000 selis-2.4/selis/client.py
--rw-r--r--   0 client     (501) staff       (20)     1472 2023-06-14 16:21:18.000000 selis-2.4/selis/selis.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 16:32:37.513940 selis-2.4/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-15 16:32:37.000000 selis-2.4/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      233 2023-06-15 16:32:37.000000 selis-2.4/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-15 16:32:37.000000 selis-2.4/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-15 16:32:37.000000 selis-2.4/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)       24 2023-06-15 16:32:37.000000 selis-2.4/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-15 16:32:37.000000 selis-2.4/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-15 16:32:37.514271 selis-2.4/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      279 2023-06-15 16:32:35.000000 selis-2.4/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 17:03:59.402172 selis-2.5/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-15 17:03:59.402025 selis-2.5/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 17:03:59.400302 selis-2.5/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-2.5/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     4692 2023-06-15 17:03:41.000000 selis-2.5/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)     1472 2023-06-14 16:21:18.000000 selis-2.5/selis/selis.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 17:03:59.401392 selis-2.5/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-15 17:03:59.000000 selis-2.5/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      233 2023-06-15 17:03:59.000000 selis-2.5/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-15 17:03:59.000000 selis-2.5/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-15 17:03:59.000000 selis-2.5/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)       24 2023-06-15 17:03:59.000000 selis-2.5/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-15 17:03:59.000000 selis-2.5/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-15 17:03:59.402219 selis-2.5/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      279 2023-06-15 17:03:34.000000 selis-2.5/setup.py
```

### Comparing `selis-2.4/selis/client.py` & `selis-2.5/selis/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,15 @@
             print(f"[-] Sever not found")
             sys.exit()
         self.send_info_user_to_sever()
         self.is_running = True
 
 
     def return_info_response(self, url):
-        headers = {"User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36"}
-        response = requests.get(url, headers=headers)
+        response = requests.get(url)
         soup = BeautifulSoup(response.content, "html.parser")
         return soup
     
 
     def get_info_user(self, soup):
         content = soup.find_all("td")
         for i, element in enumerate(content):
```

### Comparing `selis-2.4/selis/selis.py` & `selis-2.5/selis/selis.py`

 * *Files identical despite different names*

