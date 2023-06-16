# Comparing `tmp/prodiapy-3.1.tar.gz` & `tmp/prodiapy-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodiapy-3.1.tar", last modified: Fri Jun 16 04:38:30 2023, max compression
+gzip compressed data, was "prodiapy-3.2.tar", last modified: Fri Jun 16 04:43:41 2023, max compression
```

## Comparing `prodiapy-3.1.tar` & `prodiapy-3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 04:38:30.199933 prodiapy-3.1/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodiapy-3.1/LICENSE
--rw-rw-rw-   0        0        0     1050 2023-06-16 04:38:30.198796 prodiapy-3.1/PKG-INFO
--rw-rw-rw-   0        0        0      829 2023-06-16 04:38:02.000000 prodiapy-3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 04:38:30.185732 prodiapy-3.1/prodia/
--rw-rw-rw-   0        0        0      240 2023-06-15 12:59:58.000000 prodiapy-3.1/prodia/__init__.py
--rw-rw-rw-   0        0        0     4226 2023-06-14 12:51:44.000000 prodiapy-3.1/prodia/ext.py
--rw-rw-rw-   0        0        0    12226 2023-06-15 12:59:11.000000 prodiapy-3.1/prodia/main.py
-drwxrwxrwx   0        0        0        0 2023-06-16 04:38:30.197708 prodiapy-3.1/prodiapy.egg-info/
--rw-rw-rw-   0        0        0     1050 2023-06-16 04:38:30.000000 prodiapy-3.1/prodiapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-16 04:38:30.000000 prodiapy-3.1/prodiapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 04:38:30.000000 prodiapy-3.1/prodiapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-16 04:38:30.000000 prodiapy-3.1/prodiapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-16 04:38:30.000000 prodiapy-3.1/prodiapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 04:38:30.199933 prodiapy-3.1/setup.cfg
--rw-rw-rw-   0        0        0      396 2023-06-16 04:37:55.000000 prodiapy-3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:43:41.809860 prodiapy-3.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodiapy-3.2/LICENSE
+-rw-rw-rw-   0        0        0     1050 2023-06-16 04:43:41.808592 prodiapy-3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-06-16 04:43:22.000000 prodiapy-3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 04:43:41.800596 prodiapy-3.2/prodia/
+-rw-rw-rw-   0        0        0      240 2023-06-15 12:59:58.000000 prodiapy-3.2/prodia/__init__.py
+-rw-rw-rw-   0        0        0     4226 2023-06-14 12:51:44.000000 prodiapy-3.2/prodia/ext.py
+-rw-rw-rw-   0        0        0    12255 2023-06-16 04:42:15.000000 prodiapy-3.2/prodia/main.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:43:41.807259 prodiapy-3.2/prodiapy.egg-info/
+-rw-rw-rw-   0        0        0     1050 2023-06-16 04:43:41.000000 prodiapy-3.2/prodiapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-16 04:43:41.000000 prodiapy-3.2/prodiapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 04:43:41.000000 prodiapy-3.2/prodiapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-16 04:43:41.000000 prodiapy-3.2/prodiapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-16 04:43:41.000000 prodiapy-3.2/prodiapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 04:43:41.809860 prodiapy-3.2/setup.cfg
+-rw-rw-rw-   0        0        0      396 2023-06-16 04:43:12.000000 prodiapy-3.2/setup.py
```

### Comparing `prodiapy-3.1/LICENSE` & `prodiapy-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prodiapy-3.1/PKG-INFO` & `prodiapy-3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: prodiapy
-Version: 3.1
+Version: 3.2
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
-pip install prodiapy==3.1
+pip install prodiapy==3.2
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
```

### Comparing `prodiapy-3.1/README.md` & `prodiapy-3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # prodiapy
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodiapy==3.1
+pip install prodiapy==3.2
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
```

### Comparing `prodiapy-3.1/prodia/ext.py` & `prodiapy-3.2/prodia/ext.py`

 * *Files identical despite different names*

### Comparing `prodiapy-3.1/prodia/main.py` & `prodiapy-3.2/prodia/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 import requests
 import time
-import os
 import asyncio
-from prodia import endpoint, names
+import re
+from . import ext
+endpoint = ext.endpoint
+names = ext.names
+models = ext.models
+get_seed = ext.get_seed
 
 
 
+
+class free_api:
+    key1 = "89c5ea85-407c-4d57-b410-908f1a5e135c"
+
+
 async def one_txt2img(key:str = None,
                       prompt: str = None,
                       negative_prompt: str = "badly drawn",
                       model: str = names.realisticvs14,
                       sampler: str = "DDIM",
                       aspect_ratio: str = "square",
                       steps: int = 30,
@@ -136,16 +145,14 @@
             return images
         elif mode == "img2img":
             images = await asyncio.gather(*[
                 one_img2img(key=key, image_url=image_url, prompt=prompt, negative_prompt=negative_prompt, model=model, sampler=sampler,
                             denoising_strength=denoising_strength, steps=steps, cfg_scale=cfg_scale, seed=seed, upscale=upscale) for
                 _ in range(number_outputs)])
             return images
-        elif mode == "save":
-            await asyncio.gather(*[one_save(images=images) for _ in range(len(images))])
 
 
 
 class Client:
     def __init__(self, api_key:str) -> None:
         self.api_key = api_key
 
@@ -312,7 +319,8 @@
             return
         if prompt is None:
             print("Prompt cant be empty")
             return
         images = await gather(mode="img2img", key=self.api_key, image_url=image_url, prompt=prompt, negative_prompt=negative_prompt, model=model, sampler=sampler, denoising_strength=denoising_strength, steps=steps, cfg_scale=cfg_scale, seed=seed, upscale=upscale, number_outputs=number_outputs)
         return images
 
+
```

### Comparing `prodiapy-3.1/prodiapy.egg-info/PKG-INFO` & `prodiapy-3.2/prodiapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: prodiapy
-Version: 3.1
+Version: 3.2
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
-pip install prodiapy==3.1
+pip install prodiapy==3.2
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
```

