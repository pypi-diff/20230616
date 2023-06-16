# Comparing `tmp/sftpoeb-0.1.2.tar.gz` & `tmp/sftpoeb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.1.2.tar", last modified: Thu Jun 15 12:03:14 2023, max compression
+gzip compressed data, was "sftpoeb-0.1.3.tar", last modified: Fri Jun 16 11:13:19 2023, max compression
```

## Comparing `sftpoeb-0.1.2.tar` & `sftpoeb-0.1.3.tar`

### file list

```diff
@@ -1,58 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.920023 sftpoeb-0.1.2/
--rw-rw-rw-   0        0        0      661 2023-06-15 12:02:57.000000 sftpoeb-0.1.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1083 2023-06-15 12:03:14.919027 sftpoeb-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.2/README.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 12:03:14.920023 sftpoeb-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-06-15 12:02:49.000000 sftpoeb-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.750018 sftpoeb-0.1.2/sftpoeb/
--rw-rw-rw-   0        0        0       72 2023-06-15 12:00:06.000000 sftpoeb-0.1.2/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.782023 sftpoeb-0.1.2/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.2/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.790026 sftpoeb-0.1.2/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0       48 2023-06-15 12:01:46.000000 sftpoeb-0.1.2/sftpoeb/mainclass/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-06-15 12:00:49.000000 sftpoeb-0.1.2/sftpoeb/mainclass/c_recovery.py
--rw-rw-rw-   0        0        0     3558 2023-06-15 08:31:33.000000 sftpoeb-0.1.2/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.802017 sftpoeb-0.1.2/sftpoeb/method/
--rw-rw-rw-   0        0        0       95 2023-06-14 12:04:10.000000 sftpoeb-0.1.2/sftpoeb/method/__init__.py
--rw-rw-rw-   0        0        0     4839 2023-06-14 11:11:17.000000 sftpoeb-0.1.2/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      601 2023-06-14 06:57:02.000000 sftpoeb-0.1.2/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.2/sftpoeb/method/debug.py
--rw-rw-rw-   0        0        0     9657 2023-06-15 07:54:02.000000 sftpoeb-0.1.2/sftpoeb/method/mail.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.837021 sftpoeb-0.1.2/sftpoeb/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.2/sftpoeb/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.2/sftpoeb/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.2/sftpoeb/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.2/sftpoeb/sftpoeb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.839024 sftpoeb-0.1.2/sftpoeb/subclass/
--rw-rw-rw-   0        0        0      131 2023-06-15 08:04:07.000000 sftpoeb-0.1.2/sftpoeb/subclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.843020 sftpoeb-0.1.2/sftpoeb/subclass/alert/
--rw-rw-rw-   0        0        0       24 2023-06-15 07:57:29.000000 sftpoeb-0.1.2/sftpoeb/subclass/alert/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-06-15 11:41:55.000000 sftpoeb-0.1.2/sftpoeb/subclass/alert/s_c_alert.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.851018 sftpoeb-0.1.2/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.2/sftpoeb/subclass/file/__init__.py
--rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.2/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.2/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.871020 sftpoeb-0.1.2/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.2/sftpoeb/subclass/input/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.2/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.887017 sftpoeb-0.1.2/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.2/sftpoeb/subclass/output/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.2/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.903025 sftpoeb-0.1.2/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.2/sftpoeb/subclass/path/__init__.py
--rw-rw-rw-   0        0        0     5206 2023-06-14 10:57:49.000000 sftpoeb-0.1.2/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     4239 2023-06-14 10:57:44.000000 sftpoeb-0.1.2/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     2042 2023-06-15 11:58:34.000000 sftpoeb-0.1.2/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.908021 sftpoeb-0.1.2/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.1.2/sftpoeb/subclass/process/__init__.py
--rw-rw-rw-   0        0        0    30032 2023-06-15 08:48:28.000000 sftpoeb-0.1.2/sftpoeb/subclass/process/s_c_process_package_1.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:03:14.781020 sftpoeb-0.1.2/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0     1083 2023-06-15 12:03:14.000000 sftpoeb-0.1.2/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1274 2023-06-15 12:03:14.000000 sftpoeb-0.1.2/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 12:03:14.000000 sftpoeb-0.1.2/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-06-15 12:03:14.000000 sftpoeb-0.1.2/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 12:03:14.000000 sftpoeb-0.1.2/sftpoeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1107 2023-06-15 08:22:57.000000 sftpoeb-0.1.2/test.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.178984 sftpoeb-0.1.3/
+-rw-rw-rw-   0        0        0      723 2023-06-16 11:13:16.000000 sftpoeb-0.1.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1145 2023-06-16 11:13:19.176592 sftpoeb-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.798568 sftpoeb-0.1.3/home/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.792567 sftpoeb-0.1.3/home/natthawut.th/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.793570 sftpoeb-0.1.3/home/natthawut.th/kpc.prd/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.794572 sftpoeb-0.1.3/home/natthawut.th/kpc.prd/kpc.prd/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.795573 sftpoeb-0.1.3/home/natthawut.th/kpc.prd/kpc.prd/Outbound/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.796571 sftpoeb-0.1.3/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.876711 sftpoeb-0.1.3/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/
+-rw-rw-rw-   0        0        0      177 2023-06-15 12:04:47.000000 sftpoeb-0.1.3/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/20230615190447_log.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.799575 sftpoeb-0.1.3/home/sftp/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.800576 sftpoeb-0.1.3/home/sftp/kpc.prd/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.801570 sftpoeb-0.1.3/home/sftp/kpc.prd/kpc.prd/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.802568 sftpoeb-0.1.3/home/sftp/kpc.prd/kpc.prd/Outbound/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.803571 sftpoeb-0.1.3/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.881718 sftpoeb-0.1.3/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/
+-rw-rw-rw-   0        0        0      177 2023-06-15 12:04:47.000000 sftpoeb-0.1.3/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/20230615190447_log.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 11:13:19.179553 sftpoeb-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-06-16 11:12:44.000000 sftpoeb-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.886720 sftpoeb-0.1.3/sftpoeb/
+-rw-rw-rw-   0        0        0       72 2023-06-15 12:00:06.000000 sftpoeb-0.1.3/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.944712 sftpoeb-0.1.3/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.3/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.969724 sftpoeb-0.1.3/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0       48 2023-06-15 12:01:46.000000 sftpoeb-0.1.3/sftpoeb/mainclass/__init__.py
+-rw-rw-rw-   0        0        0     8509 2023-06-16 11:06:25.000000 sftpoeb-0.1.3/sftpoeb/mainclass/c_recovery.py
+-rw-rw-rw-   0        0        0     3558 2023-06-15 08:31:33.000000 sftpoeb-0.1.3/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.003710 sftpoeb-0.1.3/sftpoeb/method/
+-rw-rw-rw-   0        0        0       95 2023-06-14 12:04:10.000000 sftpoeb-0.1.3/sftpoeb/method/__init__.py
+-rw-rw-rw-   0        0        0     4800 2023-06-16 10:56:05.000000 sftpoeb-0.1.3/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      601 2023-06-14 06:57:02.000000 sftpoeb-0.1.3/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.3/sftpoeb/method/debug.py
+-rw-rw-rw-   0        0        0     9657 2023-06-15 07:54:02.000000 sftpoeb-0.1.3/sftpoeb/method/mail.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.053854 sftpoeb-0.1.3/sftpoeb/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.3/sftpoeb/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.3/sftpoeb/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.3/sftpoeb/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.3/sftpoeb/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.057855 sftpoeb-0.1.3/sftpoeb/subclass/
+-rw-rw-rw-   0        0        0      156 2023-06-16 04:43:20.000000 sftpoeb-0.1.3/sftpoeb/subclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.067858 sftpoeb-0.1.3/sftpoeb/subclass/alert/
+-rw-rw-rw-   0        0        0       24 2023-06-15 07:57:29.000000 sftpoeb-0.1.3/sftpoeb/subclass/alert/__init__.py
+-rw-rw-rw-   0        0        0     1515 2023-06-15 11:41:55.000000 sftpoeb-0.1.3/sftpoeb/subclass/alert/s_c_alert.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.080858 sftpoeb-0.1.3/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.3/sftpoeb/subclass/file/__init__.py
+-rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.3/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.3/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.088863 sftpoeb-0.1.3/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.3/sftpoeb/subclass/input/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.3/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.097857 sftpoeb-0.1.3/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.3/sftpoeb/subclass/output/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.3/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.115665 sftpoeb-0.1.3/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.3/sftpoeb/subclass/path/__init__.py
+-rw-rw-rw-   0        0        0     5375 2023-06-16 03:46:50.000000 sftpoeb-0.1.3/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     4146 2023-06-16 03:40:25.000000 sftpoeb-0.1.3/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     2042 2023-06-15 11:58:34.000000 sftpoeb-0.1.3/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.144336 sftpoeb-0.1.3/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.1.3/sftpoeb/subclass/process/__init__.py
+-rw-rw-rw-   0        0        0    30017 2023-06-16 10:56:17.000000 sftpoeb-0.1.3/sftpoeb/subclass/process/s_c_process_package_1.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.172689 sftpoeb-0.1.3/sftpoeb/subclass/recovery/
+-rw-rw-rw-   0        0        0       27 2023-06-16 04:43:48.000000 sftpoeb-0.1.3/sftpoeb/subclass/recovery/__init__.py
+-rw-rw-rw-   0        0        0    19301 2023-06-16 11:06:15.000000 sftpoeb-0.1.3/sftpoeb/subclass/recovery/s_c_recovery.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.941710 sftpoeb-0.1.3/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0     1145 2023-06-16 11:13:18.000000 sftpoeb-0.1.3/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1533 2023-06-16 11:13:18.000000 sftpoeb-0.1.3/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 11:13:18.000000 sftpoeb-0.1.3/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-16 11:13:18.000000 sftpoeb-0.1.3/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 11:13:18.000000 sftpoeb-0.1.3/sftpoeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1107 2023-06-15 08:22:57.000000 sftpoeb-0.1.3/test.py
+-rw-rw-rw-   0        0        0     1133 2023-06-16 11:07:44.000000 sftpoeb-0.1.3/test_recovery.py
```

### Comparing `sftpoeb-0.1.2/CHANGELOG.txt` & `sftpoeb-0.1.3/CHANGELOG.txt`

 * *Files 25% similar despite different names*

```diff
@@ -43,8 +43,12 @@
 
 0.1.1 (14/06/2023)
 ------------------
 - Fixbug
 
 0.1.2 (15/06/2023)
 ------------------
-- Fixbug
+- Fixbug
+
+0.1.3 (16/06/2023)
+------------------
+- Process Recovery
```

### Comparing `sftpoeb-0.1.2/LICENSE.txt` & `sftpoeb-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.2/PKG-INFO` & `sftpoeb-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.1.2
+Version: 0.1.3
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -63,7 +63,11 @@
 ------------------
 - Fixbug
 
 0.1.2 (15/06/2023)
 ------------------
 - Fixbug
 
+0.1.3 (16/06/2023)
+------------------
+- Process Recovery
+
```

### Comparing `sftpoeb-0.1.2/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.1.3/sftpoeb/mainclass/c_sftp.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.2/sftpoeb/method/callservice.py` & `sftpoeb-0.1.3/sftpoeb/method/callservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 import os,requests,time,urllib3
 urllib3.disable_warnings()
 
-def serviceSigning(data, fileNameText, fileNamePDF, pathFile,round,serviceCode,URL):
+def serviceSigning(data, fileNameText, pathFile,round,serviceCode,URL):
     multipart_data = MultipartEncoder(
         fields={
             "SellerTaxId": data['SellerTaxid'],
             "SellerBranchId": data['SellerBranchId'],
             "APIKey": data['APIKey'],
             "UserCode": data['UserCode'],
             "AccessKey": data['AccessKey'],
@@ -24,25 +24,25 @@
     try:
         response = requests.post(URL, data=multipart_data, headers=headers, verify=False)
         if response.status_code == 200:
             result = response.json()
         else:
             if round < 3:
                 time.sleep(0.5)
-                result = serviceSigning(data, fileNameText, fileNamePDF, pathFile,round+1,serviceCode)
+                result = serviceSigning(data, fileNameText, pathFile,round+1,serviceCode)
             else:
                 result = {
                     "status": "ER",
                     "errorMessage": "Service Stamp was problem.",
                     "errorCode": response.status_code
                 }
     except Exception as e:
         if round < 3:
             time.sleep(0.5)
-            result = serviceSigning(data, fileNameText, fileNamePDF, pathFile,round+1,serviceCode)
+            result = serviceSigning(data, fileNameText, pathFile,round+1,serviceCode)
         else:
             result = {
                 "status": "ER",
                 "errorCode": "EXC001",
                 "errorMessage": "send_for_getfile : " + str(e)
             }
     return result
```

### Comparing `sftpoeb-0.1.2/sftpoeb/method/checkpath.py` & `sftpoeb-0.1.3/sftpoeb/method/checkpath.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.2/sftpoeb/method/mail.py` & `sftpoeb-0.1.3/sftpoeb/method/mail.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.2/sftpoeb/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.1.3/sftpoeb/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.2/sftpoeb/subclass/alert/s_c_alert.py` & `sftpoeb-0.1.3/sftpoeb/subclass/alert/s_c_alert.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.2/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.1.3/sftpoeb/subclass/file/s_c_file.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.2/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.1.3/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.2/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.1.3/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.2/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.1.3/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.2/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.1.3/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,18 @@
         self.destinationPathCSV = custPath + "/" + sftpPath + "/Inbound/CSV/"
         self.destinationPathPDF = custPath + "/" + sftpPath + "/Inbound/PDF/"
         self.destinationHistory = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/'
         self.destinationCsvArchivePath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/CSV/Archived_File/'
         self.destinationCsvErrorPath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/CSV/Error_File/'
         self.destinationPdfArchivePath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/PDF/Archived_File/'
         self.destinationPdfErrorPath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/PDF/Error_File/'
-        self.destinationOutputPdfPath = custPath + "/" + sftpPath + '/Outbound/' + self.transformDate(dateNow) + '/PDF/'
-        self.destinationOutputXmlPath = custPath + "/" + sftpPath + '/Outbound/' + self.transformDate(dateNow) + '/XML/'
-        self.destinationLogPath = custPath + "/" + sftpPath + '/Outbound/' + self.transformDate(dateNow) + '/Logfile/'
+        self.destinationOutputPath = custPath + "/" + sftpPath + '/Outbound/'
+        self.destinationOutputPdfPath = self.destinationOutputPath + self.transformDate(dateNow) + '/PDF/'
+        self.destinationOutputXmlPath = self.destinationOutputPath + self.transformDate(dateNow) + '/XML/'
+        self.destinationLogPath = self.destinationOutputPath + self.transformDate(dateNow) + '/Logfile/'
 
 ########## SET ############
     def setDestinationPath(self,path):
         self.destinationPath = path
         return self.destinationPath
 
     def setDestinationPathCSV(self,path):
@@ -112,14 +113,17 @@
         check_path(self.destinationOutputXmlPath)
         return self.destinationOutputXmlPath
 
     def getDestinationLogPath(self):
         check_path(self.destinationLogPath)
         return self.destinationLogPath
 
+    def getDestinationOutputPath(self):
+        check_path(self.destinationOutputPath)
+        return self.destinationOutputPath
 ########## END GET ############
 
 ########## transformDate ############
     def configTransformDate(self,formatOld,formatNew):
         self.formatOld = formatOld
         self.formatNew = formatNew
```

### Comparing `sftpoeb-0.1.2/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.1.3/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,22 +4,24 @@
     def __init__(self,myPath,sftpPath,dateNow,timeNow):
         self.formatOld = '%Y%m%d'
         self.formatNew = '%Y-%m-%d'
         self.myPath = myPath
         self.localPath = myPath + "/" + sftpPath + "/Inbound/"
         self.localFilerun = self.localPath+ '/Filerun/' + self.transformDate(dateNow) + '/'
         self.localPathNow = self.localPath + "/" + str( dateNow + timeNow ) + "/"
-        self.localHistory = myPath + "/" + sftpPath + "/History/" + self.transformDate(dateNow) + '/'
-        self.localCsvArchivePath = myPath + "/" + sftpPath + "/History/" + self.transformDate(dateNow) + '/CSV/Archived_File/'
-        self.localCsvErrorPath = myPath + "/" + sftpPath + "/History/" + self.transformDate(dateNow) + '/CSV/Error_File/'
-        self.localPdfArchivePath = myPath + "/" + sftpPath + "/History/" + self.transformDate(dateNow) + '/PDF/Archived_File/'
-        self.localPdfErrorPath = myPath + "/" + sftpPath + "/History/" + self.transformDate(dateNow) + '/PDF/Error_File/'
-        self.localOutputPdfPath = myPath + "/" + sftpPath + "/Outbound/" + self.transformDate(dateNow) + '/PDF/'
-        self.localOutputXmlPath = myPath + "/" + sftpPath + "/Outbound/" + self.transformDate(dateNow) + '/XML/'
-        self.localLogPath = myPath + "/" + sftpPath + "/Outbound/" + self.transformDate(dateNow) + '/Logfile/'
+        self.localHistoryPath = myPath + "/" + sftpPath + "/History/"
+        self.localHistoryPathNow = self.localHistoryPath + self.transformDate(dateNow) + '/'
+        self.localCsvArchivePath = self.localHistoryPathNow + '/CSV/Archived_File/'
+        self.localCsvErrorPath = self.localHistoryPathNow + '/CSV/Error_File/'
+        self.localPdfArchivePath = self.localHistoryPathNow + '/PDF/Archived_File/'
+        self.localPdfErrorPath = self.localHistoryPathNow + '/PDF/Error_File/'
+        self.localOutputPath = myPath + "/" + sftpPath + "/Outbound/"
+        self.localOutputPdfPath = self.localOutputPath + self.transformDate(dateNow) + '/PDF/'
+        self.localOutputXmlPath = self.localOutputPath + self.transformDate(dateNow) + '/XML/'
+        self.localLogPath = self.localOutputPath + self.transformDate(dateNow) + '/Logfile/'
 
 ########## SET ############
     def setLocalPath(self,path):
         self.localPath = path
         return self.localPath
 
     def setLocalFileRun(self,path):
```

### Comparing `sftpoeb-0.1.2/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.1.3/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.2/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.1.3/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             try:
                 ### ทำการ copy file ไปไว้ที่ History และ ย้ายไป path local
                 shutil.copy(self.destination.destinationInbound + name + '.csv', self.local.getLocalHistory() + name + '.csv')
                 shutil.copy(self.destination.destinationInbound + name + '.csv', self.destination.getDestinationHistory() + name + '.csv')
                 shutil.move(self.destination.destinationInbound + name + '.csv', self.local.getLocalPathNow() + name + '.csv')  #### วนหยิบ PDF ตามชื่อ text ที่แตกดป็น 1:1 แล้ว
                 
                 ### นำส่งไฟล์ไปทำ E-Tax Invoice ผ่าน API
-                service = serviceSigning(self.payloadData, filename, name + '.pdf', self.local.getLocalPathNow() , 0, serviceCode,self.SERVICE_SIGNING_URL)
+                service = serviceSigning(self.payloadData, filename, self.local.getLocalPathNow() , 0, serviceCode,self.SERVICE_SIGNING_URL)
                 if service['status'] == 'OK':
                     self.success = self.success + 1
                     print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Service signing success.')
                     
                     save_pdf = saveFile(service['pdfURL'], self.local.getLocalOutputPdfPath(), name + '.pdf', 0)
                     if save_pdf['status'] == 'OK':
                         print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Save file.pdf success.')
```

### Comparing `sftpoeb-0.1.2/sftpoeb.egg-info/PKG-INFO` & `sftpoeb-0.1.3/sftpoeb.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.1.2
+Version: 0.1.3
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -63,7 +63,11 @@
 ------------------
 - Fixbug
 
 0.1.2 (15/06/2023)
 ------------------
 - Fixbug
 
+0.1.3 (16/06/2023)
+------------------
+- Process Recovery
+
```

### Comparing `sftpoeb-0.1.2/test.py` & `sftpoeb-0.1.3/test.py`

 * *Files identical despite different names*

