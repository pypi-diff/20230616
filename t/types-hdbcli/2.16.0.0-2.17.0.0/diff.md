# Comparing `tmp/types-hdbcli-2.16.0.0.tar.gz` & `tmp/types-hdbcli-2.17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-hdbcli-2.16.0.0.tar", last modified: Sat Apr 29 15:14:01 2023, max compression
+gzip compressed data, was "types-hdbcli-2.17.0.0.tar", last modified: Fri Jun 16 03:15:44 2023, max compression
```

## Comparing `types-hdbcli-2.16.0.0.tar` & `types-hdbcli-2.17.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:01.004080 types-hdbcli-2.16.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-29 15:14:01.004080 types-hdbcli-2.16.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:01.004080 types-hdbcli-2.16.0.0/hdbcli-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/hdbcli-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 15:13:39.000000 types-hdbcli-2.16.0.0/hdbcli-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-29 15:13:39.000000 types-hdbcli-2.16.0.0/hdbcli-stubs/dbapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-29 15:13:39.000000 types-hdbcli-2.16.0.0/hdbcli-stubs/resultrow.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:14:01.004080 types-hdbcli-2.16.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:01.004080 types-hdbcli-2.16.0.0/types_hdbcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/types_hdbcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/types_hdbcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/types_hdbcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/types_hdbcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:15:44.744341 types-hdbcli-2.17.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-16 03:15:42.000000 types-hdbcli-2.17.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 03:15:42.000000 types-hdbcli-2.17.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-16 03:15:44.744341 types-hdbcli-2.17.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:15:44.744341 types-hdbcli-2.17.0.0/hdbcli-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 03:15:42.000000 types-hdbcli-2.17.0.0/hdbcli-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 03:15:31.000000 types-hdbcli-2.17.0.0/hdbcli-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-16 03:15:31.000000 types-hdbcli-2.17.0.0/hdbcli-stubs/dbapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-16 03:15:31.000000 types-hdbcli-2.17.0.0/hdbcli-stubs/resultrow.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 03:15:44.744341 types-hdbcli-2.17.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-16 03:15:42.000000 types-hdbcli-2.17.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:15:44.744341 types-hdbcli-2.17.0.0/types_hdbcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-16 03:15:44.000000 types-hdbcli-2.17.0.0/types_hdbcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-16 03:15:44.000000 types-hdbcli-2.17.0.0/types_hdbcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:15:44.000000 types-hdbcli-2.17.0.0/types_hdbcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 03:15:44.000000 types-hdbcli-2.17.0.0/types_hdbcli.egg-info/top_level.txt
```

### Comparing `types-hdbcli-2.16.0.0/CHANGELOG.md` & `types-hdbcli-2.17.0.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+## 2.17.0.0 (2023-06-16)
+
+[stubsabot] Bump hdbcli to 2.17.* (#10320)
+
+Release: https://pypi.org/pypi/hdbcli/2.17.14
+Homepage: https://www.sap.com/
+
+If stubtest fails for this PR:
+- Leave this PR open (as a reminder, and to prevent stubsabot from opening another PR)
+- Fix stubtest failures in another PR, then close this PR
+
+Note that you will need to close and re-open the PR in order to trigger CI
+
+Co-authored-by: stubsabot <>
+
 ## 2.16.0.0 (2023-04-29)
 
 Update `hdbcli` to `2.16` and mark as completed (#10101)
 
 ## 2.15.0.4 (2023-04-24)
 
 hdbcli: Fix wrong connection argument name (#10070)
```

### Comparing `types-hdbcli-2.16.0.0/PKG-INFO` & `types-hdbcli-2.17.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-hdbcli
-Version: 2.16.0.0
+Version: 2.17.0.0
 Summary: Typing stubs for hdbcli
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hdbcli.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `hdbcli`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hdbcli. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
+This package was generated from typeshed commit `7544b60db7b08249b1fef3663f0a68736660cae8` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
```

### Comparing `types-hdbcli-2.16.0.0/hdbcli-stubs/dbapi.pyi` & `types-hdbcli-2.17.0.0/hdbcli-stubs/dbapi.pyi`

 * *Files identical despite different names*

### Comparing `types-hdbcli-2.16.0.0/setup.py` & `types-hdbcli-2.17.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `hdbcli`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hdbcli. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
+This package was generated from typeshed commit `7544b60db7b08249b1fef3663f0a68736660cae8` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
 '''.lstrip()
 
 setup(name=name,
-      version="2.16.0.0",
+      version="2.17.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hdbcli.md",
```

### Comparing `types-hdbcli-2.16.0.0/types_hdbcli.egg-info/PKG-INFO` & `types-hdbcli-2.17.0.0/types_hdbcli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-hdbcli
-Version: 2.16.0.0
+Version: 2.17.0.0
 Summary: Typing stubs for hdbcli
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hdbcli.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `hdbcli`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hdbcli. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
+This package was generated from typeshed commit `7544b60db7b08249b1fef3663f0a68736660cae8` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
```

