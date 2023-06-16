# Comparing `tmp/msfvenomgui-0.2.0.tar.gz` & `tmp/msfvenomgui-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msfvenomgui-0.2.0.tar", max compression
+gzip compressed data, was "msfvenomgui-0.2.1.tar", max compression
```

## Comparing `msfvenomgui-0.2.0.tar` & `msfvenomgui-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-06-07 00:42:09.938622 msfvenomgui-0.2.0/LICENSE
--rw-r--r--   0        0        0      633 2023-06-16 17:51:01.399056 msfvenomgui-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-07 00:46:11.344208 msfvenomgui-0.2.0/msfvenomgui/__init__.py
--rw-r--r--   0        0        0     3955 2023-06-16 17:51:01.399056 msfvenomgui-0.2.0/msfvenomgui/command_builder.py
--rw-r--r--   0        0        0     6770 2023-06-16 18:01:32.487844 msfvenomgui-0.2.0/msfvenomgui/gui.py
--rwxr-xr-x   0        0        0      108 2023-06-16 17:51:01.399056 msfvenomgui-0.2.0/msfvenomgui/main.py
--rw-r--r--   0        0        0      453 2023-06-16 17:51:01.399056 msfvenomgui-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 msfvenomgui-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-07 00:42:09.938622 msfvenomgui-0.2.1/LICENSE
+-rw-r--r--   0        0        0      633 2023-06-16 17:51:01.399056 msfvenomgui-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 00:46:11.344208 msfvenomgui-0.2.1/msfvenomgui/__init__.py
+-rw-r--r--   0        0        0     3955 2023-06-16 17:51:01.399056 msfvenomgui-0.2.1/msfvenomgui/command_builder.py
+-rw-r--r--   0        0        0     6770 2023-06-16 18:01:32.487844 msfvenomgui-0.2.1/msfvenomgui/gui.py
+-rwxr-xr-x   0        0        0      108 2023-06-16 17:51:01.399056 msfvenomgui-0.2.1/msfvenomgui/main.py
+-rw-r--r--   0        0        0      502 2023-06-16 18:08:28.719469 msfvenomgui-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 msfvenomgui-0.2.1/PKG-INFO
```

### Comparing `msfvenomgui-0.2.0/LICENSE` & `msfvenomgui-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `msfvenomgui-0.2.0/README.md` & `msfvenomgui-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `msfvenomgui-0.2.0/msfvenomgui/command_builder.py` & `msfvenomgui-0.2.1/msfvenomgui/command_builder.py`

 * *Files identical despite different names*

### Comparing `msfvenomgui-0.2.0/msfvenomgui/gui.py` & `msfvenomgui-0.2.1/msfvenomgui/gui.py`

 * *Files identical despite different names*

### Comparing `msfvenomgui-0.2.0/PKG-INFO` & `msfvenomgui-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msfvenomgui
-Version: 0.2.0
+Version: 0.2.1
 Summary: msfvenomgui provides a graphical UI over Metasploit's msfvenom tool.
 License: GPL-3.0-only
 Author: bluesentinelsec
 Author-email: bluesentinel@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

