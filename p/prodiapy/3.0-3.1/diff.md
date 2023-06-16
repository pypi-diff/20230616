# Comparing `tmp/prodiapy-3.0.tar.gz` & `tmp/prodiapy-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodiapy-3.0.tar", last modified: Thu Jun 15 13:06:08 2023, max compression
+gzip compressed data, was "prodiapy-3.1.tar", last modified: Fri Jun 16 04:38:30 2023, max compression
```

## Comparing `prodiapy-3.0.tar` & `prodiapy-3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 13:06:08.005341 prodiapy-3.0/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodiapy-3.0/LICENSE
--rw-rw-rw-   0        0        0     1050 2023-06-15 13:06:08.003862 prodiapy-3.0/PKG-INFO
--rw-rw-rw-   0        0        0      829 2023-06-15 13:03:38.000000 prodiapy-3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 13:06:07.994346 prodiapy-3.0/prodia/
--rw-rw-rw-   0        0        0      240 2023-06-15 12:59:58.000000 prodiapy-3.0/prodia/__init__.py
--rw-rw-rw-   0        0        0     4226 2023-06-14 12:51:44.000000 prodiapy-3.0/prodia/ext.py
--rw-rw-rw-   0        0        0    12226 2023-06-15 12:59:11.000000 prodiapy-3.0/prodia/main.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:06:08.003862 prodiapy-3.0/prodiapy.egg-info/
--rw-rw-rw-   0        0        0     1050 2023-06-15 13:06:07.000000 prodiapy-3.0/prodiapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-15 13:06:07.000000 prodiapy-3.0/prodiapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 13:06:07.000000 prodiapy-3.0/prodiapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 13:06:07.000000 prodiapy-3.0/prodiapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-15 13:06:07.000000 prodiapy-3.0/prodiapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 13:06:08.005341 prodiapy-3.0/setup.cfg
--rw-rw-rw-   0        0        0      396 2023-06-15 13:01:38.000000 prodiapy-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:38:30.199933 prodiapy-3.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodiapy-3.1/LICENSE
+-rw-rw-rw-   0        0        0     1050 2023-06-16 04:38:30.198796 prodiapy-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-06-16 04:38:02.000000 prodiapy-3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 04:38:30.185732 prodiapy-3.1/prodia/
+-rw-rw-rw-   0        0        0      240 2023-06-15 12:59:58.000000 prodiapy-3.1/prodia/__init__.py
+-rw-rw-rw-   0        0        0     4226 2023-06-14 12:51:44.000000 prodiapy-3.1/prodia/ext.py
+-rw-rw-rw-   0        0        0    12226 2023-06-15 12:59:11.000000 prodiapy-3.1/prodia/main.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:38:30.197708 prodiapy-3.1/prodiapy.egg-info/
+-rw-rw-rw-   0        0        0     1050 2023-06-16 04:38:30.000000 prodiapy-3.1/prodiapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-16 04:38:30.000000 prodiapy-3.1/prodiapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 04:38:30.000000 prodiapy-3.1/prodiapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-16 04:38:30.000000 prodiapy-3.1/prodiapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-16 04:38:30.000000 prodiapy-3.1/prodiapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 04:38:30.199933 prodiapy-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      396 2023-06-16 04:37:55.000000 prodiapy-3.1/setup.py
```

### Comparing `prodiapy-3.0/LICENSE` & `prodiapy-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prodiapy-3.0/PKG-INFO` & `prodiapy-3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: prodiapy
-Version: 3.0
+Version: 3.1
 Summary: Prodia API Python Wrapper
 Author: yoou3-cyber
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prodiapy
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodiapy==3.0
+pip install prodiapy==3.1
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
 
 key = "your-prodia-key"
 
 client = prodia.Client(api_key=key)
 
-image = prodia.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
+image = client.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
 print(image)
 ```
 `image` variable will be a url of your image
 
 [Full Documentation](https://prodiapy.readme.io/)
 
 Feel free to join out [Discord server](https://discord.gg/qX5dwV3HEp) and ask question!
```

### Comparing `prodiapy-3.0/README.md` & `prodiapy-3.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # prodiapy
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodiapy==3.0
+pip install prodiapy==3.1
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
 
 key = "your-prodia-key"
 
 client = prodia.Client(api_key=key)
 
-image = prodia.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
+image = client.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
 print(image)
 ```
 `image` variable will be a url of your image
 
 [Full Documentation](https://prodiapy.readme.io/)
 
 Feel free to join out [Discord server](https://discord.gg/qX5dwV3HEp) and ask question!
```

### Comparing `prodiapy-3.0/prodia/ext.py` & `prodiapy-3.1/prodia/ext.py`

 * *Files identical despite different names*

### Comparing `prodiapy-3.0/prodia/main.py` & `prodiapy-3.1/prodia/main.py`

 * *Files identical despite different names*

### Comparing `prodiapy-3.0/prodiapy.egg-info/PKG-INFO` & `prodiapy-3.1/prodiapy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: prodiapy
-Version: 3.0
+Version: 3.1
 Summary: Prodia API Python Wrapper
 Author: yoou3-cyber
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prodiapy
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodiapy==3.0
+pip install prodiapy==3.1
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
 
 key = "your-prodia-key"
 
 client = prodia.Client(api_key=key)
 
-image = prodia.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
+image = client.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
 print(image)
 ```
 `image` variable will be a url of your image
 
 [Full Documentation](https://prodiapy.readme.io/)
 
 Feel free to join out [Discord server](https://discord.gg/qX5dwV3HEp) and ask question!
```

