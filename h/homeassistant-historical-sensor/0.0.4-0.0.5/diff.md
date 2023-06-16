# Comparing `tmp/homeassistant-historical-sensor-0.0.4.tar.gz` & `tmp/homeassistant-historical-sensor-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant-historical-sensor-0.0.4.tar", last modified: Tue Mar 14 14:09:55 2023, max compression
+gzip compressed data, was "homeassistant-historical-sensor-0.0.5.tar", last modified: Fri Jun 16 17:13:10 2023, max compression
```

## Comparing `homeassistant-historical-sensor-0.0.4.tar` & `homeassistant-historical-sensor-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:09:55.392421 homeassistant-historical-sensor-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-03-14 14:09:55.392421 homeassistant-historical-sensor-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-14 14:09:45.000000 homeassistant-historical-sensor-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:09:55.392421 homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-14 14:09:45.000000 homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-03-14 14:09:45.000000 homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-03-14 14:09:45.000000 homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-14 14:09:45.000000 homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-14 14:09:45.000000 homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:09:55.392421 homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-03-14 14:09:55.000000 homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-14 14:09:55.000000 homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:09:55.000000 homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-14 14:09:55.000000 homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-14 14:09:45.000000 homeassistant-historical-sensor-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-14 14:09:55.396421 homeassistant-historical-sensor-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:10.251242 homeassistant-historical-sensor-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-16 17:13:10.251242 homeassistant-historical-sensor-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:10.251242 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:10.251242 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-16 17:13:10.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-16 17:13:10.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:13:10.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 17:13:10.000000 homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 17:13:00.000000 homeassistant-historical-sensor-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-16 17:13:10.251242 homeassistant-historical-sensor-0.0.5/setup.cfg
```

### Comparing `homeassistant-historical-sensor-0.0.4/PKG-INFO` & `homeassistant-historical-sensor-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.0.4
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.0.5
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
 Release (latest SemVer including pre-releases)](https://img.shields.io/github/
```

### Comparing `homeassistant-historical-sensor-0.0.4/README.md` & `homeassistant-historical-sensor-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor/__init__.py` & `homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,13 +23,17 @@
 from homeassistant.const import MAJOR_VERSION, MINOR_VERSION
 
 from .sensor import HistoricalSensor, PollUpdateMixin
 from .state import HistoricalState
 
 LOGGER = logging.getLogger(__name__)
 
-if not (MAJOR_VERSION >= 2023 and MINOR_VERSION >= 2):
-    msg = "Required homeassistant version >=2023.2.0"
+if not (MAJOR_VERSION >= 2023 and MINOR_VERSION >= 6):
+    msg = "Required homeassistant version >=2023.6.0"
     LOGGER.debug(msg)
     raise SystemError(msg)
 
-__all__ = ["HistoricalSensor", "HistoricalState", "PollUpdateMixin"]
+__all__ = [
+    "HistoricalSensor",
+    "HistoricalState",
+    "PollUpdateMixin",
+]
```

### Comparing `homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor/patches.py` & `homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/patches.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor/sensor.py` & `homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/sensor.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,26 +25,27 @@
 
 import sqlalchemy.exc
 import sqlalchemy.orm
 from homeassistant.components import recorder
 from homeassistant.components.recorder import db_schema as db_schema
 from homeassistant.components.recorder.models import StatisticData, StatisticMetaData
 from homeassistant.components.recorder.statistics import (
+    StatisticsRow,
     async_add_external_statistics,
+    async_import_statistics,
     split_statistic_id,
+    valid_statistic_id,
 )
 from homeassistant.components.sensor import SensorEntity
-from homeassistant.const import STATE_UNAVAILABLE, STATE_UNKNOWN
 from homeassistant.helpers.event import async_track_time_interval
 from homeassistant.util import dt as dtutil
-from sqlalchemy import not_, or_
 
-from .patches import _build_attributes, _stringify_state
+from . import util
+from .patches import _stringify_state
 from .state import HistoricalState
-from .util import get_last_statistics_wrapper
 
 _LOGGER = logging.getLogger(__name__)
 
 
 # You must know:
 # * DB keeps datetime object as utc
 # * Each time hass is started a new record is created, that record can be 'unknow'
@@ -94,288 +95,274 @@
     def historical_states(self):
         if hasattr(self, "_attr_historical_states"):
             return self._attr_historical_states
 
         return []
 
     @property
-    def statistics_enabled(self) -> bool:
-        if hasattr(self, "_attr_statistics_enabled"):
-            return self._attr_statistics_enabled
-
-        smd = self.get_statatistics_metadata()
-        enabled = smd["has_mean"] or smd["has_sum"]
-        return enabled
+    def recorder(self):
+        return recorder.get_instance(self.hass)
 
     @abstractmethod
     async def async_update_historical(self):
         """async_update_historical()
 
         This method should be be implemented by sensors
 
         Implement this async method to fetch historical data from provider and store
         into self._attr_historical_states
         """
         raise NotImplementedError()
 
-    async def async_calculate_statistic_data(
-        self, hist_states: List[HistoricalState], *, latest: Optional[dict]
-    ) -> List[StatisticData]:
-        """Calculate statistics data from dated states
-
-        This method may be be implemented by sensors
-        """
-        raise NotImplementedError()
-
     async def async_write_ha_historical_states(self):
         """async_write_ha_historical_states()
 
         This method writes `self.historical_states` into database
         """
 
         hist_states = self.historical_states
         if any([True for x in hist_states if x.dt.tzinfo is None]):
             _LOGGER.error("historical_states MUST include tzinfo")
             return
 
         hist_states = list(sorted(hist_states, key=lambda x: x.dt))
         _LOGGER.debug(
-            f"{self.entity_id}: {len(hist_states)} historical states collected from sensor"
+            f"{self.entity_id}: "
+            f"{len(hist_states)} historical states collected from sensor"
         )
 
         if not hist_states:
             return
 
         # Write states
-        await self._get_recorder_instance().async_add_executor_job(
-            self._save_states_into_recorder, hist_states
-        )
-
-        # Write statistics if enabled
-        if self.statistics_enabled:
-            await self._async_save_states_into_statistics(hist_states)
-        else:
-            _LOGGER.debug(f"{self.entity_id}: statistics are not enabled")
-
-    def _get_recorder_instance(self):
-        return recorder.get_instance(self.hass)
-
-    async def _async_save_states_into_statistics(
-        self, hist_states: List[HistoricalState]
-    ):
-        # Don't do this
-        #
-        # def delete_statistics():
-        #     with recorder.util.session_scope(
-        #         session=self._get_recorder_instance().get_session()
-        #     ) as session:
-        #         start_cutoff = hist_states[0].when - timedelta(hours=1)
-        #         end_cutoff = hist_states[-1].when
-        #         qs = (
-        #             session.query(db_schema.Statistics)
-        #             .join(
-        #                 db_schema.StatisticsMeta,
-        #                 db_schema.Statistics.metadata_id == db_schema.StatisticsMeta.id,
-        #                 isouter=True,
-        #             )
-        #             .filter(db_schema.Statistics.start >= start_cutoff)
-        #             .filter(db_schema.Statistics.start < end_cutoff)
-        #         )
-        #         stats = [x.id for x in qs]
-
-        #     clear_statistics(self._get_recorder_instance(), stats)
-        #     _LOGGER.debug(f"Cleared {len(stats)} statistics")
-
-        # await self._get_recorder_instance().async_add_executor_job(delete_statistics)
-
-        statistics_meta = self.get_statatistics_metadata()
-
-        latest = await get_last_statistics_wrapper(
-            self.hass, statistics_meta["statistic_id"]
+        await self.recorder.async_add_executor_job(
+            self._write_recorder_states, hist_states
         )
+        await self._write_statistic_data(hist_states)
 
-        if latest is not None:
-            cutoff = dtutil.utc_from_timestamp(latest["start"]) + timedelta(hours=1)
-            hist_states = [x for x in hist_states if x.dt > cutoff]
-
-        #
-        # Calculate stats
-        #
-        statistics_data = await self.async_calculate_statistic_data(
-            hist_states, latest=latest
-        )
-
-        for stat in statistics_data:
-            tmp = dict(stat)
-            start_dt = dtutil.as_local(tmp.pop("start"))
-            _LOGGER.debug(f"new statistic: start={start_dt}, value={tmp!r}")
-
-        # Note: Import statistics as external
-        async_add_external_statistics(self.hass, statistics_meta, statistics_data)
-        _LOGGER.debug(
-            f"{self.entity_id}: collected {len(statistics_data)} statistic points"
-        )
-
-    def _save_states_into_recorder(self, hist_states: List[HistoricalState]):
-        #
-        # 2023.2.1 Introduces last_updated_ts, last_changed_ts columns
-        #
-
+    def _write_recorder_states(self, hist_states: List[HistoricalState]):
         with recorder.util.session_scope(
-            session=self._get_recorder_instance().get_session()
+            session=self.recorder.get_session()
         ) as session:
-            base_qs = session.query(db_schema.States).filter(
-                db_schema.States.entity_id == self.entity_id
-            )
+            # base_qs = session.query(db_schema.States).filter(
+            #     db_schema.States.entity_id == self.entity_id
+            # )
 
             #
             # Delete invalid states
             #
 
             try:
-                states = base_qs.filter(
-                    or_(
-                        db_schema.States.state == STATE_UNKNOWN,
-                        db_schema.States.state == STATE_UNAVAILABLE,
-                    )
-                )
-                state_count = states.count()
-                states.delete()
-                session.commit()
+                # states = base_qs.filter(
+                #     or_(
+                #         db_schema.States.state == STATE_UNKNOWN,
+                #         db_schema.States.state == STATE_UNAVAILABLE,
+                #     )
+                # )
+                # n_states = states.count()
+                # states.delete()
+                # session.commit()
 
-                _LOGGER.debug(f"Deleted {state_count} invalid states")
+                n_states = util.delete_invalid_states(session, self.entity_id)
+                _LOGGER.debug(
+                    f"{self.entity_id}: " f"{n_states} invalid states deleted"
+                )
 
             except sqlalchemy.exc.IntegrityError:
                 session.rollback()
                 _LOGGER.debug("Warning: Current recorder schema is not supported")
                 _LOGGER.debug(
                     "Invalid states can't be deleted from recorder."
                     + "This is not critical just unsightly for some graphs "
                 )
 
             #
-            # Delete intersecting states (*)
-            #
-            # * This approach has been tested several times and always ends up
-            # causing unexpected failures. Sometimes the database schema
-            # changes and sometimes, depending on the engine, integrity
-            # failures appear.
-            # It is better to discard the new overlapping states than to
-            # delete them from the database.
-
-            # cutoff = dtutil.as_timestamp(hist_states[0].when)
-            # intersect_states = base_qs.filter(
-            #     db_schema.States.last_updated_ts >= cutoff
-            # )
-            # intersect_count = intersect_states.count()
-            # intersect_states.delete()
-            # session.commit()
-            #
-            # _LOGGER.debug(
-            #     f"Deleted {intersect_count} states after {hist_states[0].when}"
-            # )
-
-            #
             # Check latest state in the database
             #
 
             try:
-                latest_state = (
-                    base_qs.filter(
-                        not_(
-                            or_(
-                                db_schema.States.state == STATE_UNAVAILABLE,
-                                db_schema.States.state == STATE_UNKNOWN,
-                            )
-                        )
-                    )
-                    .order_by(db_schema.States.last_updated_ts.desc())
-                    .first()
-                )
+                latest = util.get_latest_state(session, self.entity_id)
+
             except sqlalchemy.exc.DatabaseError:
                 _LOGGER.debug(
                     "Error: Current recorder schema is not supported. "
                     + "This error is fatal, please file a bug"
                 )
                 return
 
             #
             # Drop historical states older than lastest db state
             #
-            if latest_state:
-                cutoff = dtutil.utc_from_timestamp(latest_state.last_updated_ts or 0)
+
+            # About deleting intersecting states instead of drop incomming
+            # overlapping states: This approach has been tested several times and
+            # always ends up causing unexpected failures. Sometimes the database
+            # schema changes and sometimes, depending on the engine, integrity
+            # failures appear. It is better to discard the new overlapping states
+            # than to delete them from the database.
+
+            if latest:
+                cutoff = dtutil.utc_from_timestamp(latest.last_updated_ts or 0)
                 _LOGGER.debug(
-                    f"{self.entity_id}: lastest state found: {latest_state.state} @ {cutoff}"
+                    f"{self.entity_id}: " f"lastest state: {latest.state} @ {cutoff}"
                 )
                 hist_states = [x for x in hist_states if x.dt > cutoff]
 
             else:
                 _LOGGER.debug(f"{self.entity_id}: no previous states found")
 
+            #
+            # Check if there are any states left
+            #
             if not hist_states:
-                _LOGGER.debug(f"{self.entity_id}: no new states from API")
+                _LOGGER.debug(f"{self.entity_id}: no new states")
                 return
 
+            state_meta, _ = util.get_states_meta(session, self.entity_id)
+
             #
-            # Build recorder State, StateAttributes and Event
+            # Build recorder States
             #
+            state_meta, _ = util.get_states_meta(
+                session, self.entity_id, create_if_missing=True
+            )
 
             db_states: List[db_schema.States] = []
             for idx, hist_state in enumerate(hist_states):
-                attrs_as_dict = _build_attributes(self, hist_state.state)
-                attrs_as_dict.update(hist_state.attributes)
-                attrs_as_str = db_schema.JSON_DUMP(attrs_as_dict)
-
-                attrs_as_bytes = (
-                    b"{}" if hist_state.state is None else attrs_as_str.encode("utf-8")
-                )
-
-                attrs_hash = db_schema.StateAttributes.hash_shared_attrs_bytes(
-                    attrs_as_bytes
-                )
-
-                state_attributes = db_schema.StateAttributes(
-                    hash=attrs_hash, shared_attrs=attrs_as_str
-                )
+                # attrs_as_dict = _build_attributes(self, hist_state.state)
+                # attrs_as_dict.update(hist_state.attributes)
+                # attrs_as_str = db_schema.JSON_DUMP(attrs_as_dict)
+
+                # attrs_as_bytes = (
+                #     b"{}" if hist_state.state is None else attrs_as_str.encode("utf-8")
+                # )
+
+                # attrs_hash = db_schema.StateAttributes.hash_shared_attrs_bytes(
+                #     attrs_as_bytes
+                # )
+
+                # state_attributes = db_schema.StateAttributes(
+                #     hash=attrs_hash, shared_attrs=attrs_as_str
+                # )
 
                 ts = dtutil.as_timestamp(hist_state.dt)
                 state = db_schema.States(
-                    entity_id=self.entity_id,
+                    # entity_id=self.entity_id,
+                    states_meta_rel=state_meta,
                     last_changed_ts=ts,
                     last_updated_ts=ts,
-                    old_state=db_states[idx - 1] if idx else latest_state,
+                    old_state=db_states[idx - 1] if idx else latest,
                     state=_stringify_state(self, hist_state.state),
-                    state_attributes=state_attributes,
+                    # state_attributes=state_attributes,
                 )
 
-                _LOGGER.debug(
-                    f"new state: dt={dtutil.as_local(hist_state.dt)} value={hist_state.state}"
-                )
+                # _LOGGER.debug(
+                #     f"new state: "
+                #     f"dt={dtutil.as_local(hist_state.dt)} value={hist_state.state}"
+                # )
                 db_states.append(state)
 
-            session.add_all(db_states)
-            session.commit()
+            util.save_states(session, db_states)
 
             _LOGGER.debug(f"{self.entity_id}: {len(db_states)} saved into the database")
 
-    def get_statatistics_metadata(self) -> StatisticMetaData:
-        statistic_id = statistic_id = self.entity_id.replace(".", ":")
-        source = split_statistic_id(statistic_id)[0]
+    async def _write_statistic_data(self, hist_states: List[HistoricalState]):
+        if self.statatistic_id is None:
+            _LOGGER.debug(f"{self.entity_id}: statistics are not enabled")
+            return
+
+        statistics_meta = self.get_statatistic_metadata()
+
+        latest = await util.get_last_statistics_wrapper(
+            self.hass, statistics_meta["statistic_id"]
+        )
+
+        # Don't do this, see notes above "About deleting intersecting states"
+        #
+        # def delete_statistics():
+        #     with recorder.util.session_scope(
+        #         session=self.recorder.get_session()
+        #     ) as session:
+        #         start_cutoff = hist_states[0].when - timedelta(hours=1)
+        #         end_cutoff = hist_states[-1].when
+        #         qs = (
+        #             session.query(db_schema.Statistics)
+        #             .join(
+        #                 db_schema.StatisticsMeta,
+        #                 db_schema.Statistics.metadata_id == db_schema.StatisticsMeta.id,
+        #                 isouter=True,
+        #             )
+        #             .filter(db_schema.Statistics.start >= start_cutoff)
+        #             .filter(db_schema.Statistics.start < end_cutoff)
+        #         )
+        #         stats = [x.id for x in qs]
+        #
+        #     clear_statistics(self.recorder, stats)
+        #     _LOGGER.debug(f"Cleared {len(stats)} statistics")
+        #
+        # await self.recorder.async_add_executor_job(delete_statistics)
+
+        hist_states = self.historical_states
+        if latest is not None:
+            cutoff = dtutil.utc_from_timestamp(latest["start"]) + timedelta(hours=1)
+            hist_states = [x for x in hist_states if x.dt > cutoff]
+
+        #
+        # Calculate stats
+        #
+        statistics_data = await self.async_calculate_statistic_data(
+            hist_states, latest=latest
+        )
+
+        for stat in statistics_data:
+            tmp = dict(stat)
+            start_dt = dtutil.as_local(tmp.pop("start"))
+            _LOGGER.debug(f"new statistic: start={start_dt}, value={tmp!r}")
+
+        if valid_statistic_id(self.statatistic_id):
+            async_add_external_statistics(self.hass, statistics_meta, statistics_data)
+        else:
+            async_import_statistics(self.hass, statistics_meta, statistics_data)
+
+        _LOGGER.debug(
+            f"{self.entity_id}: collected {len(statistics_data)} statistic points"
+        )
+
+    @property
+    def statatistic_id(self) -> Optional[str]:
+        return None
+
+    def get_statatistic_metadata(self) -> StatisticMetaData:
+        if self.statatistic_id is None:
+            raise ValueError(f"{self.entity_id} statatistics_id is None")
+
+        if valid_statistic_id(self.statatistic_id):
+            source = split_statistic_id(self.statatistic_id)[0]
+        else:
+            source = "recorder"
 
         metadata = StatisticMetaData(
             has_mean=False,
             has_sum=False,
             name=f"{self.name} Statistics",
             source=source,
-            statistic_id=statistic_id,
+            statistic_id=self.statatistic_id,
             unit_of_measurement=self.unit_of_measurement,
         )
 
         return metadata
 
+    async def async_calculate_statistic_data(
+        self,
+        hist_states: List[HistoricalState],
+        *,
+        latest: Optional[StatisticsRow] = None,
+    ) -> List[StatisticData]:
+        raise NotImplementedError()
+
 
 class PollUpdateMixin(HistoricalSensor):
     """PollUpdateMixin for simulate poll update model
 
     This mixin provides:
 
       - UPDATE_INTERVAL: timedelta
```

### Comparing `homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor/state.py` & `homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor/state.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,10 @@
     def asdict(self):
         return asdict(self)
 
     def as_value_and_timestamp(self):
         if not self.dt.tzinfo:
             raise ValueError(f"{self}.dt is missing tzinfo")
 
-        import ipdb
-
-        ipdb.set_trace()
-        pass
-
         utc = dtutil.as_utc(self.dt)
         ts = dtutil.utc_to_timestamp(utc)
         return self.state, ts
```

### Comparing `homeassistant-historical-sensor-0.0.4/homeassistant_historical_sensor.egg-info/PKG-INFO` & `homeassistant-historical-sensor-0.0.5/homeassistant_historical_sensor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.0.4
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 0.0.5
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
 Release (latest SemVer including pre-releases)](https://img.shields.io/github/
```

### Comparing `homeassistant-historical-sensor-0.0.4/setup.cfg` & `homeassistant-historical-sensor-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = homeassistant-historical-sensor
-version = 0.0.4
+version = 0.0.5
 author = Luis López
 author_email = luis@cuarentaydos.com
 description = Historical sensors for HomeAssistant
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ldotlopez/ha-historical-sensor
 project_urls =
```

