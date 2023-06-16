# Comparing `tmp/flightanalysis-0.1.6.tar.gz` & `tmp/flightanalysis-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightanalysis-0.1.6.tar", last modified: Wed Jun 14 17:43:24 2023, max compression
+gzip compressed data, was "flightanalysis-0.1.7.tar", last modified: Fri Jun 16 08:26:21 2023, max compression
```

## Comparing `flightanalysis-0.1.6.tar` & `flightanalysis-0.1.7.tar`

### file list

```diff
@@ -1,90 +1,77 @@
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    35149 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/LICENSE
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       34 2023-06-14 11:48:20.000000 flightanalysis-0.1.6/MANIFEST.in
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1160 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/README.md
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.270142 flightanalysis-0.1.6/flightanalysis/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      261 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3609 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/aircraft_analysis.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.270142 flightanalysis-0.1.6/flightanalysis/base/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       65 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/base/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2574 2023-06-14 16:19:59.000000 flightanalysis-0.1.6/flightanalysis/base/collection.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2178 2023-06-13 10:36:02.000000 flightanalysis-0.1.6/flightanalysis/base/constructs.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      221 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/base/numpy_encoder.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5436 2023-06-14 15:42:22.000000 flightanalysis-0.1.6/flightanalysis/base/table.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1693 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/controls.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.270142 flightanalysis-0.1.6/flightanalysis/criteria/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1454 2023-06-14 16:19:04.000000 flightanalysis-0.1.6/flightanalysis/criteria/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2434 2023-06-14 16:18:29.000000 flightanalysis-0.1.6/flightanalysis/criteria/combination.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1417 2023-06-14 16:16:38.000000 flightanalysis-0.1.6/flightanalysis/criteria/comparison.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2228 2023-06-14 16:17:13.000000 flightanalysis-0.1.6/flightanalysis/criteria/continuous.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      925 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/criteria/results.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1532 2023-06-14 16:16:58.000000 flightanalysis-0.1.6/flightanalysis/criteria/single.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.270142 flightanalysis-0.1.6/flightanalysis/data/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      293 2023-06-14 12:08:11.000000 flightanalysis-0.1.6/flightanalysis/data/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    79839 2023-06-14 11:06:35.000000 flightanalysis-0.1.6/flightanalysis/data/f25.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    70673 2023-06-14 11:05:48.000000 flightanalysis-0.1.6/flightanalysis/data/p23.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    73755 2023-06-14 11:05:11.000000 flightanalysis-0.1.6/flightanalysis/data/p25.json
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.270142 flightanalysis-0.1.6/flightanalysis/environment/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       91 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/environment/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1393 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/environment/environment.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4345 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/environment/wind.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      466 2023-06-13 14:30:47.000000 flightanalysis-0.1.6/flightanalysis/fc_json.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5479 2023-06-14 17:31:54.000000 flightanalysis-0.1.6/flightanalysis/fc_score.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7725 2023-06-05 21:18:18.000000 flightanalysis-0.1.6/flightanalysis/flightline.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/flightanalysis/model/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      108 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/model/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1179 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/model/coefficients.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      405 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/model/constants.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1377 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/model/flow.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      675 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/model/model.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/flightanalysis/schedule/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2888 2023-06-13 12:22:27.000000 flightanalysis-0.1.6/flightanalysis/schedule/__init__.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/flightanalysis/schedule/definition/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      695 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1482 2023-06-06 05:23:48.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/collectors.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6382 2023-06-13 08:53:43.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/element_builders.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4907 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/element_definition.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4658 2023-06-14 07:40:53.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_builder.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5202 2023-06-13 12:23:31.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_definition.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4126 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_info.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6220 2023-06-13 12:59:23.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_parameters.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7430 2023-06-06 05:26:36.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/operation.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1959 2023-06-14 11:04:57.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/schedule_definition.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/flightanalysis/schedule/elements/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7343 2023-06-14 17:36:12.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1965 2023-06-14 17:38:48.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/autorotation.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3369 2023-06-14 16:25:15.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/line.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6341 2023-06-13 12:18:07.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/loop.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2069 2023-06-14 17:37:45.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/nose_drop.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1584 2023-06-14 17:38:08.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/pitch_break.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1282 2023-06-14 17:38:30.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/recovery.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1685 2023-06-13 12:21:37.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/stall_turn.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4106 2023-06-14 15:44:45.000000 flightanalysis-0.1.6/flightanalysis/schedule/manoeuvre.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4507 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/schedule/schedule.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      891 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/simulation.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/flightanalysis/state/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1689 2023-06-14 08:27:10.000000 flightanalysis-0.1.6/flightanalysis/state/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2611 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/state/state.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/flightanalysis/state/tools/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/state/tools/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4570 2023-06-14 09:02:25.000000 flightanalysis-0.1.6/flightanalysis/state/tools/alignment.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4450 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/state/tools/builders.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2722 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/state/tools/conversions.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3635 2023-06-14 15:40:09.000000 flightanalysis-0.1.6/flightanalysis/state/tools/dumpers.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      931 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/state/tools/measurements.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2966 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/state/tools/transformers.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.270142 flightanalysis-0.1.6/flightanalysis.egg-info/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-14 17:43:24.000000 flightanalysis-0.1.6/flightanalysis.egg-info/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2693 2023-06-14 17:43:24.000000 flightanalysis-0.1.6/flightanalysis.egg-info/SOURCES.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-14 17:43:24.000000 flightanalysis-0.1.6/flightanalysis.egg-info/dependency_links.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       49 2023-06-14 17:43:24.000000 flightanalysis-0.1.6/flightanalysis.egg-info/requires.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       15 2023-06-14 17:43:24.000000 flightanalysis-0.1.6/flightanalysis.egg-info/top_level.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      446 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/setup.cfg
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      687 2023-06-14 11:51:46.000000 flightanalysis-0.1.6/setup.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/tests/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      215 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/tests/test_analysis.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      402 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/tests/test_controls.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      206 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/tests/test_data.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2268 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/tests/test_fc_json.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6855 2023-06-05 21:18:18.000000 flightanalysis-0.1.6/tests/test_flightline.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:26:21.568131 flightanalysis-0.1.7/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    35149 2023-03-28 15:54:19.000000 flightanalysis-0.1.7/LICENSE
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       34 2023-06-14 11:48:20.000000 flightanalysis-0.1.7/MANIFEST.in
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1480 2023-06-16 08:26:21.568131 flightanalysis-0.1.7/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1160 2023-03-28 15:54:19.000000 flightanalysis-0.1.7/README.md
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:26:21.560131 flightanalysis-0.1.7/flightanalysis/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      346 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/__init__.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:26:21.560131 flightanalysis-0.1.7/flightanalysis/base/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       83 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/base/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2574 2023-06-14 16:19:59.000000 flightanalysis-0.1.7/flightanalysis/base/collection.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2178 2023-06-13 10:36:02.000000 flightanalysis-0.1.7/flightanalysis/base/constructs.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      221 2023-03-28 15:54:19.000000 flightanalysis-0.1.7/flightanalysis/base/numpy_encoder.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5436 2023-06-14 15:42:22.000000 flightanalysis-0.1.7/flightanalysis/base/table.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:26:21.564131 flightanalysis-0.1.7/flightanalysis/criteria/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1541 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/criteria/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2434 2023-06-14 16:18:29.000000 flightanalysis-0.1.7/flightanalysis/criteria/combination.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1417 2023-06-14 16:16:38.000000 flightanalysis-0.1.7/flightanalysis/criteria/comparison.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2228 2023-06-14 16:17:13.000000 flightanalysis-0.1.7/flightanalysis/criteria/continuous.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      925 2023-03-28 15:54:19.000000 flightanalysis-0.1.7/flightanalysis/criteria/results.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1532 2023-06-14 16:16:58.000000 flightanalysis-0.1.7/flightanalysis/criteria/single.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:26:21.564131 flightanalysis-0.1.7/flightanalysis/data/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      293 2023-06-14 12:08:11.000000 flightanalysis-0.1.7/flightanalysis/data/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    79839 2023-06-14 11:06:35.000000 flightanalysis-0.1.7/flightanalysis/data/f25.json
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    70404 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/data/p23.json
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    73755 2023-06-14 11:05:11.000000 flightanalysis-0.1.7/flightanalysis/data/p25.json
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:26:21.564131 flightanalysis-0.1.7/flightanalysis/environment/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       91 2023-03-28 15:54:19.000000 flightanalysis-0.1.7/flightanalysis/environment/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1226 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/environment/environment.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4252 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/environment/wind.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      466 2023-06-13 14:30:47.000000 flightanalysis-0.1.7/flightanalysis/fc_json.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:26:21.564131 flightanalysis-0.1.7/flightanalysis/model/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      109 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/model/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      828 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/model/coefficients.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      405 2023-03-28 15:54:19.000000 flightanalysis-0.1.7/flightanalysis/model/constants.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1113 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/model/flow.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      675 2023-03-28 15:54:19.000000 flightanalysis-0.1.7/flightanalysis/model/model.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:26:21.564131 flightanalysis-0.1.7/flightanalysis/schedule/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2888 2023-06-13 12:22:27.000000 flightanalysis-0.1.7/flightanalysis/schedule/__init__.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:26:21.568131 flightanalysis-0.1.7/flightanalysis/schedule/definition/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      691 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/schedule/definition/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1482 2023-06-06 05:23:48.000000 flightanalysis-0.1.7/flightanalysis/schedule/definition/collectors.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6382 2023-06-13 08:53:43.000000 flightanalysis-0.1.7/flightanalysis/schedule/definition/element_builders.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4907 2023-06-05 21:18:21.000000 flightanalysis-0.1.7/flightanalysis/schedule/definition/element_definition.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4658 2023-06-14 07:40:53.000000 flightanalysis-0.1.7/flightanalysis/schedule/definition/manoeuvre_builder.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5202 2023-06-13 12:23:31.000000 flightanalysis-0.1.7/flightanalysis/schedule/definition/manoeuvre_definition.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4126 2023-06-05 21:18:21.000000 flightanalysis-0.1.7/flightanalysis/schedule/definition/manoeuvre_info.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6222 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/schedule/definition/manoeuvre_parameters.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7430 2023-06-06 05:26:36.000000 flightanalysis-0.1.7/flightanalysis/schedule/definition/operation.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1959 2023-06-14 11:04:57.000000 flightanalysis-0.1.7/flightanalysis/schedule/definition/schedule_definition.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:26:21.568131 flightanalysis-0.1.7/flightanalysis/schedule/elements/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7343 2023-06-15 15:25:25.000000 flightanalysis-0.1.7/flightanalysis/schedule/elements/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2307 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/schedule/elements/autorotation.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3372 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/schedule/elements/line.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6341 2023-06-13 12:18:07.000000 flightanalysis-0.1.7/flightanalysis/schedule/elements/loop.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2421 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/schedule/elements/nose_drop.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1958 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/schedule/elements/pitch_break.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1557 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/schedule/elements/recovery.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1685 2023-06-13 12:21:37.000000 flightanalysis-0.1.7/flightanalysis/schedule/elements/stall_turn.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4156 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/schedule/manoeuvre.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4507 2023-06-05 21:18:21.000000 flightanalysis-0.1.7/flightanalysis/schedule/schedule.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:26:21.568131 flightanalysis-0.1.7/flightanalysis/state/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       27 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/state/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    22499 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/flightanalysis/state/state.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:26:21.560131 flightanalysis-0.1.7/flightanalysis.egg-info/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1480 2023-06-16 08:26:21.000000 flightanalysis-0.1.7/flightanalysis.egg-info/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2261 2023-06-16 08:26:21.000000 flightanalysis-0.1.7/flightanalysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-16 08:26:21.000000 flightanalysis-0.1.7/flightanalysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       49 2023-06-16 08:26:21.000000 flightanalysis-0.1.7/flightanalysis.egg-info/requires.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-16 08:26:21.000000 flightanalysis-0.1.7/flightanalysis.egg-info/top_level.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      446 2023-06-16 08:26:21.568131 flightanalysis-0.1.7/setup.cfg
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      687 2023-06-14 11:51:46.000000 flightanalysis-0.1.7/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-16 08:26:21.568131 flightanalysis-0.1.7/tests/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      196 2023-06-16 08:25:50.000000 flightanalysis-0.1.7/tests/test_analysis.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      402 2023-03-28 15:54:19.000000 flightanalysis-0.1.7/tests/test_controls.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      206 2023-03-28 15:54:19.000000 flightanalysis-0.1.7/tests/test_data.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2268 2023-03-28 15:54:19.000000 flightanalysis-0.1.7/tests/test_fc_json.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6855 2023-06-05 21:18:18.000000 flightanalysis-0.1.7/tests/test_flightline.py
```

### Comparing `flightanalysis-0.1.6/LICENSE` & `flightanalysis-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/PKG-INFO` & `flightanalysis-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: flightanalysis
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for analysing flight data
 Home-page: https://github.com/PyFlightCoach/FlightAnalysis
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FlightAnalysis
 
 This package contains tools for analysing flight log data. 
 
@@ -29,7 +31,9 @@
 
 # External Dependencies:
 scipy
 fastdtw
 ardupilot_log_reader
 flightdata
 pfc-geometry
+
+
```

### Comparing `flightanalysis-0.1.6/README.md` & `flightanalysis-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/base/collection.py` & `flightanalysis-0.1.7/flightanalysis/base/collection.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/base/constructs.py` & `flightanalysis-0.1.7/flightanalysis/base/constructs.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/base/table.py` & `flightanalysis-0.1.7/flightanalysis/base/table.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/criteria/__init__.py` & `flightanalysis-0.1.7/flightanalysis/criteria/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from argparse import ArgumentTypeError
 import numpy as np
 import pandas as pd
+from pandas.api.types import is_list_like
 from typing import List, Dict, Callable
 from .results import Result, Results
 
 
 #These functions return scores for an error
 f3a_radius = lambda x : (1 - 1/(x+1)) * 4
 f3a_length = lambda x : (1 - 1/(x+1)) * 4
 f3a_angle = lambda x: x/15
 f3a_speed = lambda x : (1 - 1/(x+1))
 f3a_roll_rate = lambda x : (1 - 1/(x+1))
 imac_angle = lambda x: x/10
 hard_zero = lambda x: 0 if x==0 else 10
-free = lambda x: 0
+free = lambda x: 0 if not is_list_like(x) else np.zeros(len(x))
 
 from .single import Single
 
 basic_angle_f3a = Single(f3a_angle, lambda x : np.abs(np.degrees(x) % (2 * np.pi)))
 
 from .continuous import Continuous
```

### Comparing `flightanalysis-0.1.6/flightanalysis/criteria/combination.py` & `flightanalysis-0.1.7/flightanalysis/criteria/combination.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/criteria/comparison.py` & `flightanalysis-0.1.7/flightanalysis/criteria/comparison.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/criteria/continuous.py` & `flightanalysis-0.1.7/flightanalysis/criteria/continuous.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/criteria/results.py` & `flightanalysis-0.1.7/flightanalysis/criteria/results.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/criteria/single.py` & `flightanalysis-0.1.7/flightanalysis/criteria/single.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/data/f25.json` & `flightanalysis-0.1.7/flightanalysis/data/f25.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/data/p23.json` & `flightanalysis-0.1.7/flightanalysis/data/p23.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998291205322457%*

 * *Differences: {"'M'": "{'mps': {'speed': {'criteria': {'criteria': 'lambda x : (1 - 1/(x+1))'}, 'collectors': "*

 * *        "{delete: [9, 8, 7, 6, 4, 3, 2, 1]}}}, 'eds': {'e_1_pad1': {'props': {'speed': '30', "*

 * *        "'length': '(0.5*(line_length-(0+((abs(roll_option[0])*30)/partial_roll_rate))))'}}, "*

 * *        "'e_1_roll': {'props': {'speed': '30', 'length': "*

 * *        "'((abs(roll_option[0])*30)/partial_roll_rate)'}}, 'e_1_pad2': {'props': {'speed': '30', "*

 * *        "'length': '(0.5*(line_length-(0+((abs(roll_option[0])*30) […]*

```diff
@@ -12,35 +12,35 @@
                     "speed": "speed"
                 }
             },
             "e_1_pad1": {
                 "Kind": "Line",
                 "name": "e_1_pad1",
                 "props": {
-                    "length": "(0.5*(line_length-(0+((abs(roll_option[0])*speed)/partial_roll_rate))))",
+                    "length": "(0.5*(line_length-(0+((abs(roll_option[0])*30)/partial_roll_rate))))",
                     "roll": "0",
-                    "speed": "speed"
+                    "speed": "30"
                 }
             },
             "e_1_pad2": {
                 "Kind": "Line",
                 "name": "e_1_pad2",
                 "props": {
-                    "length": "(0.5*(line_length-(0+((abs(roll_option[0])*speed)/partial_roll_rate))))",
+                    "length": "(0.5*(line_length-(0+((abs(roll_option[0])*30)/partial_roll_rate))))",
                     "roll": "0",
-                    "speed": "speed"
+                    "speed": "30"
                 }
             },
             "e_1_roll": {
                 "Kind": "Line",
                 "name": "e_1_roll",
                 "props": {
-                    "length": "((abs(roll_option[0])*speed)/partial_roll_rate)",
+                    "length": "((abs(roll_option[0])*30)/partial_roll_rate)",
                     "roll": "roll_option[0]",
-                    "speed": "speed"
+                    "speed": "30"
                 }
             },
             "e_2": {
                 "Kind": "StallTurn",
                 "name": "e_2",
                 "props": {
                     "speed": "0.0",
@@ -49,15 +49,15 @@
             },
             "e_3": {
                 "Kind": "Line",
                 "name": "e_3",
                 "props": {
                     "length": "line_length",
                     "roll": "0.0",
-                    "speed": "speed"
+                    "speed": "30"
                 }
             },
             "e_4": {
                 "Kind": "Loop",
                 "name": "e_4",
                 "props": {
                     "angle": "-3.141592653589793",
@@ -69,50 +69,50 @@
             },
             "e_5": {
                 "Kind": "Line",
                 "name": "e_5",
                 "props": {
                     "length": "line_length",
                     "roll": "0.0",
-                    "speed": "speed"
+                    "speed": "30"
                 }
             },
             "e_6": {
                 "Kind": "StallTurn",
                 "name": "e_6",
                 "props": {
                     "speed": "0.0",
                     "yaw_rate": "stallturn_rate"
                 }
             },
             "e_7_pad1": {
                 "Kind": "Line",
                 "name": "e_7_pad1",
                 "props": {
-                    "length": "(0.5*(line_length-(0+((abs(roll_option[1])*speed)/partial_roll_rate))))",
+                    "length": "(0.5*(line_length-(0+((abs(roll_option[1])*30)/partial_roll_rate))))",
                     "roll": "0",
-                    "speed": "speed"
+                    "speed": "30"
                 }
             },
             "e_7_pad2": {
                 "Kind": "Line",
                 "name": "e_7_pad2",
                 "props": {
-                    "length": "(0.5*(line_length-(0+((abs(roll_option[1])*speed)/partial_roll_rate))))",
+                    "length": "(0.5*(line_length-(0+((abs(roll_option[1])*30)/partial_roll_rate))))",
                     "roll": "0",
-                    "speed": "speed"
+                    "speed": "30"
                 }
             },
             "e_7_roll": {
                 "Kind": "Line",
                 "name": "e_7_roll",
                 "props": {
-                    "length": "((abs(roll_option[1])*speed)/partial_roll_rate)",
+                    "length": "((abs(roll_option[1])*30)/partial_roll_rate)",
                     "roll": "roll_option[1]",
-                    "speed": "speed"
+                    "speed": "30"
                 }
             },
             "e_8": {
                 "Kind": "Loop",
                 "name": "e_8",
                 "props": {
                     "angle": "1.5707963267948966",
@@ -203,27 +203,19 @@
                 },
                 "default": 1,
                 "name": "roll_option"
             },
             "speed": {
                 "collectors": [
                     "e_0.speed",
-                    "e_1_roll.speed",
-                    "e_1_pad1.speed",
-                    "e_1_pad2.speed",
-                    "e_3.speed",
                     "e_4.speed",
-                    "e_5.speed",
-                    "e_7_roll.speed",
-                    "e_7_pad1.speed",
-                    "e_7_pad2.speed",
                     "e_8.speed"
                 ],
                 "criteria": {
-                    "criteria": "lambda x: 0",
+                    "criteria": "lambda x : (1 - 1/(x+1))",
                     "initial_value": null,
                     "kind": "Comparison"
                 },
                 "default": 30.0,
                 "name": "speed"
             },
             "stallturn_rate": {
@@ -1282,15 +1274,15 @@
             },
             "e_1": {
                 "Kind": "Line",
                 "name": "e_1",
                 "props": {
                     "length": "line_length",
                     "roll": "0.0",
-                    "speed": "speed"
+                    "speed": "25"
                 }
             },
             "e_2": {
                 "Kind": "Loop",
                 "name": "e_2",
                 "props": {
                     "angle": "1.5707963267948966",
@@ -1340,15 +1332,14 @@
                     "kind": "Comparison"
                 },
                 "default": 55.0,
                 "name": "loop_radius"
             },
             "speed": {
                 "collectors": [
-                    "e_1.speed",
                     "e_2.speed"
                 ],
                 "criteria": {
                     "criteria": "lambda x : (1 - 1/(x+1))",
                     "initial_value": null,
                     "kind": "Comparison"
                 },
```

### Comparing `flightanalysis-0.1.6/flightanalysis/data/p25.json` & `flightanalysis-0.1.7/flightanalysis/data/p25.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/environment/environment.py` & `flightanalysis-0.1.7/flightanalysis/environment/environment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 
-from flightanalysis.base.table import Table, Time
-from typing import Union
 from flightdata import Flight, Fields
-from pathlib import Path
-from flightanalysis.base.constructs import Constructs, SVar
-from geometry import Point, Quaternion, Base, P0
-from flightanalysis.state import State
+from flightanalysis import Constructs, SVar, Table
+from geometry import Point, Base, P0
 import numpy as np
 from .wind import WindModel, WindModelBuilder
 
 
 R = 287.058
 GAMMA = 1.4
 
@@ -32,15 +28,15 @@
 class Environment(Table):
     constructs = Table.constructs + Constructs([
         SVar("atm", Air, ["P", "T", "rho"], lambda tab: Air.iso_sea_level(len(tab))),
         SVar("wind", Point, ["wvx", "wvy", "wvz"], lambda tab: P0(len(tab)))
     ])
 
     @staticmethod
-    def build(flight: Flight, sec: State, wmodel: WindModel):
+    def build(flight: Flight, sec, wmodel: WindModel):
 
         df = flight.read_fields(Fields.PRESSURE)
         df = df.assign(temperature_0=291.15)
         df = df.assign(rho=get_rho(df["pressure_0"], df["temperature_0"]))
 
         return Environment.from_constructs(
             time=sec.time,
```

### Comparing `flightanalysis-0.1.6/flightanalysis/environment/wind.py` & `flightanalysis-0.1.7/flightanalysis/environment/wind.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import numpy as np
 import pandas as pd
-from geometry import Point, Points
+from geometry import Point
 from scipy.interpolate import interp1d
-from flightanalysis.state import State
-from typing import Callable, List, Tuple
-from scipy.optimize import minimize
+from typing import List, Tuple
 
 
 class WindModel:
     def __init__(self, func, kind, args):
         self.func = func
         self.kind = kind
         self.args = args
```

### Comparing `flightanalysis-0.1.6/flightanalysis/model/coefficients.py` & `flightanalysis-0.1.7/flightanalysis/model/coefficients.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,19 @@
-from flightanalysis.base.table import Table, Time, SVar
-from typing import Union
-from flightdata import Flight, Fields
-from pathlib import Path
-from flightanalysis.base.constructs import Constructs, SVar
-from geometry import Point, Quaternion, Quaternions, Points
-import numpy as np
-from flightanalysis.state import State
-from flightanalysis.model.flow import Flow
-from flightanalysis.model.constants import ACConstants
+from flightanalysis.base.table import Table, SVar, Constructs, SVar
+from geometry import Point
 
 
 class Coefficients(Table):
     constructs = Table.constructs + Constructs([
         SVar("force", Point, ["cx", "cy", "cz"], None),
         SVar("moment", Point, ["cl", "cm", "cn"], None)
     ])
 
     @staticmethod
-    def build(sec: State, flow: Flow, consts: ACConstants):
+    def build(sec, flow, consts):
         I = consts.inertia
         u = sec.vel
         du = sec.acc
         w = sec.rvel
         dw = sec.racc
         moment=I*(dw + w.cross(w)) / (flow.q * consts.s) 
         #not correct need to extend geometry module to include inertia matrix
```

### Comparing `flightanalysis-0.1.6/flightanalysis/model/flow.py` & `flightanalysis-0.1.7/flightanalysis/model/flow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 
-from flightanalysis.base.table import Table, Time, SVar
-from typing import Union
-from flightdata import Flight, Fields
-from pathlib import Path
-from flightanalysis.base.constructs import Constructs, SVar
-from flightanalysis.state import State
-from flightanalysis.environment import Environment
-from geometry import Point, Quaternion, Base, PX, Euler
+from flightanalysis import Table, Time, SVar, Constructs, SVar
+from geometry import Point, Base, PX, Euler
 import numpy as np
 
 
-
 class Attack(Base):
     cols = ['alpha', 'beta', 'q']
 
 
 class Flow(Table):
     constructs = Table.constructs + Constructs([
         SVar("aspd", Point, ["asx", "asy", "asz"], None),
         SVar("flow", Point, ["alpha", "beta", "q"], None)
     ])
 
     @staticmethod
-    def build(body: State, env: Environment):
+    def build(body, env):
 #        wind = judge.judging_to_wind(env.wind)
         airspeed = body.vel - body.att.inverse().transform_point(env.wind)
 
         np.seterr(invalid='ignore')
         alpha =  np.arctan(airspeed.z / airspeed.x) 
         
         stab_airspeed = Euler(
```

### Comparing `flightanalysis-0.1.6/flightanalysis/model/model.py` & `flightanalysis-0.1.7/flightanalysis/model/model.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/__init__.py` & `flightanalysis-0.1.7/flightanalysis/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/definition/__init__.py` & `flightanalysis-0.1.7/flightanalysis/schedule/definition/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,10 @@
     elif isinstance(arg, Number):
         return lambda mps: arg
     elif isinstance(arg, Opp):
         return arg
     
 
 from .element_definition import ElDef, ElDefs
-
 from .manoeuvre_definition import ManDef
-
 from .schedule_definition import SchedDef
-
-
 from .manoeuvre_builder import ManoeuvreBuilder, f3amb, MBTags
```

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/definition/collectors.py` & `flightanalysis-0.1.7/flightanalysis/schedule/definition/collectors.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/definition/element_builders.py` & `flightanalysis-0.1.7/flightanalysis/schedule/definition/element_builders.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/definition/element_definition.py` & `flightanalysis-0.1.7/flightanalysis/schedule/definition/element_definition.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_builder.py` & `flightanalysis-0.1.7/flightanalysis/schedule/definition/manoeuvre_builder.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_definition.py` & `flightanalysis-0.1.7/flightanalysis/schedule/definition/manoeuvre_definition.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_info.py` & `flightanalysis-0.1.7/flightanalysis/schedule/definition/manoeuvre_info.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_parameters.py` & `flightanalysis-0.1.7/flightanalysis/schedule/definition/manoeuvre_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
         Args:
             manoeuvre (Manoeuvre): The Manoeuvre to assess
 
         Returns:
             Dict[str, float]: The sum of downgrades for each ManParm
         """
-        return Results([mp.get_downgrades(manoeuvre.all_elements) for mp in self if not isinstance(mp.criteria, Combination)])
+        return Results([mp.get_downgrades(manoeuvre.all_elements()) for mp in self if not isinstance(mp.criteria, Combination)])
     
     def append_collectors(self, colls: Dict[str, Callable]):
         """Append each of a dict of collector methods to the relevant ManParm
 
         Args:
             colls (Dict[str, Callable]): dict of parmname: collector method
         """
```

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/definition/operation.py` & `flightanalysis-0.1.7/flightanalysis/schedule/definition/operation.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/definition/schedule_definition.py` & `flightanalysis-0.1.7/flightanalysis/schedule/definition/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/elements/__init__.py` & `flightanalysis-0.1.7/flightanalysis/schedule/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/elements/autorotation.py` & `flightanalysis-0.1.7/flightanalysis/schedule/elements/autorotation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import numpy as np
 from geometry import Transformation, Point, Quaternion, PX, PY, PZ, P0
 from flightanalysis import State
 from flightanalysis.base.table import Time
 from . import El, Loop, DownGrades, DownGrade, Elements
 from flightanalysis.criteria import *
 from typing import Union
@@ -22,14 +23,22 @@
             speed=self.speed,
             length=self.length,
             roll=self.roll,
             uid=self.uid
         )
     
     @property
+    def exit_scoring(self):
+        return DownGrades()
+    
+    @property
+    def intra_scoring(self):
+        return DownGrades()
+    
+    @property
     def angle(self):
         return 2 * np.pi * self.roll
 
     @property
     def rate(self):
         return self.angle * self.speed / self.length
     
@@ -53,8 +62,14 @@
         # TODO this assumes the plane is traveling forwards, create_template does not
         jit = flown.judging_itrans(transform)
         
         return self.set_parms(
             length=jit.att.inverse().transform_point(flown.pos - jit.pos).x[-1],
             roll=np.sign(np.mean(flown.p)) * abs(self.roll),
             speed=np.mean(abs(flown.vel))
-        )
+        )
+    
+    def copy_direction(self, other: Autorotation) -> Autorotation:
+        return self.set_parms(roll=abs(self.roll) * np.sign(other.roll))
+
+
+
```

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/elements/line.py` & `flightanalysis-0.1.7/flightanalysis/schedule/elements/line.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
             DownGrade("op_track", "measure_op_track", intra_f3a_angle),
         ])
 
         if not self.roll == 0:
             _intra_scoring.add(DownGrade("roll_rate", "measure_roll_rate", intra_f3a_roll_rate))
             _intra_scoring.add(DownGrade("roll_amount", "measure_end_roll_angle", basic_angle_f3a))
         else:
+            
             _intra_scoring.add(DownGrade("roll_angle", "measure_roll_angle_error", intra_f3a_angle))
         return _intra_scoring
 
 
 
     def describe(self):
         d1 = "line" if self.roll==0 else f"{self.roll} roll"
@@ -91,10 +92,7 @@
 
     @staticmethod
     def from_roll(speed: float, rate: float, angle: float):
         return Line(speed, rate * angle * speed, angle )
 
     def copy_direction(self, other):
         return self.set_parms(roll=abs(self.roll) * np.sign(other.roll))
-
-
-
```

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/elements/loop.py` & `flightanalysis-0.1.7/flightanalysis/schedule/elements/loop.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/elements/nose_drop.py` & `flightanalysis-0.1.7/flightanalysis/schedule/elements/nose_drop.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+from __future__ import annotations
 import numpy as np
 from geometry import Transformation, Point, Quaternion, PX, PY, PZ, Coord
 from flightanalysis.state import State
 from flightanalysis.base.table import Time
 from . import El, Loop, DownGrades, DownGrade, Elements
 from flightanalysis.criteria import *
 from typing import Union
 
 
-
 class NoseDrop(El):
     """A nose drop is used for spin entries. It consists of a loop to a vertical downline, with an integrated
     pitch rotation in the opposite direction to the loops pitch rotation so that the body axis finishes at
     break_angle off the vertical line"""
     parameters = El.parameters + "radius,break_angle".split(",")
     def __init__(self, speed: float, radius: float, break_angle: float, uid: str=None):
         super().__init__(uid, speed)
@@ -23,37 +23,48 @@
             kind=self.__class__.__name__,
             speed=self.speed,
             radius=self.radius,
             break_angle=self.break_angle,
             uid=self.uid
         )
 
-    def create_template(self, istate: State, time: Time=None):
+    def create_template(self, istate: State, time: Time=None) -> State:
         _inverted = 1 if istate.transform.rotation.is_inverted()[0] else -1
         
         alpha =  np.arctan2(istate.vel.z, istate.vel.x)[0]
 
         return Loop(self.speed, self.radius, 0.5*np.pi*_inverted).create_template(
             istate, time
         ).superimpose_rotation(
             PY(), 
             -alpha - abs(self.break_angle) * _inverted
         ).label(element=self.uid)
     
     def describe(self):
         return "nose drop"
 
-    def match_intention(self, transform: Transformation, flown: State):
+    def match_intention(self, transform: Transformation, flown: State) -> NoseDrop:
         _inverted = 1 if transform.rotation.is_inverted()[0] else -1
         _speed = abs(flown.vel).mean()
 
         loop = Loop(_speed, self.radius, 0.5*np.pi*_inverted).match_intention(
             transform, flown
         )
 
         alpha = np.arctan2(flown.vel.z, flown.vel.x)[-1]
 
         return self.set_parms(
             speed = _speed,
             radius = loop.radius,
             break_angle = abs(alpha)
         )
+
+    def copy_direction(self, other: NoseDrop) -> NoseDrop:
+        return self.set_parms(break_angle=abs(self.break_angle) * np.sign(other.break_angle))
+
+    @property
+    def intra_scoring(self):
+        return DownGrades()
+
+    @property
+    def exit_scoring(self):
+        return DownGrades()
```

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/elements/pitch_break.py` & `flightanalysis-0.1.7/flightanalysis/schedule/elements/pitch_break.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from __future__ import annotations
 import numpy as np
 from geometry import Transformation, Point, Quaternion, PX, PY, PZ
 from flightanalysis.state import State
 from flightanalysis.base.table import Time
 from . import El, Loop, DownGrades, DownGrade, Elements
 from flightanalysis.criteria import *
-from . import Line
+from . import Line, DownGrades
 
 
 
 class PitchBreak(El):
     parameters = El.parameters + "length,break_angle".split(",")
     def __init__(self, speed: float, length: float, break_angle: float, uid: str=None):
         super().__init__(uid, speed)
@@ -20,36 +21,46 @@
             kind=self.__class__.__name__,
             speed=self.speed,
             length=self.length,
             break_angle=self.break_angle,
             uid=self.uid
         )
 
-
-    def create_template(self, istate: State, time: Time=None):
-
+    def create_template(self, istate: State, time: Time=None) -> State:
         return Line(self.speed, self.length).create_template(
             istate, 
             time
         ).superimpose_rotation(
             PY(),
             self.break_angle
         ).label(element=self.uid)
 
     def describe(self):
         return "pitch break"
     
-    def match_intention(self, transform: Transformation, flown: State):
+    def match_intention(self, transform: Transformation, flown: State) -> PitchBreak:
         jit = flown.judging_itrans(transform)
 
         _speed = abs(flown.vel).mean()
 
         alphas = np.arctan2(flown.vel.z, flown.vel.x)
 
         return self.set_parms(
             speed = _speed,
             length = max(
                 jit.att.inverse().transform_point(flown.pos - jit.pos).x[-1],
                 5
             ) ,
             break_angle = alphas[-1]
         )
+    
+    def copy_direction(self, other: PitchBreak) -> PitchBreak:
+        return self.set_parms(break_angle=abs(self.break_angle) * np.sign(other.break_angle))
+
+
+    @property
+    def intra_scoring(self):
+        return DownGrades()
+
+    @property
+    def exit_scoring(self):
+        return DownGrades()
```

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/elements/recovery.py` & `flightanalysis-0.1.7/flightanalysis/schedule/elements/recovery.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import numpy as np
 from geometry import Transformation, Point, Quaternion, PX, PY, PZ
 from flightanalysis.state import State
 from flightanalysis.base.table import Time
 from . import El, Loop, DownGrades, DownGrade, Elements, Line
 from flightanalysis.criteria import *
 
@@ -34,8 +35,19 @@
         return "recovery"
 
     def match_intention(self, transform: Transformation, flown: State):
         jit = flown.judging_itrans(transform)
         return self.set_parms(
             length=max(jit.att.inverse().transform_point(flown.pos - jit.pos).x[-1], 5),
             speed=abs(flown.vel).mean()
-        )
+        )
+    
+    def copy_direction(self, other: Recovery) -> Recovery:
+        return self.set_parms()
+
+    @property
+    def intra_scoring(self):
+        return DownGrades()
+
+    @property
+    def exit_scoring(self):
+        return DownGrades()
```

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/elements/stall_turn.py` & `flightanalysis-0.1.7/flightanalysis/schedule/elements/stall_turn.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/manoeuvre.py` & `flightanalysis-0.1.7/flightanalysis/schedule/manoeuvre.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from geometry import Transformation, Quaternion, Coord, P0, PX, PY, PZ
 from flightanalysis.state import State
 from flightanalysis.schedule.elements import *
 from typing import List, Union
 import numpy as np
 import pandas as pd
 
@@ -94,18 +95,18 @@
         
         return Manoeuvre(elms[0], Elements(elms[1:]), self.uid), istate
 
     def match_rates(self, rates):
         new_elms = [elm.match_axis_rate(rates[elm.__class__], rates["speed"]) for elm in self.elements]
         return self.replace_elms(new_elms)
 
-    def copy_directions(self, other):
+    def copy_directions(self, other: Manoeuvre):
         return Manoeuvre.from_all_elements(
             self.uid, 
-            [es.copy_direction(eo) for es, eo in zip(self.all_elements, other.all_elements)]
+            [es.copy_direction(eo) for es, eo in zip(self.all_elements(), other.all_elements())]
         )
 
     def analyse(self, flown: State, template: State):
         
         fl=self.entry_line.get_data(flown)
         tp=self.entry_line.get_data(template).relocate(fl.pos[0])
```

### Comparing `flightanalysis-0.1.6/flightanalysis/schedule/schedule.py` & `flightanalysis-0.1.7/flightanalysis/schedule/schedule.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/flightanalysis.egg-info/PKG-INFO` & `flightanalysis-0.1.7/flightanalysis.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: flightanalysis
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for analysing flight data
 Home-page: https://github.com/PyFlightCoach/FlightAnalysis
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FlightAnalysis
 
 This package contains tools for analysing flight log data. 
 
@@ -29,7 +31,9 @@
 
 # External Dependencies:
 scipy
 fastdtw
 ardupilot_log_reader
 flightdata
 pfc-geometry
+
+
```

### Comparing `flightanalysis-0.1.6/flightanalysis.egg-info/SOURCES.txt` & `flightanalysis-0.1.7/flightanalysis.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 flightanalysis/__init__.py
-flightanalysis/aircraft_analysis.py
-flightanalysis/controls.py
 flightanalysis/fc_json.py
-flightanalysis/fc_score.py
-flightanalysis/flightline.py
-flightanalysis/simulation.py
 flightanalysis.egg-info/PKG-INFO
 flightanalysis.egg-info/SOURCES.txt
 flightanalysis.egg-info/dependency_links.txt
 flightanalysis.egg-info/requires.txt
 flightanalysis.egg-info/top_level.txt
 flightanalysis/base/__init__.py
 flightanalysis/base/collection.py
@@ -57,19 +52,12 @@
 flightanalysis/schedule/elements/loop.py
 flightanalysis/schedule/elements/nose_drop.py
 flightanalysis/schedule/elements/pitch_break.py
 flightanalysis/schedule/elements/recovery.py
 flightanalysis/schedule/elements/stall_turn.py
 flightanalysis/state/__init__.py
 flightanalysis/state/state.py
-flightanalysis/state/tools/__init__.py
-flightanalysis/state/tools/alignment.py
-flightanalysis/state/tools/builders.py
-flightanalysis/state/tools/conversions.py
-flightanalysis/state/tools/dumpers.py
-flightanalysis/state/tools/measurements.py
-flightanalysis/state/tools/transformers.py
 tests/test_analysis.py
 tests/test_controls.py
 tests/test_data.py
 tests/test_fc_json.py
 tests/test_flightline.py
```

### Comparing `flightanalysis-0.1.6/setup.py` & `flightanalysis-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/tests/test_fc_json.py` & `flightanalysis-0.1.7/tests/test_fc_json.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.6/tests/test_flightline.py` & `flightanalysis-0.1.7/tests/test_flightline.py`

 * *Files identical despite different names*

