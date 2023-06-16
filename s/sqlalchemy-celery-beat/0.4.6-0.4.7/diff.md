# Comparing `tmp/sqlalchemy_celery_beat-0.4.6.tar.gz` & `tmp/sqlalchemy_celery_beat-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_celery_beat-0.4.6.tar", last modified: Fri Jun 16 16:35:42 2023, max compression
+gzip compressed data, was "sqlalchemy_celery_beat-0.4.7.tar", last modified: Fri Jun 16 17:40:43 2023, max compression
```

## Comparing `sqlalchemy_celery_beat-0.4.6.tar` & `sqlalchemy_celery_beat-0.4.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 16:35:42.404265 sqlalchemy_celery_beat-0.4.6/
--rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.4.6/LICENSE
--rw-rw-rw-   0        0        0     9914 2023-06-16 16:35:42.400266 sqlalchemy_celery_beat-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     8955 2023-06-16 16:33:08.000000 sqlalchemy_celery_beat-0.4.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 16:35:42.405274 sqlalchemy_celery_beat-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0     3138 2023-06-16 10:58:53.000000 sqlalchemy_celery_beat-0.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 16:35:42.355267 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/
--rw-rw-rw-   0        0        0      455 2023-06-16 10:59:02.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/__init__.py
--rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/clockedschedule.py
--rw-rw-rw-   0        0        0    13436 2023-06-16 16:21:32.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/models.py
--rw-rw-rw-   0        0        0    16955 2023-06-16 03:08:50.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/schedulers.py
--rw-rw-rw-   0        0        0     3563 2023-06-16 16:21:28.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/session.py
--rw-rw-rw-   0        0        0     1323 2023-06-15 13:53:44.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/time_utils.py
--rw-rw-rw-   0        0        0     2766 2023-06-15 09:08:15.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/tzcrontab.py
-drwxrwxrwx   0        0        0        0 2023-06-16 16:35:42.397268 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat.egg-info/
--rw-rw-rw-   0        0        0     9914 2023-06-16 16:35:42.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-06-16 16:35:42.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 16:35:42.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-16 16:35:42.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-06-16 16:35:42.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-16 16:35:42.000000 sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 17:40:43.968468 sqlalchemy_celery_beat-0.4.7/
+-rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0     9914 2023-06-16 17:40:43.967475 sqlalchemy_celery_beat-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8955 2023-06-16 16:33:08.000000 sqlalchemy_celery_beat-0.4.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 17:40:43.968468 sqlalchemy_celery_beat-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     3138 2023-06-16 17:40:10.000000 sqlalchemy_celery_beat-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:40:43.936468 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/
+-rw-rw-rw-   0        0        0      455 2023-06-16 17:40:14.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/__init__.py
+-rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/clockedschedule.py
+-rw-rw-rw-   0        0        0    13539 2023-06-16 17:39:12.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/models.py
+-rw-rw-rw-   0        0        0    16955 2023-06-16 03:08:50.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/schedulers.py
+-rw-rw-rw-   0        0        0     3708 2023-06-16 17:18:27.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/session.py
+-rw-rw-rw-   0        0        0     1323 2023-06-15 13:53:44.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/time_utils.py
+-rw-rw-rw-   0        0        0     2766 2023-06-15 09:08:15.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/tzcrontab.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:40:43.964473 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/
+-rw-rw-rw-   0        0        0     9914 2023-06-16 17:40:43.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-06-16 17:40:43.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 17:40:43.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-16 17:40:43.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-06-16 17:40:43.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-16 17:40:43.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/top_level.txt
```

### Comparing `sqlalchemy_celery_beat-0.4.6/LICENSE` & `sqlalchemy_celery_beat-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.6/PKG-INFO` & `sqlalchemy_celery_beat-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_celery_beat
-Version: 0.4.6
+Version: 0.4.7
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
```

### Comparing `sqlalchemy_celery_beat-0.4.6/README.md` & `sqlalchemy_celery_beat-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.6/setup.py` & `sqlalchemy_celery_beat-0.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
     name="sqlalchemy_celery_beat",
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.4.6",
+    version="0.4.7",
     # The project's main homepage.
     url="https://github.com/farahats9/sqlalchemy-celery-beat",
     # Choose your license
 
     license='MIT',
 
     description="A Scheduler Based SQLalchemy For Celery",
```

### Comparing `sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/clockedschedule.py` & `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/clockedschedule.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/models.py` & `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,23 +242,25 @@
         if not s:
             s = connection.execute(insert(PeriodicTaskChanged),
                                    last_update=dt.datetime.now())
         else:
             s = connection.execute(update(PeriodicTaskChanged).
                                    where(PeriodicTaskChanged.id == 1).
                                    values(last_update=dt.datetime.now()))
-        connection.commit()
 
     @classmethod
-    def update_from_session(cls, session: Session):
+    def update_from_session(cls, session: Session, commit: bool = True):
         """
         :param session: the Session to use
+        :param commit: commit the session if set to true
         """
         connection = session.connection()
         cls.update_changed(None, connection, None)
+        if commit:
+            connection.commit()
 
     @classmethod
     def last_change(cls, session):
         periodic_tasks = session.query(PeriodicTaskChanged).get(1)
         if periodic_tasks:
             return periodic_tasks.last_update
```

### Comparing `sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/schedulers.py` & `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/schedulers.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/session.py` & `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """SQLAlchemy session."""
 
 import time
 from contextlib import contextmanager
 
 from celery.utils.time import get_exponential_backoff_interval
 from kombu.utils.compat import register_after_fork
-from sqlalchemy import create_engine
+from sqlalchemy import DDL, create_engine
 from sqlalchemy.exc import DatabaseError
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.pool import NullPool
 
 # from sqlalchemy.schema import CreateSchema  # does not work for SA 1.4
 
@@ -75,16 +75,19 @@
             # create them, which is a race condition. If it raises an error
             # in one iteration, the next may pass all the existence checks
             # and the call will succeed.
             retries = 0
             while True:
                 try:
                     if schema:
-                        with engine.begin() as connection:
-                            connection.execute(f'CREATE SCHEMA IF NOT EXISTS {schema};')
+                        with engine.connect() as connection:
+                            connection.execute(
+                                DDL("CREATE SCHEMA IF NOT EXISTS %(schema)s", {"schema": schema})
+                            )
+                            connection.commit()
 
                     ModelBase.metadata.create_all(engine)
                 except DatabaseError:
                     if retries < PREPARE_MODELS_MAX_RETRIES:
                         sleep_amount_ms = get_exponential_backoff_interval(
                             10, retries, 1000, True
                         )
```

### Comparing `sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/time_utils.py` & `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/time_utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat/tzcrontab.py` & `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/tzcrontab.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat.egg-info/PKG-INFO` & `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-celery-beat
-Version: 0.4.6
+Version: 0.4.7
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
```

### Comparing `sqlalchemy_celery_beat-0.4.6/sqlalchemy_celery_beat.egg-info/SOURCES.txt` & `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

