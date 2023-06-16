# Comparing `tmp/msfvenomgui-0.1.0.tar.gz` & `tmp/msfvenomgui-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msfvenomgui-0.1.0.tar", max compression
+gzip compressed data, was "msfvenomgui-0.2.0.tar", max compression
```

## Comparing `msfvenomgui-0.1.0.tar` & `msfvenomgui-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-06-07 00:42:09.938622 msfvenomgui-0.1.0/LICENSE
--rw-r--r--   0        0        0       18 2023-06-07 00:42:09.938622 msfvenomgui-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-07 00:46:11.344208 msfvenomgui-0.1.0/msfvenomgui/__init__.py
--rwxr-xr-x   0        0        0      122 2023-06-07 00:54:40.295316 msfvenomgui-0.1.0/msfvenomgui/main.py
--rw-r--r--   0        0        0      383 2023-06-07 00:53:54.007035 msfvenomgui-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 msfvenomgui-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-07 00:42:09.938622 msfvenomgui-0.2.0/LICENSE
+-rw-r--r--   0        0        0      633 2023-06-16 17:51:01.399056 msfvenomgui-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 00:46:11.344208 msfvenomgui-0.2.0/msfvenomgui/__init__.py
+-rw-r--r--   0        0        0     3955 2023-06-16 17:51:01.399056 msfvenomgui-0.2.0/msfvenomgui/command_builder.py
+-rw-r--r--   0        0        0     6770 2023-06-16 18:01:32.487844 msfvenomgui-0.2.0/msfvenomgui/gui.py
+-rwxr-xr-x   0        0        0      108 2023-06-16 17:51:01.399056 msfvenomgui-0.2.0/msfvenomgui/main.py
+-rw-r--r--   0        0        0      453 2023-06-16 17:51:01.399056 msfvenomgui-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 msfvenomgui-0.2.0/PKG-INFO
```

### Comparing `msfvenomgui-0.1.0/LICENSE` & `msfvenomgui-0.2.0/LICENSE`

 * *Files identical despite different names*

