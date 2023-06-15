# Comparing `tmp/oracledb-1.3.1.tar.gz` & `tmp/oracledb-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oracledb-1.3.1.tar", last modified: Mon Apr 24 20:03:36 2023, max compression
+gzip compressed data, was "oracledb-1.3.2.tar", last modified: Thu Jun 15 21:34:23 2023, max compression
```

## Comparing `oracledb-1.3.1.tar` & `oracledb-1.3.2.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.231150 oracledb-1.3.1/
--rw-rw-r--   0 anthony   (1030) users      (100)    12570 2023-04-21 18:03:32.000000 oracledb-1.3.1/LICENSE.txt
--rw-r--r--   0 anthony   (1030) users      (100)      398 2022-05-20 21:47:15.000000 oracledb-1.3.1/MANIFEST.in
--rw-r--r--   0 anthony   (1030) users      (100)       56 2022-05-20 21:47:15.000000 oracledb-1.3.1/NOTICE.txt
--rw-rw-r--   0 anthony   (1030) users      (100)     5062 2023-04-24 20:03:36.231150 oracledb-1.3.1/PKG-INFO
--rw-r--r--   0 anthony   (1030) users      (100)      167 2022-05-20 21:47:15.000000 oracledb-1.3.1/README.txt
--rw-r--r--   0 anthony   (1030) users      (100)    28104 2022-05-20 21:47:15.000000 oracledb-1.3.1/THIRD_PARTY_LICENSES.txt
--rw-r--r--   0 anthony   (1030) users      (100)      110 2022-05-20 21:47:15.000000 oracledb-1.3.1/pyproject.toml
--rw-r--r--   0 anthony   (1030) users      (100)     1603 2023-04-24 20:03:36.231150 oracledb-1.3.1/setup.cfg
--rw-r--r--   0 anthony   (1030) users      (100)     3990 2022-08-27 22:13:47.000000 oracledb-1.3.1/setup.py
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.216151 oracledb-1.3.1/src/
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.220151 oracledb-1.3.1/src/oracledb/
--rw-rw-r--   0 anthony   (1030) users      (100)     5922 2023-03-27 21:56:43.000000 oracledb-1.3.1/src/oracledb/__init__.py
--rw-rw-r--   0 anthony   (1030) users      (100)    19013 2023-03-27 21:56:43.000000 oracledb-1.3.1/src/oracledb/aq.py
--rw-rw-r--   0 anthony   (1030) users      (100)    14703 2023-03-21 21:27:13.000000 oracledb-1.3.1/src/oracledb/base_impl.pxd
--rw-r--r--   0 anthony   (1030) users      (100)     5404 2022-08-27 17:10:23.000000 oracledb-1.3.1/src/oracledb/base_impl.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    31296 2023-03-27 21:31:03.000000 oracledb-1.3.1/src/oracledb/connect_params.py
--rw-rw-r--   0 anthony   (1030) users      (100)    49238 2023-03-27 21:57:19.000000 oracledb-1.3.1/src/oracledb/connection.py
--rw-r--r--   0 anthony   (1030) users      (100)     4070 2023-01-18 17:02:00.000000 oracledb-1.3.1/src/oracledb/constants.py
--rw-r--r--   0 anthony   (1030) users      (100)     2909 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/constructors.py
--rw-rw-r--   0 anthony   (1030) users      (100)    35219 2023-03-27 21:57:07.000000 oracledb-1.3.1/src/oracledb/cursor.py
--rw-rw-r--   0 anthony   (1030) users      (100)    11850 2023-03-27 21:56:43.000000 oracledb-1.3.1/src/oracledb/dbobject.py
--rw-r--r--   0 anthony   (1030) users      (100)     1827 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/defaults.py
--rw-r--r--   0 anthony   (1030) users      (100)     5403 2022-09-28 15:14:10.000000 oracledb-1.3.1/src/oracledb/driver_mode.py
--rw-r--r--   0 anthony   (1030) users      (100)     3130 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/dsn.py
--rw-rw-r--   0 anthony   (1030) users      (100)    21982 2023-03-29 03:54:03.000000 oracledb-1.3.1/src/oracledb/errors.py
--rw-r--r--   0 anthony   (1030) users      (100)     1811 2022-06-10 02:53:08.000000 oracledb-1.3.1/src/oracledb/exceptions.py
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.217151 oracledb-1.3.1/src/oracledb/impl/
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.222151 oracledb-1.3.1/src/oracledb/impl/base/
--rw-r--r--   0 anthony   (1030) users      (100)     7341 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/base/bind_var.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    37428 2023-03-27 21:31:03.000000 oracledb-1.3.1/src/oracledb/impl/base/connect_params.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    11765 2022-11-01 20:32:06.000000 oracledb-1.3.1/src/oracledb/impl/base/connection.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    18951 2022-07-29 21:22:34.000000 oracledb-1.3.1/src/oracledb/impl/base/cursor.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     4808 2022-11-01 20:32:06.000000 oracledb-1.3.1/src/oracledb/impl/base/dbobject.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     2741 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/base/lob.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     4215 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/base/pool.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     4420 2022-08-02 17:00:32.000000 oracledb-1.3.1/src/oracledb/impl/base/pool_params.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     6379 2022-08-27 21:55:16.000000 oracledb-1.3.1/src/oracledb/impl/base/queue.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     4657 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/base/soda.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     1933 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/base/subscr.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)     8439 2023-03-21 21:27:13.000000 oracledb-1.3.1/src/oracledb/impl/base/types.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     8646 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/base/utils.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    12993 2023-01-18 23:20:15.000000 oracledb-1.3.1/src/oracledb/impl/base/var.pyx
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.223151 oracledb-1.3.1/src/oracledb/impl/thick/
--rw-r--r--   0 anthony   (1030) users      (100)     2256 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/thick/buffer.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    25954 2022-11-07 17:33:47.000000 oracledb-1.3.1/src/oracledb/impl/thick/connection.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    19732 2022-08-02 15:15:52.000000 oracledb-1.3.1/src/oracledb/impl/thick/cursor.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    13927 2022-11-01 20:32:06.000000 oracledb-1.3.1/src/oracledb/impl/thick/dbobject.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     9330 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/thick/json.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     7534 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/thick/lob.pyx
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.217151 oracledb-1.3.1/src/oracledb/impl/thick/odpi/
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.223151 oracledb-1.3.1/src/oracledb/impl/thick/odpi/embed/
--rw-r--r--   0 anthony   (1030) users      (100)     2569 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/embed/dpi.c
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.223151 oracledb-1.3.1/src/oracledb/impl/thick/odpi/include/
--rw-rw-r--   0 anthony   (1030) users      (100)    82859 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/include/dpi.h
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.226151 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/
--rw-rw-r--   0 anthony   (1030) users      (100)   113814 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiConn.c
--rw-rw-r--   0 anthony   (1030) users      (100)    16638 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiContext.c
--rw-r--r--   0 anthony   (1030) users      (100)    34806 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiData.c
--rw-r--r--   0 anthony   (1030) users      (100)     7443 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiDebug.c
--rw-r--r--   0 anthony   (1030) users      (100)    15574 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c
--rw-r--r--   0 anthony   (1030) users      (100)     7552 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c
--rw-r--r--   0 anthony   (1030) users      (100)     9569 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiEnv.c
--rw-r--r--   0 anthony   (1030) users      (100)    12063 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiError.c
--rw-rw-r--   0 anthony   (1030) users      (100)     9018 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h
--rw-r--r--   0 anthony   (1030) users      (100)    13052 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiGen.c
--rw-r--r--   0 anthony   (1030) users      (100)    15039 2022-11-07 17:19:09.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiGlobal.c
--rw-r--r--   0 anthony   (1030) users      (100)     5184 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiHandleList.c
--rw-r--r--   0 anthony   (1030) users      (100)     5399 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c
--rw-rw-r--   0 anthony   (1030) users      (100)   107983 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiImpl.h
--rw-rw-r--   0 anthony   (1030) users      (100)    35246 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiJson.c
--rw-r--r--   0 anthony   (1030) users      (100)    19751 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiLob.c
--rw-r--r--   0 anthony   (1030) users      (100)    23232 2022-08-27 21:56:08.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c
--rw-r--r--   0 anthony   (1030) users      (100)    40061 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiObject.c
--rw-r--r--   0 anthony   (1030) users      (100)     4894 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c
--rw-rw-r--   0 anthony   (1030) users      (100)    14713 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiObjectType.c
--rw-r--r--   0 anthony   (1030) users      (100)   179729 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiOci.c
--rw-r--r--   0 anthony   (1030) users      (100)    26914 2022-11-01 20:30:53.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiOracleType.c
--rw-r--r--   0 anthony   (1030) users      (100)    32638 2022-08-02 17:00:34.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiPool.c
--rw-r--r--   0 anthony   (1030) users      (100)    23678 2022-08-27 21:56:08.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiQueue.c
--rw-r--r--   0 anthony   (1030) users      (100)     5712 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiRowid.c
--rw-rw-r--   0 anthony   (1030) users      (100)    39581 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c
--rw-r--r--   0 anthony   (1030) users      (100)     6131 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c
--rw-r--r--   0 anthony   (1030) users      (100)    17459 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c
--rw-r--r--   0 anthony   (1030) users      (100)     9371 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c
--rw-r--r--   0 anthony   (1030) users      (100)     6134 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c
--rw-r--r--   0 anthony   (1030) users      (100)    78753 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiStmt.c
--rw-r--r--   0 anthony   (1030) users      (100)    29091 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSubscr.c
--rw-r--r--   0 anthony   (1030) users      (100)    23589 2022-11-01 20:30:53.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiUtils.c
--rw-r--r--   0 anthony   (1030) users      (100)    78379 2022-06-09 19:44:20.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiVar.c
--rw-r--r--   0 anthony   (1030) users      (100)    39137 2022-11-01 20:23:41.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi.pxd
--rw-r--r--   0 anthony   (1030) users      (100)    13694 2022-11-18 03:37:36.000000 oracledb-1.3.1/src/oracledb/impl/thick/pool.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    21424 2022-10-18 22:30:30.000000 oracledb-1.3.1/src/oracledb/impl/thick/queue.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    24041 2022-12-01 00:47:06.000000 oracledb-1.3.1/src/oracledb/impl/thick/soda.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     7249 2022-12-01 00:47:47.000000 oracledb-1.3.1/src/oracledb/impl/thick/subscr.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    21952 2023-03-21 21:27:13.000000 oracledb-1.3.1/src/oracledb/impl/thick/utils.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    11462 2022-11-01 20:34:31.000000 oracledb-1.3.1/src/oracledb/impl/thick/var.pyx
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.228150 oracledb-1.3.1/src/oracledb/impl/thin/
--rw-rw-r--   0 anthony   (1030) users      (100)    49673 2023-03-29 03:54:03.000000 oracledb-1.3.1/src/oracledb/impl/thin/buffer.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)     5330 2023-03-27 21:55:41.000000 oracledb-1.3.1/src/oracledb/impl/thin/capabilities.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    16804 2023-03-27 21:46:22.000000 oracledb-1.3.1/src/oracledb/impl/thin/connection.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    23238 2023-03-29 03:54:03.000000 oracledb-1.3.1/src/oracledb/impl/thin/constants.pxi
--rw-r--r--   0 anthony   (1030) users      (100)     7681 2022-10-18 22:29:50.000000 oracledb-1.3.1/src/oracledb/impl/thin/conversions.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     6194 2022-10-18 22:33:19.000000 oracledb-1.3.1/src/oracledb/impl/thin/crypto.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)     8773 2023-04-21 18:03:32.000000 oracledb-1.3.1/src/oracledb/impl/thin/cursor.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    23713 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/thin/data_types.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    41584 2023-03-21 23:24:10.000000 oracledb-1.3.1/src/oracledb/impl/thin/dbobject.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)     7553 2023-03-21 23:24:10.000000 oracledb-1.3.1/src/oracledb/impl/thin/lob.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    98072 2023-04-21 18:03:32.000000 oracledb-1.3.1/src/oracledb/impl/thin/messages.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    26238 2023-03-29 03:53:29.000000 oracledb-1.3.1/src/oracledb/impl/thin/oson.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    27772 2023-03-21 23:24:10.000000 oracledb-1.3.1/src/oracledb/impl/thin/packet.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    20678 2023-04-21 18:03:32.000000 oracledb-1.3.1/src/oracledb/impl/thin/pool.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    20265 2023-03-21 21:27:13.000000 oracledb-1.3.1/src/oracledb/impl/thin/protocol.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    10891 2023-04-21 18:03:32.000000 oracledb-1.3.1/src/oracledb/impl/thin/statement.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     5869 2023-01-18 23:19:35.000000 oracledb-1.3.1/src/oracledb/impl/thin/utils.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     5445 2022-10-18 22:29:50.000000 oracledb-1.3.1/src/oracledb/impl/thin/var.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)     6078 2023-03-27 21:56:43.000000 oracledb-1.3.1/src/oracledb/lob.py
--rw-rw-r--   0 anthony   (1030) users      (100)    35074 2023-03-27 21:31:03.000000 oracledb-1.3.1/src/oracledb/pool.py
--rw-r--r--   0 anthony   (1030) users      (100)    31290 2022-09-28 15:08:47.000000 oracledb-1.3.1/src/oracledb/pool_params.py
--rw-r--r--   0 anthony   (1030) users      (100)        0 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/py.typed
--rw-rw-r--   0 anthony   (1030) users      (100)    27454 2023-03-27 21:56:43.000000 oracledb-1.3.1/src/oracledb/soda.py
--rw-r--r--   0 anthony   (1030) users      (100)    11078 2022-12-01 00:48:14.000000 oracledb-1.3.1/src/oracledb/subscr.py
--rw-r--r--   0 anthony   (1030) users      (100)     3130 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/thick_impl.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)     3758 2023-03-21 23:24:10.000000 oracledb-1.3.1/src/oracledb/thin_impl.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     3382 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/utils.py
--rw-rw-r--   0 anthony   (1030) users      (100)     6393 2023-03-27 21:56:43.000000 oracledb-1.3.1/src/oracledb/var.py
--rw-rw-r--   0 anthony   (1030) users      (100)     1533 2023-04-21 18:03:32.000000 oracledb-1.3.1/src/oracledb/version.py
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.220151 oracledb-1.3.1/src/oracledb.egg-info/
--rw-r--r--   0 anthony   (1030) users      (100)     5062 2023-04-24 20:03:36.000000 oracledb-1.3.1/src/oracledb.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1030) users      (100)     5443 2023-04-24 20:03:36.000000 oracledb-1.3.1/src/oracledb.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1030) users      (100)        1 2023-04-24 20:03:36.000000 oracledb-1.3.1/src/oracledb.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1030) users      (100)        1 2023-01-19 17:26:29.000000 oracledb-1.3.1/src/oracledb.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1030) users      (100)       20 2023-04-24 20:03:36.000000 oracledb-1.3.1/src/oracledb.egg-info/requires.txt
--rw-r--r--   0 anthony   (1030) users      (100)        9 2023-04-24 20:03:36.000000 oracledb-1.3.1/src/oracledb.egg-info/top_level.txt
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.231150 oracledb-1.3.1/tests/
--rw-rw-r--   0 anthony   (1030) users      (100)     2368 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/create_schema.py
--rw-r--r--   0 anthony   (1030) users      (100)     1928 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/drop_schema.py
--rw-r--r--   0 anthony   (1030) users      (100)     7093 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_1000_module.py
--rw-rw-r--   0 anthony   (1030) users      (100)    25407 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_1100_connection.py
--rw-rw-r--   0 anthony   (1030) users      (100)    13372 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_1300_cursor_var.py
--rw-r--r--   0 anthony   (1030) users      (100)    11560 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_1400_datetime_var.py
--rw-rw-r--   0 anthony   (1030) users      (100)     9367 2023-03-21 21:27:13.000000 oracledb-1.3.1/tests/test_1500_types.py
--rw-rw-r--   0 anthony   (1030) users      (100)    19283 2023-03-29 03:49:45.000000 oracledb-1.3.1/tests/test_1600_dml_returning.py
--rw-rw-r--   0 anthony   (1030) users      (100)     3785 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_1700_error.py
--rw-r--r--   0 anthony   (1030) users      (100)     8251 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_1800_interval_var.py
--rw-r--r--   0 anthony   (1030) users      (100)    20023 2022-08-02 17:00:32.000000 oracledb-1.3.1/tests/test_1900_lob_var.py
--rw-r--r--   0 anthony   (1030) users      (100)     5306 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_2000_long_var.py
--rw-r--r--   0 anthony   (1030) users      (100)    11357 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_2100_nchar_var.py
--rw-r--r--   0 anthony   (1030) users      (100)    21431 2022-11-01 21:30:49.000000 oracledb-1.3.1/tests/test_2200_number_var.py
--rw-rw-r--   0 anthony   (1030) users      (100)    25820 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_2300_object_var.py
--rw-rw-r--   0 anthony   (1030) users      (100)    35040 2023-03-21 21:27:13.000000 oracledb-1.3.1/tests/test_2400_pool.py
--rw-r--r--   0 anthony   (1030) users      (100)    21339 2022-11-07 17:27:30.000000 oracledb-1.3.1/tests/test_2500_string_var.py
--rw-r--r--   0 anthony   (1030) users      (100)     7896 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_2600_timestamp_var.py
--rw-rw-r--   0 anthony   (1030) users      (100)    23955 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_2700_aq.py
--rw-r--r--   0 anthony   (1030) users      (100)     7672 2022-08-27 21:55:16.000000 oracledb-1.3.1/tests/test_2800_bulk_aq.py
--rw-r--r--   0 anthony   (1030) users      (100)     7813 2022-10-18 22:31:58.000000 oracledb-1.3.1/tests/test_2900_rowid.py
--rw-r--r--   0 anthony   (1030) users      (100)     7971 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_3000_subscription.py
--rw-r--r--   0 anthony   (1030) users      (100)     3943 2023-01-18 17:02:49.000000 oracledb-1.3.1/tests/test_3100_boolean_var.py
--rw-rw-r--   0 anthony   (1030) users      (100)    24905 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_3200_features_12_1.py
--rw-r--r--   0 anthony   (1030) users      (100)     5670 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_3300_soda_database.py
--rw-r--r--   0 anthony   (1030) users      (100)    21475 2022-09-29 00:05:59.000000 oracledb-1.3.1/tests/test_3400_soda_collection.py
--rw-rw-r--   0 anthony   (1030) users      (100)    10520 2023-03-21 23:24:10.000000 oracledb-1.3.1/tests/test_3500_json.py
--rw-rw-r--   0 anthony   (1030) users      (100)    25036 2023-03-21 21:27:13.000000 oracledb-1.3.1/tests/test_3600_outputtypehandler.py
--rw-rw-r--   0 anthony   (1030) users      (100)    20995 2023-03-21 23:24:10.000000 oracledb-1.3.1/tests/test_3700_var.py
--rw-r--r--   0 anthony   (1030) users      (100)    10197 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_3800_typehandler.py
--rw-rw-r--   0 anthony   (1030) users      (100)    16463 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_3900_cursor_execute.py
--rw-r--r--   0 anthony   (1030) users      (100)    13808 2022-07-29 21:22:34.000000 oracledb-1.3.1/tests/test_4000_cursor_executemany.py
--rw-r--r--   0 anthony   (1030) users      (100)     6304 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_4100_cursor_callproc.py
--rw-r--r--   0 anthony   (1030) users      (100)    10122 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_4200_cursor_scrollable.py
--rw-rw-r--   0 anthony   (1030) users      (100)    43164 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_4300_cursor_other.py
--rw-r--r--   0 anthony   (1030) users      (100)     5200 2022-11-07 16:22:37.000000 oracledb-1.3.1/tests/test_4400_tpc.py
--rw-rw-r--   0 anthony   (1030) users      (100)    30813 2023-03-27 21:31:03.000000 oracledb-1.3.1/tests/test_4500_connect_params.py
--rw-r--r--   0 anthony   (1030) users      (100)     9049 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_4600_type_changes.py
--rw-r--r--   0 anthony   (1030) users      (100)     2746 2022-08-27 17:02:29.000000 oracledb-1.3.1/tests/test_4700_pool_params.py
--rw-rw-r--   0 anthony   (1030) users      (100)     7614 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_4800_timestamp_ltz_var.py
--rw-r--r--   0 anthony   (1030) users      (100)     7315 2022-06-10 16:31:07.000000 oracledb-1.3.1/tests/test_4900_timestamp_tz_var.py
--rw-r--r--   0 anthony   (1030) users      (100)    11969 2022-08-02 17:00:32.000000 oracledb-1.3.1/tests/test_5000_externalauth.py
--rw-rw-r--   0 anthony   (1030) users      (100)    15525 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_env.py
--rw-r--r--   0 anthony   (1030) users      (100)      593 2022-12-01 16:31:07.000000 oracledb-1.3.1/tox.ini
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-06-15 21:34:23.771717 oracledb-1.3.2/
+-rw-rw-r--   0 anthony   (1030) users      (100)    12570 2023-04-21 18:03:32.000000 oracledb-1.3.2/LICENSE.txt
+-rw-r--r--   0 anthony   (1030) users      (100)      398 2022-05-20 21:47:15.000000 oracledb-1.3.2/MANIFEST.in
+-rw-r--r--   0 anthony   (1030) users      (100)       56 2022-05-20 21:47:15.000000 oracledb-1.3.2/NOTICE.txt
+-rw-rw-r--   0 anthony   (1030) users      (100)     5062 2023-06-15 21:34:23.772717 oracledb-1.3.2/PKG-INFO
+-rw-r--r--   0 anthony   (1030) users      (100)      167 2022-05-20 21:47:15.000000 oracledb-1.3.2/README.txt
+-rw-r--r--   0 anthony   (1030) users      (100)    28104 2022-05-20 21:47:15.000000 oracledb-1.3.2/THIRD_PARTY_LICENSES.txt
+-rw-r--r--   0 anthony   (1030) users      (100)      110 2022-05-20 21:47:15.000000 oracledb-1.3.2/pyproject.toml
+-rw-r--r--   0 anthony   (1030) users      (100)     1603 2023-06-15 21:34:23.772717 oracledb-1.3.2/setup.cfg
+-rw-r--r--   0 anthony   (1030) users      (100)     3990 2022-08-27 22:13:47.000000 oracledb-1.3.2/setup.py
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-06-15 21:34:23.757717 oracledb-1.3.2/src/
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-06-15 21:34:23.761717 oracledb-1.3.2/src/oracledb/
+-rw-rw-r--   0 anthony   (1030) users      (100)     5922 2023-03-27 21:56:43.000000 oracledb-1.3.2/src/oracledb/__init__.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    19013 2023-03-27 21:56:43.000000 oracledb-1.3.2/src/oracledb/aq.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    14703 2023-03-21 21:27:13.000000 oracledb-1.3.2/src/oracledb/base_impl.pxd
+-rw-r--r--   0 anthony   (1030) users      (100)     5404 2022-08-27 17:10:23.000000 oracledb-1.3.2/src/oracledb/base_impl.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    31296 2023-03-27 21:31:03.000000 oracledb-1.3.2/src/oracledb/connect_params.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    49238 2023-06-15 20:44:06.000000 oracledb-1.3.2/src/oracledb/connection.py
+-rw-r--r--   0 anthony   (1030) users      (100)     4070 2023-01-18 17:02:00.000000 oracledb-1.3.2/src/oracledb/constants.py
+-rw-r--r--   0 anthony   (1030) users      (100)     2909 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/constructors.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    35219 2023-03-27 21:57:07.000000 oracledb-1.3.2/src/oracledb/cursor.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    11850 2023-06-15 20:44:06.000000 oracledb-1.3.2/src/oracledb/dbobject.py
+-rw-r--r--   0 anthony   (1030) users      (100)     1827 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/defaults.py
+-rw-r--r--   0 anthony   (1030) users      (100)     5403 2022-09-28 15:14:10.000000 oracledb-1.3.2/src/oracledb/driver_mode.py
+-rw-r--r--   0 anthony   (1030) users      (100)     3130 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/dsn.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    22020 2023-06-15 20:52:32.000000 oracledb-1.3.2/src/oracledb/errors.py
+-rw-r--r--   0 anthony   (1030) users      (100)     1811 2022-06-10 02:53:08.000000 oracledb-1.3.2/src/oracledb/exceptions.py
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-06-15 21:34:23.758717 oracledb-1.3.2/src/oracledb/impl/
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-06-15 21:34:23.762717 oracledb-1.3.2/src/oracledb/impl/base/
+-rw-r--r--   0 anthony   (1030) users      (100)     7341 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/impl/base/bind_var.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    37567 2023-06-15 20:56:07.000000 oracledb-1.3.2/src/oracledb/impl/base/connect_params.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    11765 2022-11-01 20:32:06.000000 oracledb-1.3.2/src/oracledb/impl/base/connection.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    18951 2022-07-29 21:22:34.000000 oracledb-1.3.2/src/oracledb/impl/base/cursor.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     4808 2022-11-01 20:32:06.000000 oracledb-1.3.2/src/oracledb/impl/base/dbobject.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     2741 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/impl/base/lob.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     4215 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/impl/base/pool.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)     4420 2023-06-15 20:44:06.000000 oracledb-1.3.2/src/oracledb/impl/base/pool_params.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     6379 2022-08-27 21:55:16.000000 oracledb-1.3.2/src/oracledb/impl/base/queue.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     4657 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/impl/base/soda.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     1933 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/impl/base/subscr.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)     8439 2023-03-21 21:27:13.000000 oracledb-1.3.2/src/oracledb/impl/base/types.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     8646 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/impl/base/utils.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    12993 2023-01-18 23:20:15.000000 oracledb-1.3.2/src/oracledb/impl/base/var.pyx
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-06-15 21:34:23.763717 oracledb-1.3.2/src/oracledb/impl/thick/
+-rw-r--r--   0 anthony   (1030) users      (100)     2256 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/impl/thick/buffer.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    25954 2023-06-15 20:44:06.000000 oracledb-1.3.2/src/oracledb/impl/thick/connection.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    19732 2022-08-02 15:15:52.000000 oracledb-1.3.2/src/oracledb/impl/thick/cursor.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    13927 2022-11-01 20:32:06.000000 oracledb-1.3.2/src/oracledb/impl/thick/dbobject.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     9330 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/impl/thick/json.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     7534 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/impl/thick/lob.pyx
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-06-15 21:34:23.758717 oracledb-1.3.2/src/oracledb/impl/thick/odpi/
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-06-15 21:34:23.763717 oracledb-1.3.2/src/oracledb/impl/thick/odpi/embed/
+-rw-r--r--   0 anthony   (1030) users      (100)     2569 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/embed/dpi.c
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-06-15 21:34:23.763717 oracledb-1.3.2/src/oracledb/impl/thick/odpi/include/
+-rw-rw-r--   0 anthony   (1030) users      (100)    82859 2023-06-15 20:52:06.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/include/dpi.h
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-06-15 21:34:23.766717 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/
+-rw-rw-r--   0 anthony   (1030) users      (100)   113814 2023-06-15 20:52:06.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiConn.c
+-rw-rw-r--   0 anthony   (1030) users      (100)    16638 2023-06-15 20:52:06.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiContext.c
+-rw-r--r--   0 anthony   (1030) users      (100)    34806 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiData.c
+-rw-r--r--   0 anthony   (1030) users      (100)     7443 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiDebug.c
+-rw-r--r--   0 anthony   (1030) users      (100)    15574 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c
+-rw-r--r--   0 anthony   (1030) users      (100)     7552 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c
+-rw-r--r--   0 anthony   (1030) users      (100)     9569 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiEnv.c
+-rw-r--r--   0 anthony   (1030) users      (100)    12063 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiError.c
+-rw-rw-r--   0 anthony   (1030) users      (100)     9018 2023-06-15 20:52:06.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h
+-rw-r--r--   0 anthony   (1030) users      (100)    13052 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiGen.c
+-rw-r--r--   0 anthony   (1030) users      (100)    15039 2022-11-07 17:19:09.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiGlobal.c
+-rw-r--r--   0 anthony   (1030) users      (100)     5184 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiHandleList.c
+-rw-r--r--   0 anthony   (1030) users      (100)     5399 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c
+-rw-rw-r--   0 anthony   (1030) users      (100)   107983 2023-06-15 20:52:06.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiImpl.h
+-rw-rw-r--   0 anthony   (1030) users      (100)    35246 2023-06-15 20:52:06.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiJson.c
+-rw-r--r--   0 anthony   (1030) users      (100)    19751 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiLob.c
+-rw-r--r--   0 anthony   (1030) users      (100)    23232 2022-08-27 21:56:08.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c
+-rw-r--r--   0 anthony   (1030) users      (100)    40061 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiObject.c
+-rw-r--r--   0 anthony   (1030) users      (100)     4894 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c
+-rw-rw-r--   0 anthony   (1030) users      (100)    14713 2023-06-15 20:52:06.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiObjectType.c
+-rw-r--r--   0 anthony   (1030) users      (100)   179729 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiOci.c
+-rw-r--r--   0 anthony   (1030) users      (100)    26914 2022-11-01 20:30:53.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiOracleType.c
+-rw-r--r--   0 anthony   (1030) users      (100)    32638 2022-08-02 17:00:34.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiPool.c
+-rw-r--r--   0 anthony   (1030) users      (100)    23678 2022-08-27 21:56:08.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiQueue.c
+-rw-r--r--   0 anthony   (1030) users      (100)     5712 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiRowid.c
+-rw-rw-r--   0 anthony   (1030) users      (100)    39581 2023-06-15 20:52:06.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c
+-rw-r--r--   0 anthony   (1030) users      (100)     6131 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c
+-rw-r--r--   0 anthony   (1030) users      (100)    17459 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c
+-rw-r--r--   0 anthony   (1030) users      (100)     9371 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c
+-rw-r--r--   0 anthony   (1030) users      (100)     6134 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c
+-rw-rw-r--   0 anthony   (1030) users      (100)    78753 2023-06-15 20:52:06.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiStmt.c
+-rw-r--r--   0 anthony   (1030) users      (100)    29091 2022-05-20 22:11:04.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiSubscr.c
+-rw-r--r--   0 anthony   (1030) users      (100)    23589 2022-11-01 20:30:53.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiUtils.c
+-rw-r--r--   0 anthony   (1030) users      (100)    78379 2022-06-09 19:44:20.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiVar.c
+-rw-r--r--   0 anthony   (1030) users      (100)    39137 2022-11-01 20:23:41.000000 oracledb-1.3.2/src/oracledb/impl/thick/odpi.pxd
+-rw-r--r--   0 anthony   (1030) users      (100)    13694 2022-11-18 03:37:36.000000 oracledb-1.3.2/src/oracledb/impl/thick/pool.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    21424 2022-10-18 22:30:30.000000 oracledb-1.3.2/src/oracledb/impl/thick/queue.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    24041 2022-12-01 00:47:06.000000 oracledb-1.3.2/src/oracledb/impl/thick/soda.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     7249 2022-12-01 00:47:47.000000 oracledb-1.3.2/src/oracledb/impl/thick/subscr.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    21952 2023-03-21 21:27:13.000000 oracledb-1.3.2/src/oracledb/impl/thick/utils.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    11309 2023-06-15 21:25:26.000000 oracledb-1.3.2/src/oracledb/impl/thick/var.pyx
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-06-15 21:34:23.768717 oracledb-1.3.2/src/oracledb/impl/thin/
+-rw-rw-r--   0 anthony   (1030) users      (100)    49673 2023-06-15 20:44:06.000000 oracledb-1.3.2/src/oracledb/impl/thin/buffer.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)     5330 2023-03-27 21:55:41.000000 oracledb-1.3.2/src/oracledb/impl/thin/capabilities.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    16743 2023-06-15 21:06:37.000000 oracledb-1.3.2/src/oracledb/impl/thin/connection.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    23274 2023-06-15 21:21:05.000000 oracledb-1.3.2/src/oracledb/impl/thin/constants.pxi
+-rw-rw-r--   0 anthony   (1030) users      (100)     7681 2023-06-15 20:44:06.000000 oracledb-1.3.2/src/oracledb/impl/thin/conversions.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     6194 2022-10-18 22:33:19.000000 oracledb-1.3.2/src/oracledb/impl/thin/crypto.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)     8773 2023-06-15 21:25:26.000000 oracledb-1.3.2/src/oracledb/impl/thin/cursor.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    23713 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/impl/thin/data_types.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    41584 2023-03-21 23:24:10.000000 oracledb-1.3.2/src/oracledb/impl/thin/dbobject.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)     7553 2023-03-21 23:24:10.000000 oracledb-1.3.2/src/oracledb/impl/thin/lob.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    99283 2023-06-15 21:30:32.000000 oracledb-1.3.2/src/oracledb/impl/thin/messages.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    26238 2023-03-29 03:53:29.000000 oracledb-1.3.2/src/oracledb/impl/thin/oson.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    27913 2023-06-15 21:21:05.000000 oracledb-1.3.2/src/oracledb/impl/thin/packet.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    20678 2023-06-15 20:44:06.000000 oracledb-1.3.2/src/oracledb/impl/thin/pool.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    20224 2023-06-15 21:30:32.000000 oracledb-1.3.2/src/oracledb/impl/thin/protocol.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    10891 2023-06-15 20:44:06.000000 oracledb-1.3.2/src/oracledb/impl/thin/statement.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     5869 2023-01-18 23:19:35.000000 oracledb-1.3.2/src/oracledb/impl/thin/utils.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     5445 2022-10-18 22:29:50.000000 oracledb-1.3.2/src/oracledb/impl/thin/var.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)     6078 2023-03-27 21:56:43.000000 oracledb-1.3.2/src/oracledb/lob.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    35074 2023-03-27 21:31:03.000000 oracledb-1.3.2/src/oracledb/pool.py
+-rw-r--r--   0 anthony   (1030) users      (100)    31290 2022-09-28 15:08:47.000000 oracledb-1.3.2/src/oracledb/pool_params.py
+-rw-r--r--   0 anthony   (1030) users      (100)        0 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/py.typed
+-rw-rw-r--   0 anthony   (1030) users      (100)    27454 2023-03-27 21:56:43.000000 oracledb-1.3.2/src/oracledb/soda.py
+-rw-r--r--   0 anthony   (1030) users      (100)    11078 2022-12-01 00:48:14.000000 oracledb-1.3.2/src/oracledb/subscr.py
+-rw-r--r--   0 anthony   (1030) users      (100)     3130 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/thick_impl.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)     3758 2023-03-21 23:24:10.000000 oracledb-1.3.2/src/oracledb/thin_impl.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     3382 2022-05-20 21:47:15.000000 oracledb-1.3.2/src/oracledb/utils.py
+-rw-rw-r--   0 anthony   (1030) users      (100)     6393 2023-03-27 21:56:43.000000 oracledb-1.3.2/src/oracledb/var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)     1533 2023-06-15 20:50:56.000000 oracledb-1.3.2/src/oracledb/version.py
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-06-15 21:34:23.761717 oracledb-1.3.2/src/oracledb.egg-info/
+-rw-rw-r--   0 anthony   (1030) users      (100)     5062 2023-06-15 21:34:23.000000 oracledb-1.3.2/src/oracledb.egg-info/PKG-INFO
+-rw-rw-r--   0 anthony   (1030) users      (100)     5443 2023-06-15 21:34:23.000000 oracledb-1.3.2/src/oracledb.egg-info/SOURCES.txt
+-rw-rw-r--   0 anthony   (1030) users      (100)        1 2023-06-15 21:34:23.000000 oracledb-1.3.2/src/oracledb.egg-info/dependency_links.txt
+-rw-rw-r--   0 anthony   (1030) users      (100)        1 2023-06-15 21:34:23.000000 oracledb-1.3.2/src/oracledb.egg-info/not-zip-safe
+-rw-rw-r--   0 anthony   (1030) users      (100)       20 2023-06-15 21:34:23.000000 oracledb-1.3.2/src/oracledb.egg-info/requires.txt
+-rw-rw-r--   0 anthony   (1030) users      (100)        9 2023-06-15 21:34:23.000000 oracledb-1.3.2/src/oracledb.egg-info/top_level.txt
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-06-15 21:34:23.771717 oracledb-1.3.2/tests/
+-rw-rw-r--   0 anthony   (1030) users      (100)     2368 2023-04-21 18:03:32.000000 oracledb-1.3.2/tests/create_schema.py
+-rw-r--r--   0 anthony   (1030) users      (100)     1928 2022-05-20 21:47:15.000000 oracledb-1.3.2/tests/drop_schema.py
+-rw-r--r--   0 anthony   (1030) users      (100)     7093 2022-05-20 21:47:15.000000 oracledb-1.3.2/tests/test_1000_module.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    25460 2023-06-15 21:31:45.000000 oracledb-1.3.2/tests/test_1100_connection.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    13748 2023-06-15 21:25:26.000000 oracledb-1.3.2/tests/test_1300_cursor_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)    11560 2022-05-20 21:47:15.000000 oracledb-1.3.2/tests/test_1400_datetime_var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)     9367 2023-03-21 21:27:13.000000 oracledb-1.3.2/tests/test_1500_types.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    19283 2023-03-29 03:49:45.000000 oracledb-1.3.2/tests/test_1600_dml_returning.py
+-rw-rw-r--   0 anthony   (1030) users      (100)     3785 2023-04-21 18:03:32.000000 oracledb-1.3.2/tests/test_1700_error.py
+-rw-r--r--   0 anthony   (1030) users      (100)     8251 2022-05-20 21:47:15.000000 oracledb-1.3.2/tests/test_1800_interval_var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    20023 2023-06-15 20:44:06.000000 oracledb-1.3.2/tests/test_1900_lob_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)     5306 2022-05-20 21:47:15.000000 oracledb-1.3.2/tests/test_2000_long_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)    11357 2022-05-20 21:47:15.000000 oracledb-1.3.2/tests/test_2100_nchar_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)    21431 2022-11-01 21:30:49.000000 oracledb-1.3.2/tests/test_2200_number_var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    25820 2023-06-15 20:44:06.000000 oracledb-1.3.2/tests/test_2300_object_var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    35040 2023-06-15 20:44:06.000000 oracledb-1.3.2/tests/test_2400_pool.py
+-rw-r--r--   0 anthony   (1030) users      (100)    21339 2022-11-07 17:27:30.000000 oracledb-1.3.2/tests/test_2500_string_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)     7896 2022-05-20 21:47:15.000000 oracledb-1.3.2/tests/test_2600_timestamp_var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    23955 2023-06-15 20:44:06.000000 oracledb-1.3.2/tests/test_2700_aq.py
+-rw-r--r--   0 anthony   (1030) users      (100)     7672 2022-08-27 21:55:16.000000 oracledb-1.3.2/tests/test_2800_bulk_aq.py
+-rw-r--r--   0 anthony   (1030) users      (100)     7813 2022-10-18 22:31:58.000000 oracledb-1.3.2/tests/test_2900_rowid.py
+-rw-r--r--   0 anthony   (1030) users      (100)     7971 2022-05-20 21:47:15.000000 oracledb-1.3.2/tests/test_3000_subscription.py
+-rw-r--r--   0 anthony   (1030) users      (100)     3943 2023-01-18 17:02:49.000000 oracledb-1.3.2/tests/test_3100_boolean_var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    24905 2023-04-21 18:03:32.000000 oracledb-1.3.2/tests/test_3200_features_12_1.py
+-rw-rw-r--   0 anthony   (1030) users      (100)     5670 2023-06-15 20:44:06.000000 oracledb-1.3.2/tests/test_3300_soda_database.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    21475 2023-06-15 20:44:06.000000 oracledb-1.3.2/tests/test_3400_soda_collection.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    10520 2023-06-15 20:44:06.000000 oracledb-1.3.2/tests/test_3500_json.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    25036 2023-03-21 21:27:13.000000 oracledb-1.3.2/tests/test_3600_outputtypehandler.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    20995 2023-06-15 20:44:06.000000 oracledb-1.3.2/tests/test_3700_var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    10197 2023-06-15 20:44:06.000000 oracledb-1.3.2/tests/test_3800_typehandler.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    16463 2023-06-15 20:44:06.000000 oracledb-1.3.2/tests/test_3900_cursor_execute.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    14964 2023-06-15 21:22:32.000000 oracledb-1.3.2/tests/test_4000_cursor_executemany.py
+-rw-r--r--   0 anthony   (1030) users      (100)     6304 2022-05-20 21:47:15.000000 oracledb-1.3.2/tests/test_4100_cursor_callproc.py
+-rw-r--r--   0 anthony   (1030) users      (100)    10122 2022-05-20 21:47:15.000000 oracledb-1.3.2/tests/test_4200_cursor_scrollable.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    43237 2023-06-15 21:25:26.000000 oracledb-1.3.2/tests/test_4300_cursor_other.py
+-rw-r--r--   0 anthony   (1030) users      (100)     5200 2022-11-07 16:22:37.000000 oracledb-1.3.2/tests/test_4400_tpc.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    31190 2023-06-15 20:54:55.000000 oracledb-1.3.2/tests/test_4500_connect_params.py
+-rw-rw-r--   0 anthony   (1030) users      (100)     9049 2023-06-15 20:44:06.000000 oracledb-1.3.2/tests/test_4600_type_changes.py
+-rw-r--r--   0 anthony   (1030) users      (100)     2746 2022-08-27 17:02:29.000000 oracledb-1.3.2/tests/test_4700_pool_params.py
+-rw-rw-r--   0 anthony   (1030) users      (100)     7614 2023-04-21 18:03:32.000000 oracledb-1.3.2/tests/test_4800_timestamp_ltz_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)     7315 2022-06-10 16:31:07.000000 oracledb-1.3.2/tests/test_4900_timestamp_tz_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)    11969 2022-08-02 17:00:32.000000 oracledb-1.3.2/tests/test_5000_externalauth.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    15525 2023-06-15 20:54:55.000000 oracledb-1.3.2/tests/test_env.py
+-rw-r--r--   0 anthony   (1030) users      (100)      593 2022-12-01 16:31:07.000000 oracledb-1.3.2/tox.ini
```

### Comparing `oracledb-1.3.1/LICENSE.txt` & `oracledb-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/PKG-INFO` & `oracledb-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oracledb
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python interface to Oracle Database
 Home-page: https://oracle.github.io/python-oracledb
 Author: Anthony Tuininga
 Author-email: anthony.tuininga@oracle.com
 License: Apache and/or UPL
 Project-URL: Installation, https://python-oracledb.readthedocs.io/en/latest/user_guide/installation.html
 Project-URL: Samples, https://github.com/oracle/python-oracledb/tree/main/samples
```

### Comparing `oracledb-1.3.1/THIRD_PARTY_LICENSES.txt` & `oracledb-1.3.2/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/setup.cfg` & `oracledb-1.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/setup.py` & `oracledb-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/__init__.py` & `oracledb-1.3.2/src/oracledb/__init__.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/aq.py` & `oracledb-1.3.2/src/oracledb/aq.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/base_impl.pxd` & `oracledb-1.3.2/src/oracledb/base_impl.pxd`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/base_impl.pyx` & `oracledb-1.3.2/src/oracledb/base_impl.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/connect_params.py` & `oracledb-1.3.2/src/oracledb/connect_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/connection.py` & `oracledb-1.3.2/src/oracledb/connection.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/constants.py` & `oracledb-1.3.2/src/oracledb/constants.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/constructors.py` & `oracledb-1.3.2/src/oracledb/constructors.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/cursor.py` & `oracledb-1.3.2/src/oracledb/cursor.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/dbobject.py` & `oracledb-1.3.2/src/oracledb/dbobject.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/defaults.py` & `oracledb-1.3.2/src/oracledb/defaults.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/driver_mode.py` & `oracledb-1.3.2/src/oracledb/driver_mode.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/dsn.py` & `oracledb-1.3.2/src/oracledb/dsn.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/errors.py` & `oracledb-1.3.2/src/oracledb/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,15 +408,16 @@
             'Listener refused connection. (Similar to ORA-{error_code})',
     ERR_LOB_OF_WRONG_TYPE:
             'LOB is of type {actual_type_name} but must be of type '
             '{expected_type_name}',
     ERR_MESSAGE_HAS_NO_PAYLOAD:
             'message has no payload',
     ERR_MESSAGE_TYPE_UNKNOWN:
-            'internal error: unknown protocol message type {message_type}',
+            'internal error: unknown protocol message type {message_type} '
+            'at position {position}',
     ERR_MISSING_BIND_VALUE:
             'a bind variable replacement value for placeholder ":{name}" was '
             'not provided',
     ERR_MISSING_TYPE_NAME_FOR_OBJECT_VAR:
             'no object type specified for object variable',
     ERR_MIXED_ELEMENT_TYPES:
             'element {element} is not the same data type as previous elements',
```

### Comparing `oracledb-1.3.1/src/oracledb/exceptions.py` & `oracledb-1.3.2/src/oracledb/exceptions.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/bind_var.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/bind_var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/connect_params.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/connect_params.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -568,14 +568,17 @@
         else:
             credentials = dsn
             connect_string = None
         pos = credentials.find("/")
         if pos >= 0:
             user = credentials[:pos] or None
             password = credentials[pos + 1:] or None
+        elif connect_string is None:
+            connect_string = dsn or None
+            user = password = None
         else:
             user = credentials or None
             password = None
         return (user, password, connect_string)
 
     def parse_user(self, str user):
         """
@@ -601,15 +604,15 @@
             - in thin mode, the connect string is then parsed into its
               components and stored
             - if no dsn was specified, one is built from the components
             - the connect string is returned
         """
         if kwargs:
             self.set(kwargs)
-        if self.user is None and dsn is not None:
+        if self.user is None and not self.externalauth and dsn is not None:
             user, password, dsn = self.parse_dsn_with_credentials(dsn)
             self.set(dict(user=user, password=password))
         if dsn is not None and thin:
             self.parse_connect_string(dsn)
         if dsn is None:
             dsn = self.get_connect_string()
         return dsn
```

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/connection.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/connection.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/cursor.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/cursor.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/dbobject.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/dbobject.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/lob.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/lob.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/pool.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/pool.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/pool_params.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/pool_params.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/queue.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/queue.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/soda.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/soda.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/subscr.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/subscr.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/types.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/types.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/utils.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/utils.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/base/var.pyx` & `oracledb-1.3.2/src/oracledb/impl/base/var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/buffer.pyx` & `oracledb-1.3.2/src/oracledb/impl/thick/buffer.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/connection.pyx` & `oracledb-1.3.2/src/oracledb/impl/thick/connection.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/cursor.pyx` & `oracledb-1.3.2/src/oracledb/impl/thick/cursor.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/dbobject.pyx` & `oracledb-1.3.2/src/oracledb/impl/thick/dbobject.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/json.pyx` & `oracledb-1.3.2/src/oracledb/impl/thick/json.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/lob.pyx` & `oracledb-1.3.2/src/oracledb/impl/thick/lob.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/embed/dpi.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/embed/dpi.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/include/dpi.h` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/include/dpi.h`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiConn.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiConn.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiContext.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiContext.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiData.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiData.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiDebug.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiDebug.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiEnv.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiEnv.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiError.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiError.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiGen.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiGen.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiGlobal.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiGlobal.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiHandleList.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiHandleList.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiImpl.h` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiImpl.h`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiJson.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiJson.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiLob.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiLob.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiObject.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiObject.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiObjectType.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiObjectType.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiOci.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiOci.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiOracleType.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiOracleType.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiPool.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiPool.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiQueue.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiQueue.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiRowid.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiRowid.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiStmt.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiStmt.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSubscr.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiSubscr.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiUtils.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiUtils.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiVar.c` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi/src/dpiVar.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/odpi.pxd` & `oracledb-1.3.2/src/oracledb/impl/thick/odpi.pxd`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/pool.pyx` & `oracledb-1.3.2/src/oracledb/impl/thick/pool.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/queue.pyx` & `oracledb-1.3.2/src/oracledb/impl/thick/queue.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/soda.pyx` & `oracledb-1.3.2/src/oracledb/impl/thick/soda.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/subscr.pyx` & `oracledb-1.3.2/src/oracledb/impl/thick/subscr.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/utils.pyx` & `oracledb-1.3.2/src/oracledb/impl/thick/utils.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thick/var.pyx` & `oracledb-1.3.2/src/oracledb/impl/thick/var.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -195,17 +195,14 @@
 
         # otherwise, make use of the statement handle allocated by the variable
         else:
             data = &self._data[pos]
             if dpiStmt_addRef(data.value.asStmt) < 0:
                 _raise_from_odpi()
             cursor_impl._handle = data.value.asStmt
-        if dpiStmt_setPrefetchRows(cursor_impl._handle,
-                                   cursor_impl.prefetchrows) < 0:
-            _raise_from_odpi()
         cursor_impl._fixup_ref_cursor = True
         cursor.statement = None
 
     cdef int _set_num_elements_in_array(self, uint32_t num_elements) except -1:
         """
         Sets the number of elements in the array.
         """
```

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/buffer.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/buffer.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/capabilities.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/capabilities.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/connection.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/connection.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -233,19 +233,20 @@
         """
         cdef Statement statement
         with self._statement_cache_lock:
             statement = self._statement_cache.get(sql)
             if statement is None:
                 statement = Statement()
                 statement._prepare(sql)
-                if len(self._statement_cache) < self._statement_cache_size \
-                        and cache_statement \
-                        and not self._drcp_establish_session:
-                    self._statement_cache[sql] = statement
+                if cache_statement and not self._drcp_establish_session \
+                        and not statement._is_ddl \
+                        and self._statement_cache_size > 0:
                     statement._return_to_cache = True
+                    self._statement_cache[sql] = statement
+                    self._adjust_statement_cache()
             elif statement._in_use or not cache_statement \
                     or self._drcp_establish_session:
                 if not cache_statement:
                     del self._statement_cache[sql]
                     statement._return_to_cache = False
                 if statement._in_use or self._drcp_establish_session:
                     statement = statement.copy()
@@ -279,16 +280,14 @@
                 bind_info._bind_var_impl = None
         if statement._fetch_var_impls is not None:
             for var_impl in statement._fetch_var_impls:
                 var_impl._values = [None] * var_impl.num_elements
         with self._statement_cache_lock:
             if statement._return_to_cache:
                 statement._in_use = False
-                self._statement_cache.move_to_end(statement._sql)
-                self._adjust_statement_cache()
             elif statement._cursor_id != 0:
                 self._add_cursor_to_close(statement)
 
     def cancel(self):
         self._protocol._break_external()
 
     def change_password(self, str old_password, str new_password):
```

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/constants.pxi` & `oracledb-1.3.2/src/oracledb/impl/thin/constants.pxi`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 DEF TNS_PACKET_TYPE_DATA = 6
 DEF TNS_PACKET_TYPE_RESEND = 11
 DEF TNS_PACKET_TYPE_MARKER = 12
 DEF TNS_PACKET_TYPE_CONTROL = 14
 DEF TNS_PACKET_TYPE_REDIRECT = 5
 
 # packet flags
+DEF TNS_PACKET_FLAG_REDIRECT = 0x04
 DEF TNS_PACKET_FLAG_TLS_RENEG = 0x08
 
 # data flags
 DEF TNS_DATA_FLAGS_EOF = 0x0040
 
 # marker types
 DEF TNS_MARKER_TYPE_BREAK = 1
```

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/conversions.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/conversions.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/crypto.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/crypto.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/cursor.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/cursor.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -100,18 +100,18 @@
     cdef int _fetch_rows(self, object cursor) except -1:
         """
         Internal method used for fetching rows from the database.
         """
         cdef MessageWithData message
         if self._statement._requires_full_execute:
             message = self._create_message(ExecuteMessage, cursor)
-            message.num_execs = self._fetch_array_size
         else:
             message = self._create_message(FetchMessage, cursor)
         self._conn_impl._protocol._process_single_message(message)
+        self._statement._requires_full_execute = False
 
     cdef BaseConnImpl _get_conn_impl(self):
         """
         Internal method used to return the connection implementation associated
         with the cursor implementation.
         """
         return self._conn_impl
```

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/data_types.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/data_types.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/dbobject.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/dbobject.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/lob.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/lob.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/messages.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/messages.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,16 @@
             buf.read_ub2(&self.end_to_end_seq_num)
         elif message_type == TNS_MSG_TYPE_PARAMETER:
             self._process_return_parameters(buf)
         elif message_type == TNS_MSG_TYPE_SERVER_SIDE_PIGGYBACK:
             self._process_server_side_piggyback(buf)
         else:
             errors._raise_err(errors.ERR_MESSAGE_TYPE_UNKNOWN,
-                              message_type=message_type)
+                              message_type=message_type,
+                              position=buf._pos - 1)
 
     cdef int _process_return_parameters(self, ReadBuffer buf) except -1:
         raise NotImplementedError()
 
     cdef int _process_server_side_piggyback(self, ReadBuffer buf) except -1:
         cdef:
             uint16_t num_elements, i, temp16
@@ -347,15 +348,14 @@
     cdef object _create_cursor_from_describe(self, ReadBuffer buf,
                                              object cursor=None):
         cdef ThinCursorImpl cursor_impl
         if cursor is None:
             cursor = self.cursor.connection.cursor()
         cursor_impl = cursor._impl
         cursor_impl._statement = Statement()
-        cursor_impl._fetch_array_size = cursor.arraysize + cursor.prefetchrows
         cursor_impl._more_rows_to_fetch = True
         cursor_impl._statement._is_query = True
         cursor_impl._statement._requires_full_execute = True
         self._process_describe_info(buf, cursor, cursor_impl)
         return cursor
 
     cdef int _get_bit_vector(self, ReadBuffer buf,
@@ -736,15 +736,16 @@
 
     cdef int _process_error_info(self, ReadBuffer buf) except -1:
         cdef:
             ThinCursorImpl cursor_impl = self.cursor_impl
             ThinConnImpl conn_impl = self.conn_impl
             object exc_type
         Message._process_error_info(self, buf)
-        cursor_impl._statement._cursor_id = self.error_info.cursor_id
+        if self.error_info.cursor_id != 0:
+            cursor_impl._statement._cursor_id = self.error_info.cursor_id
         if not cursor_impl._statement._is_plsql and not self.in_fetch:
             cursor_impl.rowcount = self.error_info.rowcount
         cursor_impl._lastrowid = self.error_info.rowid
         cursor_impl._batcherrors = self.error_info.batcherrors
         if self.batcherrors and cursor_impl._batcherrors is None:
             cursor_impl._batcherrors = []
         if self.error_info.num == TNS_ERR_NO_DATA_FOUND:
@@ -781,21 +782,23 @@
 
     cdef int _process_io_vector(self, ReadBuffer buf) except -1:
         """
         An I/O vector is sent by the database in response to a PL/SQL execute.
         It indicates whether binds are IN only, IN/OUT or OUT only.
         """
         cdef:
-            uint16_t i, num_binds, num_bytes, temp16
+            uint16_t i, num_bytes, temp16
+            uint32_t temp32, num_binds
             BindInfo bind_info
         buf.skip_ub1()                      # flag
-        buf.read_ub2(&num_binds)            # num requests
-        buf.read_ub4(&self.row_index)       # iter num
+        buf.read_ub2(&temp16)               # num requests
+        buf.read_ub4(&temp32)               # num iters
+        num_binds = temp32 * 256 + temp16
         buf.skip_ub4()                      # num iters this time
-        buf.read_ub2(&temp16)               # uac buffer length
+        buf.skip_ub2()                      # uac buffer length
         buf.read_ub2(&num_bytes)            # bit vector for fast fetch
         if num_bytes > 0:
             buf.skip_raw_bytes(num_bytes)
         buf.read_ub2(&num_bytes)            # rowid
         if num_bytes > 0:
             buf.skip_raw_bytes(num_bytes)
         self.out_var_impls = []
@@ -1321,59 +1324,71 @@
         # encrypt new password
         if self.newpassword is not None:
             newpassword_with_salt = salt + self.newpassword
             encrypted_newpassword = encrypt_cbc(self.conn_impl._combo_key,
                                                 newpassword_with_salt)
             self.encoded_newpassword = encrypted_newpassword.hex().upper()
 
-    cdef int _generate_verifier(self, bint verifier_11g) except -1:
+    cdef int _generate_verifier(self) except -1:
         """
         Generate the multi-round verifier.
         """
-        cdef bytes jdwp_data
+        cdef:
+            bytes jdwp_data
+            bytearray b
+            ssize_t i
 
         # create password hash
         verifier_data = bytes.fromhex(self.session_data['AUTH_VFR_DATA'])
-        if verifier_11g:
-            keylen = 24
-            h = hashlib.sha1(self.password)
-            h.update(verifier_data)
-            password_hash = h.digest() + bytes(4)
-        else:
+        if self.verifier_type == TNS_VERIFIER_TYPE_12C:
             keylen = 32
             iterations = int(self.session_data['AUTH_PBKDF2_VGEN_COUNT'])
             salt = verifier_data + b'AUTH_PBKDF2_SPEEDY_KEY'
             password_key = get_derived_key(self.password, salt, 64,
                                            iterations)
             h = hashlib.new("sha512")
             h.update(password_key)
             h.update(verifier_data)
             password_hash = h.digest()[:32]
+        else:
+            keylen = 24
+            h = hashlib.sha1(self.password)
+            h.update(verifier_data)
+            password_hash = h.digest() + bytes(4)
 
         # decrypt first half of session key
         encoded_server_key = bytes.fromhex(self.session_data['AUTH_SESSKEY'])
         session_key_part_a = decrypt_cbc(password_hash, encoded_server_key)
 
         # generate second half of session key
-        session_key_part_b = secrets.token_bytes(32)
+        session_key_part_b = secrets.token_bytes(len(session_key_part_a))
         encoded_client_key = encrypt_cbc(password_hash, session_key_part_b)
-        self.session_key = encoded_client_key.hex().upper()[:64]
 
-        # create session key from combo key
-        mixing_salt = bytes.fromhex(self.session_data['AUTH_PBKDF2_CSK_SALT'])
-        iterations = int(self.session_data['AUTH_PBKDF2_SDER_COUNT'])
-        temp_key = session_key_part_b[:keylen] + session_key_part_a[:keylen]
-        combo_key = get_derived_key(temp_key.hex().upper().encode(),
-                                    mixing_salt, keylen, iterations)
+        # create session key and combo key
+        if len(session_key_part_a) == 48:
+            self.session_key = encoded_client_key.hex().upper()[:96]
+            b = bytearray(24)
+            for i in range(16, 40):
+                b[i - 16] = session_key_part_a[i] ^ session_key_part_b[i]
+            part1 = hashlib.md5(b[:16]).digest()
+            part2 = hashlib.md5(b[16:]).digest()
+            combo_key = (part1 + part2)[:keylen]
+        else:
+            self.session_key = encoded_client_key.hex().upper()[:64]
+            salt = bytes.fromhex(self.session_data['AUTH_PBKDF2_CSK_SALT'])
+            iterations = int(self.session_data['AUTH_PBKDF2_SDER_COUNT'])
+            temp_key = session_key_part_b[:keylen] + session_key_part_a[:keylen]
+            combo_key = get_derived_key(temp_key.hex().upper().encode(), salt,
+                                        keylen, iterations)
 
         # retain session key for use by the change password API
         self.conn_impl._combo_key = combo_key
 
         # generate speedy key for 12c verifiers
-        if not verifier_11g:
+        if self.verifier_type == TNS_VERIFIER_TYPE_12C:
             salt = secrets.token_bytes(16)
             speedy_key = encrypt_cbc(combo_key, salt + password_key)
             self.speedy_key = speedy_key[:80].hex().upper()
 
         # encrypts the passwords
         self._encrypt_passwords()
 
@@ -1533,15 +1548,14 @@
         if value_len > 0:
             buf.write_bytes_with_length(value_bytes)
         buf.write_ub4(flags)
 
     cdef int _write_message(self, WriteBuffer buf) except -1:
         cdef:
             uint8_t has_user = 1 if self.user_bytes_len > 0 else 0
-            bint verifier_11g = False
             uint32_t num_pairs
 
         # perform final determination of data to write
         if self.function_code == TNS_FUNC_AUTH_PHASE_ONE:
             num_pairs = 5
         elif self.change_password:
             self._encrypt_passwords()
@@ -1553,23 +1567,21 @@
             if self.token is not None:
                 num_pairs += 1
 
             # normal user/password authentication
             else:
                 num_pairs += 2
                 self.auth_mode |= TNS_AUTH_MODE_WITH_PASSWORD
-                if self.verifier_type in (TNS_VERIFIER_TYPE_11G_1,
-                                          TNS_VERIFIER_TYPE_11G_2):
-                    verifier_11g = True
-                elif self.verifier_type != TNS_VERIFIER_TYPE_12C:
+                if self.verifier_type == TNS_VERIFIER_TYPE_12C:
+                    num_pairs += 1
+                elif self.verifier_type not in (TNS_VERIFIER_TYPE_11G_1,
+                                                TNS_VERIFIER_TYPE_11G_2):
                     errors._raise_err(errors.ERR_UNSUPPORTED_VERIFIER_TYPE,
                                       verifier_type=self.verifier_type)
-                else:
-                    num_pairs += 1
-                self._generate_verifier(verifier_11g)
+                self._generate_verifier()
 
             # determine which other key/value pairs to write
             if self.newpassword is not None:
                 num_pairs += 1
                 self.auth_mode |= TNS_AUTH_MODE_CHANGE_PASSWORD
             if self.proxy_user is not None:
                 num_pairs += 1
@@ -1609,15 +1621,15 @@
             if self.proxy_user is not None:
                 self._write_key_value(buf, "PROXY_CLIENT_NAME",
                                       self.proxy_user)
             if self.token is not None:
                 self._write_key_value(buf, "AUTH_TOKEN", self.token)
             elif not self.change_password:
                 self._write_key_value(buf, "AUTH_SESSKEY", self.session_key, 1)
-                if not verifier_11g:
+                if self.verifier_type == TNS_VERIFIER_TYPE_12C:
                     self._write_key_value(buf, "AUTH_PBKDF2_SPEEDY_KEY",
                                           self.speedy_key)
             if self.encoded_password is not None:
                 self._write_key_value(buf, "AUTH_PASSWORD",
                                       self.encoded_password)
             if self.encoded_newpassword is not None:
                 self._write_key_value(buf, "AUTH_NEWPASSWORD",
@@ -1731,15 +1743,15 @@
             uint16_t service_options = TNS_GSO_DONT_CARE
             uint32_t connect_flags_1 = 0, connect_flags_2 = 0
             uint8_t nsi_flags = \
                     TNS_NSI_SUPPORT_SECURITY_RENEG | TNS_NSI_DISABLE_NA
         if buf._caps.supports_oob:
             service_options |= TNS_GSO_CAN_RECV_ATTENTION
             connect_flags_2 |= TNS_CHECK_OOB
-        buf.start_request(TNS_PACKET_TYPE_CONNECT)
+        buf.start_request(TNS_PACKET_TYPE_CONNECT, self.packet_flags)
         buf.write_uint16(TNS_VERSION_DESIRED)
         buf.write_uint16(TNS_VERSION_MINIMUM)
         buf.write_uint16(service_options)
         buf.write_uint16(TNS_SDU)
         buf.write_uint16(TNS_TDU)
         buf.write_uint16(TNS_PROTOCOL_CHARACTERISTICS)
         buf.write_uint16(0)                 # line turnaround
@@ -1839,21 +1851,21 @@
             options |= TNS_EXEC_OPTION_EXECUTE
         if stmt._cursor_id == 0 or stmt._is_ddl:
             options |= TNS_EXEC_OPTION_PARSE
         if stmt._is_query:
             if self.parse_only:
                 options |= TNS_EXEC_OPTION_DESCRIBE
             else:
-                if self.cursor_impl.prefetchrows > 0:
-                    options |= TNS_EXEC_OPTION_FETCH
                 if stmt._cursor_id == 0 or stmt._requires_define:
                     num_iters = self.cursor_impl.prefetchrows
-                    self.cursor_impl._fetch_array_size = num_iters
                 else:
-                    num_iters = self.cursor_impl._fetch_array_size
+                    num_iters = self.cursor_impl.arraysize
+                self.cursor_impl._fetch_array_size = num_iters
+                if num_iters > 0:
+                    options |= TNS_EXEC_OPTION_FETCH
         if not stmt._is_plsql and not self.parse_only:
             options |= TNS_EXEC_OPTION_NOT_PLSQL
         elif stmt._is_plsql and num_params > 0:
             options |= TNS_EXEC_OPTION_PLSQL_BIND
         if num_params > 0:
             options |= TNS_EXEC_OPTION_BIND
         if self.batcherrors:
@@ -2222,7 +2234,30 @@
 cdef class RollbackMessage(Message):
 
     cdef int _initialize_hook(self) except -1:
         """
         Perform initialization.
         """
         self.function_code = TNS_FUNC_ROLLBACK
+
+
+@cython.final
+cdef class SessionReleaseMessage(Message):
+
+    cdef:
+        uint32_t release_mode
+
+    cdef int _initialize_hook(self) except -1:
+        """
+        Perform initialization.
+        """
+        self.message_type = TNS_MSG_TYPE_ONEWAY_FN
+        self.function_code = TNS_FUNC_SESSION_RELEASE
+
+    cdef int _write_message(self, WriteBuffer buf) except -1:
+        """
+        Write the message for a DRCP session release.
+        """
+        self._write_function_code(buf)
+        buf.write_uint8(0)                  # pointer (tag name)
+        buf.write_uint8(0)                  # tag name length
+        buf.write_ub4(self.release_mode)    # mode
```

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/oson.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/oson.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/packet.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/packet.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -583,14 +583,15 @@
 
 
 @cython.final
 cdef class WriteBuffer(Buffer):
 
     cdef:
         uint8_t _packet_type
+        uint8_t _packet_flags
         Capabilities _caps
         object _socket
         uint8_t _seq_num
         bint _packet_sent
 
     def __cinit__(self, object sock, ssize_t max_size, Capabilities caps):
         self._socket = sock
@@ -606,15 +607,15 @@
         self._pos = 0
         if self._caps.protocol_version >= TNS_VERSION_MIN_LARGE_SDU:
             self.write_uint32(size)
         else:
             self.write_uint16(size)
             self.write_uint16(0)
         self.write_uint8(self._packet_type)
-        self.write_uint8(0)
+        self.write_uint8(self._packet_flags)
         self.write_uint16(0)
         self._pos = size
         if DEBUG_PACKETS:
             _print_packet("Sending packet:", self._socket.fileno(),
                           self._data_view[:self._pos])
         try:
             self._socket.send(self._data_view[:self._pos])
@@ -646,23 +647,25 @@
         """
         Return the maximum number of bytes that can be sent in a packet. This
         is the maximum size of the entire packet, less the bytes in the header
         and 2 bytes for the data flags.
         """
         return self._max_size - PACKET_HEADER_SIZE - 2
 
-    cdef void start_request(self, uint8_t packet_type, uint16_t data_flags=0):
+    cdef void start_request(self, uint8_t packet_type, uint8_t packet_flags=0,
+                            uint16_t data_flags=0):
         """
         Indicates that a request from the client is starting. The packet type
         is retained just in case a request spans multiple packets. The packet
         header (8 bytes in length) is written when a packet is actually being
         sent and so is skipped at this point.
         """
         self._packet_sent = False
         self._packet_type = packet_type
+        self._packet_flags = packet_flags
         self._pos = PACKET_HEADER_SIZE
         if packet_type == TNS_PACKET_TYPE_DATA:
             self.write_uint16(data_flags)
 
     cdef int write_lob_with_length(self, ThinLobImpl lob_impl) except -1:
         """
         Writes a LOB locator to the buffer.
```

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/pool.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/pool.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/protocol.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/protocol.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             # rollback any open transaction and release the DRCP session, if
             # applicable
             if self._socket is not None:
                 if self._txn_in_progress:
                     message = conn_impl._create_message(RollbackMessage)
                     self._process_message(message)
                 if conn_impl._drcp_enabled:
-                    self._release_drcp_session(self._write_buf, release_mode)
+                    self._release_drcp_session(conn_impl, release_mode)
                     conn_impl._drcp_establish_session = True
 
             # if the connection is part of a pool, return it to the pool
             if conn_impl._pool is not None:
                 return conn_impl._pool._return_connection(conn_impl)
 
             # otherwise, destroy the database object type cache, send the
@@ -129,19 +129,19 @@
         """
         Method for performing the required steps for establishing a connection
         within the scope of a retry. If the listener refuses the connection, a
         retry will be performed, if retry_count is set.
         """
         cdef:
             ConnectMessage connect_message = None
+            uint8_t packet_type, packet_flags = 0
             object ssl_context, connect_info
             ConnectParamsImpl temp_params
             str host, redirect_data
             Address temp_address
-            uint8_t packet_type
             int port, pos
 
         # store whether OOB processing is possible or not
         self._caps.supports_oob = not params.disable_oob \
                 and sys.platform != "win32"
 
         # establish initial TCP connection and get initial connect string
@@ -159,14 +159,15 @@
                 connect_message = conn_impl._create_message(ConnectMessage)
                 connect_message.host = host
                 connect_message.port = port
                 connect_message.description = description
                 connect_message.connect_string_bytes = connect_string.encode()
                 connect_message.connect_string_len = \
                         <uint16_t> len(connect_message.connect_string_bytes)
+                connect_message.packet_flags = packet_flags
 
             # process connection message
             self._process_message(connect_message)
             if connect_message.redirect_data is not None:
                 redirect_data = connect_message.redirect_data
                 pos = redirect_data.find('\x00')
                 if pos < 0:
@@ -176,14 +177,15 @@
                 temp_params._parse_connect_string(redirect_data[:pos])
                 temp_address = temp_params._get_addresses()[0]
                 host = temp_address.host
                 port = temp_address.port
                 connect_string = redirect_data[pos + 1:]
                 self._connect_tcp(params, description, address, host, port)
                 connect_message = None
+                packet_flags = TNS_PACKET_FLAG_REDIRECT
             elif connect_message.packet_type == TNS_PACKET_TYPE_ACCEPT:
                 break
 
             # for TCPS connections, OOB processing is not supported; if the
             # packet flags indicate that TLS renegotiation is required, this is
             # performed now
             if address.protocol == "tcps":
@@ -222,15 +224,16 @@
         self._process_message(conn_impl._create_message(DataTypesMessage))
 
         # send authorization packet twice, the first time to get the session
         # key and the second time to return the response to the challenge
         auth_message = conn_impl._create_message(AuthMessage)
         auth_message._set_params(params, description)
         self._process_message(auth_message)
-        self._process_message(auth_message)
+        if auth_message.resend:
+            self._process_message(auth_message)
 
         # mark protocol to indicate that connect is no longer in progress; this
         # allows the normal break/reset mechanism to fire
         self._in_connect = False
 
     cdef int _connect_tcp(self, ConnectParamsImpl params,
                           Description description, Address address, str host,
@@ -288,15 +291,15 @@
         # save final socket object
         self._set_socket(sock)
 
     cdef int _final_close(self, WriteBuffer buf) except -1:
         """
         Send the final close packet to the server and close the socket.
         """
-        buf.start_request(TNS_PACKET_TYPE_DATA, TNS_DATA_FLAGS_EOF)
+        buf.start_request(TNS_PACKET_TYPE_DATA, 0, TNS_DATA_FLAGS_EOF)
         buf.end_request()
         self._socket.shutdown(socket.SHUT_RDWR)
         self._socket.close()
         self._socket = None
 
     cdef int _force_close(self) except -1:
         """
@@ -390,28 +393,24 @@
         if message.packet_type == TNS_PACKET_TYPE_MARKER:
             self._reset(message)
         elif message.packet_type == TNS_PACKET_TYPE_REFUSE:
             self._write_buf._packet_sent = False
             buf.skip_raw_bytes(3)
             message.error_info.message = buf.read_str(TNS_CS_IMPLICIT)
 
-    cdef int _release_drcp_session(self, WriteBuffer buf,
+    cdef int _release_drcp_session(self, ThinConnImpl conn_impl,
                                    uint32_t release_mode) except -1:
         """
         Release the session back to DRCP. Standalone sessions are marked for
         deauthentication.
         """
-        buf.start_request(TNS_PACKET_TYPE_DATA)
-        buf.write_uint8(TNS_MSG_TYPE_ONEWAY_FN)
-        buf.write_uint8(TNS_FUNC_SESSION_RELEASE)
-        buf.write_uint8(0)                  # seq number
-        buf.write_uint8(0)                  # pointer (tag name)
-        buf.write_uint8(0)                  # tag name length
-        buf.write_ub4(release_mode)         # mode
-        buf.end_request()
+        cdef SessionReleaseMessage message
+        message = conn_impl._create_message(SessionReleaseMessage)
+        message.release_mode = release_mode
+        message.send(self._write_buf)
 
     cdef int _reset(self, Message message) except -1:
         cdef uint8_t marker_type
 
         # send reset marker
         self._send_marker(self._write_buf, TNS_MARKER_TYPE_RESET)
```

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/statement.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/statement.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/utils.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/utils.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/impl/thin/var.pyx` & `oracledb-1.3.2/src/oracledb/impl/thin/var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/lob.py` & `oracledb-1.3.2/src/oracledb/lob.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/pool.py` & `oracledb-1.3.2/src/oracledb/pool.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/pool_params.py` & `oracledb-1.3.2/src/oracledb/pool_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/soda.py` & `oracledb-1.3.2/src/oracledb/soda.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/subscr.py` & `oracledb-1.3.2/src/oracledb/subscr.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/thick_impl.pyx` & `oracledb-1.3.2/src/oracledb/thick_impl.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/thin_impl.pyx` & `oracledb-1.3.2/src/oracledb/thin_impl.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/utils.py` & `oracledb-1.3.2/src/oracledb/utils.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/var.py` & `oracledb-1.3.2/src/oracledb/var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/src/oracledb/version.py` & `oracledb-1.3.2/src/oracledb/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 # version.py
 #
 # Defines the version of the package. This is the only place where this is
 # found. The setup.cfg configuration file and the documentation configuration
 # file doc/src/conf.py both reference this file directly.
 #------------------------------------------------------------------------------
 
-__version__ = "1.3.1"
+__version__ = "1.3.2"
```

### Comparing `oracledb-1.3.1/src/oracledb.egg-info/PKG-INFO` & `oracledb-1.3.2/src/oracledb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oracledb
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python interface to Oracle Database
 Home-page: https://oracle.github.io/python-oracledb
 Author: Anthony Tuininga
 Author-email: anthony.tuininga@oracle.com
 License: Apache and/or UPL
 Project-URL: Installation, https://python-oracledb.readthedocs.io/en/latest/user_guide/installation.html
 Project-URL: Samples, https://github.com/oracle/python-oracledb/tree/main/samples
```

### Comparing `oracledb-1.3.1/src/oracledb.egg-info/SOURCES.txt` & `oracledb-1.3.2/src/oracledb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/create_schema.py` & `oracledb-1.3.2/tests/create_schema.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/drop_schema.py` & `oracledb-1.3.2/tests/drop_schema.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_1000_module.py` & `oracledb-1.3.2/tests/test_1000_module.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_1100_connection.py` & `oracledb-1.3.2/tests/test_1100_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,16 @@
         cursor.execute("insert into TestTempTable (IntCol) values (2)")
         other_cursor.execute("select IntCol from TestTempTable order by IntCol")
         rows = other_cursor.fetchall()
         self.assertEqual(rows, [(1,), (2,)])
 
     def test_1105_bad_connect_string(self):
         "1105 - connection to database with bad connect string"
-        self.assertRaisesRegex(oracledb.DatabaseError, "^DPY-4001:|ORA-12547:",
+        self.assertRaisesRegex(oracledb.DatabaseError,
+                               "^DPY-4000:|^DPY-4026:|^DPY-4027:|ORA-12154:",
                                oracledb.connect, test_env.get_main_user())
         self.assertRaisesRegex(oracledb.DatabaseError, "^DPY-4000:|^DPY-4001:",
                                oracledb.connect, test_env.get_main_user() + \
                                "@" + test_env.get_connect_string())
         errors = "^DPY-4000:|^DPY-4001:|^DPY-4017:|^ORA-12154:|^ORA-12521:"
         self.assertRaisesRegex(oracledb.DatabaseError, errors,
                                oracledb.connect, test_env.get_main_user() + \
```

### Comparing `oracledb-1.3.1/tests/test_1300_cursor_var.py` & `oracledb-1.3.2/tests/test_1300_cursor_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,16 +134,16 @@
         expected_value = [
             (5, 'String 5'),
             (6, 'String 6')
         ]
         rows = ref_cursor.fetchall()
         self.assertEqual(rows, expected_value)
 
-    def test_1306_refcursor_prefetchrows(self):
-        "1306 - test prefetch rows and arraysize using a refcursor"
+    def test_1306_refcursor_round_trips(self):
+        "1306 - test round trips using a REF cursor"
         self.setup_round_trip_checker()
 
         # simple DDL only requires a single round trip
         with self.connection.cursor() as cursor:
             cursor.execute("truncate table TestTempTable")
             self.assertRoundTrips(1)
 
@@ -151,22 +151,31 @@
         num_rows = 590
         with self.connection.cursor() as cursor:
             sql = "insert into TestTempTable (IntCol) values (:1)"
             data = [(n + 1,) for n in range(num_rows)]
             cursor.executemany(sql, data)
             self.assertRoundTrips(1)
 
-        # create refcursor and execute stored procedure
+        # create REF cursor and execute stored procedure
+        # (array size set before procedure is called)
         with self.connection.cursor() as cursor:
             refcursor = self.connection.cursor()
-            refcursor.prefetchrows = 150
-            refcursor.arraysize = 50
+            refcursor.arraysize = 150
             cursor.callproc("myrefcursorproc", [refcursor])
             refcursor.fetchall()
-            self.assertRoundTrips(4)
+            self.assertRoundTrips(5)
+
+        # create REF cursor and execute stored procedure
+        # (array size set after procedure is called)
+        with self.connection.cursor() as cursor:
+            refcursor = self.connection.cursor()
+            cursor.callproc("myrefcursorproc", [refcursor])
+            refcursor.arraysize = 145
+            refcursor.fetchall()
+            self.assertRoundTrips(6)
 
     def test_1307_refcursor_execute_different_sql(self):
         "1307 - test executing different SQL after getting a REF cursor"
         with self.connection.cursor() as cursor:
             refcursor = self.connection.cursor()
             cursor.callproc("myrefcursorproc", [refcursor])
             var = cursor.var(int)
```

### Comparing `oracledb-1.3.1/tests/test_1400_datetime_var.py` & `oracledb-1.3.2/tests/test_1400_datetime_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_1500_types.py` & `oracledb-1.3.2/tests/test_1500_types.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_1600_dml_returning.py` & `oracledb-1.3.2/tests/test_1600_dml_returning.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_1700_error.py` & `oracledb-1.3.2/tests/test_1700_error.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_1800_interval_var.py` & `oracledb-1.3.2/tests/test_1800_interval_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_1900_lob_var.py` & `oracledb-1.3.2/tests/test_1900_lob_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_2000_long_var.py` & `oracledb-1.3.2/tests/test_2000_long_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_2100_nchar_var.py` & `oracledb-1.3.2/tests/test_2100_nchar_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_2200_number_var.py` & `oracledb-1.3.2/tests/test_2200_number_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_2300_object_var.py` & `oracledb-1.3.2/tests/test_2300_object_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_2400_pool.py` & `oracledb-1.3.2/tests/test_2400_pool.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_2500_string_var.py` & `oracledb-1.3.2/tests/test_2500_string_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_2600_timestamp_var.py` & `oracledb-1.3.2/tests/test_2600_timestamp_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_2700_aq.py` & `oracledb-1.3.2/tests/test_2700_aq.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_2800_bulk_aq.py` & `oracledb-1.3.2/tests/test_2800_bulk_aq.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_2900_rowid.py` & `oracledb-1.3.2/tests/test_2900_rowid.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_3000_subscription.py` & `oracledb-1.3.2/tests/test_3000_subscription.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_3100_boolean_var.py` & `oracledb-1.3.2/tests/test_3100_boolean_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_3200_features_12_1.py` & `oracledb-1.3.2/tests/test_3200_features_12_1.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_3300_soda_database.py` & `oracledb-1.3.2/tests/test_3300_soda_database.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_3400_soda_collection.py` & `oracledb-1.3.2/tests/test_3400_soda_collection.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_3500_json.py` & `oracledb-1.3.2/tests/test_3500_json.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_3600_outputtypehandler.py` & `oracledb-1.3.2/tests/test_3600_outputtypehandler.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_3700_var.py` & `oracledb-1.3.2/tests/test_3700_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_3800_typehandler.py` & `oracledb-1.3.2/tests/test_3800_typehandler.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_3900_cursor_execute.py` & `oracledb-1.3.2/tests/test_3900_cursor_execute.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_4000_cursor_executemany.py` & `oracledb-1.3.2/tests/test_4000_cursor_executemany.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #------------------------------------------------------------------------------
-# Copyright (c) 2020, 2022, Oracle and/or its affiliates.
+# Copyright (c) 2020, 2023, Oracle and/or its affiliates.
 #
 # This software is dual-licensed to you under the Universal Permissive License
 # (UPL) 1.0 as shown at https://oss.oracle.com/licenses/upl and Apache License
 # 2.0 as shown at http://www.apache.org/licenses/LICENSE-2.0. You may choose
 # either license.
 #
 # If you elect to accept the software under the Apache License, Version 2.0,
@@ -306,9 +306,36 @@
         self.cursor.execute("""
                 select IntCol, NumberCol
                 from TestTempTable
                 order by IntCol""")
         fetched_data = self.cursor.fetchall()
         self.assertEqual(data, fetched_data)
 
+    def test_4022_plsql_large_number_of_binds(self):
+        "4022 - test PL/SQL with a lerge number of binds"
+        parts = []
+        bind_names = []
+        all_bind_values = []
+        out_binds = []
+        for i in range(5):
+            all_bind_values.append([])
+        for i in range(350):
+            n = len(parts) + 1
+            bind_names.extend([f"v_out_{n}_0", f"a_{n}", f"b_{n}", f"c_{n}"])
+            parts.append(f":v_out{n} := :a_{n} + :b_{n} + :c_{n};")
+            out_binds.append(self.cursor.var(int,
+                                             arraysize=len(all_bind_values)))
+            for j, bind_values in enumerate(all_bind_values):
+                bind_values.extend([out_binds[-1], n * 1 + j, n * 2 + j,
+                                    n * 3 + j])
+        lf = "\n"
+        sql = f"begin{lf}{lf.join(parts)}{lf}end;"
+        self.cursor.executemany(sql, all_bind_values)
+        init_val = 6
+        for var in out_binds:
+            expected = [init_val, init_val + 3, init_val + 6, init_val + 9,
+                        init_val + 12]
+            self.assertEqual(var.values, expected)
+            init_val += 6
+
 if __name__ == "__main__":
     test_env.run_test_cases()
```

### Comparing `oracledb-1.3.1/tests/test_4100_cursor_callproc.py` & `oracledb-1.3.2/tests/test_4100_cursor_callproc.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_4200_cursor_scrollable.py` & `oracledb-1.3.2/tests/test_4200_cursor_scrollable.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_4300_cursor_other.py` & `oracledb-1.3.2/tests/test_4300_cursor_other.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,21 +342,23 @@
         "4323 - test prefetch rows using existing cursor"
         self.setup_round_trip_checker()
 
         # Set prefetch rows on an existing cursor
         num_rows = 590
         with self.connection.cursor() as cursor:
             cursor.execute("truncate table TestTempTable")
+            self.assertRoundTrips(1)
             sql = "insert into TestTempTable (IntCol) values (:1)"
             data = [(n + 1,) for n in range(num_rows)]
             cursor.executemany(sql, data)
-            cursor.prefetchrows = 300
-            cursor.arraysize = 300
+            self.assertRoundTrips(1)
+            cursor.prefetchrows = 30
+            cursor.arraysize = 100
             cursor.execute("select IntCol from TestTempTable").fetchall()
-            self.assertRoundTrips(4)
+            self.assertRoundTrips(7)
 
     def test_4324_bind_names_with_single_line_comments(self):
         "4324 - test bindnames() with single line comments"
         self.cursor.prepare("""--begin :value2 := :a + :b + :c +:a +3; end;
                             begin :value2 := :a + :c +3; end;
                             """)
         self.assertEqual(self.cursor.bindnames(), ["VALUE2", "A", "C"])
```

### Comparing `oracledb-1.3.1/tests/test_4400_tpc.py` & `oracledb-1.3.2/tests/test_4400_tpc.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_4500_connect_params.py` & `oracledb-1.3.2/tests/test_4500_connect_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -615,9 +615,18 @@
         for dsn in ("", "/"):
             params = oracledb.ConnectParams()
             user, password, dsn = params.parse_dsn_with_credentials(dsn)
             self.assertEqual(user, None)
             self.assertEqual(password, None)
             self.assertEqual(dsn, None)
 
+    def test_4561_dsn_with_no_credentials(self):
+        "4561 - test parsing a DSN with no credentials"
+        dsn_in = "my_alias_4561"
+        params = oracledb.ConnectParams()
+        user, password, dsn_out = params.parse_dsn_with_credentials(dsn_in)
+        self.assertEqual(user, None)
+        self.assertEqual(password, None)
+        self.assertEqual(dsn_out, dsn_in)
+
 if __name__ == "__main__":
     test_env.run_test_cases()
```

### Comparing `oracledb-1.3.1/tests/test_4600_type_changes.py` & `oracledb-1.3.2/tests/test_4600_type_changes.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_4700_pool_params.py` & `oracledb-1.3.2/tests/test_4700_pool_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_4800_timestamp_ltz_var.py` & `oracledb-1.3.2/tests/test_4800_timestamp_ltz_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_4900_timestamp_tz_var.py` & `oracledb-1.3.2/tests/test_4900_timestamp_tz_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_5000_externalauth.py` & `oracledb-1.3.2/tests/test_5000_externalauth.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.1/tests/test_env.py` & `oracledb-1.3.2/tests/test_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #------------------------------------------------------------------------------
-# Copyright (c) 2020, 2022, Oracle and/or its affiliates.
+# Copyright (c) 2020, 2023, Oracle and/or its affiliates.
 #
 # This software is dual-licensed to you under the Universal Permissive License
 # (UPL) 1.0 as shown at https://oss.oracle.com/licenses/upl and Apache License
 # 2.0 as shown at http://www.apache.org/licenses/LICENSE-2.0. You may choose
 # either license.
 #
 # If you elect to accept the software under the Apache License, Version 2.0,
```

### Comparing `oracledb-1.3.1/tox.ini` & `oracledb-1.3.2/tox.ini`

 * *Files identical despite different names*

