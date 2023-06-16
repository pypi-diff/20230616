# Comparing `tmp/py_ios_device-2.3.32.2.tar.gz` & `tmp/py_ios_device-2.3.32.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ios_device-2.3.32.2.tar", last modified: Wed May 24 02:44:55 2023, max compression
+gzip compressed data, was "py_ios_device-2.3.32.4.tar", last modified: Fri Jun 16 01:58:43 2023, max compression
```

## Comparing `py_ios_device-2.3.32.2.tar` & `py_ios_device-2.3.32.4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.186875 py_ios_device-2.3.32.2/
--rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/LICENSE
--rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/MANIFEST.in
--rw-r--r--   0 rongcloud   (501) staff       (20)    11417 2023-05-24 02:44:55.186472 py_ios_device-2.3.32.2/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)    10950 2023-05-24 02:33:49.000000 py_ios_device-2.3.32.2/README.md
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.168183 py_ios_device-2.3.32.2/demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/demo/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/demo/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/demo/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2023-03-07 02:35:28.000000 py_ios_device-2.3.32.2/demo/installation_proxy.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.172827 py_ios_device-2.3.32.2/demo/instrument_demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/demo/instrument_demo/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/demo/instrument_demo/activity.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.2/demo/instrument_demo/app_lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/demo/instrument_demo/applictionListing.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.2/demo/instrument_demo/channel.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4146 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.2/demo/instrument_demo/coreprofilesessiontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.2/demo/instrument_demo/coreprofilesessiontap_parse.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2174 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.2/demo/instrument_demo/deviceinfo.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      494 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.2/demo/instrument_demo/energy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2199 2023-05-08 09:42:27.000000 py_ios_device-2.3.32.2/demo/instrument_demo/gpu.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.2/demo/instrument_demo/graphics.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      748 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.2/demo/instrument_demo/launchAPP.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 py_ios_device-2.3.32.2/demo/instrument_demo/mobileNotifications.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.2/demo/instrument_demo/netstatPID.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.2/demo/instrument_demo/networking.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2554 2023-04-20 02:17:26.000000 py_ios_device-2.3.32.2/demo/instrument_demo/sysmontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/demo/instrument_demo/xcuitest.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/demo/mobile_config.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/demo/pcapd.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/demo/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/demo/syslog.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.173453 py_ios_device-2.3.32.2/ios_device/
--rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)       25 2023-05-24 02:44:54.000000 py_ios_device-2.3.32.2/ios_device/__version__.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.175100 py_ios_device-2.3.32.2/ios_device/cli/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/cli/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    31554 2023-05-24 02:44:13.000000 py_ios_device-2.3.32.2/ios_device/cli/base.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      988 2023-04-07 02:33:45.000000 py_ios_device-2.3.32.2/ios_device/cli/cli.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    19122 2023-05-24 02:30:31.000000 py_ios_device-2.3.32.2/ios_device/cli/instruments.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    11223 2023-04-26 06:21:46.000000 py_ios_device-2.3.32.2/ios_device/cli/mobile.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      293 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/main.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.2/ios_device/py_ios_device.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.180186 py_ios_device-2.3.32.2/ios_device/servers/
--rw-r--r--   0 rongcloud   (501) staff       (20)     7287 2023-04-26 03:35:04.000000 py_ios_device-2.3.32.2/ios_device/servers/Installation.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1029 2023-04-20 02:15:07.000000 py_ios_device-2.3.32.2/ios_device/servers/Instrument.py
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/servers/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    19387 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/amfi.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      993 2023-05-22 06:59:19.000000 py_ios_device-2.3.32.2/ios_device/servers/diagnostics_relay.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7844 2023-04-20 02:15:07.000000 py_ios_device-2.3.32.2/ios_device/servers/dvt.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1223 2023-03-07 02:32:12.000000 py_ios_device-2.3.32.2/ios_device/servers/house_arrest.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3536 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/image_mounter.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     1679 2023-03-17 09:31:16.000000 py_ios_device-2.3.32.2/ios_device/servers/mc_install.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    31263 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/notification_proxy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2834 2023-04-20 02:31:19.000000 py_ios_device-2.3.32.2/ios_device/servers/os_trace.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3163 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/pcapd.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2023-01-04 04:20:57.000000 py_ios_device-2.3.32.2/ios_device/servers/simulate_location.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2023-03-31 08:20:40.000000 py_ios_device-2.3.32.2/ios_device/servers/spring_board.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3329 2023-01-04 03:41:43.000000 py_ios_device-2.3.32.2/ios_device/servers/syslog.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      864 2023-04-17 09:44:17.000000 py_ios_device-2.3.32.2/ios_device/servers/testmanagerd.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.185495 py_ios_device-2.3.32.2/ios_device/util/
--rw-r--r--   0 rongcloud   (501) staff       (20)     1860 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/util/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    11825 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/util/api_util.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    24888 2022-12-08 06:30:13.000000 py_ios_device-2.3.32.2/ios_device/util/bpylist2.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/util/ca.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/util/constants.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/util/dtx_msg.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1842 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/util/exceptions.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/util/forward.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-01-04 06:39:27.000000 py_ios_device-2.3.32.2/ios_device/util/gpu_decode.py
--rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.2/ios_device/util/kc_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    41845 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.2/ios_device/util/kperf_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    16216 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.2/ios_device/util/lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    16285 2023-04-20 02:30:51.000000 py_ios_device-2.3.32.2/ios_device/util/lockdown.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3131 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/util/plist_service.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    27335 2023-04-26 02:45:02.000000 py_ios_device-2.3.32.2/ios_device/util/plistlib.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    12592 2023-03-31 09:19:13.000000 py_ios_device-2.3.32.2/ios_device/util/usbmux.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     9513 2023-02-09 09:51:53.000000 py_ios_device-2.3.32.2/ios_device/util/utils.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4261 2023-02-14 02:46:09.000000 py_ios_device-2.3.32.2/ios_device/util/variables.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.186294 py_ios_device-2.3.32.2/py_ios_device.egg-info/
--rw-r--r--   0 rongcloud   (501) staff       (20)    11417 2023-05-24 02:44:55.000000 py_ios_device-2.3.32.2/py_ios_device.egg-info/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)     2406 2023-05-24 02:44:55.000000 py_ios_device-2.3.32.2/py_ios_device.egg-info/SOURCES.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)        1 2023-05-24 02:44:55.000000 py_ios_device-2.3.32.2/py_ios_device.egg-info/dependency_links.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       51 2023-05-24 02:44:55.000000 py_ios_device-2.3.32.2/py_ios_device.egg-info/entry_points.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      141 2023-05-24 02:44:55.000000 py_ios_device-2.3.32.2/py_ios_device.egg-info/requires.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       16 2023-05-24 02:44:55.000000 py_ios_device-2.3.32.2/py_ios_device.egg-info/top_level.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      140 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.2/requirements.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       38 2023-05-24 02:44:55.186930 py_ios_device-2.3.32.2/setup.cfg
--rw-r--r--   0 rongcloud   (501) staff       (20)      976 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.2/setup.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      959 2023-04-20 03:34:06.000000 py_ios_device-2.3.32.2/setup2.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.118786 py_ios_device-2.3.32.4/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/LICENSE
+-rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/MANIFEST.in
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11417 2023-06-16 01:58:43.118579 py_ios_device-2.3.32.4/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)    10950 2023-05-24 02:33:49.000000 py_ios_device-2.3.32.4/README.md
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.102994 py_ios_device-2.3.32.4/demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/demo/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/demo/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/demo/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2023-03-07 02:35:28.000000 py_ios_device-2.3.32.4/demo/installation_proxy.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.106148 py_ios_device-2.3.32.4/demo/instrument_demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/demo/instrument_demo/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/demo/instrument_demo/activity.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.4/demo/instrument_demo/app_lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/demo/instrument_demo/applictionListing.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.4/demo/instrument_demo/channel.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4146 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.4/demo/instrument_demo/coreprofilesessiontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.4/demo/instrument_demo/coreprofilesessiontap_parse.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2174 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.4/demo/instrument_demo/deviceinfo.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      494 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.4/demo/instrument_demo/energy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2199 2023-05-08 09:42:27.000000 py_ios_device-2.3.32.4/demo/instrument_demo/gpu.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.4/demo/instrument_demo/graphics.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      748 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.4/demo/instrument_demo/launchAPP.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 py_ios_device-2.3.32.4/demo/instrument_demo/mobileNotifications.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.4/demo/instrument_demo/netstatPID.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.4/demo/instrument_demo/networking.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2554 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.4/demo/instrument_demo/sysmontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/demo/instrument_demo/xcuitest.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/demo/mobile_config.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/demo/pcapd.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/demo/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/demo/syslog.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.106753 py_ios_device-2.3.32.4/ios_device/
+-rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)       25 2023-06-16 01:58:41.000000 py_ios_device-2.3.32.4/ios_device/__version__.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.108377 py_ios_device-2.3.32.4/ios_device/cli/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/cli/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    31554 2023-05-24 02:44:13.000000 py_ios_device-2.3.32.4/ios_device/cli/base.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      988 2023-04-07 02:33:45.000000 py_ios_device-2.3.32.4/ios_device/cli/cli.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    19122 2023-05-24 02:30:31.000000 py_ios_device-2.3.32.4/ios_device/cli/instruments.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11223 2023-04-26 06:21:46.000000 py_ios_device-2.3.32.4/ios_device/cli/mobile.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      293 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/main.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.4/ios_device/py_ios_device.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.112736 py_ios_device-2.3.32.4/ios_device/servers/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7287 2023-04-26 03:35:04.000000 py_ios_device-2.3.32.4/ios_device/servers/Installation.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1029 2023-04-20 02:15:07.000000 py_ios_device-2.3.32.4/ios_device/servers/Instrument.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/servers/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    19387 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/amfi.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      993 2023-05-22 06:59:19.000000 py_ios_device-2.3.32.4/ios_device/servers/diagnostics_relay.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7844 2023-06-16 01:58:11.000000 py_ios_device-2.3.32.4/ios_device/servers/dvt.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1223 2023-03-07 02:32:12.000000 py_ios_device-2.3.32.4/ios_device/servers/house_arrest.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3536 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/image_mounter.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     1679 2023-03-17 09:31:16.000000 py_ios_device-2.3.32.4/ios_device/servers/mc_install.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    31263 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/notification_proxy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2834 2023-04-20 02:31:19.000000 py_ios_device-2.3.32.4/ios_device/servers/os_trace.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3163 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/pcapd.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/servers/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2023-01-04 04:20:57.000000 py_ios_device-2.3.32.4/ios_device/servers/simulate_location.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2023-03-31 08:20:40.000000 py_ios_device-2.3.32.4/ios_device/servers/spring_board.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3329 2023-01-04 03:41:43.000000 py_ios_device-2.3.32.4/ios_device/servers/syslog.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      864 2023-04-17 09:44:17.000000 py_ios_device-2.3.32.4/ios_device/servers/testmanagerd.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.117568 py_ios_device-2.3.32.4/ios_device/util/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1860 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/util/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11825 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/util/api_util.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    24888 2022-12-08 06:30:13.000000 py_ios_device-2.3.32.4/ios_device/util/bpylist2.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/util/ca.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/util/constants.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2023-06-16 01:57:52.000000 py_ios_device-2.3.32.4/ios_device/util/dtx_msg.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1842 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/util/exceptions.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.4/ios_device/util/forward.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-01-04 06:39:27.000000 py_ios_device-2.3.32.4/ios_device/util/gpu_decode.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.4/ios_device/util/kc_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    41845 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.4/ios_device/util/kperf_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    16216 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.4/ios_device/util/lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    16285 2023-04-20 02:30:51.000000 py_ios_device-2.3.32.4/ios_device/util/lockdown.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3131 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.4/ios_device/util/plist_service.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    27335 2023-04-26 02:45:02.000000 py_ios_device-2.3.32.4/ios_device/util/plistlib.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    12592 2023-03-31 09:19:13.000000 py_ios_device-2.3.32.4/ios_device/util/usbmux.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     9547 2023-06-16 01:52:25.000000 py_ios_device-2.3.32.4/ios_device/util/utils.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4261 2023-02-14 02:46:09.000000 py_ios_device-2.3.32.4/ios_device/util/variables.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-06-16 01:58:43.118376 py_ios_device-2.3.32.4/py_ios_device.egg-info/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11417 2023-06-16 01:58:43.000000 py_ios_device-2.3.32.4/py_ios_device.egg-info/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2406 2023-06-16 01:58:43.000000 py_ios_device-2.3.32.4/py_ios_device.egg-info/SOURCES.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)        1 2023-06-16 01:58:43.000000 py_ios_device-2.3.32.4/py_ios_device.egg-info/dependency_links.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       51 2023-06-16 01:58:43.000000 py_ios_device-2.3.32.4/py_ios_device.egg-info/entry_points.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      141 2023-06-16 01:58:43.000000 py_ios_device-2.3.32.4/py_ios_device.egg-info/requires.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       16 2023-06-16 01:58:43.000000 py_ios_device-2.3.32.4/py_ios_device.egg-info/top_level.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      140 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.4/requirements.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       38 2023-06-16 01:58:43.118836 py_ios_device-2.3.32.4/setup.cfg
+-rw-r--r--   0 rongcloud   (501) staff       (20)      976 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.4/setup.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      958 2023-05-24 02:53:19.000000 py_ios_device-2.3.32.4/setup2.py
```

### Comparing `py_ios_device-2.3.32.2/LICENSE` & `py_ios_device-2.3.32.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/PKG-INFO` & `py_ios_device-2.3.32.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ios_device
-Version: 2.3.32.2
+Version: 2.3.32.4
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
 Maintainer: chenpeijie
 Maintainer-email: 
 License: UNKNOWN
```

### Comparing `py_ios_device-2.3.32.2/README.md` & `py_ios_device-2.3.32.4/README.md`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/afc.py` & `py_ios_device-2.3.32.4/demo/afc.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/crash_log.py` & `py_ios_device-2.3.32.4/demo/crash_log.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/installation_proxy.py` & `py_ios_device-2.3.32.4/demo/installation_proxy.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/activity.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/activity.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/app_lifecycle.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/app_lifecycle.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/applictionListing.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/applictionListing.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/coreprofilesessiontap.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/coreprofilesessiontap.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/coreprofilesessiontap_parse.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/coreprofilesessiontap_parse.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/deviceinfo.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/deviceinfo.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/gpu.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/gpu.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/graphics.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/graphics.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/launchAPP.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/launchAPP.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/mobileNotifications.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/mobileNotifications.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/netstatPID.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/netstatPID.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/networking.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/networking.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/sysmontap.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/sysmontap.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/instrument_demo/xcuitest.py` & `py_ios_device-2.3.32.4/demo/instrument_demo/xcuitest.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/mobile_config.py` & `py_ios_device-2.3.32.4/demo/mobile_config.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/pcapd.py` & `py_ios_device-2.3.32.4/demo/pcapd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/screenshotr.py` & `py_ios_device-2.3.32.4/demo/screenshotr.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/demo/syslog.py` & `py_ios_device-2.3.32.4/demo/syslog.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/cli/base.py` & `py_ios_device-2.3.32.4/ios_device/cli/base.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/cli/cli.py` & `py_ios_device-2.3.32.4/ios_device/cli/cli.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/cli/instruments.py` & `py_ios_device-2.3.32.4/ios_device/cli/instruments.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/cli/mobile.py` & `py_ios_device-2.3.32.4/ios_device/cli/mobile.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/py_ios_device.py` & `py_ios_device-2.3.32.4/ios_device/py_ios_device.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/Installation.py` & `py_ios_device-2.3.32.4/ios_device/servers/Installation.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/Instrument.py` & `py_ios_device-2.3.32.4/ios_device/servers/Instrument.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/afc.py` & `py_ios_device-2.3.32.4/ios_device/servers/afc.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/amfi.py` & `py_ios_device-2.3.32.4/ios_device/servers/amfi.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/crash_log.py` & `py_ios_device-2.3.32.4/ios_device/servers/crash_log.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/diagnostics_relay.py` & `py_ios_device-2.3.32.4/ios_device/servers/diagnostics_relay.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/dvt.py` & `py_ios_device-2.3.32.4/ios_device/servers/dvt.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/house_arrest.py` & `py_ios_device-2.3.32.4/ios_device/servers/house_arrest.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/image_mounter.py` & `py_ios_device-2.3.32.4/ios_device/servers/image_mounter.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/mc_install.py` & `py_ios_device-2.3.32.4/ios_device/servers/mc_install.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/notification_proxy.py` & `py_ios_device-2.3.32.4/ios_device/servers/notification_proxy.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/os_trace.py` & `py_ios_device-2.3.32.4/ios_device/servers/os_trace.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/pcapd.py` & `py_ios_device-2.3.32.4/ios_device/servers/pcapd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/screenshotr.py` & `py_ios_device-2.3.32.4/ios_device/servers/screenshotr.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/simulate_location.py` & `py_ios_device-2.3.32.4/ios_device/servers/simulate_location.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/spring_board.py` & `py_ios_device-2.3.32.4/ios_device/servers/spring_board.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/syslog.py` & `py_ios_device-2.3.32.4/ios_device/servers/syslog.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/servers/testmanagerd.py` & `py_ios_device-2.3.32.4/ios_device/servers/testmanagerd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/__init__.py` & `py_ios_device-2.3.32.4/ios_device/util/__init__.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/api_util.py` & `py_ios_device-2.3.32.4/ios_device/util/api_util.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/bpylist2.py` & `py_ios_device-2.3.32.4/ios_device/util/bpylist2.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/ca.py` & `py_ios_device-2.3.32.4/ios_device/util/ca.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/constants.py` & `py_ios_device-2.3.32.4/ios_device/util/constants.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/dtx_msg.py` & `py_ios_device-2.3.32.4/ios_device/util/dtx_msg.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/exceptions.py` & `py_ios_device-2.3.32.4/ios_device/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/forward.py` & `py_ios_device-2.3.32.4/ios_device/util/forward.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/gpu_decode.py` & `py_ios_device-2.3.32.4/ios_device/util/gpu_decode.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/kc_data.py` & `py_ios_device-2.3.32.4/ios_device/util/kc_data.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/kperf_data.py` & `py_ios_device-2.3.32.4/ios_device/util/kperf_data.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/lifecycle.py` & `py_ios_device-2.3.32.4/ios_device/util/lifecycle.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/lockdown.py` & `py_ios_device-2.3.32.4/ios_device/util/lockdown.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/plist_service.py` & `py_ios_device-2.3.32.4/ios_device/util/plist_service.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/plistlib.py` & `py_ios_device-2.3.32.4/ios_device/util/plistlib.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/usbmux.py` & `py_ios_device-2.3.32.4/ios_device/util/usbmux.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/ios_device/util/utils.py` & `py_ios_device-2.3.32.4/ios_device/util/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         p_record += 64
     return _list
 
 
 def convertBytes(_bytes):
     lst = ['Bytes', 'KiB', 'MiB', 'GiB', 'TiB']
     i = 0
-    if _bytes:
+    if isinstance(_bytes, int) and (_bytes > 0):
         i = int(math.floor(  # 舍弃小数点，取小
             math.log(_bytes, 1024)  # 求对数(对数：若 a**b = N 则 b 叫做以 a 为底 N 的对数)
         ))
     if i >= len(lst):
         i = len(lst) - 1
     return ('%.2f' + " " + lst[i]) % (_bytes / math.pow(1024, i))
```

### Comparing `py_ios_device-2.3.32.2/ios_device/util/variables.py` & `py_ios_device-2.3.32.4/ios_device/util/variables.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/py_ios_device.egg-info/PKG-INFO` & `py_ios_device-2.3.32.4/py_ios_device.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ios-device
-Version: 2.3.32.2
+Version: 2.3.32.4
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
 Maintainer: chenpeijie
 Maintainer-email: 
 License: UNKNOWN
```

### Comparing `py_ios_device-2.3.32.2/py_ios_device.egg-info/SOURCES.txt` & `py_ios_device-2.3.32.4/py_ios_device.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/setup.py` & `py_ios_device-2.3.32.4/setup.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.2/setup2.py` & `py_ios_device-2.3.32.4/setup2.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,11 +23,11 @@
       python_requires=">=3.7",
       classifiers=[
           "Programming Language :: Python :: 3",
           "Operating System :: OS Independent",
       ],
       entry_points={
           'console_scripts':{
-              'pyidevice=ios_device.main:cli'
+              'pyidevice=pyidevice.main:cli'
           }
       },
 )
```

