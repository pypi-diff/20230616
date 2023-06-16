# Comparing `tmp/nestedaccess-0.1.2.tar.gz` & `tmp/nestedaccess-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nestedaccess-0.1.2.tar", last modified: Fri Jun 16 05:12:43 2023, max compression
+gzip compressed data, was "dist/nestedaccess-0.1.3.tar", last modified: Fri Jun 16 05:14:58 2023, max compression
```

## Comparing `nestedaccess-0.1.2.tar` & `nestedaccess-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 05:12:43.081869 nestedaccess-0.1.2/
--rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.1.2/LICENSE
--rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.1.2/MANIFEST.in
--rw-r--r--   0 wkl        (501) staff       (20)     2821 2023-06-16 05:12:43.081278 nestedaccess-0.1.2/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)     1484 2023-06-16 04:04:24.000000 nestedaccess-0.1.2/README.md
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 05:12:43.077745 nestedaccess-0.1.2/nestedaccess/
--rw-r--r--   0 wkl        (501) staff       (20)       50 2023-06-16 04:19:27.000000 nestedaccess-0.1.2/nestedaccess/__init__.py
--rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 01:51:10.000000 nestedaccess-0.1.2/nestedaccess/nestedaccess.py
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 05:12:43.080084 nestedaccess-0.1.2/nestedaccess.egg-info/
--rw-r--r--   0 wkl        (501) staff       (20)     2821 2023-06-16 05:12:43.000000 nestedaccess-0.1.2/nestedaccess.egg-info/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      275 2023-06-16 05:12:43.000000 nestedaccess-0.1.2/nestedaccess.egg-info/SOURCES.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 05:12:43.000000 nestedaccess-0.1.2/nestedaccess.egg-info/dependency_links.txt
--rw-r--r--   0 wkl        (501) staff       (20)       40 2023-06-16 05:12:43.000000 nestedaccess-0.1.2/nestedaccess.egg-info/entry_points.txt
--rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 05:12:43.000000 nestedaccess-0.1.2/nestedaccess.egg-info/top_level.txt
--rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 05:12:43.082033 nestedaccess-0.1.2/setup.cfg
--rw-r--r--   0 wkl        (501) staff       (20)     3700 2023-06-16 05:12:38.000000 nestedaccess-0.1.2/setup.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 05:14:58.980666 nestedaccess-0.1.3/
+-rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.1.3/LICENSE
+-rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.1.3/MANIFEST.in
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 05:14:58.980021 nestedaccess-0.1.3/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)     1475 2023-06-16 05:13:48.000000 nestedaccess-0.1.3/README.md
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 05:14:58.977657 nestedaccess-0.1.3/nestedaccess/
+-rw-r--r--   0 wkl        (501) staff       (20)       50 2023-06-16 04:19:27.000000 nestedaccess-0.1.3/nestedaccess/__init__.py
+-rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 01:51:10.000000 nestedaccess-0.1.3/nestedaccess/nestedaccess.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 05:14:58.979445 nestedaccess-0.1.3/nestedaccess.egg-info/
+-rw-r--r--   0 wkl        (501) staff       (20)     2812 2023-06-16 05:14:58.000000 nestedaccess-0.1.3/nestedaccess.egg-info/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)      275 2023-06-16 05:14:58.000000 nestedaccess-0.1.3/nestedaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 05:14:58.000000 nestedaccess-0.1.3/nestedaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       40 2023-06-16 05:14:58.000000 nestedaccess-0.1.3/nestedaccess.egg-info/entry_points.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 05:14:58.000000 nestedaccess-0.1.3/nestedaccess.egg-info/top_level.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 05:14:58.980829 nestedaccess-0.1.3/setup.cfg
+-rw-r--r--   0 wkl        (501) staff       (20)     3700 2023-06-16 05:14:01.000000 nestedaccess-0.1.3/setup.py
```

### Comparing `nestedaccess-0.1.2/LICENSE` & `nestedaccess-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.1.2/PKG-INFO` & `nestedaccess-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.1.2
+Version: 0.1.3
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
@@ -27,21 +27,21 @@
                 }
             },
             'empty_list': [],
             'empty_dict': {}
         }
         
         # normal test
-        print(get_nested_data(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
+        print(nestedaccess(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
         
         # default test
-        print(get_nested_data(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
+        print(nestedaccess(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
         
         # error condition test
-        print(get_nested_data(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
+        print(nestedaccess(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
         ```
         
         # Installing Nestedaccess and Supported Versions
         
         ## Nestedaccess is available on PyPI:
         
         ```python
```

### Comparing `nestedaccess-0.1.2/README.md` & `nestedaccess-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,21 @@
         }
     },
     'empty_list': [],
     'empty_dict': {}
 }
 
 # normal test
-print(get_nested_data(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
+print(nestedaccess(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
 
 # default test
-print(get_nested_data(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
+print(nestedaccess(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
 
 # error condition test
-print(get_nested_data(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
+print(nestedaccess(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
 ```
 
 # Installing Nestedaccess and Supported Versions
 
 ## Nestedaccess is available on PyPI:
 
 ```python
```

### Comparing `nestedaccess-0.1.2/nestedaccess/nestedaccess.py` & `nestedaccess-0.1.3/nestedaccess/nestedaccess.py`

 * *Files identical despite different names*

### Comparing `nestedaccess-0.1.2/nestedaccess.egg-info/PKG-INFO` & `nestedaccess-0.1.3/nestedaccess.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaccess
-Version: 0.1.2
+Version: 0.1.3
 Summary: Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists.
 Home-page: https://github.com/Potato-OvO/nestedaccess
 Author: Potato-OvO
 Author-email: wkl1224141267@gmail.com
 License: MIT
 Description: 
         # Nestedaccess
@@ -27,21 +27,21 @@
                 }
             },
             'empty_list': [],
             'empty_dict': {}
         }
         
         # normal test
-        print(get_nested_data(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
+        print(nestedaccess(data, ['foo', 'baz', 'quux', 'grault', 1]))  # Output: 5
         
         # default test
-        print(get_nested_data(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
+        print(nestedaccess(data, ['nonexistent'], default='Not found'))  # Output: 'Not found'
         
         # error condition test
-        print(get_nested_data(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
+        print(nestedaccess(data, ['foo', 'baz', 'quux', 'corge', 'invalid']))  # Output: None (dictionary key does not exist)
         ```
         
         # Installing Nestedaccess and Supported Versions
         
         ## Nestedaccess is available on PyPI:
         
         ```python
```

### Comparing `nestedaccess-0.1.2/setup.py` & `nestedaccess-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = (
     "Nestedaccess is a simple, elegant way to retrieve nested data from deep dictionaries or lists."
 )
 URL = "https://github.com/Potato-OvO/nestedaccess"
 EMAIL = "wkl1224141267@gmail.com"
 AUTHOR = "Potato-OvO"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 LICENSE = "MIT"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
```

