# Comparing `tmp/mistune_jira-2023.6.16.0.tar.gz` & `tmp/mistune_jira-2023.6.16.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistune_jira-2023.6.16.0.tar", last modified: Fri Jun 16 16:25:20 2023, max compression
+gzip compressed data, was "mistune_jira-2023.6.16.2.tar", last modified: Fri Jun 16 17:23:23 2023, max compression
```

## Comparing `mistune_jira-2023.6.16.0.tar` & `mistune_jira-2023.6.16.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:25:20.007146 mistune_jira-2023.6.16.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-16 16:25:03.000000 mistune_jira-2023.6.16.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-16 16:25:20.007146 mistune_jira-2023.6.16.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-16 16:25:03.000000 mistune_jira-2023.6.16.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:25:20.007146 mistune_jira-2023.6.16.0/mistune_jira/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 16:25:03.000000 mistune_jira-2023.6.16.0/mistune_jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-16 16:25:03.000000 mistune_jira-2023.6.16.0/mistune_jira/jiraRenderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:25:20.007146 mistune_jira-2023.6.16.0/mistune_jira.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-16 16:25:19.000000 mistune_jira-2023.6.16.0/mistune_jira.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-16 16:25:19.000000 mistune_jira-2023.6.16.0/mistune_jira.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:25:19.000000 mistune_jira-2023.6.16.0/mistune_jira.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 16:25:19.000000 mistune_jira-2023.6.16.0/mistune_jira.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 16:25:19.000000 mistune_jira-2023.6.16.0/mistune_jira.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-16 16:25:03.000000 mistune_jira-2023.6.16.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:25:20.007146 mistune_jira-2023.6.16.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:23:23.032403 mistune_jira-2023.6.16.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-16 17:23:05.000000 mistune_jira-2023.6.16.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-16 17:23:23.032403 mistune_jira-2023.6.16.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-16 17:23:05.000000 mistune_jira-2023.6.16.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:23:23.032403 mistune_jira-2023.6.16.2/mistune_jira/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 17:23:05.000000 mistune_jira-2023.6.16.2/mistune_jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-16 17:23:05.000000 mistune_jira-2023.6.16.2/mistune_jira/jiraRenderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:23:23.032403 mistune_jira-2023.6.16.2/mistune_jira.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-16 17:23:22.000000 mistune_jira-2023.6.16.2/mistune_jira.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-16 17:23:23.000000 mistune_jira-2023.6.16.2/mistune_jira.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:23:22.000000 mistune_jira-2023.6.16.2/mistune_jira.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 17:23:22.000000 mistune_jira-2023.6.16.2/mistune_jira.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 17:23:22.000000 mistune_jira-2023.6.16.2/mistune_jira.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-16 17:23:05.000000 mistune_jira-2023.6.16.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 17:23:23.032403 mistune_jira-2023.6.16.2/setup.cfg
```

### Comparing `mistune_jira-2023.6.16.0/LICENSE` & `mistune_jira-2023.6.16.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mistune_jira-2023.6.16.0/PKG-INFO` & `mistune_jira-2023.6.16.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistune_jira
-Version: 2023.6.16.0
+Version: 2023.6.16.2
 Summary: A mostly functional plugin for mistune to render Jira's markup language
 Author-email: Chris Halbersma <chris@halbersma.us>
 License: BSD-3-Clause
 Keywords: mistune,jira,atlassian
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `mistune_jira-2023.6.16.0/README.md` & `mistune_jira-2023.6.16.2/README.md`

 * *Files identical despite different names*

### Comparing `mistune_jira-2023.6.16.0/mistune_jira/jiraRenderer.py` & `mistune_jira-2023.6.16.2/mistune_jira/jiraRenderer.py`

 * *Files identical despite different names*

### Comparing `mistune_jira-2023.6.16.0/mistune_jira.egg-info/PKG-INFO` & `mistune_jira-2023.6.16.2/mistune_jira.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistune-jira
-Version: 2023.6.16.0
+Version: 2023.6.16.2
 Summary: A mostly functional plugin for mistune to render Jira's markup language
 Author-email: Chris Halbersma <chris@halbersma.us>
 License: BSD-3-Clause
 Keywords: mistune,jira,atlassian
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `mistune_jira-2023.6.16.0/pyproject.toml` & `mistune_jira-2023.6.16.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "twine",
   "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mistune_jira"
-version = "2023.6.16.0"
+version = "2023.6.16.2"
 authors = [
     {name = "Chris Halbersma", email = "chris@halbersma.us"},
 ]
 description = "A mostly functional plugin for mistune to render Jira's markup language"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["mistune", "jira", "atlassian"]
```

