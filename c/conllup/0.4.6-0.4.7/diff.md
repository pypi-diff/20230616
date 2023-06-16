# Comparing `tmp/conllup-0.4.6.tar.gz` & `tmp/conllup-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conllup-0.4.6.tar", last modified: Tue Apr 18 13:20:14 2023, max compression
+gzip compressed data, was "conllup-0.4.7.tar", last modified: Fri Jun 16 09:08:55 2023, max compression
```

## Comparing `conllup-0.4.6.tar` & `conllup-0.4.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-18 13:20:14.257676 conllup-0.4.6/
--rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-04-18 13:20:14.257676 conllup-0.4.6/PKG-INFO
--rw-rw-r--   0 wran      (1000) wran      (1000)     3499 2023-04-18 13:19:26.000000 conllup-0.4.6/README.md
--rw-rw-r--   0 wran      (1000) wran      (1000)       24 2023-02-01 16:20:21.000000 conllup-0.4.6/long_description.rst
--rw-rw-r--   0 wran      (1000) wran      (1000)      246 2023-04-18 13:19:26.000000 conllup-0.4.6/pyproject.toml
--rw-rw-r--   0 wran      (1000) wran      (1000)      482 2023-04-18 13:20:14.257676 conllup-0.4.6/setup.cfg
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-18 13:20:14.253676 conllup-0.4.6/src/
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-18 13:20:14.253676 conllup-0.4.6/src/conllup/
--rw-rw-r--   0 wran      (1000) wran      (1000)        0 2023-01-30 16:14:25.000000 conllup-0.4.6/src/conllup/__init__.py
--rw-rw-r--   0 wran      (1000) wran      (1000)    12044 2023-04-18 13:10:04.000000 conllup-0.4.6/src/conllup/conllup.py
--rw-rw-r--   0 wran      (1000) wran      (1000)     6856 2023-04-18 13:11:48.000000 conllup-0.4.6/src/conllup/processing.py
--rw-rw-r--   0 wran      (1000) wran      (1000)      570 2023-04-18 13:10:04.000000 conllup-0.4.6/src/conllup/types.py
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-18 13:20:14.257676 conllup-0.4.6/src/conllup.egg-info/
--rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-04-18 13:20:14.000000 conllup-0.4.6/src/conllup.egg-info/PKG-INFO
--rw-rw-r--   0 wran      (1000) wran      (1000)      289 2023-04-18 13:20:14.000000 conllup-0.4.6/src/conllup.egg-info/SOURCES.txt
--rw-rw-r--   0 wran      (1000) wran      (1000)        1 2023-04-18 13:20:14.000000 conllup-0.4.6/src/conllup.egg-info/dependency_links.txt
--rw-rw-r--   0 wran      (1000) wran      (1000)        8 2023-04-18 13:20:14.000000 conllup-0.4.6/src/conllup.egg-info/top_level.txt
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-06-16 09:08:55.405999 conllup-0.4.7/
+-rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-06-16 09:08:55.405999 conllup-0.4.7/PKG-INFO
+-rw-rw-r--   0 wran      (1000) wran      (1000)     3499 2023-04-18 13:19:26.000000 conllup-0.4.7/README.md
+-rw-rw-r--   0 wran      (1000) wran      (1000)       24 2023-02-01 16:20:21.000000 conllup-0.4.7/long_description.rst
+-rw-rw-r--   0 wran      (1000) wran      (1000)      246 2023-06-16 09:08:21.000000 conllup-0.4.7/pyproject.toml
+-rw-rw-r--   0 wran      (1000) wran      (1000)      482 2023-06-16 09:08:55.405999 conllup-0.4.7/setup.cfg
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-06-16 09:08:55.401999 conllup-0.4.7/src/
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-06-16 09:08:55.405999 conllup-0.4.7/src/conllup/
+-rw-rw-r--   0 wran      (1000) wran      (1000)        0 2023-01-30 16:14:25.000000 conllup-0.4.7/src/conllup/__init__.py
+-rw-rw-r--   0 wran      (1000) wran      (1000)    11986 2023-06-16 09:06:17.000000 conllup-0.4.7/src/conllup/conllup.py
+-rw-rw-r--   0 wran      (1000) wran      (1000)     6856 2023-04-18 13:11:48.000000 conllup-0.4.7/src/conllup/processing.py
+-rw-rw-r--   0 wran      (1000) wran      (1000)      570 2023-04-18 13:10:04.000000 conllup-0.4.7/src/conllup/types.py
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-06-16 09:08:55.405999 conllup-0.4.7/src/conllup.egg-info/
+-rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-06-16 09:08:55.000000 conllup-0.4.7/src/conllup.egg-info/PKG-INFO
+-rw-rw-r--   0 wran      (1000) wran      (1000)      289 2023-06-16 09:08:55.000000 conllup-0.4.7/src/conllup.egg-info/SOURCES.txt
+-rw-rw-r--   0 wran      (1000) wran      (1000)        1 2023-06-16 09:08:55.000000 conllup-0.4.7/src/conllup.egg-info/dependency_links.txt
+-rw-rw-r--   0 wran      (1000) wran      (1000)        8 2023-06-16 09:08:55.000000 conllup-0.4.7/src/conllup.egg-info/top_level.txt
```

### Comparing `conllup-0.4.6/README.md` & `conllup-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `conllup-0.4.6/src/conllup/conllup.py` & `conllup-0.4.7/src/conllup/conllup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,20 +76,18 @@
             raise Exception(f"DUPLICATED KEY : found (among others) the duplicated `{featureKey}` key")
         featuresJson[featureKey] = featureValue
 
     return featuresJson
 
 
 def _featuresJsonToConll(featuresJson: featuresJson_T) -> str:
-    splittedFeatureConll: List[str] = []
-    for [featureKey, featureValue] in featuresJson.items():
-        splittedFeatureConll.append(f"{featureKey}={featureValue}")
-    splittedFeatureConll.sort()
+    featureItems = list(featuresJson.items())
+    featureItems.sort(key=lambda item: item[0].lower())
+    splittedFeatureConll=[f"{item[0]}={item[1]}" for item in featureItems]
     featuresConll = "|".join(splittedFeatureConll)
-    featuresConll = featuresConll
     if featuresConll == "":
         featuresConll = "_"
     return featuresConll
 
 
 def _normalizeHyphensInTab(tokenTabData: str, tabLabel: str):
     """
```

### Comparing `conllup-0.4.6/src/conllup/processing.py` & `conllup-0.4.7/src/conllup/processing.py`

 * *Files identical despite different names*

### Comparing `conllup-0.4.6/src/conllup/types.py` & `conllup-0.4.7/src/conllup/types.py`

 * *Files identical despite different names*

