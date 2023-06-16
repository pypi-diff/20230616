# Comparing `tmp/bgpneiget-1.1.0.tar.gz` & `tmp/bgpneiget-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgpneiget-1.1.0.tar", max compression
+gzip compressed data, was "bgpneiget-2.0.0.tar", max compression
```

## Comparing `bgpneiget-1.1.0.tar` & `bgpneiget-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,19 @@
--rw-r--r--   0        0        0     1322 2021-11-10 12:20:25.080531 bgpneiget-1.1.0/LICENSE
--rw-r--r--   0        0        0      288 2021-11-10 12:20:25.084530 bgpneiget-1.1.0/README.md
--rw-r--r--   0        0        0      647 2023-01-23 09:57:23.580354 bgpneiget-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-01-23 09:57:35.664500 bgpneiget-1.1.0/src/bgpneiget/__init__.py
--rw-r--r--   0        0        0    11722 2021-11-10 12:20:25.084530 bgpneiget-1.1.0/src/bgpneiget/cli.py
--rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 bgpneiget-1.1.0/setup.py
--rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 bgpneiget-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1322 2023-05-12 08:43:10.928107 bgpneiget-2.0.0/LICENSE
+-rw-r--r--   0        0        0      288 2023-05-12 08:43:10.928107 bgpneiget-2.0.0/README.md
+-rw-r--r--   0        0        0      753 2023-05-24 09:08:36.528427 bgpneiget-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      272 2023-05-12 14:51:15.927138 bgpneiget-2.0.0/src/bgpneiget/__init__.py
+-rw-r--r--   0        0        0     6599 2023-06-12 16:01:39.992571 bgpneiget-2.0.0/src/bgpneiget/cli.py
+-rw-r--r--   0        0        0        0 2023-05-12 12:50:58.436841 bgpneiget-2.0.0/src/bgpneiget/device/__init__.py
+-rw-r--r--   0        0        0      871 2023-05-17 08:19:38.384271 bgpneiget-2.0.0/src/bgpneiget/device/arista.py
+-rw-r--r--   0        0        0     2728 2023-05-18 12:43:21.775962 bgpneiget-2.0.0/src/bgpneiget/device/base.py
+-rw-r--r--   0        0        0     9974 2023-05-25 13:39:58.309156 bgpneiget-2.0.0/src/bgpneiget/device/cisco_iosxe.py
+-rw-r--r--   0        0        0     5684 2023-05-25 13:40:00.373175 bgpneiget-2.0.0/src/bgpneiget/device/cisco_iosxr.py
+-rw-r--r--   0        0        0     1089 2023-05-18 13:31:42.764240 bgpneiget-2.0.0/src/bgpneiget/device/cisco_nxos.py
+-rw-r--r--   0        0        0    10670 2023-05-24 11:08:34.802078 bgpneiget-2.0.0/src/bgpneiget/device/juniper.py
+-rw-r--r--   0        0        0     1104 2023-05-18 09:46:19.385236 bgpneiget-2.0.0/src/bgpneiget/devices.py
+-rw-r--r--   0        0        0     1574 2023-05-22 08:21:44.302857 bgpneiget-2.0.0/src/bgpneiget/runcmds.py
+-rw-r--r--   0        0        0      243 2023-05-18 09:45:03.544509 bgpneiget-2.0.0/src/bgpneiget/textfsm/cisco_iosxe_show_bgp.textfsm
+-rw-r--r--   0        0        0      529 2023-05-18 12:43:21.775962 bgpneiget-2.0.0/src/bgpneiget/textfsm/cisco_iosxe_show_bgp_vrf.textfsm
+-rw-r--r--   0        0        0      510 2023-05-17 15:12:06.559095 bgpneiget-2.0.0/src/bgpneiget/textfsm/cisco_iosxr_show_bgp.textfsm
+-rw-r--r--   0        0        0     3505 2023-06-12 15:16:04.745621 bgpneiget-2.0.0/src/bgpneiget/worker.py
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 bgpneiget-2.0.0/PKG-INFO
```

### Comparing `bgpneiget-1.1.0/LICENSE` & `bgpneiget-2.0.0/LICENSE`

 * *Files identical despite different names*

