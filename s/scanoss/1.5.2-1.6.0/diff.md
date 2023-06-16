# Comparing `tmp/scanoss-1.5.2.tar.gz` & `tmp/scanoss-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanoss-1.5.2.tar", last modified: Tue Jun 13 11:04:41 2023, max compression
+gzip compressed data, was "scanoss-1.6.0.tar", last modified: Fri Jun 16 17:04:30 2023, max compression
```

## Comparing `scanoss-1.5.2.tar` & `scanoss-1.6.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 11:04:16.000000 scanoss-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-13 11:04:16.000000 scanoss-1.5.2/PACKAGE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-13 11:04:41.213340 scanoss-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-13 11:04:16.000000 scanoss-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-13 11:04:16.000000 scanoss-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-13 11:04:41.217340 scanoss-1.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.205340 scanoss-1.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.209340 scanoss-1.5.2/src/scanoss/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/common/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/common/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/common/v2/scanoss_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/common/v2/scanoss_common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/components/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/components/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/components/v2/scanoss_components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.205340 scanoss-1.5.2/src/scanoss/api/cryptography/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/cryptography/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/dependencies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/dependencies/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/dependencies/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/scanning/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/scanning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/scanning/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/scanning/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/vulnerabilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/vulnerabilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    33722 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/csvoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/cyclonedx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 11:04:29.000000 scanoss-1.5.2/src/scanoss/data/build_date.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/data/spdx-exceptions.json
--rw-r--r--   0 runner    (1001) docker     (123)   228794 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/data/spdx-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/filecount.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/scancodedeps.py
--rw-r--r--   0 runner    (1001) docker     (123)    41153 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/scanossapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/scanossbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/scanossgrpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/scantype.py
--rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/spdxlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/threadeddependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/threadedscanning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/winnowing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-13 11:04:41.000000 scanoss-1.5.2/src/scanoss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-13 11:04:41.000000 scanoss-1.5.2/src/scanoss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:04:41.000000 scanoss-1.5.2/src/scanoss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 11:04:41.000000 scanoss-1.5.2/src/scanoss.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-13 11:04:41.000000 scanoss-1.5.2/src/scanoss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 11:04:41.000000 scanoss-1.5.2/src/scanoss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-16 17:04:04.000000 scanoss-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-16 17:04:04.000000 scanoss-1.6.0/PACKAGE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-16 17:04:30.286773 scanoss-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-16 17:04:04.000000 scanoss-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-16 17:04:04.000000 scanoss-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-16 17:04:30.286773 scanoss-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.278772 scanoss-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/common/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/common/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/common/v2/scanoss_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/common/v2/scanoss_common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/components/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/components/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/components/v2/scanoss_components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.278772 scanoss-1.6.0/src/scanoss/api/cryptography/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/cryptography/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss/api/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/dependencies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/src/scanoss/api/dependencies/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/dependencies/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/src/scanoss/api/scanning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/scanning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/src/scanoss/api/scanning/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/scanning/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/src/scanoss/api/vulnerabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/vulnerabilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34052 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/csvoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/cyclonedx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.286773 scanoss-1.6.0/src/scanoss/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 17:04:18.000000 scanoss-1.6.0/src/scanoss/data/build_date.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/data/spdx-exceptions.json
+-rw-r--r--   0 runner    (1001) docker     (123)   228794 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/data/spdx-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/filecount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/scancodedeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41214 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/scanossapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/scanossbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/scanossgrpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/scantype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/spdxlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/threadeddependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/threadedscanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14465 2023-06-16 17:04:04.000000 scanoss-1.6.0/src/scanoss/winnowing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:04:30.282773 scanoss-1.6.0/src/scanoss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-16 17:04:30.000000 scanoss-1.6.0/src/scanoss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-16 17:04:30.000000 scanoss-1.6.0/src/scanoss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:04:30.000000 scanoss-1.6.0/src/scanoss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 17:04:30.000000 scanoss-1.6.0/src/scanoss.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 17:04:30.000000 scanoss-1.6.0/src/scanoss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 17:04:30.000000 scanoss-1.6.0/src/scanoss.egg-info/top_level.txt
```

### Comparing `scanoss-1.5.2/LICENSE` & `scanoss-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/PACKAGE.md` & `scanoss-1.6.0/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/PKG-INFO` & `scanoss-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanoss
-Version: 1.5.2
+Version: 1.6.0
 Summary: Simple Python library to leverage the SCANOSS APIs
 Home-page: https://scanoss.com
 Author: SCANOSS
 Author-email: info@scanoss.com
 License: MIT
 Project-URL: Source, https://github.com/scanoss/scanoss.py
 Project-URL: Tracker, https://github.com/scanoss/scanoss.py/issues
```

### Comparing `scanoss-1.5.2/README.md` & `scanoss-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/setup.cfg` & `scanoss-1.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/__init__.py` & `scanoss-1.6.0/src/scanoss/api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,9 +17,7 @@
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
-
-__version__ = '1.5.2'
```

### Comparing `scanoss-1.5.2/src/scanoss/api/__init__.py` & `scanoss-1.6.0/src/scanoss/api/common/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/common/__init__.py` & `scanoss-1.6.0/src/scanoss/api/common/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/common/v2/__init__.py` & `scanoss-1.6.0/src/scanoss/api/components/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/common/v2/scanoss_common_pb2.py` & `scanoss-1.6.0/src/scanoss/api/common/v2/scanoss_common_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/components/__init__.py` & `scanoss-1.6.0/src/scanoss/api/components/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/components/v2/__init__.py` & `scanoss-1.6.0/src/scanoss/api/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/components/v2/scanoss_components_pb2.py` & `scanoss-1.6.0/src/scanoss/api/components/v2/scanoss_components_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py` & `scanoss-1.6.0/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py` & `scanoss-1.6.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py` & `scanoss-1.6.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/dependencies/__init__.py` & `scanoss-1.6.0/src/scanoss/api/dependencies/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/dependencies/v2/__init__.py` & `scanoss-1.6.0/src/scanoss/api/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py` & `scanoss-1.6.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py` & `scanoss-1.6.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/scanning/__init__.py` & `scanoss-1.6.0/src/scanoss/api/scanning/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/scanning/v2/__init__.py` & `scanoss-1.6.0/src/scanoss/api/vulnerabilities/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
  SPDX-License-Identifier: MIT
 
-   Copyright (c) 2021, SCANOSS
+   Copyright (c) 2022, SCANOSS
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
```

### Comparing `scanoss-1.5.2/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py` & `scanoss-1.6.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py` & `scanoss-1.6.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/vulnerabilities/__init__.py` & `scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/__init__.py` & `scanoss-1.6.0/src/scanoss/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
  SPDX-License-Identifier: MIT
 
-   Copyright (c) 2022, SCANOSS
+   Copyright (c) 2021, SCANOSS
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
@@ -17,7 +17,9 @@
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
+
+__version__ = '1.6.0'
```

### Comparing `scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py` & `scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py` & `scanoss-1.6.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/cli.py` & `scanoss-1.6.0/src/scanoss/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     p_scan.add_argument('--obfuscate', action='store_true', help='Obfuscate file paths and names')
     p_scan.add_argument('--dependencies', '-D', action='store_true', help='Add Dependency scanning')
     p_scan.add_argument('--dependencies-only', action='store_true', help='Run Dependency scanning only')
     p_scan.add_argument('--sc-command', type=str,
                         help='Scancode command and path if required (optional - default scancode).')
     p_scan.add_argument('--sc-timeout', type=int, default=600,
                         help='Timeout (in seconds) for scancode to complete (optional - default 600)')
+    p_scan.add_argument('--hpsm', '-H', action='store_true', help='Scan using High Precision Snippet Matching')
 
     # Sub-command: fingerprint
     p_wfp = subparsers.add_parser('fingerprint', aliases=['fp', 'wfp'],
                                   description=f'Fingerprint the given source base: {__version__}',
                                   help='Fingerprint source code')
     p_wfp.set_defaults(func=wfp)
     p_wfp.add_argument('scan_dir', metavar='FILE/DIR', type=str, nargs='?',
@@ -116,14 +117,15 @@
                         help='Fingerprint the file contents supplied via STDIN (optional)')
     p_wfp.add_argument('--output', '-o', type=str, help='Output result file name (optional - default stdout).')
     p_wfp.add_argument('--obfuscate', action='store_true', help='Obfuscate fingerprints')
     p_wfp.add_argument('--skip-snippets', '-S', action='store_true', help='Skip the generation of snippets')
     p_wfp.add_argument('--all-extensions', action='store_true', help='Fingerprint all file extensions')
     p_wfp.add_argument('--all-folders', action='store_true', help='Fingerprint all folders')
     p_wfp.add_argument('--all-hidden', action='store_true', help='Fingerprint all hidden files/folders')
+    p_wfp.add_argument('--hpsm', '-H', action='store_true', help='Use High Precision Snippet Matching algorithm.')
 
     # Sub-command: dependency
     p_dep = subparsers.add_parser('dependencies', aliases=['dp', 'dep'],
                                   description=f'Produce dependency file summary: {__version__}',
                                   help='Scan source code for dependencies, but do not decorate them')
     p_dep.set_defaults(func=dependency)
     p_dep.add_argument('scan_dir', metavar='FILE/DIR', type=str, nargs='?', help='A file or folder to scan')
@@ -326,15 +328,15 @@
     if args.output:
         scan_output = args.output
         open(scan_output, 'w').close()
 
     scan_options = 0 if args.skip_snippets else ScanType.SCAN_SNIPPETS.value  # Skip snippet generation or not
     scanner = Scanner(debug=args.debug, trace=args.trace, quiet=args.quiet, obfuscate=args.obfuscate,
                       scan_options=scan_options, all_extensions=args.all_extensions,
-                      all_folders=args.all_folders, hidden_files_folders=args.all_hidden)
+                      all_folders=args.all_folders, hidden_files_folders=args.all_hidden, hpsm=args.hpsm)
 
     if args.stdin:
         contents = sys.stdin.buffer.read()
         scanner.wfp_contents(args.stdin, contents, scan_output)
     elif args.scan_dir:
         if not os.path.exists(args.scan_dir):
             print_stderr(f'Error: File or folder specified does not exist: {args.scan_dir}.')
@@ -455,14 +457,16 @@
             print_stderr(f'Using Proxy {args.proxy}...')
         if args.grpc_proxy:
             print_stderr(f'Using GRPC Proxy {args.grpc_proxy}...')
         if args.pac:
             print_stderr(f'Using Proxy Auto-config (PAC) {args.pac}...')
         if args.ca_cert:
             print_stderr(f'Using Certificate {args.ca_cert}...')
+        if args.hpsm:
+            print_stderr("Setting HPSM mode...")
         if flags:
             print_stderr(f'Using flags {flags}...')
     elif not args.quiet:
         if args.timeout < 5:
             print_stderr(f'POST timeout (--timeout) too small: {args.timeout}. Reverting to default.')
         if args.retry < 0:
             print_stderr(f'POST retry (--retry) too small: {args.retry}. Reverting to default.')
@@ -480,15 +484,15 @@
                       sbom_path=sbom_path, scan_type=scan_type, scan_output=scan_output, output_format=output_format,
                       flags=flags, nb_threads=args.threads, post_size=args.post_size,
                       timeout=args.timeout, no_wfp_file=args.no_wfp_output, all_extensions=args.all_extensions,
                       all_folders=args.all_folders, hidden_files_folders=args.all_hidden,
                       scan_options=scan_options, sc_timeout=args.sc_timeout, sc_command=args.sc_command,
                       grpc_url=args.api2url, obfuscate=args.obfuscate,
                       ignore_cert_errors=args.ignore_cert_errors, proxy=args.proxy, grpc_proxy=args.grpc_proxy,
-                      pac=pac_file, ca_cert=args.ca_cert, retry=args.retry
+                      pac=pac_file, ca_cert=args.ca_cert, retry=args.retry, hpsm=args.hpsm
                       )
     if args.wfp:
         if not scanner.is_file_or_snippet_scan():
             print_stderr(f'Error: Cannot specify WFP scanning if file/snippet options are disabled ({scan_options})')
             exit(1)
         if args.threads > 1:
             scanner.scan_wfp_file_threaded(args.wfp)
```

### Comparing `scanoss-1.5.2/src/scanoss/components.py` & `scanoss-1.6.0/src/scanoss/components.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/csvoutput.py` & `scanoss-1.6.0/src/scanoss/csvoutput.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/cyclonedx.py` & `scanoss-1.6.0/src/scanoss/cyclonedx.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/data/spdx-exceptions.json` & `scanoss-1.6.0/src/scanoss/data/spdx-exceptions.json`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/data/spdx-licenses.json` & `scanoss-1.6.0/src/scanoss/data/spdx-licenses.json`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/filecount.py` & `scanoss-1.6.0/src/scanoss/filecount.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/scancodedeps.py` & `scanoss-1.6.0/src/scanoss/scancodedeps.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/scanner.py` & `scanoss-1.6.0/src/scanoss/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     def __init__(self, wfp: str = None, scan_output: str = None, output_format: str = 'plain',
                  debug: bool = False, trace: bool = False, quiet: bool = False, api_key: str = None, url: str = None,
                  sbom_path: str = None, scan_type: str = None, flags: str = None, nb_threads: int = 5,
                  post_size: int = 64, timeout: int = 120, no_wfp_file: bool = False,
                  all_extensions: bool = False, all_folders: bool = False, hidden_files_folders: bool = False,
                  scan_options: int = 7, sc_timeout: int = 600, sc_command: str = None, grpc_url: str = None,
                  obfuscate: bool = False, ignore_cert_errors: bool = False, proxy: str = None, grpc_proxy: str = None,
-                 ca_cert: str = None, pac: PACFile = None, retry: int = 5
+                 ca_cert: str = None, pac: PACFile = None, retry: int = 5, hpsm: bool = False
                  ):
         """
         Initialise scanning class, including Winnowing, ScanossApi and ThreadedScanning
         """
         super().__init__(debug, trace, quiet)
         self.wfp = wfp if wfp else "scanner_output.wfp"
         self.scan_output = scan_output
@@ -113,18 +113,19 @@
         self.no_wfp_file = no_wfp_file
         self.isatty = sys.stderr.isatty()
         self.all_extensions = all_extensions
         self.all_folders = all_folders
         self.hidden_files_folders = hidden_files_folders
         self.scan_options = scan_options
         self._skip_snippets = True if not scan_options & ScanType.SCAN_SNIPPETS.value else False
+        self.hpsm = hpsm
         ver_details = Scanner.version_details()
 
         self.winnowing = Winnowing(debug=debug, quiet=quiet, skip_snippets=self._skip_snippets,
-                                   all_extensions=all_extensions, obfuscate=obfuscate
+                                   all_extensions=all_extensions, obfuscate=obfuscate, hpsm=self.hpsm
                                    )
         self.scanoss_api = ScanossApi(debug=debug, trace=trace, quiet=quiet, api_key=api_key, url=url,
                                       sbom_path=sbom_path, scan_type=scan_type, flags=flags, timeout=timeout,
                                       ver_details=ver_details, ignore_cert_errors=ignore_cert_errors,
                                       proxy=proxy, ca_cert=ca_cert, pac=pac, retry=retry
                                       )
         sc_deps = ScancodeDeps(debug=debug, quiet=quiet, trace=trace, timeout=sc_timeout, sc_command=sc_command)
```

### Comparing `scanoss-1.5.2/src/scanoss/scanossapi.py` & `scanoss-1.6.0/src/scanoss/scanossapi.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/scanossbase.py` & `scanoss-1.6.0/src/scanoss/scanossbase.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/scanossgrpc.py` & `scanoss-1.6.0/src/scanoss/scanossgrpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/scantype.py` & `scanoss-1.6.0/src/scanoss/scantype.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/spdxlite.py` & `scanoss-1.6.0/src/scanoss/spdxlite.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/threadeddependencies.py` & `scanoss-1.6.0/src/scanoss/threadeddependencies.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/threadedscanning.py` & `scanoss-1.6.0/src/scanoss/threadedscanning.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.2/src/scanoss/winnowing.py` & `scanoss-1.6.0/src/scanoss/winnowing.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,14 +56,18 @@
     ".exe", ".zip", ".tar", ".tgz", ".gz", ".7z", ".rar", ".jar", ".war", ".ear", ".class", ".pyc",
     ".o", ".a", ".so", ".obj", ".dll", ".lib", ".out", ".app", ".bin",
     ".lst", ".dat", ".json", ".htm", ".html", ".xml", ".md", ".txt",
     ".doc", ".docx", ".xls", ".xlsx", ".ppt", ".pptx", ".odt", ".ods", ".odp", ".pages", ".key", ".numbers",
     ".pdf", ".min.js", ".mf", ".sum"
 }
 
+CRC8_MAXIM_DOW_TABLE_SIZE = 0x100
+CRC8_MAXIM_DOW_POLYNOMIAL = 0x8C # 0x31 reflected
+CRC8_MAXIM_DOW_INITIAL = 0x00 # 0x00 reflected
+CRC8_MAXIM_DOW_FINAL = 0x00 # 0x00 reflected
 
 class Winnowing(ScanossBase):
     """
     Winnowing Algorithm implementation for SCANOSS.
 
     This module implements an adaptation of the original winnowing algorithm by
     S. Schleimer, D. S. Wilkerson and A. Aiken as described in their seminal article which can be found here:
@@ -101,15 +105,16 @@
 
     Where component is the MD5 hash and path of the component container (could be a path to a compressed file or URL).
     file is the MD5 hash, file length and file path being fingerprinted, followed by
     a list of WFP fingerprints with their corresponding line numbers.
     """
 
     def __init__(self, size_limit: bool = True, debug: bool = False, trace: bool = False, quiet: bool = False,
-                 skip_snippets: bool = False, post_size: int = 64, all_extensions: bool = False, obfuscate: bool = False
+                 skip_snippets: bool = False, post_size: int = 64, all_extensions: bool = False, 
+                 obfuscate: bool = False, hpsm: bool = False
                  ):
         """
         Instantiate Winnowing class
         Parameters
         ----------
             size_limit: bool
                 Limit the size of a fingerprint to 64k (post size) - Default True
@@ -118,14 +123,17 @@
         self.size_limit = size_limit
         self.skip_snippets = skip_snippets
         self.max_post_size = post_size * 1024 if post_size > 0 else MAX_POST_SIZE
         self.all_extensions = all_extensions
         self.obfuscate = obfuscate
         self.ob_count = 1
         self.file_map = {} if obfuscate else None
+        self.hpsm = hpsm
+        if hpsm:
+            self.crc8_maxim_dow_table = []
 
     @staticmethod
     def __normalize(byte):
         """
         Normalise a given byte as an ASCII character
         Parameters
         ----------
@@ -232,14 +240,18 @@
             self.ob_count = self.ob_count + 1
             self.file_map[wfp_filename] = file  # Save the file name map for later (reverse lookup)
 
         wfp = 'file={0},{1},{2}\n'.format(file_md5, content_length, wfp_filename)
         # We don't process snippets for binaries, or other uninteresting files, or if we're requested to skip
         if bin_file or self.skip_snippets or self.__skip_snippets(file, contents.decode('utf-8', 'ignore')):
             return wfp
+        # Add HPSM
+        if self.hpsm:
+            hpsm = self.calc_hpsm(contents)
+            wfp += 'hpsm={0}\n'.format(hpsm)
         # Initialize variables
         gram = ''
         window = []
         line = 1
         last_hash = MAX_CRC32
         last_line = 0
         output = ''
@@ -293,10 +305,60 @@
             else:
                 self.print_debug(f'Warning: skipping output in WFP for {file} - "{output}"')
 
         if wfp is None or wfp == '':
             self.print_stderr(f'Warning: No WFP content data for {file}')
         return wfp
 
+    def calc_hpsm(self, content):
+        list_normalized = []    #Array of numbers
+        crc_lines = []  #Array of numbers that represent the crc8_maxim for each line of the file
+        last_line = 0
+        self.crc8_generate_table()
+        for i, byte in enumerate(content):
+            c = byte
+            if c == ASCII_LF:   #When there is a new line
+                if len(list_normalized): 
+                    crc_lines.append(self.crc8_buffer(list_normalized))
+                    list_normalized=[]
+                elif last_line+1 == i:
+                    crc_lines.append(0xFF)
+                elif i-last_line  > 1:
+                    crc_lines.append(0x00)
+                last_line = i
+            else:
+                c_normalized = self.__normalize(c)
+                if c_normalized != 0:
+                    list_normalized.append(c_normalized)
+        crc_lines_hex = []
+        for x in crc_lines:
+            crc_lines_hex.append(hex(x))
+        hpsm = ''.join('{:02x}'.format(x) for x in crc_lines)
+        return hpsm
+
+    def crc8_generate_table(self):
+        for i in range(CRC8_MAXIM_DOW_TABLE_SIZE):
+            self.crc8_maxim_dow_table.append(self.crc8_byte_checksum(0, i))
+        
+    def crc8_byte_checksum(self, crc, byte):
+        crc ^= byte
+        for count in range(8):
+            isSet = crc & 0x01
+            crc >>= 1
+            if isSet:
+                crc ^= CRC8_MAXIM_DOW_POLYNOMIAL
+        return crc
+
+    def crc8_byte(self, crc, byte):
+        index = byte ^ crc
+        return self.crc8_maxim_dow_table[ index ] ^ ( crc >> 8 )
+
+    def crc8_buffer(self, buffer):
+        crc = CRC8_MAXIM_DOW_INITIAL
+        for index in range(len(buffer)):
+            crc = self.crc8_byte(crc, buffer[index])
+        crc ^= CRC8_MAXIM_DOW_FINAL
+        return crc
+    
 #
 # End of Winnowing Class
 #
```

### Comparing `scanoss-1.5.2/src/scanoss.egg-info/PKG-INFO` & `scanoss-1.6.0/src/scanoss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanoss
-Version: 1.5.2
+Version: 1.6.0
 Summary: Simple Python library to leverage the SCANOSS APIs
 Home-page: https://scanoss.com
 Author: SCANOSS
 Author-email: info@scanoss.com
 License: MIT
 Project-URL: Source, https://github.com/scanoss/scanoss.py
 Project-URL: Tracker, https://github.com/scanoss/scanoss.py/issues
```

### Comparing `scanoss-1.5.2/src/scanoss.egg-info/SOURCES.txt` & `scanoss-1.6.0/src/scanoss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

