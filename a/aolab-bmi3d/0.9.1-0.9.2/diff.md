# Comparing `tmp/aolab-bmi3d-0.9.1.tar.gz` & `tmp/aolab-bmi3d-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aolab-bmi3d-0.9.1.tar", last modified: Fri Jun 16 19:33:20 2023, max compression
+gzip compressed data, was "aolab-bmi3d-0.9.2.tar", last modified: Fri Jun 16 20:31:04 2023, max compression
```

## Comparing `aolab-bmi3d-0.9.1.tar` & `aolab-bmi3d-0.9.2.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.604369 aolab-bmi3d-0.9.1/
--rw-r--r--   0 leoscholl   (501) staff       (20)      654 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/LICENSE
--rw-r--r--   0 leoscholl   (501) staff       (20)      247 2023-06-16 19:33:20.604219 aolab-bmi3d-0.9.1/PKG-INFO
--rw-r--r--   0 leoscholl   (501) staff       (20)     6233 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/README.md
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.575526 aolab-bmi3d-0.9.1/analysis/
--rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/analysis/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8291 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/analysis/bmi_reconstruction.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    22341 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/analysis/fa_decomp.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4269 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/analysis/performance_metrics.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    38432 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/analysis/target_capture_task_analysis.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.576247 aolab-bmi3d-0.9.1/aolab_bmi3d.egg-info/
--rw-r--r--   0 leoscholl   (501) staff       (20)      247 2023-06-16 19:33:20.000000 aolab-bmi3d-0.9.1/aolab_bmi3d.egg-info/PKG-INFO
--rw-r--r--   0 leoscholl   (501) staff       (20)     5546 2023-06-16 19:33:20.000000 aolab-bmi3d-0.9.1/aolab_bmi3d.egg-info/SOURCES.txt
--rw-r--r--   0 leoscholl   (501) staff       (20)        1 2023-06-16 19:33:20.000000 aolab-bmi3d-0.9.1/aolab_bmi3d.egg-info/dependency_links.txt
--rw-r--r--   0 leoscholl   (501) staff       (20)      129 2023-06-16 19:33:20.000000 aolab-bmi3d-0.9.1/aolab_bmi3d.egg-info/requires.txt
--rw-r--r--   0 leoscholl   (501) staff       (20)       62 2023-06-16 19:33:20.000000 aolab-bmi3d-0.9.1/aolab_bmi3d.egg-info/top_level.txt
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.577369 aolab-bmi3d-0.9.1/built_in_tasks/
--rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/built_in_tasks/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    13365 2023-01-06 22:04:22.000000 aolab-bmi3d-0.9.1/built_in_tasks/bmimultitasks.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     9374 2023-04-26 23:40:00.000000 aolab-bmi3d-0.9.1/built_in_tasks/manualcontrolmultitasks.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    10869 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.1/built_in_tasks/othertasks.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     6558 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/built_in_tasks/passivetasks.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    29694 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/built_in_tasks/target_capture_task.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     6763 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/built_in_tasks/target_graphics.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    47091 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.1/built_in_tasks/target_tracking_task.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.577807 aolab-bmi3d-0.9.1/config/
--rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/config/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     1990 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/config/bmiconfig.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.579259 aolab-bmi3d-0.9.1/db/
--rw-r--r--   0 leoscholl   (501) staff       (20)      146 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     1452 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/add_blackrock_datafiles_to_entry.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      680 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/boot_django.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      861 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/cleanup.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2286 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/compile_backup_list.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     7412 2023-06-16 18:01:15.000000 aolab-bmi3d-0.9.1/db/db_settings.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    47146 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.1/db/dbfunctions.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      497 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/maintenance.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4042 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/migrate_db.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      454 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/subclassdict.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.581149 aolab-bmi3d-0.9.1/db/tracker/
--rw-r--r--   0 leoscholl   (501) staff       (20)      229 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      841 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/admin.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    24138 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/ajax.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      128 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/apps.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      805 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/celery.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     5802 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/cloud.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     6188 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/dbq.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      135 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/exp_tracker.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      307 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/jinja2.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8346 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/json_param.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.582581 aolab-bmi3d-0.9.1/db/tracker/migrations/
--rw-r--r--   0 leoscholl   (501) staff       (20)     6078 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/migrations/0001_initial.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     1668 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/migrations/0002_auto_20191112_2306.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      662 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/migrations/0003_auto_20191113_2158.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      553 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/migrations/0004_keyvaluestore.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      410 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/migrations/0005_taskentry_sw_version.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      419 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/migrations/0006_datafile_backup_status.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      408 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/migrations/0007_taskentry_template.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      386 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/migrations/0008_taskentry_metadata.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      387 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/migrations/0009_auto_20210630_1019.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      520 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/migrations/0010_experimenter.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      915 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/migrations/0011_auto_20211017_1548.py
--rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/migrations/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    65059 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.1/db/tracker/models.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     6311 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/tasktrack.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    11590 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/trainbmi.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     9897 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/views.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     5969 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/db/tracker/websocket.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3933 2023-01-11 16:50:49.000000 aolab-bmi3d-0.9.1/db/urls.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.585718 aolab-bmi3d-0.9.1/features/
--rw-r--r--   0 leoscholl   (501) staff       (20)     3048 2023-01-11 16:50:49.000000 aolab-bmi3d-0.9.1/features/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    14392 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/arduino_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8342 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/blackrock_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8409 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/bmi_task_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      303 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/debug_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    13167 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.1/features/ecube_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     6057 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/eyetracker_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     9052 2023-04-26 23:40:00.000000 aolab-bmi3d-0.9.1/features/generator_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3163 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/hdf_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2326 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/kinarm_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    11375 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.1/features/laser_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2820 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/neural_sys_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8780 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/optitrack_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8274 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/peripheral_device_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4718 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/phasespace_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     7232 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/plexon_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    18069 2023-03-06 19:10:15.000000 aolab-bmi3d-0.9.1/features/reward_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     1894 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/serial_port_sensor.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    16758 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/simulation_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    14924 2023-04-26 23:40:00.000000 aolab-bmi3d-0.9.1/features/sync_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2310 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/touch_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4694 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.1/features/video_recording_features.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.589565 aolab-bmi3d-0.9.1/riglib/
--rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2908 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/arduino_imu.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2832 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/arduino_joystick.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.589832 aolab-bmi3d-0.9.1/riglib/audio/
--rw-r--r--   0 leoscholl   (501) staff       (20)       20 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/audio/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      385 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/audio/audio.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.590348 aolab-bmi3d-0.9.1/riglib/blackrock/
--rw-r--r--   0 leoscholl   (501) staff       (20)     1844 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/blackrock/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2721 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/blackrock/brMiscFxns.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    69366 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/blackrock/brpylib.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     6310 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/blackrock/cerelink.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.593359 aolab-bmi3d-0.9.1/riglib/bmi/
--rw-r--r--   0 leoscholl   (501) staff       (20)      171 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3578 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/accumulator.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     5618 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/assist.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    57517 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/bmi.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    43588 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/clda.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    58426 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/extractor.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    13443 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/feedback_controllers.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    13325 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/goal_calculators.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    30472 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/kfdecoder.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    18908 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/kfdecoder_fcns.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8234 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/lindecoder.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8558 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/onedim_lfp_decoder.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    16229 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/ppfdecoder.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    21222 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/rat_bmi_decoder.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    23189 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/robot_arms.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    32580 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/sim_neurons.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4399 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/sskfdecoder.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    16905 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/state_space_models.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    54922 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/bmi/train.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2002 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/button.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     6997 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/calibrations.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.593684 aolab-bmi3d-0.9.1/riglib/dio/
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.594058 aolab-bmi3d-0.9.1/riglib/dio/NIUSB6501/
--rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/dio/NIUSB6501/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3002 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/dio/NIUSB6501/control_comedi_swig.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4616 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/dio/NIUSB6501/py_comedi_control.py
--rw-r--r--   0 leoscholl   (501) staff       (20)        2 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/dio/__init__.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.594193 aolab-bmi3d-0.9.1/riglib/dio/nidaq/
--rw-r--r--   0 leoscholl   (501) staff       (20)     4839 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/dio/nidaq/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     5695 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/dio/parse.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     7951 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/e3vision.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.594873 aolab-bmi3d-0.9.1/riglib/ecube/
--rw-r--r--   0 leoscholl   (501) staff       (20)    18697 2023-04-26 23:40:00.000000 aolab-bmi3d-0.9.1/riglib/ecube/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     1613 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/ecube/file.py
--rwxr-xr-x   0 leoscholl   (501) staff       (20)    25667 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/ecube/pyeCubeStream.py
--rw-r--r--   0 leoscholl   (501) staff       (20)       68 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/ecube/spikes.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      360 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/ecube/utils.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.595879 aolab-bmi3d-0.9.1/riglib/experiment/
--rw-r--r--   0 leoscholl   (501) staff       (20)     2511 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/experiment/Pygame.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3231 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/experiment/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    32917 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.1/riglib/experiment/experiment.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3745 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/experiment/generate.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     6210 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/experiment/mocks.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2290 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/experiment/report.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     6580 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/experiment/task_wrapper.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4831 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/eyetracker.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     1459 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/filter.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.596186 aolab-bmi3d-0.9.1/riglib/fsm/
--rw-r--r--   0 leoscholl   (501) staff       (20)       72 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/fsm/__init__.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.596449 aolab-bmi3d-0.9.1/riglib/fsm/fsm/
--rw-r--r--   0 leoscholl   (501) staff       (20)       68 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/fsm/fsm/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    12237 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/fsm/fsm/fsm.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      467 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/fsm/setup.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     9089 2023-01-11 16:50:49.000000 aolab-bmi3d-0.9.1/riglib/gpio.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.596738 aolab-bmi3d-0.9.1/riglib/hdfwriter/
--rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/hdfwriter/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4026 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/hdfwriter/hdfwriter.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     1720 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/kinarmdata.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3146 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/kinarmsocket.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3255 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/master8stimulation.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     6887 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/motiontracker.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     6412 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/mp_calc.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    10149 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/mp_proxy.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.597490 aolab-bmi3d-0.9.1/riglib/optitrack_client/
--rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/optitrack_client/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     5033 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/optitrack_client/optitrack.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4930 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/optitrack_client/optitrack_interface_sijia.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2758 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/phidgets.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    19014 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/plants.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.597801 aolab-bmi3d-0.9.1/riglib/positioner/
--rw-r--r--   0 leoscholl   (501) staff       (20)    21603 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/positioner/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     1617 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/positioner/calib.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     7080 2023-01-11 16:50:49.000000 aolab-bmi3d-0.9.1/riglib/qwalor_laser.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2588 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/reward.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    11589 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/reward_crist.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4827 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/serial_dio.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      696 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/singleton.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4796 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/sink.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    22775 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/source.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.599192 aolab-bmi3d-0.9.1/riglib/stereo_opengl/
--rw-r--r--   0 leoscholl   (501) staff       (20)      167 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2399 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/environment.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    29919 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/ik.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    10855 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/models.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    14712 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/primitives.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.599994 aolab-bmi3d-0.9.1/riglib/stereo_opengl/render/
--rw-r--r--   0 leoscholl   (501) staff       (20)       93 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/render/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4515 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/render/fbo.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     6112 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/render/render.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4370 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/render/shader.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3082 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/render/ssao.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     5059 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/render/stereo.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3440 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/textures.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3093 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/utils.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    16993 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/window.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8259 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stereo_opengl/xfm.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      954 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/stimulus_pulse.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     1391 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/tablet_reward.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2478 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/riglib/touch_data.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.602029 aolab-bmi3d-0.9.1/robot/
--rw-r--r--   0 leoscholl   (501) staff       (20)    12170 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/Link.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    12789 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/Quaternion.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     6019 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/Robot.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     8978 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/SerialLink.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      282 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    14000 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/dynamics.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3155 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/jacobian.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    11506 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/kinematics.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2312 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/manipulability.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     2736 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/parsedemo.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    16411 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/plot.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3416 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/trajectory.py
--rw-r--r--   0 leoscholl   (501) staff       (20)    19266 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/transform.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3466 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/robot/utility.py
--rw-r--r--   0 leoscholl   (501) staff       (20)       38 2023-06-16 19:33:20.604413 aolab-bmi3d-0.9.1/setup.cfg
--rw-r--r--   0 leoscholl   (501) staff       (20)      679 2023-06-16 19:33:09.000000 aolab-bmi3d-0.9.1/setup.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.602851 aolab-bmi3d-0.9.1/tests/
--rw-r--r--   0 leoscholl   (501) staff       (20)     9315 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/tests/test_decoders.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3504 2023-01-11 22:17:33.000000 aolab-bmi3d-0.9.1/tests/test_ecube.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     5509 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/tests/test_features.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3583 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.1/tests/test_qwalor_laser.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     1240 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/tests/test_reward.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3797 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/tests/test_tasks.py
-drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 19:33:20.604026 aolab-bmi3d-0.9.1/utils/
--rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/utils/__init__.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     1176 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/utils/angle_utils.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      241 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/utils/constants.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      820 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/utils/drawbox.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     3175 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/utils/fixpaths.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      737 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/utils/make_autoalign.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     4315 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/utils/reassociate.py
--rw-r--r--   0 leoscholl   (501) staff       (20)     1632 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/utils/ringbuffer.py
--rw-r--r--   0 leoscholl   (501) staff       (20)      563 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.1/utils/util_fns.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.499649 aolab-bmi3d-0.9.2/
+-rw-r--r--   0 leoscholl   (501) staff       (20)      654 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/LICENSE
+-rw-r--r--   0 leoscholl   (501) staff       (20)      247 2023-06-16 20:31:04.499468 aolab-bmi3d-0.9.2/PKG-INFO
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6233 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/README.md
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.469616 aolab-bmi3d-0.9.2/analysis/
+-rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/analysis/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8291 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/analysis/bmi_reconstruction.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    22341 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/analysis/fa_decomp.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4269 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/analysis/performance_metrics.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    38432 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/analysis/target_capture_task_analysis.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.470277 aolab-bmi3d-0.9.2/aolab_bmi3d.egg-info/
+-rw-r--r--   0 leoscholl   (501) staff       (20)      247 2023-06-16 20:31:04.000000 aolab-bmi3d-0.9.2/aolab_bmi3d.egg-info/PKG-INFO
+-rw-r--r--   0 leoscholl   (501) staff       (20)     5546 2023-06-16 20:31:04.000000 aolab-bmi3d-0.9.2/aolab_bmi3d.egg-info/SOURCES.txt
+-rw-r--r--   0 leoscholl   (501) staff       (20)        1 2023-06-16 20:31:04.000000 aolab-bmi3d-0.9.2/aolab_bmi3d.egg-info/dependency_links.txt
+-rw-r--r--   0 leoscholl   (501) staff       (20)      129 2023-06-16 20:31:04.000000 aolab-bmi3d-0.9.2/aolab_bmi3d.egg-info/requires.txt
+-rw-r--r--   0 leoscholl   (501) staff       (20)       62 2023-06-16 20:31:04.000000 aolab-bmi3d-0.9.2/aolab_bmi3d.egg-info/top_level.txt
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.471278 aolab-bmi3d-0.9.2/built_in_tasks/
+-rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/built_in_tasks/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    13365 2023-01-06 22:04:22.000000 aolab-bmi3d-0.9.2/built_in_tasks/bmimultitasks.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     9374 2023-04-26 23:40:00.000000 aolab-bmi3d-0.9.2/built_in_tasks/manualcontrolmultitasks.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    10869 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.2/built_in_tasks/othertasks.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6558 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/built_in_tasks/passivetasks.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    29694 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/built_in_tasks/target_capture_task.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6763 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/built_in_tasks/target_graphics.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    47091 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.2/built_in_tasks/target_tracking_task.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.471741 aolab-bmi3d-0.9.2/config/
+-rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/config/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1990 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/config/bmiconfig.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.473208 aolab-bmi3d-0.9.2/db/
+-rw-r--r--   0 leoscholl   (501) staff       (20)      146 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1452 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/add_blackrock_datafiles_to_entry.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      680 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/boot_django.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      861 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/cleanup.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2286 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/compile_backup_list.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     7432 2023-06-16 20:30:44.000000 aolab-bmi3d-0.9.2/db/db_settings.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    47146 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.2/db/dbfunctions.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      497 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/maintenance.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4042 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/migrate_db.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      454 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/subclassdict.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.475492 aolab-bmi3d-0.9.2/db/tracker/
+-rw-r--r--   0 leoscholl   (501) staff       (20)      229 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      841 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/admin.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    24138 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/ajax.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      128 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/apps.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      805 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/celery.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     5802 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/cloud.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6188 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/dbq.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      135 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/exp_tracker.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      307 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/jinja2.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8346 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/json_param.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.477033 aolab-bmi3d-0.9.2/db/tracker/migrations/
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6078 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/migrations/0001_initial.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1668 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/migrations/0002_auto_20191112_2306.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      662 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/migrations/0003_auto_20191113_2158.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      553 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/migrations/0004_keyvaluestore.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      410 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/migrations/0005_taskentry_sw_version.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      419 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/migrations/0006_datafile_backup_status.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      408 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/migrations/0007_taskentry_template.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      386 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/migrations/0008_taskentry_metadata.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      387 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/migrations/0009_auto_20210630_1019.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      520 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/migrations/0010_experimenter.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      915 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/migrations/0011_auto_20211017_1548.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/migrations/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    65059 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.2/db/tracker/models.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6311 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/tasktrack.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    11590 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/trainbmi.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     9897 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/views.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     5969 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/db/tracker/websocket.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3933 2023-01-11 16:50:49.000000 aolab-bmi3d-0.9.2/db/urls.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.480102 aolab-bmi3d-0.9.2/features/
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3048 2023-01-11 16:50:49.000000 aolab-bmi3d-0.9.2/features/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    14392 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/arduino_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8342 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/blackrock_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8409 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/bmi_task_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      303 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/debug_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    13167 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.2/features/ecube_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6057 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/eyetracker_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     9052 2023-04-26 23:40:00.000000 aolab-bmi3d-0.9.2/features/generator_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3163 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/hdf_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2326 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/kinarm_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    11375 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.2/features/laser_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2820 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/neural_sys_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8780 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/optitrack_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8274 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/peripheral_device_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4718 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/phasespace_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     7232 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/plexon_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    18069 2023-03-06 19:10:15.000000 aolab-bmi3d-0.9.2/features/reward_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1894 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/serial_port_sensor.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    16758 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/simulation_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    14924 2023-04-26 23:40:00.000000 aolab-bmi3d-0.9.2/features/sync_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2310 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/touch_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4694 2022-12-15 00:21:24.000000 aolab-bmi3d-0.9.2/features/video_recording_features.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.484084 aolab-bmi3d-0.9.2/riglib/
+-rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2908 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/arduino_imu.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2832 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/arduino_joystick.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.484318 aolab-bmi3d-0.9.2/riglib/audio/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       20 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/audio/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      385 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/audio/audio.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.484857 aolab-bmi3d-0.9.2/riglib/blackrock/
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1844 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/blackrock/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2721 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/blackrock/brMiscFxns.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    69366 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/blackrock/brpylib.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6310 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/blackrock/cerelink.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.489152 aolab-bmi3d-0.9.2/riglib/bmi/
+-rw-r--r--   0 leoscholl   (501) staff       (20)      171 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3578 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/accumulator.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     5618 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/assist.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    57517 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/bmi.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    43588 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/clda.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    58426 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/extractor.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    13443 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/feedback_controllers.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    13325 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/goal_calculators.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    30472 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/kfdecoder.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    18908 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/kfdecoder_fcns.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8234 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/lindecoder.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8558 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/onedim_lfp_decoder.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    16229 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/ppfdecoder.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    21222 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/rat_bmi_decoder.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    23189 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/robot_arms.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    32580 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/sim_neurons.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4399 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/sskfdecoder.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    16905 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/state_space_models.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    54922 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/bmi/train.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2002 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/button.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6997 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/calibrations.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.489626 aolab-bmi3d-0.9.2/riglib/dio/
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.490412 aolab-bmi3d-0.9.2/riglib/dio/NIUSB6501/
+-rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/dio/NIUSB6501/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3002 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/dio/NIUSB6501/control_comedi_swig.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4616 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/dio/NIUSB6501/py_comedi_control.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)        2 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/dio/__init__.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.490612 aolab-bmi3d-0.9.2/riglib/dio/nidaq/
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4839 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/dio/nidaq/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     5695 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/dio/parse.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     7951 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/e3vision.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.491322 aolab-bmi3d-0.9.2/riglib/ecube/
+-rw-r--r--   0 leoscholl   (501) staff       (20)    18697 2023-04-26 23:40:00.000000 aolab-bmi3d-0.9.2/riglib/ecube/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1613 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/ecube/file.py
+-rwxr-xr-x   0 leoscholl   (501) staff       (20)    25667 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/ecube/pyeCubeStream.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)       68 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/ecube/spikes.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      360 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/ecube/utils.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.492222 aolab-bmi3d-0.9.2/riglib/experiment/
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2511 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/experiment/Pygame.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3231 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/experiment/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    32917 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.2/riglib/experiment/experiment.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3745 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/experiment/generate.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6210 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/experiment/mocks.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2290 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/experiment/report.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6580 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/experiment/task_wrapper.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4831 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/eyetracker.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1459 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/filter.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.492461 aolab-bmi3d-0.9.2/riglib/fsm/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       72 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/fsm/__init__.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.492728 aolab-bmi3d-0.9.2/riglib/fsm/fsm/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       68 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/fsm/fsm/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    12237 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/fsm/fsm/fsm.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      467 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/fsm/setup.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     9089 2023-01-11 16:50:49.000000 aolab-bmi3d-0.9.2/riglib/gpio.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.492961 aolab-bmi3d-0.9.2/riglib/hdfwriter/
+-rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/hdfwriter/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4026 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/hdfwriter/hdfwriter.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1720 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/kinarmdata.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3146 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/kinarmsocket.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3255 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/master8stimulation.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6887 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/motiontracker.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6412 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/mp_calc.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    10149 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/mp_proxy.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.493323 aolab-bmi3d-0.9.2/riglib/optitrack_client/
+-rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/optitrack_client/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     5033 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/optitrack_client/optitrack.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4930 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/optitrack_client/optitrack_interface_sijia.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2758 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/phidgets.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    19014 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/plants.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.493627 aolab-bmi3d-0.9.2/riglib/positioner/
+-rw-r--r--   0 leoscholl   (501) staff       (20)    21603 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/positioner/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1617 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/positioner/calib.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     7080 2023-01-11 16:50:49.000000 aolab-bmi3d-0.9.2/riglib/qwalor_laser.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2588 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/reward.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    11589 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/reward_crist.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4827 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/serial_dio.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      696 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/singleton.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4796 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/sink.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    22775 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/source.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.494796 aolab-bmi3d-0.9.2/riglib/stereo_opengl/
+-rw-r--r--   0 leoscholl   (501) staff       (20)      167 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2399 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/environment.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    29919 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/ik.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    10855 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/models.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    14712 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/primitives.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.495549 aolab-bmi3d-0.9.2/riglib/stereo_opengl/render/
+-rw-r--r--   0 leoscholl   (501) staff       (20)       93 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/render/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4515 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/render/fbo.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6112 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/render/render.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4370 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/render/shader.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3082 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/render/ssao.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     5059 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/render/stereo.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3440 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/textures.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3093 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/utils.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    16993 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/window.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8259 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stereo_opengl/xfm.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      954 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/stimulus_pulse.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1391 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/tablet_reward.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2478 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/riglib/touch_data.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.497355 aolab-bmi3d-0.9.2/robot/
+-rw-r--r--   0 leoscholl   (501) staff       (20)    12170 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/Link.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    12789 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/Quaternion.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     6019 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/Robot.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     8978 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/SerialLink.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      282 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    14000 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/dynamics.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3155 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/jacobian.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    11506 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/kinematics.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2312 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/manipulability.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     2736 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/parsedemo.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    16411 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/plot.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3416 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/trajectory.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)    19266 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/transform.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3466 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/robot/utility.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)       38 2023-06-16 20:31:04.499689 aolab-bmi3d-0.9.2/setup.cfg
+-rw-r--r--   0 leoscholl   (501) staff       (20)      679 2023-06-16 20:30:58.000000 aolab-bmi3d-0.9.2/setup.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.498208 aolab-bmi3d-0.9.2/tests/
+-rw-r--r--   0 leoscholl   (501) staff       (20)     9315 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/tests/test_decoders.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3504 2023-01-11 22:17:33.000000 aolab-bmi3d-0.9.2/tests/test_ecube.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     5509 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/tests/test_features.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3583 2023-06-16 18:00:48.000000 aolab-bmi3d-0.9.2/tests/test_qwalor_laser.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1240 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/tests/test_reward.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3797 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/tests/test_tasks.py
+drwxr-xr-x   0 leoscholl   (501) staff       (20)        0 2023-06-16 20:31:04.499235 aolab-bmi3d-0.9.2/utils/
+-rw-r--r--   0 leoscholl   (501) staff       (20)        0 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/utils/__init__.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1176 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/utils/angle_utils.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      241 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/utils/constants.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      820 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/utils/drawbox.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     3175 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/utils/fixpaths.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      737 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/utils/make_autoalign.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     4315 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/utils/reassociate.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)     1632 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/utils/ringbuffer.py
+-rw-r--r--   0 leoscholl   (501) staff       (20)      563 2022-12-15 00:21:25.000000 aolab-bmi3d-0.9.2/utils/util_fns.py
```

### Comparing `aolab-bmi3d-0.9.1/LICENSE` & `aolab-bmi3d-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/README.md` & `aolab-bmi3d-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/analysis/bmi_reconstruction.py` & `aolab-bmi3d-0.9.2/analysis/bmi_reconstruction.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/analysis/fa_decomp.py` & `aolab-bmi3d-0.9.2/analysis/fa_decomp.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/analysis/performance_metrics.py` & `aolab-bmi3d-0.9.2/analysis/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/analysis/target_capture_task_analysis.py` & `aolab-bmi3d-0.9.2/analysis/target_capture_task_analysis.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/aolab_bmi3d.egg-info/SOURCES.txt` & `aolab-bmi3d-0.9.2/aolab_bmi3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/built_in_tasks/bmimultitasks.py` & `aolab-bmi3d-0.9.2/built_in_tasks/bmimultitasks.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/built_in_tasks/manualcontrolmultitasks.py` & `aolab-bmi3d-0.9.2/built_in_tasks/manualcontrolmultitasks.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/built_in_tasks/othertasks.py` & `aolab-bmi3d-0.9.2/built_in_tasks/othertasks.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/built_in_tasks/passivetasks.py` & `aolab-bmi3d-0.9.2/built_in_tasks/passivetasks.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/built_in_tasks/target_capture_task.py` & `aolab-bmi3d-0.9.2/built_in_tasks/target_capture_task.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/built_in_tasks/target_graphics.py` & `aolab-bmi3d-0.9.2/built_in_tasks/target_graphics.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/built_in_tasks/target_tracking_task.py` & `aolab-bmi3d-0.9.2/built_in_tasks/target_tracking_task.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/config/bmiconfig.py` & `aolab-bmi3d-0.9.2/config/bmiconfig.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/add_blackrock_datafiles_to_entry.py` & `aolab-bmi3d-0.9.2/db/add_blackrock_datafiles_to_entry.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/boot_django.py` & `aolab-bmi3d-0.9.2/db/boot_django.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/cleanup.py` & `aolab-bmi3d-0.9.2/db/cleanup.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/compile_backup_list.py` & `aolab-bmi3d-0.9.2/db/compile_backup_list.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/db_settings.py` & `aolab-bmi3d-0.9.2/db/db_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import glob
 import re
 import socket
 import json
 from django.core.exceptions import ImproperlyConfigured
 
 BASE_DIR = os.path.abspath(os.path.dirname(__file__))
-CONFIG_DIR = os.path.join('~', '.config', 'bmi3d')
+CONFIG_DIR = os.path.join(os.path.expanduser("~"), '.config', 'bmi3d')
 HOSTNAME = socket.gethostname()
 
 def get_sqlite3_databases():
     dbs = dict()
     db_files = glob.glob(os.path.join(BASE_DIR, '*.sql'))
     for db in db_files:
         db_name_re = re.match('db(.*?).sql', os.path.basename(db))
```

### Comparing `aolab-bmi3d-0.9.1/db/dbfunctions.py` & `aolab-bmi3d-0.9.2/db/dbfunctions.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/migrate_db.py` & `aolab-bmi3d-0.9.2/db/migrate_db.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/admin.py` & `aolab-bmi3d-0.9.2/db/tracker/admin.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/ajax.py` & `aolab-bmi3d-0.9.2/db/tracker/ajax.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/celery.py` & `aolab-bmi3d-0.9.2/db/tracker/celery.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/cloud.py` & `aolab-bmi3d-0.9.2/db/tracker/cloud.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/dbq.py` & `aolab-bmi3d-0.9.2/db/tracker/dbq.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/json_param.py` & `aolab-bmi3d-0.9.2/db/tracker/json_param.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/migrations/0001_initial.py` & `aolab-bmi3d-0.9.2/db/tracker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/migrations/0002_auto_20191112_2306.py` & `aolab-bmi3d-0.9.2/db/tracker/migrations/0002_auto_20191112_2306.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/migrations/0003_auto_20191113_2158.py` & `aolab-bmi3d-0.9.2/db/tracker/migrations/0003_auto_20191113_2158.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/migrations/0004_keyvaluestore.py` & `aolab-bmi3d-0.9.2/db/tracker/migrations/0004_keyvaluestore.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/migrations/0010_experimenter.py` & `aolab-bmi3d-0.9.2/db/tracker/migrations/0010_experimenter.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/migrations/0011_auto_20211017_1548.py` & `aolab-bmi3d-0.9.2/db/tracker/migrations/0011_auto_20211017_1548.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/models.py` & `aolab-bmi3d-0.9.2/db/tracker/models.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/tasktrack.py` & `aolab-bmi3d-0.9.2/db/tracker/tasktrack.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/trainbmi.py` & `aolab-bmi3d-0.9.2/db/tracker/trainbmi.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/views.py` & `aolab-bmi3d-0.9.2/db/tracker/views.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/tracker/websocket.py` & `aolab-bmi3d-0.9.2/db/tracker/websocket.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/db/urls.py` & `aolab-bmi3d-0.9.2/db/urls.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/__init__.py` & `aolab-bmi3d-0.9.2/features/__init__.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/arduino_features.py` & `aolab-bmi3d-0.9.2/features/arduino_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/blackrock_features.py` & `aolab-bmi3d-0.9.2/features/blackrock_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/bmi_task_features.py` & `aolab-bmi3d-0.9.2/features/bmi_task_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/ecube_features.py` & `aolab-bmi3d-0.9.2/features/ecube_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/eyetracker_features.py` & `aolab-bmi3d-0.9.2/features/eyetracker_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/generator_features.py` & `aolab-bmi3d-0.9.2/features/generator_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/hdf_features.py` & `aolab-bmi3d-0.9.2/features/hdf_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/kinarm_features.py` & `aolab-bmi3d-0.9.2/features/kinarm_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/laser_features.py` & `aolab-bmi3d-0.9.2/features/laser_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/neural_sys_features.py` & `aolab-bmi3d-0.9.2/features/neural_sys_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/optitrack_features.py` & `aolab-bmi3d-0.9.2/features/optitrack_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/peripheral_device_features.py` & `aolab-bmi3d-0.9.2/features/peripheral_device_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/phasespace_features.py` & `aolab-bmi3d-0.9.2/features/phasespace_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/plexon_features.py` & `aolab-bmi3d-0.9.2/features/plexon_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/reward_features.py` & `aolab-bmi3d-0.9.2/features/reward_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/serial_port_sensor.py` & `aolab-bmi3d-0.9.2/features/serial_port_sensor.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/simulation_features.py` & `aolab-bmi3d-0.9.2/features/simulation_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/sync_features.py` & `aolab-bmi3d-0.9.2/features/sync_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/touch_features.py` & `aolab-bmi3d-0.9.2/features/touch_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/features/video_recording_features.py` & `aolab-bmi3d-0.9.2/features/video_recording_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/arduino_imu.py` & `aolab-bmi3d-0.9.2/riglib/arduino_imu.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/arduino_joystick.py` & `aolab-bmi3d-0.9.2/riglib/arduino_joystick.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/blackrock/__init__.py` & `aolab-bmi3d-0.9.2/riglib/blackrock/__init__.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/blackrock/brMiscFxns.py` & `aolab-bmi3d-0.9.2/riglib/blackrock/brMiscFxns.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/blackrock/brpylib.py` & `aolab-bmi3d-0.9.2/riglib/blackrock/brpylib.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/blackrock/cerelink.py` & `aolab-bmi3d-0.9.2/riglib/blackrock/cerelink.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/accumulator.py` & `aolab-bmi3d-0.9.2/riglib/bmi/accumulator.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/assist.py` & `aolab-bmi3d-0.9.2/riglib/bmi/assist.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/bmi.py` & `aolab-bmi3d-0.9.2/riglib/bmi/bmi.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/clda.py` & `aolab-bmi3d-0.9.2/riglib/bmi/clda.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/extractor.py` & `aolab-bmi3d-0.9.2/riglib/bmi/extractor.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/feedback_controllers.py` & `aolab-bmi3d-0.9.2/riglib/bmi/feedback_controllers.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/goal_calculators.py` & `aolab-bmi3d-0.9.2/riglib/bmi/goal_calculators.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/kfdecoder.py` & `aolab-bmi3d-0.9.2/riglib/bmi/kfdecoder.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/kfdecoder_fcns.py` & `aolab-bmi3d-0.9.2/riglib/bmi/kfdecoder_fcns.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/lindecoder.py` & `aolab-bmi3d-0.9.2/riglib/bmi/lindecoder.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/onedim_lfp_decoder.py` & `aolab-bmi3d-0.9.2/riglib/bmi/onedim_lfp_decoder.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/ppfdecoder.py` & `aolab-bmi3d-0.9.2/riglib/bmi/ppfdecoder.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/rat_bmi_decoder.py` & `aolab-bmi3d-0.9.2/riglib/bmi/rat_bmi_decoder.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/robot_arms.py` & `aolab-bmi3d-0.9.2/riglib/bmi/robot_arms.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/sim_neurons.py` & `aolab-bmi3d-0.9.2/riglib/bmi/sim_neurons.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/sskfdecoder.py` & `aolab-bmi3d-0.9.2/riglib/bmi/sskfdecoder.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/state_space_models.py` & `aolab-bmi3d-0.9.2/riglib/bmi/state_space_models.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/bmi/train.py` & `aolab-bmi3d-0.9.2/riglib/bmi/train.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/button.py` & `aolab-bmi3d-0.9.2/riglib/button.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/calibrations.py` & `aolab-bmi3d-0.9.2/riglib/calibrations.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/dio/NIUSB6501/control_comedi_swig.py` & `aolab-bmi3d-0.9.2/riglib/dio/NIUSB6501/control_comedi_swig.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/dio/NIUSB6501/py_comedi_control.py` & `aolab-bmi3d-0.9.2/riglib/dio/NIUSB6501/py_comedi_control.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/dio/nidaq/__init__.py` & `aolab-bmi3d-0.9.2/riglib/dio/nidaq/__init__.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/dio/parse.py` & `aolab-bmi3d-0.9.2/riglib/dio/parse.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/e3vision.py` & `aolab-bmi3d-0.9.2/riglib/e3vision.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/ecube/__init__.py` & `aolab-bmi3d-0.9.2/riglib/ecube/__init__.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/ecube/file.py` & `aolab-bmi3d-0.9.2/riglib/ecube/file.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/ecube/pyeCubeStream.py` & `aolab-bmi3d-0.9.2/riglib/ecube/pyeCubeStream.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/experiment/Pygame.py` & `aolab-bmi3d-0.9.2/riglib/experiment/Pygame.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/experiment/__init__.py` & `aolab-bmi3d-0.9.2/riglib/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/experiment/experiment.py` & `aolab-bmi3d-0.9.2/riglib/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/experiment/generate.py` & `aolab-bmi3d-0.9.2/riglib/experiment/generate.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/experiment/mocks.py` & `aolab-bmi3d-0.9.2/riglib/experiment/mocks.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/experiment/report.py` & `aolab-bmi3d-0.9.2/riglib/experiment/report.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/experiment/task_wrapper.py` & `aolab-bmi3d-0.9.2/riglib/experiment/task_wrapper.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/eyetracker.py` & `aolab-bmi3d-0.9.2/riglib/eyetracker.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/filter.py` & `aolab-bmi3d-0.9.2/riglib/filter.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/fsm/fsm/fsm.py` & `aolab-bmi3d-0.9.2/riglib/fsm/fsm/fsm.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/gpio.py` & `aolab-bmi3d-0.9.2/riglib/gpio.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/hdfwriter/hdfwriter.py` & `aolab-bmi3d-0.9.2/riglib/hdfwriter/hdfwriter.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/kinarmdata.py` & `aolab-bmi3d-0.9.2/riglib/kinarmdata.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/kinarmsocket.py` & `aolab-bmi3d-0.9.2/riglib/kinarmsocket.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/master8stimulation.py` & `aolab-bmi3d-0.9.2/riglib/master8stimulation.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/motiontracker.py` & `aolab-bmi3d-0.9.2/riglib/motiontracker.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/mp_calc.py` & `aolab-bmi3d-0.9.2/riglib/mp_calc.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/mp_proxy.py` & `aolab-bmi3d-0.9.2/riglib/mp_proxy.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/optitrack_client/optitrack.py` & `aolab-bmi3d-0.9.2/riglib/optitrack_client/optitrack.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/optitrack_client/optitrack_interface_sijia.py` & `aolab-bmi3d-0.9.2/riglib/optitrack_client/optitrack_interface_sijia.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/phidgets.py` & `aolab-bmi3d-0.9.2/riglib/phidgets.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/plants.py` & `aolab-bmi3d-0.9.2/riglib/plants.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/positioner/__init__.py` & `aolab-bmi3d-0.9.2/riglib/positioner/__init__.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/positioner/calib.py` & `aolab-bmi3d-0.9.2/riglib/positioner/calib.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/qwalor_laser.py` & `aolab-bmi3d-0.9.2/riglib/qwalor_laser.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/reward.py` & `aolab-bmi3d-0.9.2/riglib/reward.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/reward_crist.py` & `aolab-bmi3d-0.9.2/riglib/reward_crist.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/serial_dio.py` & `aolab-bmi3d-0.9.2/riglib/serial_dio.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/singleton.py` & `aolab-bmi3d-0.9.2/riglib/singleton.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/sink.py` & `aolab-bmi3d-0.9.2/riglib/sink.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/source.py` & `aolab-bmi3d-0.9.2/riglib/source.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stereo_opengl/environment.py` & `aolab-bmi3d-0.9.2/riglib/stereo_opengl/environment.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stereo_opengl/ik.py` & `aolab-bmi3d-0.9.2/riglib/stereo_opengl/ik.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stereo_opengl/models.py` & `aolab-bmi3d-0.9.2/riglib/stereo_opengl/models.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stereo_opengl/primitives.py` & `aolab-bmi3d-0.9.2/riglib/stereo_opengl/primitives.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stereo_opengl/render/fbo.py` & `aolab-bmi3d-0.9.2/riglib/stereo_opengl/render/fbo.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stereo_opengl/render/render.py` & `aolab-bmi3d-0.9.2/riglib/stereo_opengl/render/render.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stereo_opengl/render/shader.py` & `aolab-bmi3d-0.9.2/riglib/stereo_opengl/render/shader.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stereo_opengl/render/ssao.py` & `aolab-bmi3d-0.9.2/riglib/stereo_opengl/render/ssao.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stereo_opengl/render/stereo.py` & `aolab-bmi3d-0.9.2/riglib/stereo_opengl/render/stereo.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stereo_opengl/textures.py` & `aolab-bmi3d-0.9.2/riglib/stereo_opengl/textures.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stereo_opengl/utils.py` & `aolab-bmi3d-0.9.2/riglib/stereo_opengl/utils.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stereo_opengl/window.py` & `aolab-bmi3d-0.9.2/riglib/stereo_opengl/window.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stereo_opengl/xfm.py` & `aolab-bmi3d-0.9.2/riglib/stereo_opengl/xfm.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/stimulus_pulse.py` & `aolab-bmi3d-0.9.2/riglib/stimulus_pulse.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/tablet_reward.py` & `aolab-bmi3d-0.9.2/riglib/tablet_reward.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/riglib/touch_data.py` & `aolab-bmi3d-0.9.2/riglib/touch_data.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/robot/Link.py` & `aolab-bmi3d-0.9.2/robot/Link.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/robot/Quaternion.py` & `aolab-bmi3d-0.9.2/robot/Quaternion.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/robot/Robot.py` & `aolab-bmi3d-0.9.2/robot/Robot.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/robot/SerialLink.py` & `aolab-bmi3d-0.9.2/robot/SerialLink.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/robot/dynamics.py` & `aolab-bmi3d-0.9.2/robot/dynamics.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/robot/jacobian.py` & `aolab-bmi3d-0.9.2/robot/jacobian.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/robot/kinematics.py` & `aolab-bmi3d-0.9.2/robot/kinematics.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/robot/manipulability.py` & `aolab-bmi3d-0.9.2/robot/manipulability.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/robot/parsedemo.py` & `aolab-bmi3d-0.9.2/robot/parsedemo.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/robot/plot.py` & `aolab-bmi3d-0.9.2/robot/plot.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/robot/trajectory.py` & `aolab-bmi3d-0.9.2/robot/trajectory.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/robot/transform.py` & `aolab-bmi3d-0.9.2/robot/transform.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/robot/utility.py` & `aolab-bmi3d-0.9.2/robot/utility.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/setup.py` & `aolab-bmi3d-0.9.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="aolab-bmi3d",
-    version="0.9.1",
+    version="0.9.2",
     author="Lots of people",
     description="electrophysiology experimental rig library",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
```

### Comparing `aolab-bmi3d-0.9.1/tests/test_decoders.py` & `aolab-bmi3d-0.9.2/tests/test_decoders.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/tests/test_ecube.py` & `aolab-bmi3d-0.9.2/tests/test_ecube.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/tests/test_features.py` & `aolab-bmi3d-0.9.2/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/tests/test_qwalor_laser.py` & `aolab-bmi3d-0.9.2/tests/test_qwalor_laser.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/tests/test_reward.py` & `aolab-bmi3d-0.9.2/tests/test_reward.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/tests/test_tasks.py` & `aolab-bmi3d-0.9.2/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/utils/angle_utils.py` & `aolab-bmi3d-0.9.2/utils/angle_utils.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/utils/drawbox.py` & `aolab-bmi3d-0.9.2/utils/drawbox.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/utils/fixpaths.py` & `aolab-bmi3d-0.9.2/utils/fixpaths.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/utils/make_autoalign.py` & `aolab-bmi3d-0.9.2/utils/make_autoalign.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/utils/reassociate.py` & `aolab-bmi3d-0.9.2/utils/reassociate.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/utils/ringbuffer.py` & `aolab-bmi3d-0.9.2/utils/ringbuffer.py`

 * *Files identical despite different names*

### Comparing `aolab-bmi3d-0.9.1/utils/util_fns.py` & `aolab-bmi3d-0.9.2/utils/util_fns.py`

 * *Files identical despite different names*

