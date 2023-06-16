# Comparing `tmp/th2_data_services-2.0.0.dev5280132551.tar.gz` & `tmp/th2_data_services-2.0.0.dev5290873151.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev5280132551.tar", last modified: Thu Jun 15 14:38:05 2023, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev5290873151.tar", last modified: Fri Jun 16 14:08:51 2023, max compression
```

## Comparing `th2_data_services-2.0.0.dev5280132551.tar` & `th2_data_services-2.0.0.dev5290873151.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    28243 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23148 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-15 14:37:53.000000 th2_data_services-2.0.0.dev5280132551/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    36192 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    15883 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (122)     3296 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     6805 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10508 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/sse_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     6538 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-06-15 14:34:10.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    28243 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-15 14:38:05.000000 th2_data_services-2.0.0.dev5280132551/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    28243 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23148 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-16 14:08:41.000000 th2_data_services-2.0.0.dev5290873151/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35647 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15883 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3296 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6805 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10508 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/sse_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6538 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-06-16 14:07:58.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    28243 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-16 14:08:51.000000 th2_data_services-2.0.0.dev5290873151/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev5280132551/PKG-INFO` & `th2_data_services-2.0.0.dev5290873151/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3532 3830 3133 3235 3531 0a53 756d 6d61  5280132551.Summa
+00000040: 3532 3930 3837 3331 3531 0a53 756d 6d61  5290873151.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev5280132551/README.md` & `th2_data_services-2.0.0.dev5290873151/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/setup.py` & `th2_data_services-2.0.0.dev5290873151/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/data.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -764,54 +764,36 @@
 
         data_obj = cls([], cache=True)
         data_obj._set_custom_cache_destination(filename=filename)
         data_obj.update_metadata({"source_file": filename})
         return data_obj
 
     @classmethod
-    def from_json(cls, filename, buffer_limit=250) -> "Data[dict]":
+    def from_json(cls, filename, buffer_limit=250, gzip=False) -> "Data[dict]":
         """Creates Data object from json file with provided name.
 
         Args:
             filename: Name or path to cache file.
             buffer_limit: If limit is 0 buffer will not be used. Number of messages in buffer before parsing.
+            gzip: Set to true if file is json file compressed using gzip.
 
         Returns:
             Data: Data object.
 
         Raises:
             FileNotFoundError if provided file does not exist.
 
         """
         if not Path(filename).resolve().exists():
             raise FileNotFoundError(f"{filename} doesn't exist")
 
-        data = cls(iter_json_file(filename, buffer_limit))
-        data.update_metadata({"source_file": filename})
-        return data
-    
-    @classmethod
-    def from_json_gzip(cls, filename, buffer_limit=250) -> "Data[dict]":
-        """Creates Data object from json file with provided name.
-
-        Args:
-            filename: Name or path to cache file.
-            buffer_limit: If limit is 0 buffer will not be used. Number of messages in buffer before parsing.
-
-        Returns:
-            Data: Data object.
-
-        Raises:
-            FileNotFoundError if provided file does not exist.
-
-        """
-        if not Path(filename).resolve().exists():
-            raise FileNotFoundError(f"{filename} doesn't exist")
-
-        data = cls(iter_json_gzip_file(filename, buffer_limit))
+        if gzip:
+            data = cls(iter_json_gzip_file(filename, buffer_limit))
+        else:
+            data = cls(iter_json_file(filename, buffer_limit))
         data.update_metadata({"source_file": filename})
         return data
 
     @classmethod
     def from_any_file(cls, filename, mode="r") -> "Data[str]":
         """Creates Data object from any file with provided name.
```

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev5290873151/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev5290873151/th2_data_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3532 3830 3133 3235 3531 0a53 756d 6d61  5280132551.Summa
+00000040: 3532 3930 3837 3331 3531 0a53 756d 6d61  5290873151.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev5290873151/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5280132551/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev5290873151/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

