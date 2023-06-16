# Comparing `tmp/aiovantage-0.1.0.tar.gz` & `tmp/aiovantage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiovantage-0.1.0.tar", last modified: Tue Jun 13 02:22:59 2023, max compression
+gzip compressed data, was "aiovantage-0.1.1.tar", last modified: Fri Jun 16 06:42:14 2023, max compression
```

## Comparing `aiovantage-0.1.0.tar` & `aiovantage-0.1.1.tar`

### file list

```diff
@@ -1,108 +1,158 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 02:22:59.104928 aiovantage-0.1.0/
--rw-r--r--   0 james      (501) staff       (20)     1068 2023-06-13 02:18:48.000000 aiovantage-0.1.0/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     2285 2023-06-13 02:22:59.104807 aiovantage-0.1.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1769 2023-06-13 02:11:39.000000 aiovantage-0.1.0/README.md
--rw-r--r--   0 james      (501) staff       (20)      929 2023-06-13 02:17:46.000000 aiovantage-0.1.0/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-13 02:22:59.104967 aiovantage-0.1.0/setup.cfg
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 02:22:59.073011 aiovantage-0.1.0/src/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 02:22:59.075134 aiovantage-0.1.0/src/aiovantage/
--rw-r--r--   0 james      (501) staff       (20)     6939 2023-06-05 21:01:16.000000 aiovantage-0.1.0/src/aiovantage/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 02:22:59.077510 aiovantage-0.1.0/src/aiovantage/command_client/
--rw-r--r--   0 james      (501) staff       (20)    29403 2023-06-02 22:18:06.000000 aiovantage-0.1.0/src/aiovantage/command_client/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      835 2023-05-29 02:35:31.000000 aiovantage-0.1.0/src/aiovantage/command_client/errors.py
--rw-r--r--   0 james      (501) staff       (20)      763 2023-06-02 22:32:36.000000 aiovantage-0.1.0/src/aiovantage/command_client/events.py
--rw-r--r--   0 james      (501) staff       (20)      410 2023-05-29 02:35:31.000000 aiovantage-0.1.0/src/aiovantage/command_client/helpers.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 02:22:59.080888 aiovantage-0.1.0/src/aiovantage/command_client/interfaces/
--rw-r--r--   0 james      (501) staff       (20)      587 2023-06-03 19:34:22.000000 aiovantage-0.1.0/src/aiovantage/command_client/interfaces/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      502 2023-06-02 22:31:32.000000 aiovantage-0.1.0/src/aiovantage/command_client/interfaces/base.py
--rw-r--r--   0 james      (501) staff       (20)     3672 2023-06-05 20:00:44.000000 aiovantage-0.1.0/src/aiovantage/command_client/interfaces/blind.py
--rw-r--r--   0 james      (501) staff       (20)     2846 2023-06-05 17:57:38.000000 aiovantage-0.1.0/src/aiovantage/command_client/interfaces/button.py
--rw-r--r--   0 james      (501) staff       (20)     1703 2023-06-05 17:50:59.000000 aiovantage-0.1.0/src/aiovantage/command_client/interfaces/color_temperature.py
--rw-r--r--   0 james      (501) staff       (20)      734 2023-06-05 17:49:29.000000 aiovantage-0.1.0/src/aiovantage/command_client/interfaces/introspection.py
--rw-r--r--   0 james      (501) staff       (20)     3248 2023-06-05 17:51:25.000000 aiovantage-0.1.0/src/aiovantage/command_client/interfaces/load.py
--rw-r--r--   0 james      (501) staff       (20)     1129 2023-06-05 17:57:07.000000 aiovantage-0.1.0/src/aiovantage/command_client/interfaces/object.py
--rw-r--r--   0 james      (501) staff       (20)     8660 2023-06-05 18:15:27.000000 aiovantage-0.1.0/src/aiovantage/command_client/interfaces/rgb_load.py
--rw-r--r--   0 james      (501) staff       (20)      912 2023-06-06 17:24:15.000000 aiovantage-0.1.0/src/aiovantage/command_client/interfaces/sensor.py
--rw-r--r--   0 james      (501) staff       (20)     2757 2023-06-05 17:56:23.000000 aiovantage-0.1.0/src/aiovantage/command_client/interfaces/task.py
--rw-r--r--   0 james      (501) staff       (20)      487 2023-05-29 02:35:31.000000 aiovantage-0.1.0/src/aiovantage/command_client/ssl.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 02:22:59.081974 aiovantage-0.1.0/src/aiovantage/config_client/
--rw-r--r--   0 james      (501) staff       (20)     8726 2023-05-24 21:00:52.000000 aiovantage-0.1.0/src/aiovantage/config_client/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     2432 2023-06-05 20:32:45.000000 aiovantage-0.1.0/src/aiovantage/config_client/helpers.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 02:22:59.082336 aiovantage-0.1.0/src/aiovantage/config_client/methods/
--rw-r--r--   0 james      (501) staff       (20)      304 2023-05-19 23:15:38.000000 aiovantage-0.1.0/src/aiovantage/config_client/methods/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 02:22:59.084390 aiovantage-0.1.0/src/aiovantage/config_client/methods/configuration/
--rw-r--r--   0 james      (501) staff       (20)      310 2023-05-19 20:30:26.000000 aiovantage-0.1.0/src/aiovantage/config_client/methods/configuration/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      347 2023-05-18 22:03:20.000000 aiovantage-0.1.0/src/aiovantage/config_client/methods/configuration/close_filter.py
--rw-r--r--   0 james      (501) staff       (20)      777 2023-05-18 22:03:20.000000 aiovantage-0.1.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py
--rw-r--r--   0 james      (501) staff       (20)      616 2023-05-18 22:03:20.000000 aiovantage-0.1.0/src/aiovantage/config_client/methods/configuration/get_object.py
--rw-r--r--   0 james      (501) staff       (20)      642 2023-05-25 23:56:38.000000 aiovantage-0.1.0/src/aiovantage/config_client/methods/configuration/object_choice.py
--rw-r--r--   0 james      (501) staff       (20)      646 2023-05-31 19:53:36.000000 aiovantage-0.1.0/src/aiovantage/config_client/methods/configuration/open_filter.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 02:22:59.084915 aiovantage-0.1.0/src/aiovantage/config_client/methods/introspection/
--rw-r--r--   0 james      (501) staff       (20)       69 2023-04-15 05:17:46.000000 aiovantage-0.1.0/src/aiovantage/config_client/methods/introspection/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      566 2023-05-19 16:45:00.000000 aiovantage-0.1.0/src/aiovantage/config_client/methods/introspection/get_version.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 02:22:59.085472 aiovantage-0.1.0/src/aiovantage/config_client/methods/login/
--rw-r--r--   0 james      (501) staff       (20)       53 2023-04-10 19:10:19.000000 aiovantage-0.1.0/src/aiovantage/config_client/methods/login/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      464 2023-05-18 22:03:20.000000 aiovantage-0.1.0/src/aiovantage/config_client/methods/login/login.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 02:22:59.100452 aiovantage-0.1.0/src/aiovantage/config_client/objects/
--rw-r--r--   0 james      (501) staff       (20)     1910 2023-06-05 21:17:01.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      111 2023-05-18 21:58:35.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/anemo_sensor.py
--rw-r--r--   0 james      (501) staff       (20)      129 2023-05-18 21:58:30.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/area.py
--rw-r--r--   0 james      (501) staff       (20)      556 2023-06-13 01:30:13.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/blind.py
--rw-r--r--   0 james      (501) staff       (20)      346 2023-06-05 21:23:33.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/blind_group.py
--rw-r--r--   0 james      (501) staff       (20)      748 2023-05-30 23:17:35.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/button.py
--rw-r--r--   0 james      (501) staff       (20)      133 2023-05-18 21:58:14.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/dc_power_profile.py
--rw-r--r--   0 james      (501) staff       (20)      161 2023-06-05 18:50:37.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/ddg_color_load.py
--rw-r--r--   0 james      (501) staff       (20)      159 2023-05-18 21:58:21.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/dg_color_load.py
--rw-r--r--   0 james      (501) staff       (20)      143 2023-05-18 21:58:18.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/dimmer.py
--rw-r--r--   0 james      (501) staff       (20)      308 2023-05-30 23:13:29.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/dry_contact.py
--rw-r--r--   0 james      (501) staff       (20)      157 2023-05-02 22:11:52.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/dual_relay_station.py
--rw-r--r--   0 james      (501) staff       (20)      158 2023-05-02 22:11:55.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/eq_ctrl.py
--rw-r--r--   0 james      (501) staff       (20)      162 2023-05-02 22:11:58.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/eq_ux.py
--rw-r--r--   0 james      (501) staff       (20)     1344 2023-05-26 21:08:22.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/gmem.py
--rw-r--r--   0 james      (501) staff       (20)      154 2023-05-02 22:12:05.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/keypad.py
--rw-r--r--   0 james      (501) staff       (20)      111 2023-05-02 22:12:08.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/light_sensor.py
--rw-r--r--   0 james      (501) staff       (20)     1171 2023-05-30 23:59:57.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/load.py
--rw-r--r--   0 james      (501) staff       (20)      294 2023-06-01 00:27:19.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/load_group.py
--rw-r--r--   0 james      (501) staff       (20)      271 2023-06-01 00:10:15.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/location_object.py
--rw-r--r--   0 james      (501) staff       (20)      402 2023-05-18 22:03:20.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/master.py
--rw-r--r--   0 james      (501) staff       (20)      850 2023-05-31 23:33:47.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/omni_sensor.py
--rw-r--r--   0 james      (501) staff       (20)      381 2023-05-18 22:03:20.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/power_profile.py
--rw-r--r--   0 james      (501) staff       (20)      141 2023-05-02 22:12:27.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/pwm_power_profile.py
--rw-r--r--   0 james      (501) staff       (20)      105 2023-06-05 20:11:50.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/qis_blind.py
--rw-r--r--   0 james      (501) staff       (20)      106 2023-06-05 20:13:05.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/qube_blind.py
--rw-r--r--   0 james      (501) staff       (20)      107 2023-06-05 20:13:14.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/relay_blind.py
--rw-r--r--   0 james      (501) staff       (20)     1551 2023-06-05 20:15:26.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/rgb_load.py
--rw-r--r--   0 james      (501) staff       (20)      151 2023-05-02 22:12:35.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/scene_point_relay.py
--rw-r--r--   0 james      (501) staff       (20)      228 2023-05-31 00:24:33.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/sensor.py
--rw-r--r--   0 james      (501) staff       (20)      227 2023-05-18 22:03:20.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/station_bus.py
--rw-r--r--   0 james      (501) staff       (20)      283 2023-05-18 22:03:20.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/station_object.py
--rw-r--r--   0 james      (501) staff       (20)      477 2023-06-05 20:31:10.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/system_object.py
--rw-r--r--   0 james      (501) staff       (20)      268 2023-05-30 20:16:11.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/task.py
--rw-r--r--   0 james      (501) staff       (20)      111 2023-05-02 22:12:53.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/temperature.py
--rw-r--r--   0 james      (501) staff       (20)      136 2023-06-05 21:16:17.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/urtsi_2_group_child.py
--rw-r--r--   0 james      (501) staff       (20)      120 2023-06-05 21:35:45.000000 aiovantage-0.1.0/src/aiovantage/config_client/objects/urtsi_2_shade_child.py
--rw-r--r--   0 james      (501) staff       (20)      721 2023-06-05 20:01:05.000000 aiovantage-0.1.0/src/aiovantage/config_client/xml_dataclass.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 02:22:59.104557 aiovantage-0.1.0/src/aiovantage/controllers/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-03-27 06:12:40.000000 aiovantage-0.1.0/src/aiovantage/controllers/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      399 2023-06-05 20:54:30.000000 aiovantage-0.1.0/src/aiovantage/controllers/areas.py
--rw-r--r--   0 james      (501) staff       (20)    10059 2023-06-05 20:29:32.000000 aiovantage-0.1.0/src/aiovantage/controllers/base.py
--rw-r--r--   0 james      (501) staff       (20)      945 2023-06-06 17:23:59.000000 aiovantage-0.1.0/src/aiovantage/controllers/blind_groups.py
--rw-r--r--   0 james      (501) staff       (20)     1206 2023-06-05 22:56:50.000000 aiovantage-0.1.0/src/aiovantage/controllers/blinds.py
--rw-r--r--   0 james      (501) staff       (20)      929 2023-06-05 20:54:12.000000 aiovantage-0.1.0/src/aiovantage/controllers/buttons.py
--rw-r--r--   0 james      (501) staff       (20)      955 2023-06-07 16:47:39.000000 aiovantage-0.1.0/src/aiovantage/controllers/dry_contacts.py
--rw-r--r--   0 james      (501) staff       (20)     2854 2023-06-05 20:54:06.000000 aiovantage-0.1.0/src/aiovantage/controllers/gmem.py
--rw-r--r--   0 james      (501) staff       (20)      593 2023-06-05 20:54:01.000000 aiovantage-0.1.0/src/aiovantage/controllers/load_groups.py
--rw-r--r--   0 james      (501) staff       (20)     1921 2023-06-05 20:53:54.000000 aiovantage-0.1.0/src/aiovantage/controllers/loads.py
--rw-r--r--   0 james      (501) staff       (20)      338 2023-06-05 19:47:50.000000 aiovantage-0.1.0/src/aiovantage/controllers/masters.py
--rw-r--r--   0 james      (501) staff       (20)     2605 2023-06-05 20:53:48.000000 aiovantage-0.1.0/src/aiovantage/controllers/omni_sensors.py
--rw-r--r--   0 james      (501) staff       (20)     4237 2023-06-05 20:53:45.000000 aiovantage-0.1.0/src/aiovantage/controllers/rgb_loads.py
--rw-r--r--   0 james      (501) staff       (20)      378 2023-06-05 19:55:09.000000 aiovantage-0.1.0/src/aiovantage/controllers/stations.py
--rw-r--r--   0 james      (501) staff       (20)     1326 2023-06-05 20:53:38.000000 aiovantage-0.1.0/src/aiovantage/controllers/tasks.py
--rw-r--r--   0 james      (501) staff       (20)      135 2023-05-25 07:35:19.000000 aiovantage-0.1.0/src/aiovantage/events.py
--rw-r--r--   0 james      (501) staff       (20)     5711 2023-05-26 20:42:31.000000 aiovantage-0.1.0/src/aiovantage/query.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 02:22:59.075976 aiovantage-0.1.0/src/aiovantage.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2285 2023-06-13 02:22:59.000000 aiovantage-0.1.0/src/aiovantage.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     4370 2023-06-13 02:22:59.000000 aiovantage-0.1.0/src/aiovantage.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-13 02:22:59.000000 aiovantage-0.1.0/src/aiovantage.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       13 2023-06-13 02:22:59.000000 aiovantage-0.1.0/src/aiovantage.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       11 2023-06-13 02:22:59.000000 aiovantage-0.1.0/src/aiovantage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.843158 aiovantage-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.811159 aiovantage-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.819158 aiovantage-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-16 06:42:00.000000 aiovantage-0.1.1/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-16 06:42:00.000000 aiovantage-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-16 06:42:00.000000 aiovantage-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-16 06:42:14.843158 aiovantage-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-16 06:42:00.000000 aiovantage-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.819158 aiovantage-0.1.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.819158 aiovantage-0.1.1/examples/areas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/areas/dump_areas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.819158 aiovantage-0.1.1/examples/blind_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/blind_groups/dump_blind_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/blinds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/blinds/dump_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/blinds/monitor_blinds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/buttons/dump_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/buttons/monitor_buttons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/command_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/command_client/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/command_client/status_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/config_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/config_client/dump_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/config_client/get_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/dry_contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/dry_contacts/dump_dry_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/dry_contacts/monitor_dry_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/dump_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/gmem/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/gmem/dump_gmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/gmem/monitor_gmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/gmem/set_gmem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/load_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/load_groups/dump_load_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/loads/
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/loads/control_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/loads/dump_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/loads/monitor_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/loads/poll_on_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/loads/toggle_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/monitor_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.823158 aiovantage-0.1.1/examples/omni_sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/omni_sensors/dump_omni_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/omni_sensors/monitor_omni_sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.827158 aiovantage-0.1.1/examples/rgb_loads/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/rgb_loads/dump_rgb_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/rgb_loads/monitor_rgb_loads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.827158 aiovantage-0.1.1/examples/stations/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/stations/dump_stations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.827158 aiovantage-0.1.1/examples/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/tasks/dump_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-16 06:42:00.000000 aiovantage-0.1.1/examples/tasks/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-16 06:42:00.000000 aiovantage-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:42:14.843158 aiovantage-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.815158 aiovantage-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.827158 aiovantage-0.1.1/src/aiovantage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.827158 aiovantage-0.1.1/src/aiovantage/command_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    29576 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.831158 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/blind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/color_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/gmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/rgb_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/interfaces/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/command_client/ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.831158 aiovantage-0.1.1/src/aiovantage/config_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.831158 aiovantage-0.1.1/src/aiovantage/config_client/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.831158 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/close_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/get_filter_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/get_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/object_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/open_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.831158 aiovantage-0.1.1/src/aiovantage/config_client/methods/introspection/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/introspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/introspection/get_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.835158 aiovantage-0.1.1/src/aiovantage/config_client/methods/login/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/methods/login/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.839158 aiovantage-0.1.1/src/aiovantage/config_client/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/anemo_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/blind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/blind_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/dc_power_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/ddg_color_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/dg_color_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/dry_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/dual_relay_station.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/eq_ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/eq_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/gmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/keypad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/light_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/load_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/location_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/omni_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/power_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/pwm_power_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/qis_blind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/qube_blind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/relay_blind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/rgb_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/scene_point_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/station_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/station_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/system_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/urtsi_2_group_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/objects/urtsi_2_shade_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/config_client/xml_dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.843158 aiovantage-0.1.1/src/aiovantage/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/areas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/blind_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/dry_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/gmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/load_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/masters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/omni_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/rgb_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/controllers/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-16 06:42:00.000000 aiovantage-0.1.1/src/aiovantage/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:42:14.827158 aiovantage-0.1.1/src/aiovantage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-16 06:42:14.000000 aiovantage-0.1.1/src/aiovantage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-16 06:42:14.000000 aiovantage-0.1.1/src/aiovantage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:42:14.000000 aiovantage-0.1.1/src/aiovantage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 06:42:14.000000 aiovantage-0.1.1/src/aiovantage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 06:42:14.000000 aiovantage-0.1.1/src/aiovantage.egg-info/top_level.txt
```

### Comparing `aiovantage-0.1.0/LICENSE` & `aiovantage-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/pyproject.toml` & `aiovantage-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
+requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiovantage"
-version = "0.1.0"
 authors = [
     {name = "James Smith", email = "james@loopj.com"},
 ]
 description = "Python module to talk to Vantage InFusion controllers."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
@@ -18,14 +17,17 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "xsdata==23.5",
 ]
+dynamic = ["version"]
+
+[tool.setuptools_scm]
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 files = "src"
 mypy_path = "src"
@@ -34,8 +36,8 @@
 explicit_package_bases = true
 implicit_reexport = true
 show_error_codes = true
 strict = true
 enable_error_code = [
     "redundant-expr",
     "truthy-bool",
-]
+]
```

### Comparing `aiovantage-0.1.0/src/aiovantage/__init__.py` & `aiovantage-0.1.1/src/aiovantage/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/command_client/__init__.py` & `aiovantage-0.1.1/src/aiovantage/command_client/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "ClientTimeoutError",
     "CommandError",
     "LoginFailedError",
     "LoginRequiredError",
 ]
 
 import asyncio
+from decimal import Decimal
 import logging
 from collections import defaultdict
 from contextlib import suppress
 from dataclasses import dataclass
 from inspect import iscoroutinefunction
 from ssl import SSLContext
 from types import TracebackType
@@ -54,15 +55,15 @@
     ClientError,
     ClientTimeoutError,
     CommandError,
     LoginFailedError,
     LoginRequiredError,
 )
 from .events import Event, EventType
-from .helpers import tokenize_response
+from .helpers import tokenize_response, encode_params
 from .ssl import create_ssl_context
 
 
 # Type aliases for callbacks for event subscriptions
 EventCallback = Union[Callable[[Event], None], Callable[[Event], Awaitable[None]]]
 EventFilter = Callable[[Event], bool]
 EventSubscription = Tuple[EventCallback, Optional[EventFilter]]
@@ -208,42 +209,42 @@
     @property
     def closed(self) -> bool:
         """Whether the connection is closed."""
 
         return self._writer is None or self._writer.is_closing()
 
     async def command(
-        self, command: str, *params: Union[int, float, str]
+        self,
+        command: str,
+        *params: Union[str, int, float, Decimal, bool],
+        force_quotes: bool = False,
     ) -> CommandResponse:
         """
         Send a command with parameters to the Host Command service and wait for a
         response.
 
         Handles encoding the parameters correctly, and raises an exception if the
         response line is R:ERROR.
 
         Args:
             command: The command to send, should be a single word string.
-            params: The parameters to send with the command, int, float, or str.
+            params: The parameters to send with the command.
+            force_quotes: Whether to force string params to be wrapped in double quotes.
 
         Returns:
             A CommandResponse instance.
         """
 
         # Make sure we're connected
         if self._writer is None or self._writer.is_closing():
             raise ClientConnectionError("Not connected to Vantage Host Command service")
 
-        # Validate parameters
-        if not all(isinstance(param, (int, float, str)) for param in params):
-            raise TypeError("Command parameters must be int, float, or str")
-
         # Build the request string, encoding the parameters if necessary
         if params:
-            request = f"{command} {' '.join([str(p) for p in params])}"
+            request = f"{command} {encode_params(*params, force_quotes=force_quotes)}"
         else:
             request = command
 
         # Send the request and wait for the response as a single transaction
         async with self._command_lock:
             # Send the request
             try:
@@ -470,33 +471,37 @@
             self._event_handler_task = None
 
         # Close the connections
         if self._connection is not None:
             self._connection.close()
 
     async def command(
-        self, command: str, *params: Union[int, float, str]
+        self,
+        command: str,
+        *params: Union[str, int, float, Decimal, bool],
+        force_quotes: bool = False,
     ) -> CommandResponse:
         """
         Send a command with parameters to the Host Command service and wait for a
         response.
 
         Handles encoding the parameters correctly, and raises an exception if the
         response line is R:ERROR.
 
         Args:
             command: The command to send, should be a single word string.
-            params: The parameters to send with the command, int, float, or str.
+            params: The parameters to send with the command.
+            force_quotes: Whether to force string params to be wrapped in double quotes.
 
         Returns:
             A CommandResponse instance.
         """
 
         conn = await self.connection()
-        return await conn.command(command, *params)
+        return await conn.command(command, *params, force_quotes=force_quotes)
 
     def subscribe(
         self,
         callback: EventCallback,
         event_filter: Union[EventType, Iterable[EventType], EventFilter, None] = None,
     ) -> Callable[[], None]:
         """
```

### Comparing `aiovantage-0.1.0/src/aiovantage/command_client/errors.py` & `aiovantage-0.1.1/src/aiovantage/command_client/errors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/command_client/events.py` & `aiovantage-0.1.1/src/aiovantage/command_client/events.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/command_client/interfaces/__init__.py` & `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from .blind import BlindInterface
 from .button import ButtonInterface
 from .color_temperature import ColorTemperatureInterface
+from .gmem import GMemInterface
 from .introspection import IntrospectionInterface
 from .load import LoadInterface
 from .object import ObjectInterface
 from .rgb_load import RGBLoadInterface
 from .sensor import SensorInterface
 from .task import TaskInterface
 
 __all__ = [
     "BlindInterface",
     "ButtonInterface",
     "ColorTemperatureInterface",
+    "GMemInterface",
     "IntrospectionInterface",
     "LoadInterface",
     "ObjectInterface",
     "RGBLoadInterface",
     "SensorInterface",
     "TaskInterface",
 ]
```

### Comparing `aiovantage-0.1.0/src/aiovantage/command_client/interfaces/blind.py` & `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/command_client/interfaces/button.py` & `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/command_client/interfaces/color_temperature.py` & `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/color_temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/command_client/interfaces/load.py` & `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/command_client/interfaces/object.py` & `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/command_client/interfaces/rgb_load.py` & `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/command_client/interfaces/sensor.py` & `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/command_client/interfaces/task.py` & `aiovantage-0.1.1/src/aiovantage/command_client/interfaces/task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/__init__.py` & `aiovantage-0.1.1/src/aiovantage/config_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/helpers.py` & `aiovantage-0.1.1/src/aiovantage/config_client/helpers.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py` & `aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/get_filter_results.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/methods/configuration/get_object.py` & `aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/get_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/methods/configuration/object_choice.py` & `aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/object_choice.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/methods/configuration/open_filter.py` & `aiovantage-0.1.1/src/aiovantage/config_client/methods/configuration/open_filter.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/methods/introspection/get_version.py` & `aiovantage-0.1.1/src/aiovantage/config_client/methods/introspection/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/objects/__init__.py` & `aiovantage-0.1.1/src/aiovantage/config_client/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/objects/blind.py` & `aiovantage-0.1.1/src/aiovantage/config_client/objects/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/objects/button.py` & `aiovantage-0.1.1/src/aiovantage/config_client/objects/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/objects/load.py` & `aiovantage-0.1.1/src/aiovantage/config_client/objects/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/objects/omni_sensor.py` & `aiovantage-0.1.1/src/aiovantage/config_client/objects/omni_sensor.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         @dataclass
         class Formula:
             return_type: str = xml_attribute("ReturnType")
             level_type: str = xml_attribute("LevelType")
 
         formula: Formula = xml_element("Formula")
         method: str = xml_element("Method")
+        method_hw: str = xml_element("MethodHW")
 
     get: GetMethodType = xml_element("Get")
     parent_id: int = xml_element("Parent")
 
     @property
     def is_current_sensor(self) -> bool:
         return self.model == "Current"
```

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/objects/rgb_load.py` & `aiovantage-0.1.1/src/aiovantage/config_client/objects/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/config_client/xml_dataclass.py` & `aiovantage-0.1.1/src/aiovantage/config_client/xml_dataclass.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 def xml_element(name: str, **kwargs: Any) -> Any:
     metadata = {}
     metadata.update(kwargs.pop("metadata", {}))
     metadata.update({"name": name, "type": "Element"})
 
     return field(metadata=metadata, **kwargs)
 
+def xml_text(**kwargs: Any) -> Any:
+    metadata = {}
+    metadata.update(kwargs.pop("metadata", {}))
+    metadata.update({"type": "Text"})
+
+    return field(metadata=metadata, **kwargs)
 
 def xml_tag_from_class(cls: Type[Any]) -> str:
     """Get the XML tag name for a class."""
 
     meta = cls.Meta if "Meta" in cls.__dict__ else None
     name = getattr(meta, "name", cls.__qualname__)
```

### Comparing `aiovantage-0.1.0/src/aiovantage/controllers/base.py` & `aiovantage-0.1.1/src/aiovantage/controllers/base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/controllers/blind_groups.py` & `aiovantage-0.1.1/src/aiovantage/controllers/blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/controllers/blinds.py` & `aiovantage-0.1.1/src/aiovantage/controllers/blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/controllers/buttons.py` & `aiovantage-0.1.1/src/aiovantage/controllers/buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/controllers/dry_contacts.py` & `aiovantage-0.1.1/src/aiovantage/controllers/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/controllers/load_groups.py` & `aiovantage-0.1.1/src/aiovantage/controllers/load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/controllers/loads.py` & `aiovantage-0.1.1/src/aiovantage/controllers/loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/controllers/omni_sensors.py` & `aiovantage-0.1.1/src/aiovantage/controllers/omni_sensors.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,32 +32,33 @@
             return
 
         state: Dict[str, Any] = {}
         state["level"] = self.parse_get_level_status(omni_sensor, args)
 
         self.update_state(id, state)
 
-    async def get_level(self, id: int) -> Union[int, Decimal]:
+    async def get_level(self, id: int, cached: bool = False) -> Union[int, Decimal]:
         """
         Get the level of an OmniSensor.
 
         Args:
             id: The ID of the sensor.
 
         Returns:
             The level of the sensor.
         """
 
         omni_sensor: OmniSensor = self[id]
 
+        # Figure out which get method to use, hardware or software (cached)
+        method = omni_sensor.get.method if cached else omni_sensor.get.method_hw
+
         # INVOKE <id> <method>
         # -> R:INVOKE <id> <value> <method>
-        response = await self.command_client.command(
-            "INVOKE", id, omni_sensor.get.method
-        )
+        response = await self.command_client.command("INVOKE", id, method)
 
         # Convert the level to the correct type
         if omni_sensor.get.formula.return_type == "fixed":
             level = Decimal(response.args[1])
             if omni_sensor.get.formula.level_type == "fixed":
                 return level
             else:
```

### Comparing `aiovantage-0.1.0/src/aiovantage/controllers/rgb_loads.py` & `aiovantage-0.1.1/src/aiovantage/controllers/rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/controllers/tasks.py` & `aiovantage-0.1.1/src/aiovantage/controllers/tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.1.0/src/aiovantage/query.py` & `aiovantage-0.1.1/src/aiovantage/query.py`

 * *Files identical despite different names*

