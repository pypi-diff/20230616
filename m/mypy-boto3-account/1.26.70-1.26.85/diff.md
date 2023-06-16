# Comparing `tmp/mypy-boto3-account-1.26.70.tar.gz` & `tmp/mypy-boto3-account-1.26.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-account-1.26.70.tar", last modified: Mon Feb 13 20:27:09 2023, max compression
+gzip compressed data, was "mypy-boto3-account-1.26.85.tar", last modified: Mon Mar  6 20:27:45 2023, max compression
```

## Comparing `mypy-boto3-account-1.26.70.tar` & `mypy-boto3-account-1.26.85.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:27:09.130620 mypy-boto3-account-1.26.70/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-13 20:26:57.000000 mypy-boto3-account-1.26.70/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-02-13 20:27:09.130620 mypy-boto3-account-1.26.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-02-13 20:26:57.000000 mypy-boto3-account-1.26.70/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:27:09.126620 mypy-boto3-account-1.26.70/mypy_boto3_account/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-13 20:26:57.000000 mypy-boto3-account-1.26.70/mypy_boto3_account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-13 20:26:57.000000 mypy-boto3-account-1.26.70/mypy_boto3_account/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-13 20:26:57.000000 mypy-boto3-account-1.26.70/mypy_boto3_account/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-02-13 20:26:57.000000 mypy-boto3-account-1.26.70/mypy_boto3_account/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-02-13 20:26:57.000000 mypy-boto3-account-1.26.70/mypy_boto3_account/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-02-13 20:26:58.000000 mypy-boto3-account-1.26.70/mypy_boto3_account/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-02-13 20:26:57.000000 mypy-boto3-account-1.26.70/mypy_boto3_account/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 20:26:57.000000 mypy-boto3-account-1.26.70/mypy_boto3_account/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-02-13 20:26:58.000000 mypy-boto3-account-1.26.70/mypy_boto3_account/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-02-13 20:26:58.000000 mypy-boto3-account-1.26.70/mypy_boto3_account/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-13 20:26:57.000000 mypy-boto3-account-1.26.70/mypy_boto3_account/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:27:09.130620 mypy-boto3-account-1.26.70/mypy_boto3_account.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-02-13 20:27:09.000000 mypy-boto3-account-1.26.70/mypy_boto3_account.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-13 20:27:09.000000 mypy-boto3-account-1.26.70/mypy_boto3_account.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 20:27:09.000000 mypy-boto3-account-1.26.70/mypy_boto3_account.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 20:27:09.000000 mypy-boto3-account-1.26.70/mypy_boto3_account.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-13 20:27:09.000000 mypy-boto3-account-1.26.70/mypy_boto3_account.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-13 20:27:09.000000 mypy-boto3-account-1.26.70/mypy_boto3_account.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 20:27:09.130620 mypy-boto3-account-1.26.70/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-13 20:26:57.000000 mypy-boto3-account-1.26.70/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:45.496845 mypy-boto3-account-1.26.85/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-03-06 20:27:45.496845 mypy-boto3-account-1.26.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:45.496845 mypy-boto3-account-1.26.85/mypy_boto3_account/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-03-06 20:27:34.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:45.496845 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-03-06 20:27:45.000000 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-06 20:27:45.000000 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 20:27:45.000000 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 20:27:45.000000 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-06 20:27:45.000000 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-06 20:27:45.000000 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 20:27:45.496845 mypy-boto3-account-1.26.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/setup.py
```

### Comparing `mypy-boto3-account-1.26.70/LICENSE` & `mypy-boto3-account-1.26.85/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.26.70/PKG-INFO` & `mypy-boto3-account-1.26.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-account
-Version: 1.26.70
-Summary: Type annotations for boto3.Account 1.26.70 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.85
+Summary: Type annotations for boto3.Account 1.26.85 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-account?color=blue)](https://pypistats.org/packages/mypy-boto3-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Account 1.26.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[boto3.Account 1.26.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-account docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-account-1.26.70/README.md` & `mypy-boto3-account-1.26.85/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-account?color=blue)](https://pypistats.org/packages/mypy-boto3-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Account 1.26.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[boto3.Account 1.26.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-account docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-account-1.26.70/mypy_boto3_account/__main__.py` & `mypy-boto3-account-1.26.85/mypy_boto3_account/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Account 1.26.70\nVersion:         1.26.70\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Account 1.26.85\nVersion:         1.26.85\nBuilder version:"
+        " 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.70")
+    print("1.26.85")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-account-1.26.70/mypy_boto3_account/client.py` & `mypy-boto3-account-1.26.85/mypy_boto3_account/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.26.70/mypy_boto3_account/client.pyi` & `mypy-boto3-account-1.26.85/mypy_boto3_account/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.26.70/mypy_boto3_account/literals.py` & `mypy-boto3-account-1.26.85/mypy_boto3_account/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -351,14 +352,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-account-1.26.70/mypy_boto3_account/literals.pyi` & `mypy-boto3-account-1.26.85/mypy_boto3_account/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -349,14 +350,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-account-1.26.70/mypy_boto3_account/type_defs.py` & `mypy-boto3-account-1.26.85/mypy_boto3_account/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.26.70/mypy_boto3_account/type_defs.pyi` & `mypy-boto3-account-1.26.85/mypy_boto3_account/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.26.70/mypy_boto3_account.egg-info/PKG-INFO` & `mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-account
-Version: 1.26.70
-Summary: Type annotations for boto3.Account 1.26.70 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.85
+Summary: Type annotations for boto3.Account 1.26.85 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-account?color=blue)](https://pypistats.org/packages/mypy-boto3-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Account 1.26.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[boto3.Account 1.26.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-account docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-account-1.26.70/mypy_boto3_account.egg-info/SOURCES.txt` & `mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.26.70/setup.py` & `mypy-boto3-account-1.26.85/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-account",
-    version="1.26.70",
+    version="1.26.85",
     packages=["mypy_boto3_account"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Account 1.26.70 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Account 1.26.85 service generated with mypy-boto3-builder"
+        " 7.12.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

