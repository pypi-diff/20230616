# Comparing `tmp/sftpoeb-0.1.3.tar.gz` & `tmp/sftpoeb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.1.3.tar", last modified: Fri Jun 16 11:13:19 2023, max compression
+gzip compressed data, was "sftpoeb-0.1.4.tar", last modified: Fri Jun 16 11:56:59 2023, max compression
```

## Comparing `sftpoeb-0.1.3.tar` & `sftpoeb-0.1.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.178984 sftpoeb-0.1.3/
--rw-rw-rw-   0        0        0      723 2023-06-16 11:13:16.000000 sftpoeb-0.1.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1145 2023-06-16 11:13:19.176592 sftpoeb-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.798568 sftpoeb-0.1.3/home/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.792567 sftpoeb-0.1.3/home/natthawut.th/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.793570 sftpoeb-0.1.3/home/natthawut.th/kpc.prd/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.794572 sftpoeb-0.1.3/home/natthawut.th/kpc.prd/kpc.prd/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.795573 sftpoeb-0.1.3/home/natthawut.th/kpc.prd/kpc.prd/Outbound/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.796571 sftpoeb-0.1.3/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.876711 sftpoeb-0.1.3/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/
--rw-rw-rw-   0        0        0      177 2023-06-15 12:04:47.000000 sftpoeb-0.1.3/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/20230615190447_log.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.799575 sftpoeb-0.1.3/home/sftp/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.800576 sftpoeb-0.1.3/home/sftp/kpc.prd/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.801570 sftpoeb-0.1.3/home/sftp/kpc.prd/kpc.prd/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.802568 sftpoeb-0.1.3/home/sftp/kpc.prd/kpc.prd/Outbound/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.803571 sftpoeb-0.1.3/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.881718 sftpoeb-0.1.3/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/
--rw-rw-rw-   0        0        0      177 2023-06-15 12:04:47.000000 sftpoeb-0.1.3/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/20230615190447_log.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 11:13:19.179553 sftpoeb-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-06-16 11:12:44.000000 sftpoeb-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.886720 sftpoeb-0.1.3/sftpoeb/
--rw-rw-rw-   0        0        0       72 2023-06-15 12:00:06.000000 sftpoeb-0.1.3/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.944712 sftpoeb-0.1.3/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.3/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.969724 sftpoeb-0.1.3/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0       48 2023-06-15 12:01:46.000000 sftpoeb-0.1.3/sftpoeb/mainclass/__init__.py
--rw-rw-rw-   0        0        0     8509 2023-06-16 11:06:25.000000 sftpoeb-0.1.3/sftpoeb/mainclass/c_recovery.py
--rw-rw-rw-   0        0        0     3558 2023-06-15 08:31:33.000000 sftpoeb-0.1.3/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.003710 sftpoeb-0.1.3/sftpoeb/method/
--rw-rw-rw-   0        0        0       95 2023-06-14 12:04:10.000000 sftpoeb-0.1.3/sftpoeb/method/__init__.py
--rw-rw-rw-   0        0        0     4800 2023-06-16 10:56:05.000000 sftpoeb-0.1.3/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      601 2023-06-14 06:57:02.000000 sftpoeb-0.1.3/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.3/sftpoeb/method/debug.py
--rw-rw-rw-   0        0        0     9657 2023-06-15 07:54:02.000000 sftpoeb-0.1.3/sftpoeb/method/mail.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.053854 sftpoeb-0.1.3/sftpoeb/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.3/sftpoeb/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.3/sftpoeb/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.3/sftpoeb/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.3/sftpoeb/sftpoeb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.057855 sftpoeb-0.1.3/sftpoeb/subclass/
--rw-rw-rw-   0        0        0      156 2023-06-16 04:43:20.000000 sftpoeb-0.1.3/sftpoeb/subclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.067858 sftpoeb-0.1.3/sftpoeb/subclass/alert/
--rw-rw-rw-   0        0        0       24 2023-06-15 07:57:29.000000 sftpoeb-0.1.3/sftpoeb/subclass/alert/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-06-15 11:41:55.000000 sftpoeb-0.1.3/sftpoeb/subclass/alert/s_c_alert.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.080858 sftpoeb-0.1.3/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.3/sftpoeb/subclass/file/__init__.py
--rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.3/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.3/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.088863 sftpoeb-0.1.3/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.3/sftpoeb/subclass/input/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.3/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.097857 sftpoeb-0.1.3/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.3/sftpoeb/subclass/output/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.3/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.115665 sftpoeb-0.1.3/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.3/sftpoeb/subclass/path/__init__.py
--rw-rw-rw-   0        0        0     5375 2023-06-16 03:46:50.000000 sftpoeb-0.1.3/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     4146 2023-06-16 03:40:25.000000 sftpoeb-0.1.3/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     2042 2023-06-15 11:58:34.000000 sftpoeb-0.1.3/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.144336 sftpoeb-0.1.3/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.1.3/sftpoeb/subclass/process/__init__.py
--rw-rw-rw-   0        0        0    30017 2023-06-16 10:56:17.000000 sftpoeb-0.1.3/sftpoeb/subclass/process/s_c_process_package_1.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:19.172689 sftpoeb-0.1.3/sftpoeb/subclass/recovery/
--rw-rw-rw-   0        0        0       27 2023-06-16 04:43:48.000000 sftpoeb-0.1.3/sftpoeb/subclass/recovery/__init__.py
--rw-rw-rw-   0        0        0    19301 2023-06-16 11:06:15.000000 sftpoeb-0.1.3/sftpoeb/subclass/recovery/s_c_recovery.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:13:18.941710 sftpoeb-0.1.3/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0     1145 2023-06-16 11:13:18.000000 sftpoeb-0.1.3/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1533 2023-06-16 11:13:18.000000 sftpoeb-0.1.3/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 11:13:18.000000 sftpoeb-0.1.3/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-06-16 11:13:18.000000 sftpoeb-0.1.3/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 11:13:18.000000 sftpoeb-0.1.3/sftpoeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1107 2023-06-15 08:22:57.000000 sftpoeb-0.1.3/test.py
--rw-rw-rw-   0        0        0     1133 2023-06-16 11:07:44.000000 sftpoeb-0.1.3/test_recovery.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.064041 sftpoeb-0.1.4/
+-rw-rw-rw-   0        0        0      808 2023-06-16 11:55:05.000000 sftpoeb-0.1.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1230 2023-06-16 11:56:59.063040 sftpoeb-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.903136 sftpoeb-0.1.4/home/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.899135 sftpoeb-0.1.4/home/natthawut.th/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.900135 sftpoeb-0.1.4/home/natthawut.th/kpc.prd/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.900135 sftpoeb-0.1.4/home/natthawut.th/kpc.prd/kpc.prd/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.901138 sftpoeb-0.1.4/home/natthawut.th/kpc.prd/kpc.prd/Outbound/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.902137 sftpoeb-0.1.4/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.941174 sftpoeb-0.1.4/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/
+-rw-rw-rw-   0        0        0      177 2023-06-15 12:04:47.000000 sftpoeb-0.1.4/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/20230615190447_log.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.903136 sftpoeb-0.1.4/home/sftp/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.904135 sftpoeb-0.1.4/home/sftp/kpc.prd/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.905137 sftpoeb-0.1.4/home/sftp/kpc.prd/kpc.prd/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.905137 sftpoeb-0.1.4/home/sftp/kpc.prd/kpc.prd/Outbound/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.906137 sftpoeb-0.1.4/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.943134 sftpoeb-0.1.4/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/
+-rw-rw-rw-   0        0        0      177 2023-06-15 12:04:47.000000 sftpoeb-0.1.4/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/20230615190447_log.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 11:56:59.065045 sftpoeb-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-06-16 11:56:43.000000 sftpoeb-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.946137 sftpoeb-0.1.4/sftpoeb/
+-rw-rw-rw-   0        0        0       72 2023-06-15 12:00:06.000000 sftpoeb-0.1.4/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.970137 sftpoeb-0.1.4/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.4/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.978136 sftpoeb-0.1.4/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0       48 2023-06-15 12:01:46.000000 sftpoeb-0.1.4/sftpoeb/mainclass/__init__.py
+-rw-rw-rw-   0        0        0    11520 2023-06-16 11:54:11.000000 sftpoeb-0.1.4/sftpoeb/mainclass/c_recovery.py
+-rw-rw-rw-   0        0        0     3558 2023-06-15 08:31:33.000000 sftpoeb-0.1.4/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.991138 sftpoeb-0.1.4/sftpoeb/method/
+-rw-rw-rw-   0        0        0       95 2023-06-14 12:04:10.000000 sftpoeb-0.1.4/sftpoeb/method/__init__.py
+-rw-rw-rw-   0        0        0     4800 2023-06-16 10:56:05.000000 sftpoeb-0.1.4/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      601 2023-06-14 06:57:02.000000 sftpoeb-0.1.4/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.4/sftpoeb/method/debug.py
+-rw-rw-rw-   0        0        0     9657 2023-06-15 07:54:02.000000 sftpoeb-0.1.4/sftpoeb/method/mail.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.002137 sftpoeb-0.1.4/sftpoeb/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.4/sftpoeb/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.4/sftpoeb/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.4/sftpoeb/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.4/sftpoeb/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.004135 sftpoeb-0.1.4/sftpoeb/subclass/
+-rw-rw-rw-   0        0        0      156 2023-06-16 04:43:20.000000 sftpoeb-0.1.4/sftpoeb/subclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.010135 sftpoeb-0.1.4/sftpoeb/subclass/alert/
+-rw-rw-rw-   0        0        0       24 2023-06-15 07:57:29.000000 sftpoeb-0.1.4/sftpoeb/subclass/alert/__init__.py
+-rw-rw-rw-   0        0        0     1515 2023-06-15 11:41:55.000000 sftpoeb-0.1.4/sftpoeb/subclass/alert/s_c_alert.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.018137 sftpoeb-0.1.4/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.4/sftpoeb/subclass/file/__init__.py
+-rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.4/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.4/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.024137 sftpoeb-0.1.4/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.4/sftpoeb/subclass/input/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.4/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.032139 sftpoeb-0.1.4/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.4/sftpoeb/subclass/output/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.4/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.047137 sftpoeb-0.1.4/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.4/sftpoeb/subclass/path/__init__.py
+-rw-rw-rw-   0        0        0     5375 2023-06-16 03:46:50.000000 sftpoeb-0.1.4/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     4154 2023-06-16 11:18:57.000000 sftpoeb-0.1.4/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     2042 2023-06-15 11:58:34.000000 sftpoeb-0.1.4/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.053138 sftpoeb-0.1.4/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.1.4/sftpoeb/subclass/process/__init__.py
+-rw-rw-rw-   0        0        0    30017 2023-06-16 10:56:17.000000 sftpoeb-0.1.4/sftpoeb/subclass/process/s_c_process_package_1.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.060040 sftpoeb-0.1.4/sftpoeb/subclass/recovery/
+-rw-rw-rw-   0        0        0       27 2023-06-16 04:43:48.000000 sftpoeb-0.1.4/sftpoeb/subclass/recovery/__init__.py
+-rw-rw-rw-   0        0        0    21628 2023-06-16 11:42:28.000000 sftpoeb-0.1.4/sftpoeb/subclass/recovery/s_c_recovery.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.968137 sftpoeb-0.1.4/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0     1230 2023-06-16 11:56:58.000000 sftpoeb-0.1.4/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1533 2023-06-16 11:56:58.000000 sftpoeb-0.1.4/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 11:56:58.000000 sftpoeb-0.1.4/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-16 11:56:58.000000 sftpoeb-0.1.4/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 11:56:58.000000 sftpoeb-0.1.4/sftpoeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1107 2023-06-15 08:22:57.000000 sftpoeb-0.1.4/test.py
+-rw-rw-rw-   0        0        0     1150 2023-06-16 11:54:21.000000 sftpoeb-0.1.4/test_recovery.py
```

### Comparing `sftpoeb-0.1.3/CHANGELOG.txt` & `sftpoeb-0.1.4/CHANGELOG.txt`

 * *Files 14% similar despite different names*

```diff
@@ -47,8 +47,13 @@
 
 0.1.2 (15/06/2023)
 ------------------
 - Fixbug
 
 0.1.3 (16/06/2023)
 ------------------
-- Process Recovery
+- Process Recovery
+
+0.1.4 (16/06/2023)
+------------------
+- Process Recovery all
+- Fixbux variable
```

### Comparing `sftpoeb-0.1.3/LICENSE.txt` & `sftpoeb-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/PKG-INFO` & `sftpoeb-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.1.3
+Version: 0.1.4
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -67,7 +67,12 @@
 ------------------
 - Fixbug
 
 0.1.3 (16/06/2023)
 ------------------
 - Process Recovery
 
+0.1.4 (16/06/2023)
+------------------
+- Process Recovery all
+- Fixbux variable
+
```

### Comparing `sftpoeb-0.1.3/sftpoeb/mainclass/c_recovery.py` & `sftpoeb-0.1.4/sftpoeb/mainclass/c_recovery.py`

 * *Files 14% similar despite different names*

```diff
@@ -91,14 +91,15 @@
             result = {"status": "OK", "message": "Process Recovery done."}
         except Exception as e:
             print(str(self.dateNow + self.timeNow) + '>> API Recovery error : ' + str(debug_row(e)))
             result = {"status": "ER","errorCode":"PR999", "errorMessage": 'API Recovery error : '+str(debug_row(e))}
 
     def sign(self):
         try:
+            ### Get List Folder To Recovery
             pending_folder_sign = [jsd for jsd in listdir(self.recovery.recoveryPathSign) if isdir(join(self.recovery.recoveryPathSign, jsd))]
             if len(pending_folder_sign) > 0:
                 for folder_sign in pending_folder_sign:
                     ### Folder to do now in this round
                     recovery_pathsign_now = self.recovery.recoveryPathSign + folder_sign + '/'
                     print("recovery_pathsign_now -> " , recovery_pathsign_now)
                     ### List File to do in this round
@@ -132,8 +133,54 @@
                         pool.close()
                         pool.join()
                         
             print(str(self.dateNow + self.timeNow) + '>> API Recovery : Process Recovery done.')
             result = {"status": "OK", "message": "Process Recovery done."}
         except Exception as e:
             print(str(self.dateNow + self.timeNow) + '>> API Recovery error : ' + str(debug_row(e)))
-            result = {"status": "ER","errorCode":"PR999", "errorMessage": 'API Recovery error : '+str(debug_row(e))}
+            result = {"status": "ER","errorCode":"PR999", "errorMessage": 'API Recovery error : '+str(debug_row(e))}
+
+    def save(self):
+        try:
+            ### Get List Folder To Recovery
+            pending_folder_save = [jsd for jsd in listdir(self.recovery.recoveryPathSave) if isdir(join(self.recovery.recoveryPathSave, jsd))]
+            if len(pending_folder_save) > 0:
+                for folder_save in pending_folder_save:
+                    ### Folder to do now in this round
+                    recovery_pathsave_now = self.recovery.recoveryPathSave + folder_save + '/'
+                    print("recovery_pathsave_now -> " , recovery_pathsave_now)
+                    ### List File to do in this round
+                    pending_save = [jsf for jsf in listdir(recovery_pathsave_now) if isfile(join(recovery_pathsave_now, jsf))]
+                    print("List File to do in this round -> " , pending_save)
+                    if len(pending_save) > 0:
+                        ### SetPath To Use
+                        local_path_output = self.local.localOutputPath + pending_save + '/'
+                        remote_path_output = self.destination.getDestinationPath()
+                        check_path(local_path_output)
+                        path_history = self.local.localHistoryPath + folder_save + "/"
+                        check_path(path_history)
+                        path_recover_save_now = self.recovery.recoveryPathSave + folder_save + "/" + self.process_now + "/"
+                        check_path(path_recover_save_now)
+
+                        ### Move File To Recovery Temp Now
+                        for file_check in pending_save:
+                            shutil.move(recovery_pathsave_now + file_check , path_recover_save_now+file_check)
+
+                        ### Get List File To Recovery Now
+                        all_check = [ac for ac in listdir(path_recover_save_now) if isfile(join(path_recover_save_now, ac))]
+
+                        ### Thread Process Reovery
+                        pool = ThreadPool(3)
+                        func = partial(self.recovery_process.recover_save , 
+                                       recovery_pathsave_now,
+                                       self.recovery.recoveryPath , 
+                                       path_recover_save_now , local_path_output , 
+                                       remote_path_output , folder_save , self.timeNow , path_history)
+                        pool.map(func, all_check)
+                        pool.close()
+                        pool.join()
+                        
+            print(str(self.dateNow + self.timeNow) + '>> API Recovery : Process Recovery done.')
+            result = {"status": "OK", "message": "Process Recovery done."}
+        except Exception as e:
+            print(str(self.dateNow + self.timeNow) + '>> API Recovery error : ' + str(debug_row(e)))
+            result = {"status": "ER","errorCode":"PR999", "errorMessage": 'API Recovery error : '+str(debug_row(e))}
```

### Comparing `sftpoeb-0.1.3/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.1.4/sftpoeb/mainclass/c_sftp.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/sftpoeb/method/callservice.py` & `sftpoeb-0.1.4/sftpoeb/method/callservice.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/sftpoeb/method/checkpath.py` & `sftpoeb-0.1.4/sftpoeb/method/checkpath.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/sftpoeb/method/mail.py` & `sftpoeb-0.1.4/sftpoeb/method/mail.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/sftpoeb/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.1.4/sftpoeb/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/sftpoeb/subclass/alert/s_c_alert.py` & `sftpoeb-0.1.4/sftpoeb/subclass/alert/s_c_alert.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.1.4/sftpoeb/subclass/file/s_c_file.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.1.4/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.1.4/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.1.4/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.1.4/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.1.4/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,16 @@
         self.localLogPath = path
         return self.localLogPath
     
 ########## END SET ############
 
 ########## GET ############
     def getLocalHistory(self):
-        check_path(self.localHistory)
-        return self.localHistory
+        check_path(self.localHistoryPath)
+        return self.localHistoryPath
 
     def getLocalPath(self):
         check_path(self.localPath)
         return self.localPath
 
     def getLocalFileRun(self):
         check_path(self.localFilerun)
```

### Comparing `sftpoeb-0.1.3/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.1.4/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.1.4/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/sftpoeb/subclass/recovery/s_c_recovery.py` & `sftpoeb-0.1.4/sftpoeb/subclass/recovery/s_c_recovery.py`

 * *Files 11% similar despite different names*

```diff
@@ -246,8 +246,40 @@
                 self.losemessage.append({
                     'InvoiceName': str(name),
                     'Process DTM': str(date_now + time_now),
                     'errorCode': 'ER888',
                     'errorMessage': 'Failed to Generate Invoice. : ' + str(e)
                 })
 
-    
+    def recover_save(self, path_recover_save, path_save_now, output_local_path, output_remote_path, date_now, time_now, file):
+        try:
+            filename = str(file.split('.')[0])
+            recover_data = json.loads(open(path_save_now + '/' + file, 'r', encoding='UTF-8').read())
+            transactionCode = str(recover_data["transactionCode"])
+            recheck_trans = checkStatus(self.payload,transactionCode, 0)
+            if recheck_trans["status"] == "OK":
+                save_pdf = saveFile(recheck_trans['pdfURL'], output_local_path + '/PDF/', filename+'.pdf', 0)
+                if save_pdf["status"] == "OK":
+                    print(str(date_now + time_now) + '>> ' + filename + ' Save PDF success.')
+                    shutil.copy(output_local_path + '/PDF/' + filename + '.pdf', output_remote_path + '/PDF/' + filename + '.pdf')
+                    print(str(date_now + time_now) + '>> ' + str(filename) + ' Put file.pdf success.')
+                    output_pdf = True
+                else:
+                    output_pdf = False
+                    print(str(date_now + time_now) + '>> ' + filename + ' Save PDF fail. : ' + str(save_pdf["errorMessage"]))
+                save_xml = saveFile(recheck_trans['xmlURL'], output_local_path + '/XML/', filename+'.xml', 0)
+                if save_xml["status"] == "OK":
+                    print(str(date_now + time_now) + '>> ' + filename + ' Save XML success.')
+                    shutil.copy(output_local_path + '/XML/' + filename + '.xml', output_remote_path + '/XML/' + filename + '.xml')
+                    print(str(date_now + time_now) + '>> ' + str(filename) + ' Put file.pdf success.')
+                    output_xml = True
+                else:
+                    output_xml = False
+                    print(str(date_now + time_now) + '>> ' + filename + ' Save XML fail. : ' + str(save_xml["errorMessage"]))
+                if not output_pdf or not output_xml:
+                    shutil.move(path_save_now + file, path_recover_save + file)
+                else:
+                    os.remove(path_save_now+'/'+file)
+            else:
+                shutil.move(path_save_now + file, path_recover_save + file)
+        except Exception:
+            shutil.move(path_save_now + file, path_recover_save + file)
```

### Comparing `sftpoeb-0.1.3/sftpoeb.egg-info/PKG-INFO` & `sftpoeb-0.1.4/sftpoeb.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.1.3
+Version: 0.1.4
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -67,7 +67,12 @@
 ------------------
 - Fixbug
 
 0.1.3 (16/06/2023)
 ------------------
 - Process Recovery
 
+0.1.4 (16/06/2023)
+------------------
+- Process Recovery all
+- Fixbux variable
+
```

### Comparing `sftpoeb-0.1.3/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.1.4/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/test.py` & `sftpoeb-0.1.4/test.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.3/test_recovery.py` & `sftpoeb-0.1.4/test_recovery.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 sftpPath = ''
 
 
 ### เรียกคลาส SFTP
 recovery = c_recovery.RECOVERY(myPath,sftpPath,custPath,payloadData)
 recovery.alert.setReceiverMail(payloadData["receiver_mail"])
 recovery.check()
-recovery.sign()
+recovery.sign()
+recovery.save()
```

