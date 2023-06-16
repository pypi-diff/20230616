# Comparing `tmp/anodb-8.0.tar.gz` & `tmp/anodb-8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anodb-8.0.tar", last modified: Fri Jun 16 05:56:34 2023, max compression
+gzip compressed data, was "anodb-8.1.tar", last modified: Fri Jun 16 06:22:42 2023, max compression
```

## Comparing `anodb-8.0.tar` & `anodb-8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 05:56:34.371598 anodb-8.0/
--rw-------   0 fabien    (1001) fabien    (1001)       33 2023-05-14 12:33:50.000000 anodb-8.0/LICENSE
--rw-------   0 fabien    (1001) fabien    (1001)       49 2023-05-14 12:33:50.000000 anodb-8.0/MANIFEST.in
--rw-------   0 fabien    (1001) fabien    (1001)     1178 2023-06-16 05:51:21.000000 anodb-8.0/Makefile
--rw-------   0 fabien    (1001) fabien    (1001)     4703 2023-06-16 05:56:34.371598 anodb-8.0/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)     3753 2023-06-15 13:10:50.000000 anodb-8.0/README.md
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 05:56:34.371598 anodb-8.0/anodb.egg-info/
--rw-------   0 fabien    (1001) fabien    (1001)     4703 2023-06-16 05:56:34.000000 anodb-8.0/anodb.egg-info/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)      239 2023-06-16 05:56:34.000000 anodb-8.0/anodb.egg-info/SOURCES.txt
--rw-------   0 fabien    (1001) fabien    (1001)        1 2023-06-16 05:56:34.000000 anodb-8.0/anodb.egg-info/dependency_links.txt
--rw-------   0 fabien    (1001) fabien    (1001)      213 2023-06-16 05:56:34.000000 anodb-8.0/anodb.egg-info/requires.txt
--rw-------   0 fabien    (1001) fabien    (1001)        6 2023-06-16 05:56:34.000000 anodb-8.0/anodb.egg-info/top_level.txt
--rwx------   0 fabien    (1001) fabien    (1001)     8814 2023-06-16 05:53:35.000000 anodb-8.0/anodb.py
--rw-------   0 fabien    (1001) fabien    (1001)     1269 2023-06-15 09:39:26.000000 anodb-8.0/pyproject.toml
--rw-------   0 fabien    (1001) fabien    (1001)       38 2023-06-16 05:56:34.371598 anodb-8.0/setup.cfg
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 05:56:34.371598 anodb-8.0/test/
--rw-------   0 fabien    (1001) fabien    (1001)      399 2023-06-15 09:59:54.000000 anodb-8.0/test/Makefile
--rw-------   0 fabien    (1001) fabien    (1001)     8943 2023-06-15 09:43:43.000000 anodb-8.0/test/test_anodb.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 06:22:42.046711 anodb-8.1/
+-rw-------   0 fabien    (1001) fabien    (1001)       33 2023-05-14 12:33:50.000000 anodb-8.1/LICENSE
+-rw-------   0 fabien    (1001) fabien    (1001)       49 2023-05-14 12:33:50.000000 anodb-8.1/MANIFEST.in
+-rw-------   0 fabien    (1001) fabien    (1001)     1178 2023-06-16 05:51:21.000000 anodb-8.1/Makefile
+-rw-------   0 fabien    (1001) fabien    (1001)     4703 2023-06-16 06:22:42.046711 anodb-8.1/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)     3753 2023-06-15 13:10:50.000000 anodb-8.1/README.md
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 06:22:42.046711 anodb-8.1/anodb.egg-info/
+-rw-------   0 fabien    (1001) fabien    (1001)     4703 2023-06-16 06:22:42.000000 anodb-8.1/anodb.egg-info/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)      239 2023-06-16 06:22:42.000000 anodb-8.1/anodb.egg-info/SOURCES.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        1 2023-06-16 06:22:42.000000 anodb-8.1/anodb.egg-info/dependency_links.txt
+-rw-------   0 fabien    (1001) fabien    (1001)      213 2023-06-16 06:22:42.000000 anodb-8.1/anodb.egg-info/requires.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        6 2023-06-16 06:22:42.000000 anodb-8.1/anodb.egg-info/top_level.txt
+-rwx------   0 fabien    (1001) fabien    (1001)     8820 2023-06-16 06:02:12.000000 anodb-8.1/anodb.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1269 2023-06-16 06:21:14.000000 anodb-8.1/pyproject.toml
+-rw-------   0 fabien    (1001) fabien    (1001)       38 2023-06-16 06:22:42.046711 anodb-8.1/setup.cfg
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 06:22:42.046711 anodb-8.1/test/
+-rw-------   0 fabien    (1001) fabien    (1001)      399 2023-06-15 09:59:54.000000 anodb-8.1/test/Makefile
+-rw-------   0 fabien    (1001) fabien    (1001)     8943 2023-06-15 09:43:43.000000 anodb-8.1/test/test_anodb.py
```

### Comparing `anodb-8.0/Makefile` & `anodb-8.1/Makefile`

 * *Files identical despite different names*

### Comparing `anodb-8.0/PKG-INFO` & `anodb-8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anodb
-Version: 8.0
+Version: 8.1
 Summary: Convenient Wrapper around AioSQL and a Database Connection
 Author-email: Fabien Coelho <ano.db@coelho.net>
 License: CC0
 Project-URL: repository, https://github.com/zx80/anodb
 Project-URL: documentation, https://zx80.github.io/anodb/
 Project-URL: issues, https://github.com/zx80/anodb/issues
 Project-URL: package, https://pypi.org/project/anodb/
```

### Comparing `anodb-8.0/README.md` & `anodb-8.1/README.md`

 * *Files identical despite different names*

### Comparing `anodb-8.0/anodb.egg-info/PKG-INFO` & `anodb-8.1/anodb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anodb
-Version: 8.0
+Version: 8.1
 Summary: Convenient Wrapper around AioSQL and a Database Connection
 Author-email: Fabien Coelho <ano.db@coelho.net>
 License: CC0
 Project-URL: repository, https://github.com/zx80/anodb
 Project-URL: documentation, https://zx80.github.io/anodb/
 Project-URL: issues, https://github.com/zx80/anodb/issues
 Project-URL: package, https://pypi.org/project/anodb/
```

### Comparing `anodb-8.0/anodb.py` & `anodb-8.1/anodb.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             module = "mysqlclient"
         elif self._db in ("mysql-connector", "mysql.connector"):  # pragma: no cover
             import mysql.connector as db  # type: ignore
 
             module = "mysql.connector"
         elif self._db == "mariadb":  # pragma: no cover
             import mariadb as db  # type: ignore
-        elif self._db == "":  # pragma: no cover
+        elif self._db == "duckdb":  # pragma: no cover
             import duckdb as db  # type: ignore
         else:  # pragma: no cover
             raise Exception(f"unexpected db {self._db}")
         # get version if needed
         if not hasattr(self, "_db_version"):
             if hasattr(db, "__version__"):
                 self._db_version = db.__version__
```

### Comparing `anodb-8.0/pyproject.toml` & `anodb-8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anodb"
-version = "8.0"
+version = "8.1"
 authors = [ { name = "Fabien Coelho", email = "ano.db@coelho.net" } ]
 description = "Convenient Wrapper around AioSQL and a Database Connection"
 readme = "README.md"
 license = { text = "CC0" }
 requires-python = ">= 3.8"
 dependencies = [ "aiosql >= 8.0" ]
 classifiers = [
```

### Comparing `anodb-8.0/test/test_anodb.py` & `anodb-8.1/test/test_anodb.py`

 * *Files identical despite different names*

