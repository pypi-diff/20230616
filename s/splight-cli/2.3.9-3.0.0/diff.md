# Comparing `tmp/splight-cli-2.3.9.tar.gz` & `tmp/splight-cli-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-cli-2.3.9.tar", last modified: Mon Apr  3 11:29:34 2023, max compression
+gzip compressed data, was "splight-cli-3.0.0.tar", last modified: Fri Jun 16 12:53:12 2023, max compression
```

## Comparing `splight-cli-2.3.9.tar` & `splight-cli-3.0.0.tar`

### file list

```diff
@@ -1,100 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.772240 splight-cli-2.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-03 11:29:34.772240 splight-cli-2.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-04-03 11:29:33.000000 splight-cli-2.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.764240 splight-cli-2.3.9/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/component/
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/component/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/templates/Initialization
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/templates/auto_readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/templates/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/templates/spec.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/component/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/tests/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/tests/test_initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/tests/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/context/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/context/framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/context/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/deployment/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/alert/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/alert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/asset/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/attribute/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/attribute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/component/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/component/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/datalake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/datalake/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/datalake/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/datalake/tests/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/datalake/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/datalake/tests/test_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/file/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/manager/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/query/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/secret/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/setpoint/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/setpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/hub/component/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/hub/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/hub/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/hub/component/hub_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/tests/TestHub/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/tests/TestHub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/tests/test_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/tests/test_generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/api_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 11:29:34.772240 splight-cli-2.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-03 11:29:33.000000 splight-cli-2.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.772240 splight-cli-2.3.9/splight_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-03 11:29:34.000000 splight-cli-2.3.9/splight_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-03 11:29:34.000000 splight-cli-2.3.9/splight_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 11:29:34.000000 splight-cli-2.3.9/splight_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-03 11:29:34.000000 splight-cli-2.3.9/splight_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-03 11:29:34.000000 splight-cli-2.3.9/splight_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 11:29:34.000000 splight-cli-2.3.9/splight_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.184711 splight-cli-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-16 12:53:12.184711 splight-cli-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-06-16 12:53:11.000000 splight-cli-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/component/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/.splightignore
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/Initialization
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/auto_readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/templates/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/component/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/component/tests/test_component_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/context/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/alert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/attribute/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/attribute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/datalake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17092 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/manager/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/engine/setpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/engine/setpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.180711 splight-cli-3.0.0/cli/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.184711 splight-cli-3.0.0/cli/hub/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/hub/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/hub/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/hub/component/hub_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.184711 splight-cli-3.0.0/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/utils/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.184711 splight-cli-3.0.0/cli/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-16 12:53:11.000000 splight-cli-3.0.0/cli/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:53:12.184711 splight-cli-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-16 12:53:11.000000 splight-cli-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:53:12.184711 splight-cli-3.0.0/splight_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-16 12:53:12.000000 splight-cli-3.0.0/splight_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-16 12:53:12.000000 splight-cli-3.0.0/splight_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:53:12.000000 splight-cli-3.0.0/splight_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-16 12:53:12.000000 splight-cli-3.0.0/splight_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-16 12:53:12.000000 splight-cli-3.0.0/splight_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 12:53:12.000000 splight-cli-3.0.0/splight_cli.egg-info/top_level.txt
```

### Comparing `splight-cli-2.3.9/README.md` & `splight-cli-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -304,18 +304,19 @@
 
 ```bash
 splight workspace <sub-command>
 ```
 
 The available subcommands are
 
-- `create` for creating new workspace. After the creation of a new worskpace you need to configure _Splight CLI_ with `splightcli configure`.
-- `delete` for deleting an existing workspace.
-- `list` for listing the differents configured workspaces and showing the workspace in use.
-- `select` for switching between the different configured workspaces.
+- `create <name>` to create a new workspace. After the creation of a new worskpace you need to configure _Splight CLI_ with `splight configure`.
+- `delete <name>` to delete an existing workspace.
+- `list` to list all workspaces. Current workspace displays a '*' to the left.
+- `select <name>` to switch between different configured workspaces.
+- `show <name>` to display the contents of an existing workspace.
 
 ## Developing Components
 
 Now it's time to talk about the process for developing components.
 
 ### What is a component?
 
@@ -534,12 +535,39 @@
 ```
 
 This is just an example but you can create custom types as complex as you want,
 the limit is your imagination.
 
 #### Running Locally
 
-You can run the component locally before pushing it to the platform
+You can run the component locally before pushing it to the platform with the `--local` option:
 
 ```bash
-splight component run <component directory>
+splight component run <component directory> --local
 ```
+
+This way, the component will run using local clients for database and datalake. This is extremely
+useful for development since you can create instances of the different database objects in the 
+local database for running different scenearios or differents tests. The same can be applied for 
+datalake data, the local client stores the data in files. In both cases, for database and datalake,
+the files are created in the same directory as the `__init__.py` file of the component, so you 
+can modified it based on your needs.
+
+You can interact with the local databases using the library, for example
+
+```python
+from splight_models import Asset, Attribute, Number
+from splight_lib.client.database import LocalDatabaseClient
+from splight_lib.client.datalake import LocalDatalakeClient
+
+
+component_path = ...
+db_client = LocalDatabaseClient(namespace="default", path=component_path)
+dl_client = LocalDatalakeClient(namespace="default", path=component_path)
+
+all_assets = db_client.get(Asset)
+attribute = Attribute(name="SomeAttribute")
+
+db_client.save(attribute)
+
+df = client.get_dataframe(Number, asset=all_assets[0].id, attribute=attribute.id)
+```
```

### Comparing `splight-cli-2.3.9/cli/component/exceptions.py` & `splight-cli-3.0.0/cli/engine/manager/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,47 @@
-from typing import Set
+from typing import Dict
 
 
-class InvalidCSVColumns(Exception):
-    def __init__(self, columns: Set[str]):
-        self._msg = (
-            "CSV file does not have the necessary columns. "
-            f"The required columns are {columns}."
-        )
+class InvalidComponentId(Exception):
+    """Exception raised when a component id is invalid."""
+
+    def __init__(self, id: str):
+        self._msg = f"Component with id {id} does not exist."
 
     def __str__(self) -> str:
         return self._msg
 
 
-class InvalidSplightCLIVersion(Exception):
-    def __init__(self, component_cli_version: str, cli_version: str):
-        self._msg = (
-            f"Component uses splight cli version {component_cli_version} but "
-            f"should be {cli_version}"
-        )
+class VersionUpdateError(Exception):
+    """Exception raised when the component is already updated."""
+
+    def __init__(self, name: str, version: str):
+        self._msg = f"Component {name} is already at version {version}."
 
     def __str__(self) -> str:
         return self._msg
 
 
-class ReadmeExists(Exception):
-    def __init__(self, readme_path: str):
+class ComponentCreateError(Exception):
+    """Exception raised when the component could not be saved."""
+
+    def __init__(
+        self, name: str, version: str, input_params: Dict, msg: str = None
+    ):
         self._msg = (
-            f"\nReadme already exists at {readme_path}"
-            f"\nRemove it or use --force to overwrite it"
+            f"An error occurred creating component {name}-{version}. "
+            f"Input parameters: {input_params}."
+            f"Error message: {msg}"
         )
 
     def __str__(self) -> str:
         return self._msg
+
+
+class UpdateParametersError(Exception):
+    """Exception when some parameter could not be updated."""
+
+    def __init__(self, param: Dict):
+        self._error = f"An error occurred updating parameter {param}"
+
+    def __str__(self) -> str:
+        return self._error
```

### Comparing `splight-cli-2.3.9/cli/component/templates/auto_readme.md` & `splight-cli-3.0.0/cli/component/templates/auto_readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,30 @@
 
 {% if custom_types is not none -%}
 The custom types defined by the component are:
 
 {% for item in custom_types -%}
   - {{item.name}}
      {% for p in item.fields -%}
-       {{p.name}} [{{p.type}}]: (Default: {{p.value}}) {{p.description}}
+      - {{p.name}} [{{p.type}}]: (Default: {{p.value}}) {{p.description}}
      {% endfor %}
 {% endfor -%}
 {%- else -%}
 This component does not have any custom type.
 {%- endif -%}
 
 ### Output
 
 {% if output is not none -%}
 The component's output are:
 
 {% for out in output -%}
   - {{out.name}}:
     {% for field in out.fields -%}
-      {{field.name}} [{{field.type}}]
+      - {{field.name}} [{{field.type}}]
     {% endfor %}
 {% endfor %}
 {%- else -%}
 This component does not have any output.
 {%- endif -%}
 
 ### Bindings
```

### Comparing `splight-cli-2.3.9/cli/component/templates/component.py` & `splight-cli-3.0.0/cli/component/templates/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 import random
-from typing import TypeVar
-from splight_lib.component import AbstractComponent
-from splight_lib.execution import Task
-from splight_lib import logging
-
-# Logging tool
-logger = logging.getLogger()
+from typing import Type
 
-# Custom Types
-## NOTE: In case you want to create new instances of this Class
-## You can find this model in self.custom_model.MyAsset inside the Main class
-MyAsset = TypeVar('MyAsset')
+import typer
+from splight_lib.component import SplightBaseComponent
+from splight_lib.execution import Task
+from splight_lib.logging import getLogger
+from splight_lib.models import Number
 
+app = typer.Typer(pretty_exceptions_enable=False)
+MyAsset = Type["MyAsset"]
 
-class Main(AbstractComponent):
 
-    # Init
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.my_assets = {
-            item.id: item
-            for item in self.database_client.get(self.custom_types.MyAsset)
-        }
-        logger.info(f"Starting randomizer in range {self.input.min} - {self.input.max}")
+class {{component_name}}(SplightBaseComponent):
+    def __init__(self, component_id: str):
+        super().__init__(component_id)
+        self._logger = getLogger("MyComponent")
 
-    # Starting point
     def start(self):
-        self.execution_client.start(
-            Task(handler=self._give_a_random_number, args=(self.input.min, self.input.max), period=self.input.period)
+        self.execution_engine.start(
+            Task(
+                handler=self._run,
+                args=(self.input.min, self.input.max),
+                period=self.input.period,
+            )
+        )
+
+    def _run(self, min_value: float, max_value: float):
+        value = self._give_a_random_value(
+            self.input.lower_bound, self.input.upper_bound
         )
-        self.execution_client.start(
-            Task(handler=self._list_assets, args=(), period=self.input.period)
+        preds = Number(
+            value=value,
         )
+        preds.save()
+        self._logger.info(f"\nValue = {value}\n")
 
-    # Periodic Tasks
-    def _give_a_random_number(self, min, max):
-        chosen_number = random.randint(min, max)
-        logger.info(f"Random number: {chosen_number}")
-        out = self.output.Value(value=chosen_number)
-        self.datalake_client.save(instances=[out])
+    def _give_a_random_value(self, min: float, max: float) -> float:
+        return (max - min) * random.random() + min
 
-    def _list_assets(self):
-        logger.info(f"List of myassets: List[MyAsset] {self.my_assets}")
+    def command_myasset_print(self, my_asset: MyAsset):
+        print("Command for MyAsset")
 
-    # Bindings
     def handle_myasset_create(self, my_asset: MyAsset):
-        self.my_assets[my_asset.id] = my_asset
-        logger.info(f"CREATED MyAsset: {my_asset}")
+        print("MyAsset create")
 
     def handle_myasset_delete(self, my_asset: MyAsset):
-        try:
-            logger.info(f"DELETED MyAsset: {my_asset}")
-            del self.my_assets[my_asset.id]
-        except KeyError:
-            pass
-
-    # Commands
-    def command_myasset_print(self, myasset: MyAsset):
-        logger.info(f"PRINTED MyAsset: {myasset}")
-        return myasset.dict()
+        print("MyAsset delete")
+
+
+@app.command()
+def main(component_id: str = typer.Option(...)):
+    logger = getLogger("MyComponent")
+    component = {{component_name}}(component_id=component_id)
+    try:
+        component.start()
+    except Exception as exc:
+        logger.exception(exc, tags="EXCEPTION")
+        component.stop()
+
+
+if __name__ == "__main__":
+    app()
```

### Comparing `splight-cli-2.3.9/cli/component/templates/spec.json` & `splight-cli-3.0.0/cli/component/templates/spec.json`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.9/cli/config/__init__.py` & `splight-cli-3.0.0/cli/config/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-import sys
 import json
+import sys
 
 import typer
-
-from cli.settings import SplightCLISettings, CONFIG_VARS
+from cli.settings import CONFIG_VARS, SplightCLISettings
 
 config_app = typer.Typer(
     name="Splight CLI Configure",
     add_completion=True,
 )
 
 
 @config_app.callback(invoke_without_command=True)
 def config(
     ctx: typer.Context,
     from_json: str = typer.Option(
-        None,
-        "--from-json",
-        help="Configuration by json instaed of prompt")
+        None, "--from-json", help="Configuration by json instaed of prompt"
+    ),
 ):
     if ctx.invoked_subcommand:
         return
 
     cli_context = ctx.obj
     try:
         if from_json:
@@ -30,32 +28,32 @@
         else:
             new_settings_data = {}
             for config_var in CONFIG_VARS:
                 default = getattr(
                     cli_context.workspace.settings, config_var, None
                 )
                 value = typer.prompt(
-                    typer.style(config_var, fg='yellow'),
+                    typer.style(config_var, fg="yellow"),
                     type=str,
                     default=default,
-                    show_default=True
+                    show_default=True,
                 )
                 new_settings_data.update({config_var: value})
             new_settings = SplightCLISettings.parse_obj(new_settings_data)
         cli_context.workspace.update_workspace(new_settings)
         typer.echo("Configuration saved successfully", color="green")
     except Exception as e:
         typer.echo(f"Error configuring Splight CLI: {str(e)}", color="red")
         sys.exit(1)
 
 
 @config_app.command(name="get")
 def get_variable(
     ctx: typer.Context,
-    var_name: str = typer.Argument(..., help="The variable name to get value")
+    var_name: str = typer.Argument(..., help="The variable name to get value"),
 ):
     """Prints the value of the requested variable.
 
     Parameters
     ----------
     ctx: Context
         The current context
@@ -70,15 +68,15 @@
         typer.echo(value)
 
 
 @config_app.command(name="set")
 def set_variable(
     ctx: typer.Context,
     var_name: str = typer.Argument(..., help="The variable name to update"),
-    value: str = typer.Argument(..., help="The new value")
+    value: str = typer.Argument(..., help="The new value"),
 ):
     """Sets a value of a variable in the current workspace.
 
     Parameters
     ----------
     ctx: Context
         The current context
```

### Comparing `splight-cli-2.3.9/cli/constants.py` & `splight-cli-3.0.0/cli/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import os
 from pathlib import Path
-from pydantic import AnyUrl
-from rich.style import Style
 
 from cli.settings import SplightCLISettings
+from pydantic import AnyUrl
+from rich.style import Style
 
 error_style = Style(color="red", bold=True)
 success_style = Style(color="green")
 warning_style = Style(color="yellow")
 
-SPLIGHT_PATH = os.path.join(os.path.expanduser("~"), '.splight')
+SPLIGHT_PATH = os.path.join(os.path.expanduser("~"), ".splight")
 BASE_DIR = Path(__file__).resolve().parent.parent
 TEMPLATES_FOLDER = os.path.join(BASE_DIR, "cli", "component", "templates")
 
 COMPRESSION_TYPE = "7z"
-DEFAULT_NAMESPACE = 'NO_NAMESPACE'
+DEFAULT_NAMESPACE = "NO_NAMESPACE"
 DEFAULT_COMPONENT_ID = "DEMO"
-DEFAULT_WORKSPACE_NAME = 'default'
+DEFAULT_WORKSPACE_NAME = "default"
 DEFAULT_WORKSPACE = SplightCLISettings().dict()
-DEFAULT_WORKSPACES = {
-    DEFAULT_WORKSPACE_NAME: DEFAULT_WORKSPACE
-}
+DEFAULT_WORKSPACES = {DEFAULT_WORKSPACE_NAME: DEFAULT_WORKSPACE}
 
-CONFIG_FILE = os.path.join(SPLIGHT_PATH, 'config')
-COMPONENT_FILE = "__init__.py"
+CONFIG_FILE = os.path.join(SPLIGHT_PATH, "config")
+PYTHON_COMPONENT_FILE = "main.py"
 SPEC_FILE = "spec.json"
 INIT_FILE = "Initialization"
-README_FILE_1 = "README.md" 
-README_FILE_2 = "README" 
+README_FILE = "README.md"
+README_FILE_2 = "README"
 MAIN_CLASS_NAME = "Main"
 SPLIGHT_IGNORE = ".splightignore"
+PYTHON_TESTS_FILE = "tests.py"
+
+PYTHON_CMD = "python"
+PYTHON_TEST_CMD = "pytest"
 
 REQUIRED_DATALAKE_COLUMNS = {
     "timestamp",
     "asset",
     "attribute",
     "value",
-    "output_format"
+    "output_format",
 }
 
 VALID_PARAMETER_VALUES = {
     "int": int,
     "bool": bool,
     "str": str,
     "float": float,
@@ -48,15 +50,15 @@
     "datetime": None,
     "file": None,  # UUID
     "File": None,  # UUID
     "Asset": None,  # UUID,
     "Attribute": None,  # UUID,
     "Component": None,  # UUID,
     "Graph": None,  # UUID,
-    "Query": None, # UUID,
-    "Mapping": None, # UUID
+    "Query": None,  # UUID,
+    "Mapping": None,  # UUID
 }
 
 VALID_DEPENDS_ON = [
     ("Asset", "Graph"),
     ("Attribute", "Asset"),
 ]
```

### Comparing `splight-cli-2.3.9/cli/context/workspace.py` & `splight-cli-3.0.0/cli/context/workspace.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,7 +95,12 @@
     def create_workspace(self, workspace_name: str):
         if workspace_name in self._config.workspaces:
             raise Exception("Name already exists")
         self._config.workspaces.update({workspace_name: DEFAULT_WORKSPACE})
         self._config.current_workspace = workspace_name
         self._current_workspace = workspace_name
         save_yaml_to_file(self._config.dict(), self.config_file)
+
+    def list_workspace_contents(self, workspace_name: str):
+        if workspace_name not in self._config.workspaces:
+            raise NotExistingWorkspace(workspace_name)
+        return self._config.workspaces[workspace_name]
```

### Comparing `splight-cli-2.3.9/cli/engine/__init__.py` & `splight-cli-3.0.0/cli/engine/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 import typer
-
 from cli.context import check_credentials
 from cli.engine.alert import alert_app
 from cli.engine.asset import asset_app
 from cli.engine.attribute import attribute_app
 from cli.engine.component import component_app
-from cli.engine.graph import graph_app
-from cli.engine.query import query_app
+from cli.engine.datalake import datalake_app
 from cli.engine.file import file_app
 from cli.engine.secret import secret_app
 from cli.engine.setpoint import setpoint_app
-from cli.engine.datalake import datalake_app
 
 engine_app = typer.Typer(
     name="Splight Engine",
     add_completion=True,
     rich_markup_mode="rich",
     no_args_is_help=True,
 )
 
 engine_app.add_typer(alert_app, name="alert")
 engine_app.add_typer(asset_app, name="asset")
 engine_app.add_typer(attribute_app, name="attribute")
 engine_app.add_typer(component_app, name="component")
-engine_app.add_typer(graph_app, name="graph")
-engine_app.add_typer(query_app, name="query")
+engine_app.add_typer(datalake_app, name="datalake")
 engine_app.add_typer(file_app, name="file")
 engine_app.add_typer(secret_app, name="secret")
 engine_app.add_typer(setpoint_app, name="setpoint")
-engine_app.add_typer(datalake_app, name="datalake")
 
 
 @engine_app.callback(invoke_without_command=True)
 def engine_callback(ctx: typer.Context):
     check_credentials(ctx)
```

### Comparing `splight-cli-2.3.9/cli/engine/alert/__init__.py` & `splight-cli-3.0.0/cli/engine/setpoint/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,78 @@
 import json
 from typing import List, Optional
 
 import typer
-from rich.console import Console
-from splight_models import Alert
-
 from cli.constants import error_style
 from cli.engine.manager import ResourceManager, ResourceManagerException
+from rich.console import Console
+from splight_lib.models import SetPoint
 
-alert_app = typer.Typer(
-    name="Splight Engine Alert",
+setpoint_app = typer.Typer(
+    name="Splight Engine SetPoint",
     add_completion=True,
     rich_markup_mode="rich",
     no_args_is_help=True,
 )
 
 console = Console()
-MODEL = Alert
+MODEL = SetPoint
 
 
-@alert_app.command()
+@setpoint_app.command()
 def list(
     ctx: typer.Context,
     filters: Optional[List[str]] = typer.Option(
         None,
         "--filter",
         "-f",
         help="Query param in the form key=value",
-    )
+    ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     params = manager.get_query_params(filters)
     manager.list(params)
 
 
-@alert_app.command()
+@setpoint_app.command()
 def get(
     ctx: typer.Context,
-    instance_id: str = typer.Argument(..., help="The Alert's ID"),
+    instance_id: str = typer.Argument(..., help="The setpoit's ID"),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     try:
         manager.get(instance_id)
     except ResourceManagerException as exc:
         console.print(exc, style=error_style)
 
 
-@alert_app.command()
+@setpoint_app.command()
 def create(
     ctx: typer.Context,
     path: str = typer.Argument(
         ..., help="Path to JSON file with resource data"
     ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     with open(path, "r") as fid:
         body = json.load(fid)
     manager.create(data=body)
 
 
-@alert_app.command()
-def delete(
+@setpoint_app.command()
+def download(
     ctx: typer.Context,
     instance_id: str = typer.Argument(
-        ..., help="The ID of the instance to be removed"
+        ..., help="The ID of the instance to download"
     ),
+    path: str = typer.Option(".", help="Path to download file"),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
-    manager.delete(instance_id)
+    manager.download(instance_id, path=path)
```

### Comparing `splight-cli-2.3.9/cli/engine/asset/__init__.py` & `splight-cli-3.0.0/cli/engine/secret/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,87 @@
-import json
 from typing import List, Optional
 
 import typer
-from rich.console import Console
-from splight_models import Asset
-
 from cli.constants import error_style
 from cli.engine.manager import ResourceManager, ResourceManagerException
+from rich.console import Console
+from splight_lib.models import Secret
 
-asset_app = typer.Typer(
-    name="Splight Engine Asset",
+secret_app = typer.Typer(
+    name="Splight Engine Secret",
     add_completion=True,
     rich_markup_mode="rich",
     no_args_is_help=True,
 )
 
 console = Console()
-MODEL = Asset
+MODEL = Secret
 
 
-@asset_app.command()
+@secret_app.command()
 def list(
     ctx: typer.Context,
     filters: Optional[List[str]] = typer.Option(
         None,
         "--filter",
         "-f",
         help="Query param in the form key=value",
-    )
+    ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     params = manager.get_query_params(filters)
     manager.list(params)
 
 
-@asset_app.command()
+@secret_app.command()
 def get(
     ctx: typer.Context,
-    instance_id: str = typer.Argument(..., help="The Asset's ID"),
+    instance_id: str = typer.Argument(..., help="The Secret's ID"),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     try:
-        manager.get(instance_id)
+        manager.get(instance_id, exclude_fields=["value"])
     except ResourceManagerException as exc:
         console.print(exc, style=error_style)
 
 
-@asset_app.command()
+@secret_app.command()
 def create(
     ctx: typer.Context,
-    path: str = typer.Argument(
-        ..., help="Path to JSON file with resource data"
-    ),
+    name: str = typer.Argument(..., help="Name of the secret"),
+    value: str = typer.Argument(..., help="Value of the secret"),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
-    with open(path, "r") as fid:
-        body = json.load(fid)
-    manager.create(data=body)
+    manager.create({"name": name, "value": value})
 
 
-@asset_app.command()
+@secret_app.command()
 def delete(
     ctx: typer.Context,
     instance_id: str = typer.Argument(
         ..., help="The ID of the instance to be removed"
     ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     manager.delete(instance_id)
+
+
+@secret_app.command()
+def download(
+    ctx: typer.Context,
+    instance_id: str = typer.Argument(
+        ..., help="The ID of the instance to be removed"
+    ),
+    path: str = typer.Option(".", help="Path to download file"),
+):
+    manager = ResourceManager(
+        model=MODEL,
+    )
+    manager.download(instance_id, path=path)
```

### Comparing `splight-cli-2.3.9/cli/engine/attribute/__init__.py` & `splight-cli-3.0.0/cli/engine/asset/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,91 @@
 import json
 from typing import List, Optional
 
 import typer
-from rich.console import Console
-from splight_models import Attribute
-
 from cli.constants import error_style
 from cli.engine.manager import ResourceManager, ResourceManagerException
+from rich.console import Console
+from splight_lib.models import Asset
 
-attribute_app = typer.Typer(
-    name="Splight Engine Attribute",
+asset_app = typer.Typer(
+    name="Splight Engine Asset",
     add_completion=True,
     rich_markup_mode="rich",
     no_args_is_help=True,
 )
 
 console = Console()
-MODEL = Attribute
+MODEL = Asset
 
 
-@attribute_app.command()
+@asset_app.command()
 def list(
     ctx: typer.Context,
     filters: Optional[List[str]] = typer.Option(
         None,
         "--filter",
         "-f",
         help="Query param in the form key=value",
-    )
+    ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     params = manager.get_query_params(filters)
     manager.list(params)
 
 
-@attribute_app.command()
+@asset_app.command()
 def get(
     ctx: typer.Context,
     instance_id: str = typer.Argument(..., help="The Asset's ID"),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     try:
         manager.get(instance_id)
     except ResourceManagerException as exc:
         console.print(exc, style=error_style)
 
 
-@attribute_app.command()
+@asset_app.command()
 def create(
     ctx: typer.Context,
     path: str = typer.Argument(
         ..., help="Path to JSON file with resource data"
     ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     with open(path, "r") as fid:
         body = json.load(fid)
     manager.create(data=body)
 
 
-@attribute_app.command()
+@asset_app.command()
 def delete(
     ctx: typer.Context,
     instance_id: str = typer.Argument(
         ..., help="The ID of the instance to be removed"
     ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     manager.delete(instance_id)
+
+
+@asset_app.command()
+def download(
+    ctx: typer.Context,
+    instance_id: str = typer.Argument(
+        ..., help="The ID of the instance to download"
+    ),
+    path: str = typer.Option(".", help="Path to download file"),
+):
+    manager = ResourceManager(
+        model=MODEL,
+    )
+    manager.download(instance_id, path=path)
```

### Comparing `splight-cli-2.3.9/cli/engine/component/__init__.py` & `splight-cli-3.0.0/cli/engine/alert/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,91 @@
 import json
-from typing import Optional, List
+from typing import List, Optional
 
 import typer
-from rich.console import Console
-from splight_models import Component
-
 from cli.constants import error_style
 from cli.engine.manager import ResourceManager, ResourceManagerException
+from rich.console import Console
+from splight_lib.models import Alert
 
-component_app = typer.Typer(
-    name="Splight Engine Component",
+alert_app = typer.Typer(
+    name="Splight Engine Alert",
     add_completion=True,
     rich_markup_mode="rich",
     no_args_is_help=True,
 )
 
 console = Console()
-MODEL = Component
+MODEL = Alert
 
 
-@component_app.command()
+@alert_app.command()
 def list(
     ctx: typer.Context,
     filters: Optional[List[str]] = typer.Option(
         None,
         "--filter",
         "-f",
         help="Query param in the form key=value",
-    )
+    ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     params = manager.get_query_params(filters)
-    manager.list(params=params)
+    manager.list(params)
 
 
-@component_app.command()
+@alert_app.command()
 def get(
     ctx: typer.Context,
-    instance_id: str = typer.Argument(..., help="The Asset's ID"),
+    instance_id: str = typer.Argument(..., help="The Alert's ID"),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     try:
         manager.get(instance_id)
     except ResourceManagerException as exc:
         console.print(exc, style=error_style)
 
 
-@component_app.command()
+@alert_app.command()
 def create(
     ctx: typer.Context,
     path: str = typer.Argument(
         ..., help="Path to JSON file with resource data"
     ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     with open(path, "r") as fid:
         body = json.load(fid)
     manager.create(data=body)
 
 
-@component_app.command()
+@alert_app.command()
 def delete(
     ctx: typer.Context,
     instance_id: str = typer.Argument(
         ..., help="The ID of the instance to be removed"
     ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     manager.delete(instance_id)
+
+
+@alert_app.command()
+def download(
+    ctx: typer.Context,
+    instance_id: str = typer.Argument(
+        ..., help="The ID of the instance to download"
+    ),
+    path: str = typer.Option(".", help="Path to download file"),
+):
+    manager = ResourceManager(
+        model=MODEL,
+    )
+    manager.download(instance_id, path=path)
```

### Comparing `splight-cli-2.3.9/cli/engine/datalake/__init__.py` & `splight-cli-3.0.0/cli/engine/attribute/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,88 +1,91 @@
-from typing import List
+import json
+from typing import List, Optional
 
 import typer
-from rich.console import Console
 from cli.constants import error_style
-from cli.engine.manager import DatalakeManager, DatalakeManagerException
+from cli.engine.manager import ResourceManager, ResourceManagerException
+from rich.console import Console
+from splight_lib.models import Attribute
 
-datalake_app = typer.Typer(
-    name="Splight Engine Datalake",
+attribute_app = typer.Typer(
+    name="Splight Engine Attribute",
     add_completion=True,
     rich_markup_mode="rich",
     no_args_is_help=True,
 )
-console = Console()
 
-
-def _parse_filter_option(values):
-    result = {}
-    for value in values:
-        k, v = value.split('=')
-        result[k] = v
-    return result
+console = Console()
+MODEL = Attribute
 
 
-@datalake_app.command()
+@attribute_app.command()
 def list(
     ctx: typer.Context,
-    skip: int = typer.Option(
-        0, "--skip", "-s", help="Number of element to skip"
-    ),
-    limit: int = typer.Option(
-        -1, "--limit", "-l", help="Limit the number of listed elements"
+    filters: Optional[List[str]] = typer.Option(
+        None,
+        "--filter",
+        "-f",
+        help="Query param in the form key=value",
     ),
 ):
-    manager = DatalakeManager(
-        db_client=ctx.obj.framework.setup.DATABASE_CLIENT(),
-        dl_client=ctx.obj.framework.setup.DATALAKE_CLIENT(),
+    manager = ResourceManager(
+        model=MODEL,
     )
-    manager.list(skip, limit)
+    params = manager.get_query_params(filters)
+    manager.list(params)
 
 
-@datalake_app.command()
-def dump(
+@attribute_app.command()
+def get(
     ctx: typer.Context,
-    collection: str = typer.Argument(
-        ..., help="Collection name to dump"
-    ),
-    path: str = typer.Option(
-        './dump.csv', "--path", "-p", help="Path name to dump"
-    ),
-    filter: List[str] = typer.Option(
-        None, "--filter", "-f", help="Filter to apply"
-    ),
+    instance_id: str = typer.Argument(..., help="The Asset's ID"),
 ):
-    filters = _parse_filter_option(filter)
-    manager = DatalakeManager(
-        db_client=ctx.obj.framework.setup.DATABASE_CLIENT(),
-        dl_client=ctx.obj.framework.setup.DATALAKE_CLIENT(),
+    manager = ResourceManager(
+        model=MODEL,
     )
     try:
-        manager.dump(
-            collection=collection,
-            path=path,
-            filters=filters
-        )
-    except DatalakeManagerException as exc:
+        manager.get(instance_id)
+    except ResourceManagerException as exc:
         console.print(exc, style=error_style)
 
 
-@datalake_app.command()
-def load(
+@attribute_app.command()
+def create(
     ctx: typer.Context,
-    collection: str = typer.Argument(..., help="Collection name to load"),
-    path: str = typer.Option(
-        ..., "--path", "-p", help="Path to file to load"
+    path: str = typer.Argument(
+        ..., help="Path to JSON file with resource data"
     ),
 ):
-    manager = DatalakeManager(
-        db_client=ctx.obj.framework.setup.DATABASE_CLIENT(),
-        dl_client=ctx.obj.framework.setup.DATALAKE_CLIENT(),
+    manager = ResourceManager(
+        model=MODEL,
     )
-    try:
-        manager.load(
-            collection=collection,
-            path=path
-        )
-    except DatalakeManagerException as exc:
-        console.print(exc, style=error_style)
+    with open(path, "r") as fid:
+        body = json.load(fid)
+    manager.create(data=body)
+
+
+@attribute_app.command()
+def delete(
+    ctx: typer.Context,
+    instance_id: str = typer.Argument(
+        ..., help="The ID of the instance to be removed"
+    ),
+):
+    manager = ResourceManager(
+        model=MODEL,
+    )
+    manager.delete(instance_id)
+
+
+@attribute_app.command()
+def download(
+    ctx: typer.Context,
+    instance_id: str = typer.Argument(
+        ..., help="The ID of the instance to be removed"
+    ),
+    path: str = typer.Option(".", help="Path to download file"),
+):
+    manager = ResourceManager(
+        model=MODEL,
+    )
+    manager.download(instance_id, path=path)
```

### Comparing `splight-cli-2.3.9/cli/engine/file/__init__.py` & `splight-cli-3.0.0/cli/engine/file/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import List, Optional
 
 import typer
-from rich.console import Console
-from splight_models import File
-
 from cli.constants import error_style
 from cli.engine.manager import ResourceManager, ResourceManagerException
+from rich.console import Console
+from splight_lib.models import File
 
 file_app = typer.Typer(
     name="Splight Engine File",
     add_completion=True,
     rich_markup_mode="rich",
     no_args_is_help=True,
 )
@@ -22,18 +21,17 @@
 def list(
     ctx: typer.Context,
     filters: Optional[List[str]] = typer.Option(
         None,
         "--filter",
         "-f",
         help="Query param in the form key=value",
-    )
+    ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     params = manager.get_query_params(filters)
     manager.list(params)
 
 
 @file_app.command()
@@ -41,38 +39,34 @@
     ctx: typer.Context,
     instance_id: str = typer.Argument(..., help="The File's ID"),
     path: str = typer.Option(
         None, "--path", "-p", help="Path to save the file"
     ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     try:
         manager.download(instance_id, path)
     except ResourceManagerException as exc:
         console.print(exc, style=error_style)
 
 
 @file_app.command()
 def create(
     ctx: typer.Context,
-    path: str = typer.Argument(
-        ..., help="Path to file to upload"
-    ),
+    path: str = typer.Argument(..., help="Path to file to upload"),
     description: str = typer.Option(
         None, "--description", "-d", help="Description of the file"
     ),
     encrypt: bool = typer.Option(
         False, "--encrypt", "-e", help="Encrypt the file"
     ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     file = MODEL(
         description=description,
         encrypted=encrypt,
         file=path,
     )
@@ -83,11 +77,24 @@
 def delete(
     ctx: typer.Context,
     instance_id: str = typer.Argument(
         ..., help="The ID of the instance to be removed"
     ),
 ):
     manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
         model=MODEL,
     )
     manager.delete(instance_id)
+
+
+@file_app.command()
+def download(
+    ctx: typer.Context,
+    instance_id: str = typer.Argument(
+        ..., help="The ID of the instance to download"
+    ),
+    path: str = typer.Option(".", help="Path to download file"),
+):
+    manager = ResourceManager(
+        model=MODEL,
+    )
+    manager.download(instance_id, path=path)
```

### Comparing `splight-cli-2.3.9/cli/engine/graph/__init__.py` & `splight-cli-3.0.0/cli/engine/datalake/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,79 @@
-import json
-from typing import List, Optional
+from typing import List
 
 import typer
-from rich.console import Console
-from splight_models import Graph
-
 from cli.constants import error_style
-from cli.engine.manager import ResourceManager, ResourceManagerException
+from cli.engine.manager import DatalakeManager, DatalakeManagerException
+from rich.console import Console
+from splight_lib.models import Boolean, Number, String
 
-graph_app = typer.Typer(
-    name="Splight Engine Graph",
+datalake_app = typer.Typer(
+    name="Splight Engine Datalake",
     add_completion=True,
     rich_markup_mode="rich",
     no_args_is_help=True,
 )
-
 console = Console()
-MODEL = Graph
 
-
-@graph_app.command()
-def list(
-    ctx: typer.Context,
-    filters: Optional[List[str]] = typer.Option(
-        None,
-        "--filter",
-        "-f",
-        help="Query param in the form key=value",
-    )
-):
-    manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
-        model=MODEL,
-    )
-    params = manager.get_query_params(filters)
-    manager.list(params)
+MODEL_MAP = {
+    "Number": Number,
+    "String": String,
+    "Boolean": Boolean,
+}
+
+
+def _parse_filter_option(values):
+    result = {}
+    for value in values:
+        k, v = value.split("=")
+        result[k] = v
+    return result
 
 
-@graph_app.command()
-def get(
+@datalake_app.command()
+def dump(
     ctx: typer.Context,
-    instance_id: str = typer.Argument(..., help="The Graph's ID"),
+    type: str = typer.Argument(
+        ..., help="Data type to dump eg. Number, String, Boolean"
+    ),
+    asset: str = typer.Argument(..., help="Asset id to dump"),
+    attribute: str = typer.Argument(..., help="Attribute id to dump"),
+    path: str = typer.Option(
+        "./dump.csv", "--path", "-p", help="Path name to dump"
+    ),
+    filter: List[str] = typer.Option(
+        None, "--filter", "-f", help="Filter to apply"
+    ),
 ):
-    manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
-        model=MODEL,
+    if type not in MODEL_MAP:
+        raise typer.BadParameter(f"Type {type} not supported")
+
+    filters = _parse_filter_option(filter)
+    filters.update({"asset": asset, "attribute": attribute})
+    manager = DatalakeManager(
+        model=MODEL_MAP[type],
     )
     try:
-        manager.get(instance_id)
-    except ResourceManagerException as exc:
+        manager.dump(path=path, filters=filters)
+    except DatalakeManagerException as exc:
         console.print(exc, style=error_style)
 
 
-@graph_app.command()
-def create(
+@datalake_app.command()
+def load(
     ctx: typer.Context,
-    path: str = typer.Argument(
-        ..., help="Path to JSON file with resource data"
+    type: str = typer.Argument(
+        ..., help="Data type to dump eg. Number, String, Boolean"
     ),
+    path: str = typer.Option(..., "--path", "-p", help="Path to file to load"),
 ):
-    manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
-        model=MODEL,
-    )
-    with open(path, "r") as fid:
-        body = json.load(fid)
-    manager.create(data=body)
+    if type not in MODEL_MAP:
+        raise typer.BadParameter(f"Type {type} not supported")
 
-
-@graph_app.command()
-def delete(
-    ctx: typer.Context,
-    instance_id: str = typer.Argument(
-        ..., help="The ID of the instance to be removed"
-    ),
-):
-    manager = ResourceManager(
-        client=ctx.obj.framework.setup.DATABASE_CLIENT(),
-        model=MODEL,
+    manager = DatalakeManager(
+        model=MODEL_MAP[type],
     )
-    manager.delete(instance_id)
+
+    try:
+        manager.load(path=path)
+    except DatalakeManagerException as exc:
+        console.print(exc, style=error_style)
```

### Comparing `splight-cli-2.3.9/cli/hub/component/__init__.py` & `splight-cli-3.0.0/cli/hub/component/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import typer
-from rich.console import Console
-from splight_models import Component
-
 from cli.constants import error_style
 from cli.hub.component.hub_manager import HubComponentManager
+from rich.console import Console
+from splight_lib.models import Component
 
 component_app = typer.Typer(
     name="Splight Engine Component",
     add_completion=True,
     rich_markup_mode="rich",
     no_args_is_help=True,
 )
@@ -24,58 +23,50 @@
         False,
         "--force",
         "-f",
         help="Overwrite existing component in Splight HUB",
     ),
 ):
     try:
-        manager = HubComponentManager(
-            client=ctx.obj.framework.setup.HUB_CLIENT()
-        )
+        manager = HubComponentManager()
         manager.push(path, force=force)
     except Exception as exc:
         console.print(f"Error pushing component {exc}", style=error_style)
         raise typer.Exit(1)
 
 
 @component_app.command()
 def pull(
     ctx: typer.Context,
     name: str = typer.Argument(..., help="The component's name"),
     version: str = typer.Argument(..., help="The component's version"),
 ):
     try:
-        manager = HubComponentManager(
-            client=ctx.obj.framework.setup.HUB_CLIENT()
-        )
+        manager = HubComponentManager()
         manager.pull(name=name, version=version)
     except Exception as exc:
         console.print(f"Error pulling component {exc}", style=error_style)
         raise typer.Exit(1)
 
 
 @component_app.command()
 def list(ctx: typer.Context):
     try:
-        manager = HubComponentManager(
-            client=ctx.obj.framework.setup.HUB_CLIENT()
-        )
+        manager = HubComponentManager()
         manager.list_components()
     except Exception as exc:
         console.print(f"Error listing components {exc}", style=error_style)
         raise typer.Exit(1)
 
 
 @component_app.command()
 def versions(
     ctx: typer.Context, name: str = typer.Argument(..., help="Componet's name")
 ):
     try:
-        manager = HubComponentManager(
-            client=ctx.obj.framework.setup.HUB_CLIENT()
-        )
+        manager = HubComponentManager()
         manager.versions(name=name)
     except Exception as exc:
         console.print(
             f"Error showing component's version {exc}", style=error_style
         )
         raise typer.Exit(1)
```

### Comparing `splight-cli-2.3.9/cli/hub/component/exceptions.py` & `splight-cli-3.0.0/cli/hub/component/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,7 +24,17 @@
 
 class ComponentDirectoryAlreadyExists(Exception):
     def __init__(self, directory: str):
         self._msg = f"Directory with name {directory} already exists in path"
 
     def __str__(self) -> str:
         return self._msg
+
+
+class HubComponentNotFound(Exception):
+    """Exception raised when a version is invalid."""
+
+    def __init__(self, name: str, version: str):
+        self._msg = f"Hub component {name} version {version} not found."
+
+    def __str__(self) -> str:
+        return self._msg
```

### Comparing `splight-cli-2.3.9/cli/utils/loader.py` & `splight-cli-3.0.0/cli/utils/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,65 @@
 from itertools import cycle
 from shutil import get_terminal_size
 from threading import Thread
 from time import sleep
+from typing import Optional
+
 from colorama import Fore, Style
 
 
 class Loader:
-    def __init__(self, desc="Loading...", end="", timeout=0.1):
+    def __init__(
+        self,
+        desc: str = "Loading...",
+        end: Optional[str] = None,
+        timeout: float = 0.1,
+        msg: Optional[str] = None,
+    ):
         """
         A loader-like context manager
 
         Args:
             desc (str, optional): The loader's description. Defaults to "Loading...".
-            end (str, optional): Final print. Defaults to "Done!".
+            end (str, optional): Final print. Defaults to None.
             timeout (float, optional): Sleep time between prints. Defaults to 0.1.
+            msg (str, optional): Custom message to print when stopping. Defaults to None.
         """
         self.desc = desc
-        self.end = end
+        self.end = end if end is not None else "Done!"
         self.timeout = timeout
+        self.msg = msg
 
         self._thread = Thread(target=self._animate, daemon=True)
         self.steps = ["⢿", "⣻", "⣽", "⣾", "⣷", "⣯", "⣟", "⡿"]
         self.done = False
 
     def start(self):
         self._thread.start()
         return self
 
     def _animate(self):
         for c in cycle(self.steps):
             if self.done:
                 break
-            print(f"\r{c} {Fore.BLUE}{self.desc}{Style.RESET_ALL} ", flush=True, end="")
+            print(
+                f"\r{c} {Fore.BLUE}{self.desc}{Style.RESET_ALL} ",
+                flush=True,
+                end="",
+            )
             sleep(self.timeout)
 
     def __enter__(self):
         self.start()
 
     def stop(self):
         self.done = True
         cols = get_terminal_size((80, 20)).columns
         print("\r" + " " * cols, end="", flush=True)
-        print(f"\r{self.end}", flush=True)
+        if self.msg is not None:
+            print(f"\r{self.msg}", flush=True)
 
-    def __exit__(self, exc_type, exc_value, tb):
-        # handle exceptions with those variables ^
-        self.stop()
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if exc_type is not None:
+            self.stop()
+            raise exc_type(exc_val)
+        self.stop()
```

### Comparing `splight-cli-2.3.9/cli/utils/pprint.py` & `splight-cli-3.0.0/cli/utils/pprint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# import click
 import typer
 
 
 class Printer:
     DEFAULT_COLOR = "white"
 
     @staticmethod
```

### Comparing `splight-cli-2.3.9/cli/utils/yaml.py` & `splight-cli-3.0.0/cli/utils/yaml.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import os
+
 import yaml
 
 
 def get_yaml_from_file(file_path: str):
     if not os.path.isfile(file_path):
-        raise Exception(f"String provided: \"{file_path}\" is not a file, please provide a filepath or use -fs flag")
-    with open(file_path, 'r') as f:
+        raise Exception(
+            f'String provided: "{file_path}" is not a file, please provide a'
+            " filepath or use -fs flag"
+        )
+    with open(file_path, "r") as f:
         try:
             data = yaml.load(f, Loader=yaml.FullLoader)
             return data if data is not None else {}
         except yaml.YAMLError as e:
             raise Exception("File is not a valid YAML") from e
 
 
 def save_yaml_to_file(payload: str, file_path: str):
-    with open(file_path, 'w+') as f:
-        yaml.Dumper.ignore_aliases = lambda *args : True  # TOO RISKY to add refs on repetitions
+    with open(file_path, "w+") as f:
+        yaml.Dumper.ignore_aliases = (
+            lambda *args: True
+        )  # TOO RISKY to add refs on repetitions
         yaml.dump(payload, f)
```

### Comparing `splight-cli-2.3.9/cli/workspace/__init__.py` & `splight-cli-3.0.0/cli/workspace/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import typer
+from cli.constants import error_style, success_style
 from rich.console import Console
 from rich.table import Table
 
-from cli.constants import error_style, success_style
-
 workspace_app = typer.Typer(
     name="Splight CLI Workspace",
     add_completion=True,
     rich_markup_mode="rich",
 )
 console = Console()
 
@@ -47,14 +46,32 @@
         console.print(
             f"Error configuring Splight Hub: {str(e)}", style=error_style
         )
         typer.Exit(1)
 
 
 @workspace_app.command()
+def show(
+    ctx: typer.Context,
+    name: str = typer.Argument(..., help="The workspace name"),
+) -> None:
+    try:
+        results = ctx.obj.workspace.list_workspace_contents(name)
+        table = Table("WORKSPACE CONTENTS", show_lines=True, show_edge=True)
+        for item in results:
+            table.add_row(item[0].lower(), item[1])
+        console.print(table)
+    except Exception as e:
+        console.print(
+            f"Error showing workspace contents: {str(e)}", style=error_style
+        )
+        typer.Exit(1)
+
+
+@workspace_app.command()
 def delete(
     ctx: typer.Context,
     name: str = typer.Argument(..., help="The workspace's name"),
 ) -> None:
     try:
         ctx.obj.workspace.delete_workspace(name)
         console.print(f"Deleted workspace {name}", style=success_style)
```

### Comparing `splight-cli-2.3.9/splight_cli.egg-info/SOURCES.txt` & `splight-cli-3.0.0/splight_cli.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,65 +5,49 @@
 cli/constants.py
 cli/settings.py
 cli/version.py
 cli/component/__init__.py
 cli/component/component.py
 cli/component/exceptions.py
 cli/component/loaders.py
-cli/component/spec.py
+cli/component/templates/.splightignore
 cli/component/templates/Initialization
 cli/component/templates/README.md
 cli/component/templates/auto_readme.md
-cli/component/templates/component.py
+cli/component/templates/main.py
 cli/component/templates/spec.json
+cli/component/templates/tests.py
 cli/component/tests/__init__.py
-cli/component/tests/test_create.py
-cli/component/tests/test_initialize.py
-cli/component/tests/test_run.py
+cli/component/tests/test_component_manager.py
 cli/config/__init__.py
 cli/context/__init__.py
-cli/context/framework.py
+cli/context/context.py
 cli/context/workspace.py
-cli/deployment/__init__.py
-cli/deployment/deployment.py
 cli/engine/__init__.py
 cli/engine/alert/__init__.py
 cli/engine/asset/__init__.py
 cli/engine/attribute/__init__.py
 cli/engine/component/__init__.py
 cli/engine/datalake/__init__.py
-cli/engine/datalake/tests/__init__.py
-cli/engine/datalake/tests/test_dump.py
-cli/engine/datalake/tests/test_list.py
-cli/engine/datalake/tests/test_load.py
 cli/engine/file/__init__.py
-cli/engine/graph/__init__.py
 cli/engine/manager/__init__.py
+cli/engine/manager/exceptions.py
 cli/engine/manager/manager.py
-cli/engine/query/__init__.py
 cli/engine/secret/__init__.py
 cli/engine/setpoint/__init__.py
 cli/hub/__init__.py
 cli/hub/component/__init__.py
 cli/hub/component/exceptions.py
 cli/hub/component/hub_manager.py
-cli/tests/__init__.py
-cli/tests/test_configure.py
-cli/tests/test_generic.py
-cli/tests/TestHub/__init__.py
 cli/utils/__init__.py
-cli/utils/api_requests.py
-cli/utils/headers.py
 cli/utils/input.py
 cli/utils/json.py
 cli/utils/loader.py
 cli/utils/pprint.py
 cli/utils/template.py
-cli/utils/uuid.py
-cli/utils/validation.py
 cli/utils/yaml.py
 cli/workspace/__init__.py
 splight_cli.egg-info/PKG-INFO
 splight_cli.egg-info/SOURCES.txt
 splight_cli.egg-info/dependency_links.txt
 splight_cli.egg-info/entry_points.txt
 splight_cli.egg-info/requires.txt
```

