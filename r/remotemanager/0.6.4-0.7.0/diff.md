# Comparing `tmp/remotemanager-0.6.4.tar.gz` & `tmp/remotemanager-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.6.4.tar", last modified: Tue Jun 13 14:19:40 2023, max compression
+gzip compressed data, was "remotemanager-0.7.0.tar", last modified: Fri Jun 16 11:23:06 2023, max compression
```

## Comparing `remotemanager-0.6.4.tar` & `remotemanager-0.7.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.618359 remotemanager-0.6.4/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.6.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-13 14:19:40.618359 remotemanager-0.6.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.6.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-06-12 10:37:37.000000 remotemanager-0.6.4/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.610359 remotemanager-0.6.4/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-06-12 10:37:37.000000 remotemanager-0.6.4/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.610359 remotemanager-0.6.4/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15718 2023-06-08 13:33:35.000000 remotemanager-0.6.4/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.610359 remotemanager-0.6.4/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12730 2023-06-13 13:42:38.000000 remotemanager-0.6.4/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.6.4/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.6.4/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.6.4/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.6.4/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    24882 2023-06-08 11:36:38.000000 remotemanager-0.6.4/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.614359 remotemanager-0.6.4/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    49754 2023-06-12 08:57:29.000000 remotemanager-0.6.4/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)    22474 2023-06-12 08:57:29.000000 remotemanager-0.6.4/remotemanager/dataset/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.614359 remotemanager-0.6.4/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.6.4/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4873 2023-05-25 09:38:01.000000 remotemanager-0.6.4/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.614359 remotemanager-0.6.4/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4325 2023-06-08 11:36:38.000000 remotemanager-0.6.4/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.6.4/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.6.4/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.6.4/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.614359 remotemanager-0.6.4/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.6.4/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.6.4/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.614359 remotemanager-0.6.4/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.6.4/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.6.4/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.618359 remotemanager-0.6.4/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.6.4/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.6.4/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)     9262 2023-06-02 09:40:16.000000 remotemanager-0.6.4/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.618359 remotemanager-0.6.4/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.6.4/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:19:40.610359 remotemanager-0.6.4/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-13 14:19:40.000000 remotemanager-0.6.4/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1788 2023-06-13 14:19:40.000000 remotemanager-0.6.4/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 14:19:40.000000 remotemanager-0.6.4/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-13 14:19:40.000000 remotemanager-0.6.4/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 14:19:40.000000 remotemanager-0.6.4/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 14:19:40.618359 remotemanager-0.6.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.6.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.694952 remotemanager-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-16 11:23:06.694952 remotemanager-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.7.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-06-15 14:41:51.000000 remotemanager-0.7.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.686952 remotemanager-0.7.0/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-06-15 14:41:51.000000 remotemanager-0.7.0/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.686952 remotemanager-0.7.0/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.7.0/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.686952 remotemanager-0.7.0/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12730 2023-06-13 13:42:38.000000 remotemanager-0.7.0/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.7.0/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.7.0/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.7.0/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.7.0/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    25087 2023-06-16 10:42:35.000000 remotemanager-0.7.0/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.690952 remotemanager-0.7.0/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    50282 2023-06-15 12:40:25.000000 remotemanager-0.7.0/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)    22383 2023-06-14 09:06:03.000000 remotemanager-0.7.0/remotemanager/dataset/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.690952 remotemanager-0.7.0/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.7.0/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4921 2023-06-15 11:08:04.000000 remotemanager-0.7.0/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.690952 remotemanager-0.7.0/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.7.0/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.7.0/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.7.0/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.7.0/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.690952 remotemanager-0.7.0/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.7.0/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.7.0/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.7.0/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.690952 remotemanager-0.7.0/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.7.0/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.7.0/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.694952 remotemanager-0.7.0/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.7.0/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.7.0/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9283 2023-06-14 07:47:50.000000 remotemanager-0.7.0/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.694952 remotemanager-0.7.0/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.7.0/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:23:06.686952 remotemanager-0.7.0/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-16 11:23:06.000000 remotemanager-0.7.0/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-06-16 11:23:06.000000 remotemanager-0.7.0/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 11:23:06.000000 remotemanager-0.7.0/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-16 11:23:06.000000 remotemanager-0.7.0/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-16 11:23:06.000000 remotemanager-0.7.0/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 11:23:06.694952 remotemanager-0.7.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.7.0/setup.py
```

### Comparing `remotemanager-0.6.4/LICENSE` & `remotemanager-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/PKG-INFO` & `remotemanager-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.6.4
+Version: 0.7.0
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.6.4/README.md` & `remotemanager-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/pyproject.toml` & `remotemanager-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.6.4"
+current_version = "0.7.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.6.4/remotemanager/connection/cmd.py` & `remotemanager-0.7.0/remotemanager/connection/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
 
         Returns (int):
             the PID of the spawned shell for this command
         """
         return self._pid
 
     @property
-    def returncode(self) -> int:
+    def returncode(self) -> [int, None]:
         """
         Attempt to retrieve the returncode of the subprocess. This call will
         not disturb an asynchronous run, returning None
 
         Returns (int, None):
                 The exit status of the subprocess, None if it is still running.
                 None otherwise.
@@ -346,14 +346,15 @@
         Returns:
             None
         """
         file = self.tempfile
         with open(file, "w+") as o:
             o.write(self._cmd)
 
+        # noinspection PyTypedDict
         self._redirect["execfile"] = file
 
         t0 = time.time()
         self._subprocess = subprocess.Popen(
             f"bash {file}",
             stdout=stdout,
             stderr=stderr,
@@ -416,14 +417,15 @@
         if std or err:  # skip if all None
             self._logger.debug("caching results")
             self._cached = True
 
         if self._redirect["execfile"] is not None:
             tf = self._redirect["execfile"]
             try:
+                # noinspection PyTypeChecker
                 os.remove(tf)
                 self._redirect["execfile"] = None
                 self._logger.info(f"removed temp file {tf}")
             except FileNotFoundError:
                 self._logger.info(f"temp file {tf} not found")
                 pass
```

### Comparing `remotemanager-0.6.4/remotemanager/connection/computers/base.py` & `remotemanager-0.7.0/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/connection/computers/example.py` & `remotemanager-0.7.0/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/connection/computers/options.py` & `remotemanager-0.7.0/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/connection/computers/parsers.py` & `remotemanager-0.7.0/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/connection/testing_object.py` & `remotemanager-0.7.0/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/connection/url.py` & `remotemanager-0.7.0/remotemanager/connection/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         self._keyfile = keyfile
         self._passfile = passfile
         self._raise_errors = raise_errors
         self._ssh_override = None
         self.ssh_prepend = None
 
         self._logger.info(
-            "new url created with url details:" f"{format_iterable(self._conn)}"
+            f"new url created with url details:{format_iterable(self._conn)}"
         )
 
         self._callcount = 0
 
         self._latency = 0
         self._connection_test = None
 
@@ -178,14 +178,17 @@
     def python(self, python):
         self._python = python
 
     @property
     def submitter(self):
         if self._submitter is not None:
             return self._submitter
+        if self._shell is not None:
+            self._logger.debug("submitter is None but shell is set, returning shell")
+            return self._shell
         return URL._defaults["submitter"]
 
     @submitter.setter
     def submitter(self, submitter):
         self._submitter = submitter
 
     @property
@@ -266,26 +269,26 @@
 
     @property
     def keyfile(self):
         if self._keyfile is None:
             return
         p = self._keyfile.replace("~", os.environ["HOME"])
         if not os.path.isfile(p):
-            raise RuntimeError(f"could not find ssh key file at " f"{self._keyfile}")
+            raise RuntimeError(f"could not find ssh key file at {self._keyfile}")
 
         return self._keyfile
 
     @property
     def passfile(self):
         if self._passfile is None:
             return
 
         p = self._passfile.replace("~", os.environ["HOME"])
         if not os.path.isfile(p):
-            raise RuntimeError(f"could not find password file at " f"{self._passfile}")
+            raise RuntimeError(f"could not find password file at {self._passfile}")
 
         return self._passfile
 
     @property
     def is_tunnel(self):
         """
         Uses the presence of an assigned port to determine if we are tunnelling
@@ -484,15 +487,15 @@
         Args:
             newdepth (int):
                 new depth to capture
         Returns:
 
         """
         self._logger.info(
-            f"updating history depth from {self.cmd_history_depth} " f"to {newdepth}"
+            f"updating history depth from {self.cmd_history_depth} to {newdepth}"
         )
         self._cmd_history_depth = newdepth
 
         newqueue = deque(maxlen=self.cmd_history_depth)
 
         for item in self.cmd_history:
             newqueue.append(item)
@@ -548,14 +551,17 @@
         Returns:
             (float): connection latency in seconds, if available. Else None
         """
         if self._connection_test is not None:
             return self._connection_test.latency
         return None
 
+    def script(self, **kwargs):
+        raise NotImplementedError
+
 
 class URLUtils:
     """
     Extra functions to go with the URL class, called via URL.utils
 
     As it requires a parent `URL` to function, and is instantiated with a
     `URL`, there is little to no purpose to using this class exclusively
```

### Comparing `remotemanager-0.6.4/remotemanager/dataset/dataset.py` & `remotemanager-0.7.0/remotemanager/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import collections
 import gc
 import os
 import typing
 import time
 import shutil
+import warnings
 
 from remotemanager.connection.detect_locale_error import detect_locale_error
 from remotemanager.storage.remotefunction import cached_functions
 from remotemanager.connection.url import URL
 from remotemanager.storage.database import Database
 from remotemanager.storage.function import Function
 from remotemanager.dataset.runner import Runner, localwinerror
@@ -54,35 +55,36 @@
     """
 
     _do_not_package = ["_database"]
 
     # DEV NOTE: arguments must be None for computer-url override to function
     def __init__(
         self,
-        function: typing.Callable,
+        function: [typing.Callable, str],
         url: URL = None,
         dbfile: str = None,
         transport: tp.transport.Transport = None,
         serialiser: sr.serial = None,
         script: str = None,
         name: str = None,
-        block_reinit: bool = False,
         extra_files_send: list = None,
         extra_files_recv: list = None,
         verbose: int = None,
         add_newline: bool = True,
+        block_reinit: bool = None,
+        skip: bool = False,
         **global_run_args,
     ):
         self._verbose = Verbosity(verbose)
 
         self._logger.info("dataset initialised")
 
         self._function = Function(function)
 
-        self._global_run_args = {"skip": True}
+        self._global_run_args = {}
         if " " in global_run_args.get("remote_dir", ""):
             raise ValueError(f"Space character detected in remote_dir")
         if " " in global_run_args.get("run_dir", ""):
             raise ValueError(f"Space character detected in run_dir")
         if " " in os.path.abspath(global_run_args.get("local_dir", "")):
             raise ValueError(f"Space character detected in local_dir")
         self._global_run_args.update(global_run_args)
@@ -110,16 +112,21 @@
         self._dbfile_override = dbfile
         self._dependency = None
         self._do_not_recurse = False
 
         self.url = url
         self.transport = transport
         self.serialiser = serialiser
+        self._submitter = None
 
-        if block_reinit:
+        if block_reinit is not None:
+            warnings.warn("block_reinit is soon to be deprecated, use skip instead")
+            skip = block_reinit
+
+        if skip:
             try:
                 os.remove(self.dbfile)
                 self._logger.warning(
                     f"deleted database file {self.dbfile}", silent=True
                 )
             except FileNotFoundError:
                 pass
@@ -420,14 +427,15 @@
         arguments: dict = None,
         name: str = None,
         extra_files_send: list = None,
         extra_files_recv: list = None,
         dependency_call: bool = False,
         verbose: int = None,
         quiet: bool = False,
+        skip: bool = True,
         **run_args,
     ):
         """
         Serialise arguments for later runner construction
 
         Args:
             args (dict):
@@ -440,14 +448,18 @@
                 extra files to send with this run
             extra_files_recv (list, str):
                 extra files to retrieve with this run
             dependency_call (bool):
                 True if called via the dependency handler
             verbose (int, Verbose, None):
                 verbose level for this runner (defaults to Dataset level)
+            quiet (bool):
+                disable printing for this append if True
+            skip (bool):
+                ignores checks for an existing runner if set to False
             run_args:
                 any extra arguments to pass to runner
         """
         self._logger.debug("Dataset append_run called")
         Quiet.state = quiet
         if args is None and arguments is not None:
             args = arguments
@@ -459,14 +471,15 @@
             return self.dependency.append_run(
                 self,
                 args=args,
                 name=name,
                 extra_files_send=extra_files_send,  # noqa: E251
                 extra_files_recv=extra_files_recv,  # noqa: E251
                 verbose=verbose,
+                skip=skip,
                 **run_args,
             )
 
         # first grab global arguments and update them with explicit args
         run_arguments = {k: v for k, v in self._global_run_args.items()}
         run_arguments.update(run_args)
 
@@ -477,15 +490,15 @@
         rnum = len(self.runners)
         if name is not None:
             run_arguments["name"] = name
             r_id = name
 
             if name in self.runner_dict:
                 self._logger.warning(
-                    f"{self} overwriting already " f"existing runner {r_id}"
+                    f"{self} overwriting already existing runner {r_id}"
                 )
         else:
             r_id = f"runner-{rnum}"
 
         tmp = Runner(
             arguments=args,
             dbfile=self.dbfile,
@@ -495,15 +508,19 @@
             extra_files_recv=extra_files_recv,
             verbose=verbose,
             **run_arguments,
         )
 
         tmp.result_extension = self.serialiser.extension
 
-        if tmp.uuid not in self._uuids:
+        if not skip:
+            self._runs[r_id] = tmp
+            self._uuids.append(tmp.uuid)
+            self._logger.important(f"force appended run {tmp.name}")
+        elif tmp.uuid not in self._uuids:
             self._runs[r_id] = tmp
             self._uuids.append(tmp.uuid)
             self._logger.important(f"appended run {tmp.name}")
         else:
             self._logger.important(f"runner {tmp.name} already exists")
 
         self.database.update(self.pack())
@@ -690,17 +707,15 @@
             for attr in attrs:
                 remotes += [f.remote for f in self._collect_files(attr)]
 
         self._logger.warning(f"removing remote(s): {remotes}")
 
         if len(remotes) > 1:
             remotestring = ",".join(remotes)
-            self._logger.info(
-                f"removing several remotes with " f"string {remotestring}"
-            )
+            self._logger.info(f"removing several remotes with string {remotestring}")
             self.url.cmd(f"rm -r {{{remotestring}}}", raise_errors=False)
         else:
             self.url.cmd(f"rm -r {remotes[0]}", raise_errors=False)
 
     def hard_reset(self, files_only: bool = False) -> None:
         """
         Hard reset the dataset, including wiping local and remote folders
@@ -776,15 +791,15 @@
             self._logger.info("creating a jobscript for the login nodes")
             return self._script
         if not self._computer:
             self._logger.info("not a computer, returning base script")
             return self._script
         if "name" not in sub_args:
             self._logger.info(
-                f"name not found in args, " f"appending self name {self.name}"
+                f"name not found in args, appending self name {self.name}"
             )
             sub_args["name"] = self.name
         return self.url.script(**sub_args)
 
     @property
     def script(self, **sub_args) -> str:
         """
@@ -832,19 +847,20 @@
 
     @property
     def url(self) -> URL:
         """
         Currently stored URL object
         """
         if not hasattr(self, "_url"):
+            # noinspection PyTypeChecker
             self.url = None
         return self._url
 
     @url.setter
-    def url(self, url=None) -> None:
+    def url(self, url: [URL, None] = None) -> None:
         """
         Verifies and sets the URL to be used.
         Will create an empty (local) url connection if url is None
 
         Args:
             url (URL):
                 url to be verified
@@ -871,19 +887,20 @@
 
     @property
     def transport(self) -> tp.transport.Transport:
         """
         Currently stored Transport system
         """
         if not hasattr(self, "_transport"):
+            # noinspection PyTypeChecker
             self.transport = None
         return self._transport
 
     @transport.setter
-    def transport(self, transport: tp.transport.Transport = None) -> None:
+    def transport(self, transport: [tp.transport.Transport, None] = None) -> None:
         """
         Verifies and sets the Transport to be used.
         Will use rsync if transport is None
 
         Args:
             transport (Transport):
                 transport to be verified
@@ -1042,15 +1059,15 @@
         """
         self._logger.debug("Dataset run called")
         Quiet.state = quiet
 
         if os.name == "nt" and self.url.is_local:
             raise RuntimeError(localwinerror)
         if self.is_parent:
-            self._logger.warning(f"dataset {self} is a parent, " f"skipping run")
+            self._logger.warning(f"dataset {self} is a parent, skipping run")
             Quiet.state = quiet
             return
 
         if self.dependency:
             self._logger.runtime(
                 f"dataset {self} is a part of a dependency "
                 f"chain, calling from there"
@@ -1105,15 +1122,15 @@
             self.transport.queue_for_push(
                 [runner.jobscript.name, runner.runfile.name],
                 runner.local_dir,
                 runner.remote_dir,
             )
 
             if avoid_nodes:
-                submitter = getattr(self, "submitter", "bash")
+                submitter = self.submitter or "bash"
             else:
                 submitter = self.url.submitter
             runline = f"{submitter} {runner.jobscript.name}"
 
             asynchronous = runner.run_option("asynchronous", True)
             if asynchronous and self.url.submitter == "bash":
                 self._logger.debug('appending "&" for async run')
@@ -1137,15 +1154,15 @@
         i = 0
         for remote, lines in master_scripts.items():
             scriptname = f"{i}-{self.master_script}"
             i += 1
             _scriptfile = TrackedFile(self.local_dir, remote, scriptname)
             self._master_scripts.append(_scriptfile)
             # newline='\n' is required to stop windows clients adding the \r\n
-            self._logger.info(f"writing to master script at " f"{_scriptfile.local}")
+            self._logger.info(f"writing to master script at {_scriptfile.local}")
 
             if asynchronous and self.url.submitter == "bash":
                 # adds the content of the stderr file back into stderr
                 lines.append(
                     f"if [ -e {self.stderr_dump} ]; "
                     f"then >&2 cat {self.stderr_dump}; fi"
                 )
@@ -1387,15 +1404,15 @@
                 if presence:
                     errs.append(self.url.cmd(f"cat {file}").stdout)
 
             if len([e for e in errs if e != ""]) == 0:
                 self._logger.info(f"all errors are empty files")
                 return
 
-        print(f"There are {len(errs)} errors, printing " f"(most recent call last):")
+        print(f"There are {len(errs)} errors, printing (most recent call last):")
 
         error_summaries = []
         locale_errors = []
         for error in errs:
             locale_errors.append(detect_locale_error(error))
             self._logger.error(error)
             error_summaries.append(error.split("\n")[-1])
@@ -1433,24 +1450,21 @@
         """
         if not verbose:
             Quiet.state = True
         # initialise an empty return dict
         ret = {r.uuid: None for r in self.runners}
         # if we're skipping, check in with the runners
         # since the runner.is_finished will be valid...
-        if self.skip:
-            self._logger.info("skip is true, checking runner first")
-            for runner in self.runners:
-                # ...unless we're forcing a run
-                if runner.run_args.get("force", False):
-                    self._logger.info("runner was force run, ignoring")
-                    continue
+        for runner in self.runners:
+            if not runner.run_args.get("skip") or runner.run_args.get("force", False):
+                continue
+            self._logger.info(f"checking in with runner {runner}")
 
-                if runner.is_finished:
-                    ret[runner.uuid] = True
+            if runner.is_finished:
+                ret[runner.uuid] = True
 
         errs = {}
         if files is None:
             self._logger.runtime("checking for files")
             # look for the resultfiles
             files, errs = self._check_for_runner_outputs()
```

### Comparing `remotemanager-0.6.4/remotemanager/dataset/dependency.py` & `remotemanager-0.7.0/remotemanager/dataset/dependency.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/dataset/runner.py` & `remotemanager-0.7.0/remotemanager/dataset/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,32 +62,30 @@
 
         self._extra_files = {
             "send": extra_files_send if extra_files_send is not None else [],
             "recv": extra_files_recv if extra_files_recv is not None else [],
         }
 
         if arguments is not None and not isinstance(arguments, dict):
-            raise ValueError(
-                f"runner arguments ({type(arguments)}) " "must be dict-type"
-            )
+            raise ValueError(f"runner arguments ({type(arguments)}) must be dict-type")
 
         # parent and id setting
         self._parent = parent
         self._parent_uuid = parent.uuid  # used for parent memory recovery
 
         self._id = self_id
 
         # check that we can properly serialise the args
         # this needs to be within the runner, so we can properly generate uuids
         self._args_replaced = False
         try:
             json.dumps(arguments)
             uuid_slug = copy.deepcopy(arguments) or {}
         except TypeError:
-            file = f"{self.parent.argfile}-" f"{self.id}{self.serialiser.extension}"
+            file = f"{self.parent.argfile}-{self.id}{self.serialiser.extension}"
             lpath = os.path.join(self.parent.local_dir, file)
 
             if not os.path.isdir(self.parent.local_dir):
                 os.makedirs(self.parent.local_dir)
 
             content = self.parent.serialiser.dumps(arguments)
             with open(lpath, self.serialiser.write_mode) as o:
@@ -119,15 +117,15 @@
 
         self._dbfile = dbfile
 
         self._manual_run = False
         self._history = {}
         self.state = "created"
 
-        self._identifier = f"{self.parent.name}-" f"{self.parent.short_uuid}-{self.id}"
+        self._identifier = f"{self.parent.name}-{self.parent.short_uuid}-{self.id}"
 
     def __hash__(self) -> hash:
         return hash(self.uuid)
 
     def __repr__(self) -> str:
         return self.identifier
 
@@ -209,15 +207,15 @@
                 file type. Jobscript, result file, etc.
             ext (str):
                 file extension
 
         Returns:
             str: formatted filename
         """
-        self._logger.info(f"creating filename for {ftype} and " f"extension {ext}")
+        self._logger.info(f"creating filename for {ftype} and extension {ext}")
         return f"{self.identifier}-{ftype}{ext}"
 
     @property
     def runfile(self) -> TrackedFile:
         """
         Filename of the python runfile
         """
@@ -362,15 +360,15 @@
     def read_resultfile(self):
         rfile = self.resultfile.local
         self._logger.info("reading locally discovered runfile")
         result = self.parent.serialiser.load(rfile)
 
         timestamp = int(os.path.getmtime(rfile))
         if timestamp < self.last_submitted and not self.is_finished:
-            self._logger.warning(f"{self}: " f"calculation not completed yet")
+            self._logger.warning(f"{self}: calculation not completed yet")
             return False
 
         mtime = datetime.fromtimestamp(timestamp)
         self.insert_history(mtime, "resultfile created remotely")
 
         self.result = result
         return True
@@ -503,28 +501,26 @@
         Args:
             t (datetime.time):
                 time this state change occurred
             newstate (str):
                 status to update
         """
         if not isinstance(t, datetime):
-            raise ValueError(
-                f"time of type {type(t)} should be a datetime " f"instance"
-            )
+            raise ValueError(f"time of type {type(t)} should be a datetime instance")
 
         base_timekey = self.format_time(t)
         idx = 0
         timekey = f"{base_timekey}/{idx}"
         while timekey in self._history:
             idx += 1
 
             timekey = f"{base_timekey}/{idx}"
 
         self._logger.info(
-            f"({timekey}) updating runner {self.short_uuid} state -> " f"{newstate}"
+            f"({timekey}) updating runner {self.short_uuid} state -> {newstate}"
         )
         self._history[timekey] = newstate
 
     def run(self, dry_run: bool = False, **kwargs) -> None:
         """
         Perform a manual run
 
@@ -715,15 +711,15 @@
         Attempts to determine if this runner has completed its run
 
         Returns (bool):
             completion status
         """
         fin = hasattr(self, "_result")
         self._logger.info(
-            f"checking finished state of runner " f"{self.short_uuid} -> {fin}"
+            f"checking finished state of runner {self.short_uuid} -> {fin}"
         )
         return fin
 
     def update_run_options(self, run_args: dict) -> None:
         """
         Update run args with dict `run_args`
         Args:
```

### Comparing `remotemanager-0.6.4/remotemanager/jupyter/magic.py` & `remotemanager-0.7.0/remotemanager/jupyter/magic.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,20 @@
         args = self.extract_in_scope(",".join(sanzu), local_ns)
         fargs = self.extract_in_scope(",".join(sargs), local_ns)
         fstr = self.parse_line(cell_actual, list(fargs), spull)
 
         self._logger.info(f"generated function string {fstr}")
         self._logger.info(f"Dataset args: {args}")
         self._logger.info(f"Function args: {fargs}")
+
+        run_skip = args.pop("skip", True)
         # Build the runner and run
-        ds = Dataset(function=fstr, block_reinit=False, **args)
+        ds = Dataset(function=fstr, skip=False, **args)
         ds.append_run(args=fargs)
-        ds.run()
+        ds.run(skip=run_skip)
 
         for cmd in ds.run_cmds:
             if cmd.stderr:
                 raise RuntimeError(f"error detected in magic run: " f"{cmd.stderr}")
         Quiet.state = True
         ds.wait(1)
         ds.fetch_results()
```

### Comparing `remotemanager-0.6.4/remotemanager/logging/__init__.py` & `remotemanager-0.7.0/remotemanager/logging/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import logging
 from remotemanager.logging.quiet import Quiet
 
 
 class LoggingMixin:
+    _logobj = None
+
     @property
     def _logger(self):
         def create_logger():
             self._logobj = LoggerInsert(f"{__name__}.{self.__class__.__name__}", self)
 
-        if not hasattr(self, "_logobj"):
+        if self._logobj is not None:
             create_logger()
 
         if not isinstance(self._logobj, LoggerInsert):
             create_logger()
         return self._logobj
```

### Comparing `remotemanager-0.6.4/remotemanager/logging/log.py` & `remotemanager-0.7.0/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/logging/utils.py` & `remotemanager-0.7.0/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/logging/verbosity.py` & `remotemanager-0.7.0/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/serialisation/serial.py` & `remotemanager-0.7.0/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.7.0/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.7.0/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/storage/database.py` & `remotemanager-0.7.0/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/storage/function.py` & `remotemanager-0.7.0/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/storage/remotefunction.py` & `remotemanager-0.7.0/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/storage/sendablemixin.py` & `remotemanager-0.7.0/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/storage/trackedfile.py` & `remotemanager-0.7.0/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/transport/cp.py` & `remotemanager-0.7.0/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/transport/rsync.py` & `remotemanager-0.7.0/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/transport/scp.py` & `remotemanager-0.7.0/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/transport/transport.py` & `remotemanager-0.7.0/remotemanager/transport/transport.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self._remote_address = None
         self._url = url if url is not None else URL()
         self.set_remote(url)
 
         self._flags = Flags()
         self._transfers = {}
 
-    def queue_for_push(self, files: list, local: str = None, remote: str = None):
+    def queue_for_push(self, files: [list, str], local: str = None, remote: str = None):
         """
         Queue file(s) for sending (pushing)
 
         Args:
             files (list[str], str):
                 list of files (or file) to add to push queue
             local (str):
@@ -41,15 +41,15 @@
                 remote/destination folder for the file(s)
         Returns:
             None
         """
         self._logger.info(f"adding to PUSH queue")
         self.add_transfer(files, local, remote, "push")
 
-    def queue_for_pull(self, files: list, local: str = None, remote: str = None):
+    def queue_for_pull(self, files: [list, str], local: str = None, remote: str = None):
         """
         Queue file(s) for retrieving (pulling)
 
         Args:
             files (list[str], str):
                 list of files (or file) to add to pull queue
             local (str):
@@ -58,15 +58,15 @@
                 remote/origin folder for the file(s)
         Returns:
             None
         """
         self._logger.info(f"adding to PULL queue")
         self.add_transfer(files, remote, local, "pull")
 
-    def add_transfer(self, files: list, origin: str, target: str, mode: str):
+    def add_transfer(self, files: [list, str], origin: str, target: str, mode: str):
         """
         Create a transfer to be executed. The ordering of the origin/target
         files should be considered as this transport instance being a
         "tunnel" between wherever it is executed (origin), and the destination
         (target)
 
         Args:
```

### Comparing `remotemanager-0.6.4/remotemanager/utils/__init__.py` & `remotemanager-0.7.0/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/utils/flags.py` & `remotemanager-0.7.0/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager/utils/version.py` & `remotemanager-0.7.0/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.4/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.7.0/remotemanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.6.4
+Version: 0.7.0
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.6.4/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.7.0/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

