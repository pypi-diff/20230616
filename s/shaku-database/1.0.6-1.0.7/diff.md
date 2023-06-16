# Comparing `tmp/shaku-database-1.0.6.tar.gz` & `tmp/shaku-database-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku-database-1.0.6.tar", last modified: Thu Jun 15 09:50:50 2023, max compression
+gzip compressed data, was "shaku-database-1.0.7.tar", last modified: Fri Jun 16 06:22:37 2023, max compression
```

## Comparing `shaku-database-1.0.6.tar` & `shaku-database-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:50:50.491097 shaku-database-1.0.6/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.0.6/LICENSE
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7160 2023-06-15 09:50:50.490950 shaku-database-1.0.6/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.0.6/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:50:50.488894 shaku-database-1.0.6/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.6/database/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:50:50.489122 shaku-database-1.0.6/database/bigquery/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.6/database/bigquery/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-15 08:42:39.000000 shaku-database-1.0.6/database/bigquery/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:50:50.489383 shaku-database-1.0.6/database/cloud_sql/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.6/database/cloud_sql/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)      689 2023-06-08 02:35:46.000000 shaku-database-1.0.6/database/cloud_sql/crud.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:50:50.489658 shaku-database-1.0.6/database/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.6/database/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-06-08 02:35:46.000000 shaku-database-1.0.6/database/cloud_storage/util.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-06-15 09:50:50.491140 shaku-database-1.0.6/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1056 2023-06-15 09:50:44.000000 shaku-database-1.0.6/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:50:50.490732 shaku-database-1.0.6/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7160 2023-06-15 09:50:50.000000 shaku-database-1.0.6/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      416 2023-06-15 09:50:50.000000 shaku-database-1.0.6/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-06-15 09:50:50.000000 shaku-database-1.0.6/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)      417 2023-06-15 09:50:50.000000 shaku-database-1.0.6/shaku_database.egg-info/requires.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        9 2023-06-15 09:50:50.000000 shaku-database-1.0.6/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-16 06:22:37.179284 shaku-database-1.0.7/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.0.7/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7160 2023-06-16 06:22:37.179149 shaku-database-1.0.7/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.0.7/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-16 06:22:37.177171 shaku-database-1.0.7/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.7/database/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-16 06:22:37.177404 shaku-database-1.0.7/database/bigquery/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.7/database/bigquery/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-15 08:42:39.000000 shaku-database-1.0.7/database/bigquery/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-16 06:22:37.177824 shaku-database-1.0.7/database/cloud_sql/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.7/database/cloud_sql/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1131 2023-06-16 06:21:20.000000 shaku-database-1.0.7/database/cloud_sql/crud.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-16 06:22:37.178087 shaku-database-1.0.7/database/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.7/database/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-06-08 02:35:46.000000 shaku-database-1.0.7/database/cloud_storage/util.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-06-16 06:22:37.179324 shaku-database-1.0.7/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1056 2023-06-16 06:21:48.000000 shaku-database-1.0.7/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-16 06:22:37.178954 shaku-database-1.0.7/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7160 2023-06-16 06:22:37.000000 shaku-database-1.0.7/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      416 2023-06-16 06:22:37.000000 shaku-database-1.0.7/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-06-16 06:22:37.000000 shaku-database-1.0.7/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      417 2023-06-16 06:22:37.000000 shaku-database-1.0.7/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        9 2023-06-16 06:22:37.000000 shaku-database-1.0.7/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku-database-1.0.6/LICENSE` & `shaku-database-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shaku-database-1.0.6/PKG-INFO` & `shaku-database-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.0.6
+Version: 1.0.7
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.0.6/README.md` & `shaku-database-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `shaku-database-1.0.6/database/bigquery/util.py` & `shaku-database-1.0.7/database/bigquery/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.0.6/database/cloud_sql/crud.py` & `shaku-database-1.0.7/database/cloud_sql/crud.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,7 +19,21 @@
     with engine.connect() as conn:
         try:
             conn.execute(s, sql_data)
             conn.commit()
         except Exception as e:
             print(e)
             conn.rollback()
+
+
+def batch_insert_data(sql_list, data_list, connection_string):
+    try:
+        engine = create_engine(connection_string)
+        with engine.connect() as conn:
+            for sql, data in zip(sql_list, data_list):
+                sql_data = data.to_dict(orient='records')
+                s = text(sql)
+                conn.execute(s, sql_data)
+            conn.commit()
+    except Exception as e:
+        print(e)
+        conn.rollback()
```

### Comparing `shaku-database-1.0.6/database/cloud_storage/util.py` & `shaku-database-1.0.7/database/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.0.6/setup.py` & `shaku-database-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = f.read()
 HERE = pathlib.Path(__file__).parent.resolve()
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 INSTALL_REQUIRES = {s.strip().split('==')[0]: s.strip().split('==')[1] if len(s.strip().split('==')) > 1 else "" for s
                     in requirements.split("\n")}
 setup(
     name="shaku-database",
-    version="1.0.6",
+    version="1.0.7",
     author="hawktorng",
     author_email="hawktorng@shaku.com.tw",
     description="Shaku Database util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/hawktorng1/test_shaku",
     packages=find_packages(),
```

### Comparing `shaku-database-1.0.6/shaku_database.egg-info/PKG-INFO` & `shaku-database-1.0.7/shaku_database.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.0.6
+Version: 1.0.7
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

