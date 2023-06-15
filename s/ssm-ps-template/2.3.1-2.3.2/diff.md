# Comparing `tmp/ssm-ps-template-2.3.1.tar.gz` & `tmp/ssm-ps-template-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-2.3.1.tar", last modified: Fri Jun  9 17:01:16 2023, max compression
+gzip compressed data, was "ssm-ps-template-2.3.2.tar", last modified: Thu Jun 15 23:04:14 2023, max compression
```

## Comparing `ssm-ps-template-2.3.1.tar` & `ssm-ps-template-2.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:01:16.053104 ssm-ps-template-2.3.1/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    12318 2023-06-09 17:01:16.049104 ssm-ps-template-2.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9682 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1879 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 17:01:16.053104 ssm-ps-template-2.3.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:01:16.045104 ssm-ps-template-2.3.1/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3254 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/ssm_ps_template/discovery.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     3462 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:01:16.049104 ssm-ps-template-2.3.1/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12318 2023-06-09 17:01:16.000000 ssm-ps-template-2.3.1/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2023-06-09 17:01:16.000000 ssm-ps-template-2.3.1/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 17:01:16.000000 ssm-ps-template-2.3.1/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-09 17:01:16.000000 ssm-ps-template-2.3.1/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      246 2023-06-09 17:01:16.000000 ssm-ps-template-2.3.1/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-09 17:01:16.000000 ssm-ps-template-2.3.1/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:01:16.049104 ssm-ps-template-2.3.1/tests/
--rw-r--r--   0 root         (0) root         (0)     2833 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/tests/test_discovery.py
--rw-r--r--   0 root         (0) root         (0)     1332 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/tests/test_render.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-06-09 17:01:06.000000 ssm-ps-template-2.3.1/tests/test_ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:04:14.803370 ssm-ps-template-2.3.2/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    12318 2023-06-15 23:04:14.803370 ssm-ps-template-2.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9682 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 23:04:14.803370 ssm-ps-template-2.3.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:04:14.803370 ssm-ps-template-2.3.2/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/ssm_ps_template/discovery.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:04:14.803370 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12318 2023-06-15 23:04:14.000000 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2023-06-15 23:04:14.000000 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 23:04:14.000000 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-15 23:04:14.000000 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-15 23:04:14.000000 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-15 23:04:14.000000 ssm-ps-template-2.3.2/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 23:04:14.803370 ssm-ps-template-2.3.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     2833 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/tests/test_discovery.py
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/tests/test_render.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-06-15 23:04:04.000000 ssm-ps-template-2.3.2/tests/test_ssm.py
```

### Comparing `ssm-ps-template-2.3.1/LICENSE.txt` & `ssm-ps-template-2.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.1/PKG-INFO` & `ssm-ps-template-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.3.1
+Version: 2.3.2
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
```

### Comparing `ssm-ps-template-2.3.1/README.md` & `ssm-ps-template-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.1/pyproject.toml` & `ssm-ps-template-2.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ssm-ps-template"
-version = "2.3.1"
+version = "2.3.2"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: BSD License",
@@ -14,15 +14,15 @@
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Natural Language :: English",
     "Topic :: Text Processing",
     "Topic :: Utilities"
 ]
 dependencies = [
-    "boto3>=1.26.127,<2",
+    "boto3>=1.26,<2",
     "flatdict>=4,<5",
     "jinja2>=3,<4",
     "pyyaml>=5.3.1,<6",
     "toml>=0.10,<1"
 ]
 keywords = ["aws", "ssm", "parameter store", "templating"]
 license = {file = "LICENSE.txt"}
```

### Comparing `ssm-ps-template-2.3.1/ssm_ps_template/__main__.py` & `ssm-ps-template-2.3.2/ssm_ps_template/__main__.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.1/ssm_ps_template/config.py` & `ssm-ps-template-2.3.2/ssm_ps_template/config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.1/ssm_ps_template/discovery.py` & `ssm-ps-template-2.3.2/ssm_ps_template/discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.1/ssm_ps_template/render.py` & `ssm-ps-template-2.3.2/ssm_ps_template/render.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.1/ssm_ps_template/ssm.py` & `ssm-ps-template-2.3.2/ssm_ps_template/ssm.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.1/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-2.3.2/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.3.1
+Version: 2.3.2
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
```

### Comparing `ssm-ps-template-2.3.1/ssm_ps_template.egg-info/SOURCES.txt` & `ssm-ps-template-2.3.2/ssm_ps_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.1/tests/test_config.py` & `ssm-ps-template-2.3.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.1/tests/test_discovery.py` & `ssm-ps-template-2.3.2/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.1/tests/test_main.py` & `ssm-ps-template-2.3.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.1/tests/test_render.py` & `ssm-ps-template-2.3.2/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.3.1/tests/test_ssm.py` & `ssm-ps-template-2.3.2/tests/test_ssm.py`

 * *Files identical despite different names*

