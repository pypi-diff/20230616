# Comparing `tmp/anodb-7.3.tar.gz` & `tmp/anodb-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anodb-7.3.tar", last modified: Sat Jan 21 06:42:56 2023, max compression
+gzip compressed data, was "anodb-8.0.tar", last modified: Fri Jun 16 05:56:34 2023, max compression
```

## Comparing `anodb-7.3.tar` & `anodb-8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-01-21 06:42:56.931873 anodb-7.3/
--rw-------   0 fabien    (1001) fabien    (1001)       33 2020-07-27 14:33:41.000000 anodb-7.3/LICENSE
--rw-------   0 fabien    (1001) fabien    (1001)       49 2021-04-20 05:46:05.000000 anodb-7.3/MANIFEST.in
--rw-------   0 fabien    (1001) fabien    (1001)     1330 2022-09-11 17:31:38.000000 anodb-7.3/Makefile
--rw-------   0 fabien    (1001) fabien    (1001)     4438 2023-01-21 06:42:56.931873 anodb-7.3/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)     3752 2023-01-21 06:40:37.000000 anodb-7.3/README.md
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-01-21 06:42:56.931873 anodb-7.3/anodb.egg-info/
--rw-------   0 fabien    (1001) fabien    (1001)     4438 2023-01-21 06:42:56.000000 anodb-7.3/anodb.egg-info/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)      243 2023-01-21 06:42:56.000000 anodb-7.3/anodb.egg-info/SOURCES.txt
--rw-------   0 fabien    (1001) fabien    (1001)        1 2023-01-21 06:42:56.000000 anodb-7.3/anodb.egg-info/dependency_links.txt
--rw-------   0 fabien    (1001) fabien    (1001)       12 2023-01-21 06:42:56.000000 anodb-7.3/anodb.egg-info/requires.txt
--rw-------   0 fabien    (1001) fabien    (1001)        6 2023-01-21 06:42:56.000000 anodb-7.3/anodb.egg-info/top_level.txt
--rwx------   0 fabien    (1001) fabien    (1001)     8716 2023-01-21 06:05:54.000000 anodb-7.3/anodb.py
--rw-------   0 fabien    (1001) fabien    (1001)      702 2023-01-21 06:42:56.931873 anodb-7.3/setup.cfg
--rw-------   0 fabien    (1001) fabien    (1001)       89 2021-04-20 05:39:24.000000 anodb-7.3/setup.py
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-01-21 06:42:56.931873 anodb-7.3/test/
--rw-------   0 fabien    (1001) fabien    (1001)      393 2022-08-08 06:23:26.000000 anodb-7.3/test/Makefile
--rw-------   0 fabien    (1001) fabien    (1001)     8527 2022-09-11 17:23:58.000000 anodb-7.3/test/test_anodb.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 05:56:34.371598 anodb-8.0/
+-rw-------   0 fabien    (1001) fabien    (1001)       33 2023-05-14 12:33:50.000000 anodb-8.0/LICENSE
+-rw-------   0 fabien    (1001) fabien    (1001)       49 2023-05-14 12:33:50.000000 anodb-8.0/MANIFEST.in
+-rw-------   0 fabien    (1001) fabien    (1001)     1178 2023-06-16 05:51:21.000000 anodb-8.0/Makefile
+-rw-------   0 fabien    (1001) fabien    (1001)     4703 2023-06-16 05:56:34.371598 anodb-8.0/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)     3753 2023-06-15 13:10:50.000000 anodb-8.0/README.md
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 05:56:34.371598 anodb-8.0/anodb.egg-info/
+-rw-------   0 fabien    (1001) fabien    (1001)     4703 2023-06-16 05:56:34.000000 anodb-8.0/anodb.egg-info/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)      239 2023-06-16 05:56:34.000000 anodb-8.0/anodb.egg-info/SOURCES.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        1 2023-06-16 05:56:34.000000 anodb-8.0/anodb.egg-info/dependency_links.txt
+-rw-------   0 fabien    (1001) fabien    (1001)      213 2023-06-16 05:56:34.000000 anodb-8.0/anodb.egg-info/requires.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        6 2023-06-16 05:56:34.000000 anodb-8.0/anodb.egg-info/top_level.txt
+-rwx------   0 fabien    (1001) fabien    (1001)     8814 2023-06-16 05:53:35.000000 anodb-8.0/anodb.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1269 2023-06-15 09:39:26.000000 anodb-8.0/pyproject.toml
+-rw-------   0 fabien    (1001) fabien    (1001)       38 2023-06-16 05:56:34.371598 anodb-8.0/setup.cfg
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 05:56:34.371598 anodb-8.0/test/
+-rw-------   0 fabien    (1001) fabien    (1001)      399 2023-06-15 09:59:54.000000 anodb-8.0/test/Makefile
+-rw-------   0 fabien    (1001) fabien    (1001)     8943 2023-06-15 09:43:43.000000 anodb-8.0/test/test_anodb.py
```

### Comparing `anodb-7.3/Makefile` & `anodb-8.0/Makefile`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 SHELL	= /bin/bash
 .ONESHELL:
 
 MODULE	= anodb
 PYTHON	= python
-PIP		= venv/bin/pip
+PIP		= pip
 
 .PHONY: check check.mypy check.flake8 check.black check.pytest check.coverage check.pymarkdown
-check: check.mypy check.flake8 check.black check.pytest check.coverage check.pymarkdown
+check: check.mypy check.flake8 check.pytest check.coverage check.pymarkdown
 
-check.mypy: $(MODULE).egg-info
+check.mypy: venv
 	source venv/bin/activate
 	mypy $(MODULE).py
 
-check.flake8:
+check.flake8: venv
 	source venv/bin/activate
-	flake8 --ignore=E127,E402,E501,W503 $(MODULE).py
+	flake8 --ignore=E127,E227,E402,E501,W503 $(MODULE).py
 
-check.black:
+check.black: venv
 	source venv/bin/activate
 	black --check $(MODULE).py test/test_anodb.py
 
-check.pytest: $(MODULE).egg-info
+check.pytest: venv
 	source venv/bin/activate
 	$(MAKE) -C test check
 
-check.coverage: $(MODULE).egg-info
+check.coverage: venv
 	source venv/bin/activate
 	$(MAKE) -C test coverage
 
-check.pymarkdown:
+check.pymarkdown: venv
 	source venv/bin/activate
 	pymarkdown scan *.md
 
 .PHONY: clean clean.venv
 clean:
-	$(RM) -r __pycache__ */__pycache__ *.egg-info dist build .mypy_cache .pytest_cache
+	$(RM) -r __pycache__ */__pycache__ dist build .mypy_cache .pytest_cache
 	$(MAKE) -C test clean
 
 clean.venv: clean
-	$(RM) -r venv
+	$(RM) -r venv *.egg-info
 
 # venv
-$(MODULE).egg-info: venv
-	$(PIP) install -e .
-
 venv:
 	$(PYTHON) -m venv venv
+	source venv/bin/activate
 	$(PIP) install -U pip
-
-.PHONY: venv.dev
-venv.dev: $(MODULE).egg-info
-	$(PIP) install -r dev-requirements.txt
-
-venv.dev: $(MODULE).egg-info
+	$(PIP) install -e .[dev,pub,postgres]
 
 # distribution
-dist:
-	$(PYTHON) setup.py sdist bdist_wheel
+dist: venv
+	source venv/bin/activate
+	$(PYTHON) -m build
 
 .PHONY: publish
 publish: dist
 	# provide pypi ids in ~/.pypirc
-	echo twine upload --repository $(MODULE) dist/*
+	echo twine upload dist/*
```

### Comparing `anodb-7.3/PKG-INFO` & `anodb-8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 Metadata-Version: 2.1
 Name: anodb
-Version: 7.3
+Version: 8.0
 Summary: Convenient Wrapper around AioSQL and a Database Connection
-Home-page: https://github.com/zx80/anodb
-Author: Fabien Coelho
-Author-email: ano.db@coelho.net
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: Fabien Coelho <ano.db@coelho.net>
+License: CC0
+Project-URL: repository, https://github.com/zx80/anodb
+Project-URL: documentation, https://zx80.github.io/anodb/
+Project-URL: issues, https://github.com/zx80/anodb/issues
+Project-URL: package, https://pypi.org/project/anodb/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: pub
+Provides-Extra: postgres
+Provides-Extra: mysql
 License-File: LICENSE
 
 # AnoDB
 
 Convenient Wrapper around [aiosql](https://github.com/nackjicholson/aiosql)
 and a [Database Connection](https://www.python.org/dev/peps/pep-0249).
 
 ![Status](https://github.com/zx80/anodb/actions/workflows/anodb-package.yml/badge.svg?branch=master&style=flat)
 ![Tests](https://img.shields.io/badge/tests-11%20✓-success)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-success)
 ![Python](https://img.shields.io/badge/python-3-informational)
-![Databases](https://img.shields.io/badge/databases-4-informational)
-![Drivers](https://img.shields.io/badge/drivers-9-informational)
+![Databases](https://img.shields.io/badge/databases-5-informational)
+![Drivers](https://img.shields.io/badge/drivers-10-informational)
 ![Version](https://img.shields.io/pypi/v/anodb)
 ![Badges](https://img.shields.io/badge/badges-9-informational)
 ![License](https://img.shields.io/pypi/l/anodb?style=flat)
 
 ## Description
 
 This class creates a persistent database connection and imports
@@ -117,9 +123,7 @@
 [documentation](https://zx80.github.io/anodb/) and
 [issues](https://github.com/zx80/anodb/issues)
 are available on [GitHub](https://github.com/).
 
 Latest version is *7.3* on 2023-01-21.
 
 See [all versions](VERSIONS.md)
-
-
```

### Comparing `anodb-7.3/README.md` & `anodb-8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 Convenient Wrapper around [aiosql](https://github.com/nackjicholson/aiosql)
 and a [Database Connection](https://www.python.org/dev/peps/pep-0249).
 
 ![Status](https://github.com/zx80/anodb/actions/workflows/anodb-package.yml/badge.svg?branch=master&style=flat)
 ![Tests](https://img.shields.io/badge/tests-11%20✓-success)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-success)
 ![Python](https://img.shields.io/badge/python-3-informational)
-![Databases](https://img.shields.io/badge/databases-4-informational)
-![Drivers](https://img.shields.io/badge/drivers-9-informational)
+![Databases](https://img.shields.io/badge/databases-5-informational)
+![Drivers](https://img.shields.io/badge/drivers-10-informational)
 ![Version](https://img.shields.io/pypi/v/anodb)
 ![Badges](https://img.shields.io/badge/badges-9-informational)
 ![License](https://img.shields.io/pypi/l/anodb?style=flat)
 
 ## Description
 
 This class creates a persistent database connection and imports
```

### Comparing `anodb-7.3/anodb.egg-info/PKG-INFO` & `anodb-8.0/anodb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 Metadata-Version: 2.1
 Name: anodb
-Version: 7.3
+Version: 8.0
 Summary: Convenient Wrapper around AioSQL and a Database Connection
-Home-page: https://github.com/zx80/anodb
-Author: Fabien Coelho
-Author-email: ano.db@coelho.net
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: Fabien Coelho <ano.db@coelho.net>
+License: CC0
+Project-URL: repository, https://github.com/zx80/anodb
+Project-URL: documentation, https://zx80.github.io/anodb/
+Project-URL: issues, https://github.com/zx80/anodb/issues
+Project-URL: package, https://pypi.org/project/anodb/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: pub
+Provides-Extra: postgres
+Provides-Extra: mysql
 License-File: LICENSE
 
 # AnoDB
 
 Convenient Wrapper around [aiosql](https://github.com/nackjicholson/aiosql)
 and a [Database Connection](https://www.python.org/dev/peps/pep-0249).
 
 ![Status](https://github.com/zx80/anodb/actions/workflows/anodb-package.yml/badge.svg?branch=master&style=flat)
 ![Tests](https://img.shields.io/badge/tests-11%20✓-success)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-success)
 ![Python](https://img.shields.io/badge/python-3-informational)
-![Databases](https://img.shields.io/badge/databases-4-informational)
-![Drivers](https://img.shields.io/badge/drivers-9-informational)
+![Databases](https://img.shields.io/badge/databases-5-informational)
+![Drivers](https://img.shields.io/badge/drivers-10-informational)
 ![Version](https://img.shields.io/pypi/v/anodb)
 ![Badges](https://img.shields.io/badge/badges-9-informational)
 ![License](https://img.shields.io/pypi/l/anodb?style=flat)
 
 ## Description
 
 This class creates a persistent database connection and imports
@@ -117,9 +123,7 @@
 [documentation](https://zx80.github.io/anodb/) and
 [issues](https://github.com/zx80/anodb/issues)
 are available on [GitHub](https://github.com/).
 
 Latest version is *7.3* on 2023-01-21.
 
 See [all versions](VERSIONS.md)
-
-
```

### Comparing `anodb-7.3/anodb.py` & `anodb-8.0/anodb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #
 # This marvelous code is Public Domain.
 #
 
-from typing import Any, Dict, Set, List, Union, Optional
+from typing import Any
 import logging
 import functools as ft
 import aiosql as sql  # type: ignore
 
 log = logging.getLogger("anodb")
 
 # get package version
-import pkg_resources as pkg  # type: ignore
-
-__version__ = pkg.require("anodb")[0].version
+from importlib.metadata import version as pkg_version
+__version__ = pkg_version("anodb")
 
 
 #
 # DB (Database) class
 #
 class DB:
     """Hides database connection and queries in here.
@@ -29,17 +28,17 @@
     SQLITE = ("sqlite3", "sqlite")
     POSTGRES = ("psycopg", "pg", "postgres", "postgresql", "psycopg3")
     # others stay as-is: psycopg2 pg8000…
 
     def __init__(
         self,
         db: str,
-        conn: Optional[str],
-        queries: Union[str, List[str]] = [],
-        options: Union[str, Dict[str, Any]] = {},
+        conn: str|None,
+        queries: str|list[str] = [],
+        options: str|dict[str, Any] = {},
         auto_reconnect: bool = True,
         debug: bool = False,
         **conn_options,
     ):
         """DB constructor
 
         - db: database engine/driver)
@@ -47,25 +46,25 @@
         - queries: file(s) holding queries for `aiosql`, may be empty
         - options: database-specific options in various forms
         - auto_reconnect: whether to reconnect on connection errors
         - debug: debug mode generate more logs through `logging`
         - conn_options: database-specific `kwargs` constructor options
         """
         self.__version__ = __version__
-        self.__aiosql_version__ = pkg.require("aiosql")[0].version
+        self.__aiosql_version__ = pkg_version("aiosql")
         log.info(f"creating DB for {db}")
         # this is the class name
         self._db = (
             "sqlite3" if db in self.SQLITE else "psycopg" if db in self.POSTGRES else db
         ).lower()
         assert self._db in sql.aiosql._ADAPTERS, f"database {db} is supported"
         # connection…
         self._conn = None
         self._conn_str = conn
-        self._conn_options: Dict[str, Any] = {}
+        self._conn_options: dict[str, Any] = {}
         if isinstance(options, str):
             import ast
 
             self._conn_options.update(ast.literal_eval(options))
         elif isinstance(options, dict):
             self._conn_options.update(options)
         else:
@@ -73,17 +72,17 @@
         self._conn_options.update(conn_options)
         # various boolean flags
         self._debug = debug
         self._auto_reconnect = auto_reconnect
         self._reconn = False
         # queries… keep track of calls
         self._queries_file = [queries] if isinstance(queries, str) else queries
-        self._queries: List[sql.aiosql.Queries] = []
-        self._count: Dict[str, int] = {}
-        self._available_queries: Set[str] = set()
+        self._queries: list[sql.aiosql.Queries] = []
+        self._count: dict[str, int] = {}
+        self._available_queries: set[str] = set()
         for fn in self._queries_file:
             self.add_queries_from_path(fn)
         # last thing is to actually create the connection, which may fail
         self._conn = self._connect()
 
     def _call_fn(self, query, fn, *args, **kwargs):
         """Forward method call to aiosql query
@@ -169,34 +168,36 @@
             import psycopg2 as db  # type: ignore
         elif self._db == "pg8000":
             import pg8000 as db  # type: ignore
         elif self._db == "pygresql":
             import pgdb as db  # type: ignore
 
             module = "pgdb"
-        elif self._db == "pymysql":
+        elif self._db == "pymysql":  # pragma: no cover
             import pymysql as db  # type: ignore
-        elif self._db in ("MySQLdb", "mysqldb"):
+        elif self._db in ("MySQLdb", "mysqldb"):  # pragma: no cover
             import MySQLdb as db  # type: ignore
 
             module = "mysqlclient"
-        elif self._db in ("mysql-connector", "mysql.connector"):
+        elif self._db in ("mysql-connector", "mysql.connector"):  # pragma: no cover
             import mysql.connector as db  # type: ignore
 
             module = "mysql.connector"
         elif self._db == "mariadb":  # pragma: no cover
             import mariadb as db  # type: ignore
+        elif self._db == "":  # pragma: no cover
+            import duckdb as db  # type: ignore
         else:  # pragma: no cover
             raise Exception(f"unexpected db {self._db}")
         # get version if needed
         if not hasattr(self, "_db_version"):
             if hasattr(db, "__version__"):
                 self._db_version = db.__version__
-            else:
-                self._db_version = pkg.require(module)[0].version
+            else:  # pragma: no cover
+                self._db_version = pkg_version(module)
         # do connect
         return (
             db.connect(self._conn_str, **self._conn_options)
             if self._conn_str
             else db.connect(**self._conn_options)
         )
```

### Comparing `anodb-7.3/test/test_anodb.py` & `anodb-8.0/test/test_anodb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import pytest  # type: ignore
 import anodb
 import re
 from os import environ as ENV
 import logging
 from pathlib import Path
+import shutil
 
 log = logging.getLogger(__name__)
 
 for f in ["test.sql", "test/test.sql"]:
     if Path(f).exists():
         TEST_SQL = f
 assert TEST_SQL
 
+
 # check that the db connection cursor works
 def run_42(db: anodb.DB):
     assert db is not None
     cur = db.cursor()
     cur.execute("SELECT 42 AS fourtytwo")
     assert cur.description[0][0] == "fourtytwo"
     assert cur.fetchone()[0] == 42
@@ -25,38 +27,38 @@
 
 # do various stuff, common to sqlite & pg tests
 def run_stuff(db: anodb.DB):
     assert db is not None
     # create table Foo
     db.create_foo()
     # with some data
-    assert db.count_foo()[0] == 0
+    assert list(db.count_foo())[0] == 0
     db.insert_foo(pk=1, val="one")
-    assert db.count_foo()[0] == 1
+    assert list(db.count_foo())[0] == 1
     db.insert_foo(pk=2, val="two")
     db.commit()
     # more checks
-    assert db.count_foo()[0] == 2
-    assert re.search(r"two", db.select_foo_pk(pk=2)[0][0])
+    assert list(db.count_foo())[0] == 2
+    assert re.search(r"two", list(db.select_foo_pk(pk=2))[0][0])
     db.update_foo_pk(pk=2, val="deux")
     db.delete_foo_pk(pk=1)
     db.commit()
-    assert db.count_foo()[0] == 1
-    assert re.search(r"deux", db.select_foo_pk(pk=2)[0][0])
+    assert list(db.count_foo())[0] == 1
+    assert re.search(r"deux", list(db.select_foo_pk(pk=2))[0][0])
     # data cleanup
     db.delete_foo_all()
     db.commit()
-    assert db.count_foo()[0] == 0
+    assert list(db.count_foo())[0] == 0
     # check rollback
     db.insert_foo(pk=3, val="three")
     db.insert_foo(pk=4, val="four")
     db.insert_foo(pk=5, val="five")
-    assert db.count_foo()[0] == 3
+    assert list(db.count_foo())[0] == 3
     db.rollback()
-    assert db.count_foo()[0] == 0
+    assert list(db.count_foo())[0] == 0
     # table cleanup
     db.drop_foo()
     db.commit()
     # check reconnection
     db.close()
     db.connect()
     run_42(db)
@@ -164,14 +166,18 @@
     try:
         __import__(name)
         return True
     except ModuleNotFoundError:
         return False
 
 
+def has_command(cmd):
+    return shutil.which(cmd) is not None
+
+
 @pytest.mark.skipif(
     not has_module("pytest_postgresql"), reason="missing pytest_postgresql for test"
 )
 @pytest.mark.skipif(not has_module("psycopg"), reason="missing psycopg for test")
 def test_psycopg(pg_dsn):
     run_postgres("psycopg", pg_dsn)
 
@@ -221,35 +227,38 @@
 @pytest.fixture
 def my_dsn(mysql_proc):
     p = mysql_proc
     log.debug(f"unix socket={p.unixsocket} port={p.port}")
     yield {"user": p.user, "host": p.host, "port": p.port, "password": ""}
 
 
+@pytest.mark.skipif(not has_command("mysqld"), reason="missing mysqd for test")
 @pytest.mark.skipif(
     not has_module("pytest_mysql"), reason="missing pytest_mysql for test"
 )
 @pytest.mark.skipif(not has_module("MySQLdb"), reason="missing MySQLdb for test")
 def test_mysqldb(my_dsn, mysql, mysql_proc):
     my_dsn["database"] = "test"
     if mysql_proc.unixsocket:
         my_dsn["unix_socket"] = mysql_proc.unixsocket
         del my_dsn["port"]
     db = run_test_sql("MySQLdb", my_dsn)
 
 
+@pytest.mark.skipif(not has_command("mysqld"), reason="missing mysqd for test")
 @pytest.mark.skipif(
     not has_module("pytest_mysql"), reason="missing pytest_mysql for test"
 )
 @pytest.mark.skipif(not has_module("pymysql"), reason="missing pymysql for test")
 def test_pymysql(my_dsn, mysql):
     my_dsn["database"] = "test"
     db = run_test_sql("pymysql", my_dsn)
 
 
+@pytest.mark.skipif(not has_command("mysqld"), reason="missing mysqd for test")
 @pytest.mark.skipif(
     not has_module("pytest_mysql"), reason="missing pytest_mysql for test"
 )
 @pytest.mark.skipif(
     not has_module("mysql.connector"), reason="missing mysql.connector for test"
 )
 def test_myco(my_dsn, mysql):
@@ -258,25 +267,25 @@
 
 
 # test from-string queries
 def test_from_str():
     db = anodb.DB("sqlite", ":memory:")
     assert "connection to sqlite" in str(db)
     db.add_queries_from_str("-- name: next\nSELECT :arg + 1 AS next;\n")
-    assert db.next(arg=1)[0][0] == 2
+    assert list(db.next(arg=1))[0][0] == 2
     db.add_queries_from_str("-- name: prev\nSELECT :arg - 1 AS prev;\n")
-    assert db.next(arg=41)[0][0] == 42
-    assert db.prev(arg=42)[0][0] == 41
+    assert list(db.next(arg=41))[0][0] == 42
+    assert list(db.prev(arg=42))[0][0] == 41
     # override previous definition
     db.add_queries_from_str("-- name: foo\nSELECT :arg + 42 AS foo;\n")
-    assert db.foo(arg=0)[0][0] == 42
+    assert list(db.foo(arg=0))[0][0] == 42
     db.add_queries_from_str("-- name: foo\nSELECT :arg - 42 AS foo;\n")
-    assert db.foo(arg=42)[0][0] == 0
-    assert db.next(arg=42)[0][0] == 43
-    assert db.prev(arg=43)[0][0] == 42
+    assert list(db.foo(arg=42))[0][0] == 0
+    assert list(db.next(arg=42))[0][0] == 43
+    assert list(db.prev(arg=43))[0][0] == 42
     assert sorted(db._available_queries) == [
         "foo",
         "foo_cursor",
         "next",
         "next_cursor",
         "prev",
         "prev_cursor",
```

