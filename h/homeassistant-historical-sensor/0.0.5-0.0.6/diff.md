# Comparing `tmp/homeassistant-historical-sensor-0.0.5.tar.gz` & `tmp/homeassistant-historical-sensor-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant-historical-sensor-0.0.5.tar", last modified: Fri Jun 16 17:13:10 2023, max compression
+gzip compressed data, was "homeassistant-historical-sensor-0.0.6.tar", last modified: Fri Jun 16 17:49:08 2023, max compression
```

## Comparing `homeassistant-historical-sensor-0.0.5.tar` & `homeassistant-historical-sensor-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:10.251242 homeassistant-historical-sensor-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-16 17:13:10.251242 homeassistant-historical-sensor-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:10.251242 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:10.251242 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-16 17:13:10.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-16 17:13:10.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:13:10.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 17:13:10.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-16 17:13:10.251242 homeassistant-historical-sensor-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:08.788144 homeassistant-historical-sensor-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-16 17:49:08.788144 homeassistant-historical-sensor-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:08.788144 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:08.788144 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-16 17:49:08.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-16 17:49:08.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:49:08.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 17:49:08.000000 homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 17:48:57.000000 homeassistant-historical-sensor-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-16 17:49:08.788144 homeassistant-historical-sensor-0.0.6/setup.cfg
```

### Comparing `homeassistant-historical-sensor-0.0.5/PKG-INFO` & `homeassistant-historical-sensor-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 0.0.5
+Version: 0.0.6
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.0.5
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.0.6
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
 Release (latest SemVer including pre-releases)](https://img.shields.io/github/
```

### Comparing `homeassistant-historical-sensor-0.0.5/README.md` & `homeassistant-historical-sensor-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/__init__.py` & `homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/patches.py` & `homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/patches.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/sensor.py` & `homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,22 +213,18 @@
             #
             # Check if there are any states left
             #
             if not hist_states:
                 _LOGGER.debug(f"{self.entity_id}: no new states")
                 return
 
-            state_meta, _ = util.get_states_meta(session, self.entity_id)
-
             #
             # Build recorder States
             #
-            state_meta, _ = util.get_states_meta(
-                session, self.entity_id, create_if_missing=True
-            )
+            state_meta = util.get_states_meta(session, self.entity_id)
 
             db_states: List[db_schema.States] = []
             for idx, hist_state in enumerate(hist_states):
                 # attrs_as_dict = _build_attributes(self, hist_state.state)
                 # attrs_as_dict.update(hist_state.attributes)
                 # attrs_as_str = db_schema.JSON_DUMP(attrs_as_dict)
```

### Comparing `homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/state.py` & `homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/state.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/util.py` & `homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,25 +50,23 @@
     )
     if not res:
         return None
 
     return res[statistic_id][0]
 
 
-def get_states_meta(session: Session, entity_id: str, *, create_if_missing=False):
+def get_states_meta(session: Session, entity_id: str) -> db_schema.StatesMeta:
     ret = session.execute(_get_base_stmt(session, entity_id)).scalar()
 
-    created = False
-
-    if not ret and create_if_missing:
+    if not ret:
         ret = db_schema.StatesMeta(entity_id=entity_id)
         session.add(ret)
-        created = True
+        session.commit()
 
-    return ret, created
+    return ret
 
 
 def _get_base_stmt(session: Session, entity_id: str):
     return (
         select(db_schema.States)
         .join(db_schema.StatesMeta)
         .where(db_schema.StatesMeta.entity_id == entity_id)
```

### Comparing `homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor.egg-info/PKG-INFO` & `homeassistant-historical-sensor-0.0.6/homeassistant_historical_sensor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 0.0.5
+Version: 0.0.6
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.0.5
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.0.6
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
 Release (latest SemVer including pre-releases)](https://img.shields.io/github/
```

### Comparing `homeassistant-historical-sensor-0.0.5/setup.cfg` & `homeassistant-historical-sensor-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = homeassistant-historical-sensor
-version = 0.0.5
+version = 0.0.6
 author = Luis López
 author_email = luis@cuarentaydos.com
 description = Historical sensors for HomeAssistant
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ldotlopez/ha-historical-sensor
 project_urls =
```

