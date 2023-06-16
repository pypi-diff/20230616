# Comparing `tmp/nestedaccess-0.1.0.tar.gz` & `tmp/nestedaccess-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nestedaccess-0.1.0.tar", last modified: Thu Jun 15 10:15:56 2023, max compression
+gzip compressed data, was "dist/nestedaccess-0.1.1.tar", last modified: Fri Jun 16 04:53:22 2023, max compression
```

## Comparing `nestedaccess-0.1.0.tar` & `nestedaccess-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-15 10:15:56.368938 nestedaccess-0.1.0/
--rw-r--r--   0 wkl        (501) staff       (20)      262 2023-06-15 10:15:56.368632 nestedaccess-0.1.0/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      274 2023-06-15 09:54:02.000000 nestedaccess-0.1.0/README.md
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-15 10:15:56.367055 nestedaccess-0.1.0/nestedaccess/
--rw-r--r--   0 wkl        (501) staff       (20)        0 2023-06-15 09:55:53.000000 nestedaccess-0.1.0/nestedaccess/__init__.py
--rw-r--r--   0 wkl        (501) staff       (20)     1464 2023-06-15 09:57:28.000000 nestedaccess-0.1.0/nestedaccess/nestedaccess.py
-drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-15 10:15:56.368195 nestedaccess-0.1.0/nestedaccess.egg-info/
--rw-r--r--   0 wkl        (501) staff       (20)      262 2023-06-15 10:15:56.000000 nestedaccess-0.1.0/nestedaccess.egg-info/PKG-INFO
--rw-r--r--   0 wkl        (501) staff       (20)      216 2023-06-15 10:15:56.000000 nestedaccess-0.1.0/nestedaccess.egg-info/SOURCES.txt
--rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-15 10:15:56.000000 nestedaccess-0.1.0/nestedaccess.egg-info/dependency_links.txt
--rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-15 10:15:56.000000 nestedaccess-0.1.0/nestedaccess.egg-info/top_level.txt
--rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-15 10:15:56.369033 nestedaccess-0.1.0/setup.cfg
--rw-r--r--   0 wkl        (501) staff       (20)      349 2023-06-15 10:09:39.000000 nestedaccess-0.1.0/setup.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 04:53:22.724133 nestedaccess-0.1.1/
+-rw-r--r--   0 wkl        (501) staff       (20)     1063 2023-06-15 09:54:02.000000 nestedaccess-0.1.1/LICENSE
+-rw-r--r--   0 wkl        (501) staff       (20)       26 2023-06-16 02:46:32.000000 nestedaccess-0.1.1/MANIFEST.in
+-rw-r--r--   0 wkl        (501) staff       (20)     2821 2023-06-16 04:53:22.723887 nestedaccess-0.1.1/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)     1484 2023-06-16 04:04:24.000000 nestedaccess-0.1.1/README.md
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 04:53:22.720288 nestedaccess-0.1.1/nestedaccess/
+-rw-r--r--   0 wkl        (501) staff       (20)       50 2023-06-16 04:19:27.000000 nestedaccess-0.1.1/nestedaccess/__init__.py
+-rw-r--r--   0 wkl        (501) staff       (20)     1508 2023-06-16 01:51:10.000000 nestedaccess-0.1.1/nestedaccess/nestedaccess.py
+drwxr-xr-x   0 wkl        (501) staff       (20)        0 2023-06-16 04:53:22.723436 nestedaccess-0.1.1/nestedaccess.egg-info/
+-rw-r--r--   0 wkl        (501) staff       (20)     2821 2023-06-16 04:53:22.000000 nestedaccess-0.1.1/nestedaccess.egg-info/PKG-INFO
+-rw-r--r--   0 wkl        (501) staff       (20)      236 2023-06-16 04:53:22.000000 nestedaccess-0.1.1/nestedaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 wkl        (501) staff       (20)        1 2023-06-16 04:53:22.000000 nestedaccess-0.1.1/nestedaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       13 2023-06-16 04:53:22.000000 nestedaccess-0.1.1/nestedaccess.egg-info/top_level.txt
+-rw-r--r--   0 wkl        (501) staff       (20)       38 2023-06-16 04:53:22.724225 nestedaccess-0.1.1/setup.cfg
+-rw-r--r--   0 wkl        (501) staff       (20)     3698 2023-06-16 04:10:13.000000 nestedaccess-0.1.1/setup.py
```

### Comparing `nestedaccess-0.1.0/nestedaccess/nestedaccess.py` & `nestedaccess-0.1.1/nestedaccess/nestedaccess.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,23 +16,24 @@
         print(value)  # Output: 2
     """
     try:
         for key in keys:
             if isinstance(data, dict):
                 data = data.get(key, default)
                 if data is default:
-                    raise KeyError(f"字段 '{key}' 不存在")
+                    raise KeyError(f"field '{key}' does not exist")
             elif isinstance(data, list):
                 if isinstance(key, int):
                     if -len(data) <= key < len(data):
                         data = data[key]
                     else:
-                        raise IndexError(f"列表索引 '{key}' 超出范围")
+                        raise IndexError(f"list index '{key}' out of range")
                 else:
-                    raise TypeError("列表索引必须为整数")
+                    raise TypeError("list indices must be integers")
             else:
-                raise TypeError(f"无法获取嵌套数据，因为类型为 {type(data).__name__} 的对象没有键或索引")
+                raise TypeError(
+                    f"cannot fetch nested data because object of type {type(data).__name__} has no key or index"
+                )
     except (KeyError, IndexError, TypeError) as e:
-        print(f"发生错误: {str(e)}")
+        print(f"an error occurred: {str(e)}")
         return default
-
-    return data
+    return data
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

