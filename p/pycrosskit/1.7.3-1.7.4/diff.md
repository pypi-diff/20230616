# Comparing `tmp/pycrosskit-1.7.3.tar.gz` & `tmp/pycrosskit-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrosskit-1.7.3.tar", last modified: Fri Jun 16 07:33:04 2023, max compression
+gzip compressed data, was "pycrosskit-1.7.4.tar", last modified: Fri Jun 16 07:35:34 2023, max compression
```

## Comparing `pycrosskit-1.7.3.tar` & `pycrosskit-1.7.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:33:04.636598 pycrosskit-1.7.3/pycrosskit/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/pycrosskit/env_platforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/env_platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/env_platforms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/env_platforms/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/env_platforms/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/envariables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/pycrosskit/shortcut_platforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/shortcut_platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/shortcut_platforms/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/shortcut_platforms/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/pycrosskit/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/pycrosskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:33:04.000000 pycrosskit-1.7.3/pycrosskit.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:33:04.640598 pycrosskit-1.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/tests/test_env_vars_linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/tests/test_env_vars_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-16 07:32:51.000000 pycrosskit-1.7.3/tests/test_shortcut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:34.840077 pycrosskit-1.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-16 07:35:34.840077 pycrosskit-1.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:34.836077 pycrosskit-1.7.4/pycrosskit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/pycrosskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/pycrosskit/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/pycrosskit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:34.836077 pycrosskit-1.7.4/pycrosskit/env_platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/pycrosskit/env_platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/pycrosskit/env_platforms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/pycrosskit/env_platforms/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/pycrosskit/env_platforms/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/pycrosskit/envariables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:34.840077 pycrosskit-1.7.4/pycrosskit/shortcut_platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/pycrosskit/shortcut_platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/pycrosskit/shortcut_platforms/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/pycrosskit/shortcut_platforms/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/pycrosskit/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:34.836077 pycrosskit-1.7.4/pycrosskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-16 07:35:34.000000 pycrosskit-1.7.4/pycrosskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-16 07:35:34.000000 pycrosskit-1.7.4/pycrosskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:35:34.000000 pycrosskit-1.7.4/pycrosskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 07:35:34.000000 pycrosskit-1.7.4/pycrosskit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-16 07:35:34.000000 pycrosskit-1.7.4/pycrosskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 07:35:34.000000 pycrosskit-1.7.4/pycrosskit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:35:34.000000 pycrosskit-1.7.4/pycrosskit.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 07:35:34.840077 pycrosskit-1.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:34.840077 pycrosskit-1.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/tests/test_env_vars_linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/tests/test_env_vars_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-16 07:35:22.000000 pycrosskit-1.7.4/tests/test_shortcut.py
```

### Comparing `pycrosskit-1.7.3/LICENSE.md` & `pycrosskit-1.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.3/PKG-INFO` & `pycrosskit-1.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pycrosskit
-Version: 1.7.3
+Version: 1.7.4
 Summary: Cross Platform Toolkit for Windows and Linux in order to make variables and shortcuts easy 
 Home-page: https://github.com/jiri-otoupal/py-cross-kit
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: Apache 2.0
 Keywords: Python Cross Platform Toolkit
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6,<4
+Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # Python Cross Platform Toolkit for Windows and Linux variables, shortcuts and start menu shortcuts
 
 Simple Cross Platform creation of shortcuts and Persistent Environment Variables
```

### Comparing `pycrosskit-1.7.3/README.md` & `pycrosskit-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.3/pycrosskit/__init__.py` & `pycrosskit-1.7.4/pycrosskit/__init__.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.3/pycrosskit/env_platforms/linux.py` & `pycrosskit-1.7.4/pycrosskit/env_platforms/linux.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.3/pycrosskit/env_platforms/windows.py` & `pycrosskit-1.7.4/pycrosskit/env_platforms/windows.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.3/pycrosskit/envariables.py` & `pycrosskit-1.7.4/pycrosskit/envariables.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.3/pycrosskit/shortcut_platforms/linux.py` & `pycrosskit-1.7.4/pycrosskit/shortcut_platforms/linux.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.3/pycrosskit/shortcut_platforms/windows.py` & `pycrosskit-1.7.4/pycrosskit/shortcut_platforms/windows.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.3/pycrosskit/shortcuts.py` & `pycrosskit-1.7.4/pycrosskit/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.3/pycrosskit.egg-info/PKG-INFO` & `pycrosskit-1.7.4/pycrosskit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pycrosskit
-Version: 1.7.3
+Version: 1.7.4
 Summary: Cross Platform Toolkit for Windows and Linux in order to make variables and shortcuts easy 
 Home-page: https://github.com/jiri-otoupal/py-cross-kit
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: Apache 2.0
 Keywords: Python Cross Platform Toolkit
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6,<4
+Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # Python Cross Platform Toolkit for Windows and Linux variables, shortcuts and start menu shortcuts
 
 Simple Cross Platform creation of shortcuts and Persistent Environment Variables
```

### Comparing `pycrosskit-1.7.3/pycrosskit.egg-info/SOURCES.txt` & `pycrosskit-1.7.4/pycrosskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.3/setup.py` & `pycrosskit-1.7.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,28 +23,27 @@
     long_description_content_type="text/markdown",
     version=about["__version__"],
     author=about["__author__"],
     author_email=about["__author_email__"],
     url=about["__url__"],
     packages=find_packages(),
     include_package_data=True,
-    python_requires=">=3.6,<4",
+    python_requires=">=3.7,<4",
     install_requires=["pywin32>=300; sys_platform == 'win32'"],
     extras_require={
         "dev": ["black>=22,<24", "flake8<6.1", "pre-commit<3.3", "pytest<7.4"],
     },
     license=about["__license__"],
     zip_safe=True,
     entry_points={
         "console_scripts": ["pycrosskit=entry_points:main"],
     },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     keywords="Python Cross Platform Toolkit",
```

### Comparing `pycrosskit-1.7.3/tests/test_env_vars_linux.py` & `pycrosskit-1.7.4/tests/test_env_vars_linux.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.3/tests/test_env_vars_windows.py` & `pycrosskit-1.7.4/tests/test_env_vars_windows.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.7.3/tests/test_shortcut.py` & `pycrosskit-1.7.4/tests/test_shortcut.py`

 * *Files identical despite different names*

