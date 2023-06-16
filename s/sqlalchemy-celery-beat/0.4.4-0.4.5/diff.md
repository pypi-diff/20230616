# Comparing `tmp/sqlalchemy_celery_beat-0.4.4.tar.gz` & `tmp/sqlalchemy_celery_beat-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_celery_beat-0.4.4.tar", last modified: Thu Jun 15 17:41:11 2023, max compression
+gzip compressed data, was "sqlalchemy_celery_beat-0.4.5.tar", last modified: Fri Jun 16 00:57:27 2023, max compression
```

## Comparing `sqlalchemy_celery_beat-0.4.4.tar` & `sqlalchemy_celery_beat-0.4.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 17:41:11.110450 sqlalchemy_celery_beat-0.4.4/
--rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.4.4/LICENSE
--rw-rw-rw-   0        0        0     9410 2023-06-15 17:41:11.109451 sqlalchemy_celery_beat-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     8462 2023-06-15 17:35:29.000000 sqlalchemy_celery_beat-0.4.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 17:41:11.110450 sqlalchemy_celery_beat-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     2982 2023-06-15 17:35:46.000000 sqlalchemy_celery_beat-0.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 17:41:11.078447 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/
--rw-rw-rw-   0        0        0      255 2023-06-15 17:39:21.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/__init__.py
--rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/clockedschedule.py
--rw-rw-rw-   0        0        0    13060 2023-06-15 17:22:39.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/models.py
--rw-rw-rw-   0        0        0    16954 2023-06-15 17:34:05.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/schedulers.py
--rw-rw-rw-   0        0        0     2272 2023-06-15 12:12:30.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/session.py
--rw-rw-rw-   0        0        0     1323 2023-06-15 13:53:44.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/time_utils.py
--rw-rw-rw-   0        0        0     2766 2023-06-15 09:08:15.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/tzcrontab.py
-drwxrwxrwx   0        0        0        0 2023-06-15 17:41:11.107449 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/
--rw-rw-rw-   0        0        0     9410 2023-06-15 17:41:11.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-06-15 17:41:11.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 17:41:11.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-06-15 17:41:11.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-15 17:41:11.000000 sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 00:57:27.419358 sqlalchemy_celery_beat-0.4.5/
+-rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0     9410 2023-06-16 00:57:27.418361 sqlalchemy_celery_beat-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8462 2023-06-15 17:35:29.000000 sqlalchemy_celery_beat-0.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 00:57:27.419358 sqlalchemy_celery_beat-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     2982 2023-06-16 00:55:59.000000 sqlalchemy_celery_beat-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 00:57:27.372359 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/
+-rw-rw-rw-   0        0        0      255 2023-06-15 17:39:21.000000 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/__init__.py
+-rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/clockedschedule.py
+-rw-rw-rw-   0        0        0    13060 2023-06-15 17:22:39.000000 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/models.py
+-rw-rw-rw-   0        0        0    16954 2023-06-15 17:34:05.000000 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/schedulers.py
+-rw-rw-rw-   0        0        0     2259 2023-06-16 00:54:54.000000 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/session.py
+-rw-rw-rw-   0        0        0     1323 2023-06-15 13:53:44.000000 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/time_utils.py
+-rw-rw-rw-   0        0        0     2766 2023-06-15 09:08:15.000000 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/tzcrontab.py
+drwxrwxrwx   0        0        0        0 2023-06-16 00:57:27.415357 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat.egg-info/
+-rw-rw-rw-   0        0        0     9410 2023-06-16 00:57:27.000000 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-06-16 00:57:27.000000 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 00:57:27.000000 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-06-16 00:57:27.000000 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-16 00:57:27.000000 sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat.egg-info/top_level.txt
```

### Comparing `sqlalchemy_celery_beat-0.4.4/LICENSE` & `sqlalchemy_celery_beat-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.4/PKG-INFO` & `sqlalchemy_celery_beat-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_celery_beat
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
```

### Comparing `sqlalchemy_celery_beat-0.4.4/README.md` & `sqlalchemy_celery_beat-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.4/setup.py` & `sqlalchemy_celery_beat-0.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
     name="sqlalchemy_celery_beat",
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.4.4",
+    version="0.4.5",
     # The project's main homepage.
     url="https://github.com/farahats9/sqlalchemy-celery-beat",
     # Choose your license
 
     license='MIT',
 
     description="A Scheduler Based SQLalchemy For Celery",
```

### Comparing `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/clockedschedule.py` & `sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/clockedschedule.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/models.py` & `sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/models.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/schedulers.py` & `sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/schedulers.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/session.py` & `sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from contextlib import contextmanager
 
 from sqlalchemy import create_engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.pool import NullPool
-from sqlalchemy.schema import CreateSchema
+# from sqlalchemy.schema import CreateSchema  # does not work for SA 1.4
 
 from kombu.utils.compat import register_after_fork
 
 ModelBase = declarative_base()
 
 
 @contextmanager
@@ -62,12 +62,11 @@
             return engine, self._sessions[dburi]
         else:
             return engine, sessionmaker(bind=engine)
 
     def prepare_models(self, engine, schema=None):
         if not self.prepared:
             if schema:
-                with engine.connect() as connection:
-                    connection.execute(CreateSchema(schema, if_not_exists=True))
-                    connection.commit()
+                with engine.begin() as connection:
+                    connection.execute(f'CREATE SCHEMA IF NOT EXISTS {schema};')
             ModelBase.metadata.create_all(engine)
             self.prepared = True
```

### Comparing `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/time_utils.py` & `sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/time_utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat/tzcrontab.py` & `sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat/tzcrontab.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/PKG-INFO` & `sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-celery-beat
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
```

### Comparing `sqlalchemy_celery_beat-0.4.4/sqlalchemy_celery_beat.egg-info/SOURCES.txt` & `sqlalchemy_celery_beat-0.4.5/sqlalchemy_celery_beat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

