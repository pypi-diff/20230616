# Comparing `tmp/sqlite3_to_mysql-2.0.0.tar.gz` & `tmp/sqlite3_to_mysql-2.0.1.tar.gz`

## Comparing `sqlite3_to_mysql-2.0.0.tar` & `sqlite3_to_mysql-2.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/requirements_dev.txt
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/__init__.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/cli.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/click_utils.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/debug_info.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/mysql_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/py.typed
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/sqlite_utils.py
--rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/transporter.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0    11208 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/database.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/factories.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/func/__init__.py
--rw-r--r--   0        0        0    24132 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/func/sqlite3_to_mysql_test.py
--rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/func/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/unit/__init__.py
--rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/tests/unit/sqlite3_to_mysql_test.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/LICENSE
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/README.md
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/requirements_dev.txt
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/__init__.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/cli.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/click_utils.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/debug_info.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/mysql_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/py.typed
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/sqlite_utils.py
+-rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/transporter.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/__init__.py
+-rw-r--r--   0        0        0    11192 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/database.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/factories.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/func/__init__.py
+-rw-r--r--   0        0        0    24132 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/func/sqlite3_to_mysql_test.py
+-rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/func/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/unit/sqlite3_to_mysql_test.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/LICENSE
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/README.md
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/PKG-INFO
```

### Comparing `sqlite3_to_mysql-2.0.0/CODE-OF-CONDUCT.md` & `sqlite3_to_mysql-2.0.1/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/cli.py` & `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/cli.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/click_utils.py` & `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/click_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/debug_info.py` & `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/debug_info.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/mysql_utils.py` & `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/mysql_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/sqlite_utils.py` & `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/transporter.py` & `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/transporter.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/sqlite3_to_mysql/types.py` & `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/types.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/tests/conftest.py` & `sqlite3_to_mysql-2.0.1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 from requests import HTTPError
 from sqlalchemy import create_engine
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.orm import Session
 from sqlalchemy_utils import database_exists, drop_database
 
-from .database import Database
-from .factories import ArticleFactory, AuthorFactory, ImageFactory, MediaFactory, MiscFactory, TagFactory
+from . import database, factories
 
 
 def pytest_addoption(parser: "Parser") -> None:
     parser.addoption(
         "--sqlite-file",
         dest="sqlite_file",
         default=None,
@@ -124,15 +123,15 @@
         try:
             yield
         except exception:
             raise pytest.fail(f"DID RAISE {exception}")
 
     @staticmethod
     @contextmanager
-    def session_scope(db: Database) -> t.Generator:
+    def session_scope(db: database.Database) -> t.Generator:
         """Provide a transactional scope around a series of operations."""
         session: Session = db.Session()
         try:
             yield session
             session.commit()
         except Exception:
             session.rollback()
@@ -153,26 +152,26 @@
         if not isfile(realpath(db_file)):
             pytest.fail(f"{db_file} does not exist")
         return str(realpath(db_file))
 
     temp_data_dir: LocalPath = tmpdir_factory.mktemp("data")
     temp_image_dir: LocalPath = tmpdir_factory.mktemp("images")
     db_file = temp_data_dir.join(Path("db.sqlite3"))
-    db: Database = Database(f"sqlite:///{db_file}")
+    db: database.Database = database.Database(f"sqlite:///{db_file}")
 
     with Helpers.session_scope(db) as session:
         for _ in range(_session_faker.pyint(min_value=12, max_value=24)):
-            article = ArticleFactory()
-            article.authors.append(AuthorFactory())
-            article.tags.append(TagFactory())
-            article.misc.append(MiscFactory())
-            article.media.append(MediaFactory())
+            article = factories.ArticleFactory()
+            article.authors.append(factories.AuthorFactory())
+            article.tags.append(factories.TagFactory())
+            article.misc.append(factories.MiscFactory())
+            article.media.append(factories.MediaFactory())
             for _ in range(_session_faker.pyint(min_value=1, max_value=4)):
                 article.images.append(
-                    ImageFactory(
+                    factories.ImageFactory(
                         path=join(
                             str(temp_image_dir),
                             _session_faker.year(),
                             _session_faker.month(),
                             _session_faker.day_of_month(),
                             _session_faker.file_name(extension="jpg"),
                         )
```

### Comparing `sqlite3_to_mysql-2.0.0/tests/database.py` & `sqlite3_to_mysql-2.0.1/tests/database.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/tests/models.py` & `sqlite3_to_mysql-2.0.1/tests/models.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/tests/func/sqlite3_to_mysql_test.py` & `sqlite3_to_mysql-2.0.1/tests/func/sqlite3_to_mysql_test.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/tests/func/test_cli.py` & `sqlite3_to_mysql-2.0.1/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/tests/unit/sqlite3_to_mysql_test.py` & `sqlite3_to_mysql-2.0.1/tests/unit/sqlite3_to_mysql_test.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/.gitignore` & `sqlite3_to_mysql-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/LICENSE` & `sqlite3_to_mysql-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/README.md` & `sqlite3_to_mysql-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/pyproject.toml` & `sqlite3_to_mysql-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.0/PKG-INFO` & `sqlite3_to_mysql-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite3-to-mysql
-Version: 2.0.0
+Version: 2.0.1
 Summary: A simple Python tool to transfer data from SQLite 3 to MySQL
 Project-URL: Source, https://github.com/techouse/sqlite3-to-mysql
 Author-email: Klemen Tusar <techouse@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: data,migrate,migration,mysql,sqlite3,transfer
 Classifier: Development Status :: 5 - Production/Stable
```

