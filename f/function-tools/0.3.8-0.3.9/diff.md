# Comparing `tmp/function-tools-0.3.8.tar.gz` & `tmp/function-tools-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function-tools-0.3.8.tar", last modified: Tue Nov 15 07:53:22 2022, max compression
+gzip compressed data, was "function-tools-0.3.9.tar", last modified: Fri Jun 16 09:11:04 2023, max compression
```

## Comparing `function-tools-0.3.8.tar` & `function-tools-0.3.9.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 07:53:22.173423 function-tools-0.3.8/
--rw-r--r--   0 root         (0) root         (0)     9716 2022-11-15 07:53:15.000000 function-tools-0.3.8/CHANGES.md
--rw-r--r--   0 root         (0) root         (0)     1069 2022-02-16 11:53:12.000000 function-tools-0.3.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      275 2022-07-12 08:20:24.000000 function-tools-0.3.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    18164 2022-11-15 07:53:22.174423 function-tools-0.3.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7804 2022-02-16 11:53:12.000000 function-tools-0.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 07:53:22.143423 function-tools-0.3.8/function_tools/
--rw-r--r--   0 root         (0) root         (0)       63 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2022-08-01 11:26:19.000000 function-tools-0.3.8/function_tools/apps.py
--rw-r--r--   0 root         (0) root         (0)    19868 2022-07-13 10:58:16.000000 function-tools-0.3.8/function_tools/caches.py
--rw-r--r--   0 root         (0) root         (0)      114 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/consts.py
--rw-r--r--   0 root         (0) root         (0)      458 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/decorators.py
--rw-r--r--   0 root         (0) root         (0)      245 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/enums.py
--rw-r--r--   0 root         (0) root         (0)      451 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 07:53:22.144423 function-tools-0.3.8/function_tools/function_templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-05 13:57:48.000000 function-tools-0.3.8/function_tools/function_templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 07:53:22.163423 function-tools-0.3.8/function_tools/function_templates/function_sync_template/
--rw-r--r--   0 root         (0) root         (0)      271 2022-07-05 13:57:48.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/README.md
--rw-r--r--   0 root         (0) root         (0)       92 2022-07-05 13:57:48.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/__init__.py-tpl
--rw-r--r--   0 root         (0) root         (0)      329 2022-07-13 10:58:16.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/apps.py-tpl
--rw-r--r--   0 root         (0) root         (0)      651 2022-07-27 13:25:54.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/caches.py-tpl
--rw-r--r--   0 root         (0) root         (0)       66 2022-07-05 13:57:48.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/consts.py-tpl
--rw-r--r--   0 root         (0) root         (0)       93 2022-07-05 13:57:48.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/enums.py-tpl
--rw-r--r--   0 root         (0) root         (0)      257 2022-07-12 08:20:24.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/errors.py-tpl
--rw-r--r--   0 root         (0) root         (0)     2831 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/functions.py-tpl
--rw-r--r--   0 root         (0) root         (0)     1310 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/helpers.py-tpl
--rw-r--r--   0 root         (0) root         (0)     1601 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/managers.py-tpl
--rw-r--r--   0 root         (0) root         (0)      326 2022-07-12 08:20:24.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/presenters.py-tpl
--rw-r--r--   0 root         (0) root         (0)      609 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/results.py-tpl
--rw-r--r--   0 root         (0) root         (0)     2841 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/runners.py-tpl
--rw-r--r--   0 root         (0) root         (0)      181 2022-07-05 13:57:48.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/strings.py-tpl
--rw-r--r--   0 root         (0) root         (0)       59 2022-07-05 13:57:48.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/tests.py-tpl
--rw-r--r--   0 root         (0) root         (0)      911 2022-07-13 12:17:45.000000 function-tools-0.3.8/function_tools/function_templates/function_sync_template/validators.py-tpl
--rw-r--r--   0 root         (0) root         (0)    10489 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/functions.py
--rw-r--r--   0 root         (0) root         (0)     5362 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/general.py
--rw-r--r--   0 root         (0) root         (0)     2244 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 07:53:22.165423 function-tools-0.3.8/function_tools/management/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 07:53:22.167423 function-tools-0.3.8/function_tools/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7507 2022-07-27 13:25:54.000000 function-tools-0.3.8/function_tools/management/commands/register_entities.py
--rw-r--r--   0 root         (0) root         (0)    18386 2022-08-17 08:42:13.000000 function-tools-0.3.8/function_tools/management/commands/startfunction.py
--rw-r--r--   0 root         (0) root         (0)       52 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/management/consts.py
--rw-r--r--   0 root         (0) root         (0)      598 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/management/strategies.py
--rw-r--r--   0 root         (0) root         (0)     4957 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 07:53:22.173423 function-tools-0.3.8/function_tools/migrations/
--rw-r--r--   0 root         (0) root         (0)     1124 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      520 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/migrations/0002_registeredfunction_tags.py
--rw-r--r--   0 root         (0) root         (0)      795 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/migrations/0003_implementationstrategy.py
--rw-r--r--   0 root         (0) root         (0)      477 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/migrations/0004_implementationstrategy_order_number.py
--rw-r--r--   0 root         (0) root         (0)     2736 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/migrations/0005_auto_20220724_0050.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-12 12:03:22.000000 function-tools-0.3.8/function_tools/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6434 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/mixins.py
--rw-r--r--   0 root         (0) root         (0)     4534 2022-11-01 12:27:02.000000 function-tools-0.3.8/function_tools/models.py
--rw-r--r--   0 root         (0) root         (0)      685 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/presenters.py
--rw-r--r--   0 root         (0) root         (0)      369 2022-07-27 13:25:54.000000 function-tools-0.3.8/function_tools/receivers.py
--rw-r--r--   0 root         (0) root         (0)     2386 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/results.py
--rw-r--r--   0 root         (0) root         (0)    12097 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/runners.py
--rw-r--r--   0 root         (0) root         (0)    12291 2022-11-15 07:53:15.000000 function-tools-0.3.8/function_tools/storages.py
--rw-r--r--   0 root         (0) root         (0)    17851 2022-07-25 11:47:49.000000 function-tools-0.3.8/function_tools/strategies.py
--rw-r--r--   0 root         (0) root         (0)      693 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/strings.py
--rw-r--r--   0 root         (0) root         (0)      603 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/types.py
--rw-r--r--   0 root         (0) root         (0)     3234 2022-03-03 06:03:15.000000 function-tools-0.3.8/function_tools/utils.py
--rw-r--r--   0 root         (0) root         (0)      408 2022-02-16 11:53:12.000000 function-tools-0.3.8/function_tools/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 07:53:22.144423 function-tools-0.3.8/function_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18164 2022-11-15 07:53:22.000000 function-tools-0.3.8/function_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2648 2022-11-15 07:53:22.000000 function-tools-0.3.8/function_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 07:53:22.000000 function-tools-0.3.8/function_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2022-11-15 07:53:22.000000 function-tools-0.3.8/function_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-11-15 07:53:22.000000 function-tools-0.3.8/function_tools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       47 2022-07-05 13:57:48.000000 function-tools-0.3.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2022-11-15 07:53:22.174423 function-tools-0.3.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1707 2022-11-15 07:53:15.000000 function-tools-0.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.141263 function-tools-0.3.9/
+-rw-r--r--   0 root         (0) root         (0)    10327 2023-06-16 09:10:54.000000 function-tools-0.3.9/CHANGES.md
+-rw-r--r--   0 root         (0) root         (0)     1069 2022-02-16 11:53:12.000000 function-tools-0.3.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      275 2022-07-12 08:20:24.000000 function-tools-0.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    18775 2023-06-16 09:11:04.141263 function-tools-0.3.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7804 2022-02-16 11:53:12.000000 function-tools-0.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.109263 function-tools-0.3.9/function_tools/
+-rw-r--r--   0 root         (0) root         (0)       63 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2022-08-01 11:26:19.000000 function-tools-0.3.9/function_tools/apps.py
+-rw-r--r--   0 root         (0) root         (0)    19868 2022-07-13 10:58:16.000000 function-tools-0.3.9/function_tools/caches.py
+-rw-r--r--   0 root         (0) root         (0)      114 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/consts.py
+-rw-r--r--   0 root         (0) root         (0)      458 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      245 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/enums.py
+-rw-r--r--   0 root         (0) root         (0)      451 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.112263 function-tools-0.3.9/function_tools/function_templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.130263 function-tools-0.3.9/function_tools/function_templates/function_sync_template/
+-rw-r--r--   0 root         (0) root         (0)      271 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/README.md
+-rw-r--r--   0 root         (0) root         (0)       92 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/__init__.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      329 2022-07-13 10:58:16.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/apps.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      651 2022-07-27 13:25:54.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/caches.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       66 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/consts.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       93 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/enums.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      257 2022-07-12 08:20:24.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/errors.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     2831 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/functions.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     1310 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/helpers.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     1601 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/managers.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      326 2022-07-12 08:20:24.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/presenters.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      609 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/results.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     2841 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/runners.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      181 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/strings.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       59 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/tests.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      911 2022-07-13 12:17:45.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/validators.py-tpl
+-rw-r--r--   0 root         (0) root         (0)    10489 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/functions.py
+-rw-r--r--   0 root         (0) root         (0)     5362 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/general.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.132263 function-tools-0.3.9/function_tools/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.134263 function-tools-0.3.9/function_tools/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2022-07-27 13:25:54.000000 function-tools-0.3.9/function_tools/management/commands/register_entities.py
+-rw-r--r--   0 root         (0) root         (0)    17844 2023-06-16 09:10:54.000000 function-tools-0.3.9/function_tools/management/commands/startfunction.py
+-rw-r--r--   0 root         (0) root         (0)       52 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/management/consts.py
+-rw-r--r--   0 root         (0) root         (0)      598 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/management/strategies.py
+-rw-r--r--   0 root         (0) root         (0)     4957 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.140263 function-tools-0.3.9/function_tools/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1124 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      520 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/migrations/0002_registeredfunction_tags.py
+-rw-r--r--   0 root         (0) root         (0)      795 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/migrations/0003_implementationstrategy.py
+-rw-r--r--   0 root         (0) root         (0)      477 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/migrations/0004_implementationstrategy_order_number.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/migrations/0005_auto_20220724_0050.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-12 12:03:22.000000 function-tools-0.3.9/function_tools/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/mixins.py
+-rw-r--r--   0 root         (0) root         (0)     4534 2022-11-01 12:27:02.000000 function-tools-0.3.9/function_tools/models.py
+-rw-r--r--   0 root         (0) root         (0)      685 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/presenters.py
+-rw-r--r--   0 root         (0) root         (0)      369 2022-07-27 13:25:54.000000 function-tools-0.3.9/function_tools/receivers.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/results.py
+-rw-r--r--   0 root         (0) root         (0)    12097 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/runners.py
+-rw-r--r--   0 root         (0) root         (0)    11548 2023-06-16 09:10:54.000000 function-tools-0.3.9/function_tools/storages.py
+-rw-r--r--   0 root         (0) root         (0)    17851 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/strategies.py
+-rw-r--r--   0 root         (0) root         (0)      693 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/strings.py
+-rw-r--r--   0 root         (0) root         (0)      603 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/types.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2022-03-03 06:03:15.000000 function-tools-0.3.9/function_tools/utils.py
+-rw-r--r--   0 root         (0) root         (0)      408 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.112263 function-tools-0.3.9/function_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18775 2023-06-16 09:11:04.000000 function-tools-0.3.9/function_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-06-16 09:11:04.000000 function-tools-0.3.9/function_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 09:11:04.000000 function-tools-0.3.9/function_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-16 09:11:04.000000 function-tools-0.3.9/function_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-16 09:11:04.000000 function-tools-0.3.9/function_tools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2022-07-05 13:57:48.000000 function-tools-0.3.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-16 09:11:04.142263 function-tools-0.3.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-06-16 09:10:54.000000 function-tools-0.3.9/setup.py
```

### Comparing `function-tools-0.3.8/CHANGES.md` & `function-tools-0.3.9/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # История изменений
 
+**0.3.9**
+
+- EDUSCHL-19156 Убрана часть кода вызывающая ошибку поиска сущностей, при наличии подключенного приложения, находящегося выше по иерархии, чем, например, функция;
+- EDUSCHL-19156 Добавление описания команды создания Функции;
+- EDUSCHL-19156 Перевод команды создания Функций на использование стратегий из Хранилища;
+- EDUSCHL-19156 Исправление опечаток.
+
 **0.3.8**
 
 - EDUSCHL-18335 Поиск модулей будет осуществляться только в зарегистрированных приложениях без рекурсивного поиска.
 
 **0.3.7**
 
 - EDUSCHL-14355 Добавление on_delete в модель Entity.
```

### Comparing `function-tools-0.3.8/LICENSE` & `function-tools-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/PKG-INFO` & `function-tools-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-tools
-Version: 0.3.8
+Version: 0.3.9
 Summary: Tools for creating functions
 Home-page: https://github.com/sandanilenko/function-tools
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -97,14 +97,21 @@
 Подробная актуальная диаграммка классов представлена на Рисунке 2.
 
 ![Рисунок 2](/docs/source/_static/images/class_diagram.png)
 
 С подробной документацией можно ознакомиться на [function-tools.readthedocs.io](https://function-tools.readthedocs.io/ru/latest/)
 # История изменений
 
+**0.3.9**
+
+- EDUSCHL-19156 Убрана часть кода вызывающая ошибку поиска сущностей, при наличии подключенного приложения, находящегося выше по иерархии, чем, например, функция;
+- EDUSCHL-19156 Добавление описания команды создания Функции;
+- EDUSCHL-19156 Перевод команды создания Функций на использование стратегий из Хранилища;
+- EDUSCHL-19156 Исправление опечаток.
+
 **0.3.8**
 
 - EDUSCHL-18335 Поиск модулей будет осуществляться только в зарегистрированных приложениях без рекурсивного поиска.
 
 **0.3.7**
 
 - EDUSCHL-14355 Добавление on_delete в модель Entity.
```

### Comparing `function-tools-0.3.8/README.md` & `function-tools-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/caches.py` & `function-tools-0.3.9/function_tools/caches.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/function_templates/function_sync_template/caches.py-tpl` & `function-tools-0.3.9/function_tools/function_templates/function_sync_template/caches.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/function_templates/function_sync_template/functions.py-tpl` & `function-tools-0.3.9/function_tools/function_templates/function_sync_template/functions.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/function_templates/function_sync_template/helpers.py-tpl` & `function-tools-0.3.9/function_tools/function_templates/function_sync_template/helpers.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/function_templates/function_sync_template/managers.py-tpl` & `function-tools-0.3.9/function_tools/function_templates/function_sync_template/managers.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/function_templates/function_sync_template/results.py-tpl` & `function-tools-0.3.9/function_tools/function_templates/function_sync_template/results.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/function_templates/function_sync_template/runners.py-tpl` & `function-tools-0.3.9/function_tools/function_templates/function_sync_template/runners.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/function_templates/function_sync_template/validators.py-tpl` & `function-tools-0.3.9/function_tools/function_templates/function_sync_template/validators.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/functions.py` & `function-tools-0.3.9/function_tools/functions.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/general.py` & `function-tools-0.3.9/function_tools/general.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/helpers.py` & `function-tools-0.3.9/function_tools/helpers.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/management/commands/register_entities.py` & `function-tools-0.3.9/function_tools/management/commands/register_entities.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/management/commands/startfunction.py` & `function-tools-0.3.9/function_tools/management/commands/startfunction.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
 import function_tools
 from function_tools.management.consts import (
     PARAMETERS_DIALOG_WINDOW,
 )
 from function_tools.models import (
     EntityType,
-    ImplementationStrategy,
 )
 from function_tools.storages import (
     EntityStorage,
 )
 
 
 class PatchedTemplateCommand(TemplateCommand):
@@ -80,14 +79,17 @@
         self.camel_case_value = None
         self.extra_files = None
         self.extensions = None
 
         self._top_dir_path = None
         self._python_path_value = None
 
+        self._entity_storage = EntityStorage()
+        self._entity_storage.prepare()
+
     def _get_conf_dir_parent_path(self):
         """
         Возвращает абсолютный путь директории, содержащей директорию conf с шаблонами внутри.
         """
         return django.__path__[0]
 
     def _sort_imports(
@@ -338,15 +340,15 @@
     """
     Команда для создания Функции приложения
     """
 
     help = (
         """
         Команда для создания Функции приложения. В неименованном параметре передается наименование функции в стиле 
-        camel_case. Переданное имя будет служить в качестве наименования пакета. Также будет произведено 
+        snake_case. Переданное имя будет служить в качестве наименования пакета. Также будет произведено 
         преобразование переданного наименования к виду CamelCase, которое будет использоваться в наименовании классов.
         
         Существует несколько стратегий реализации Функции. Указать необходимую можно при помощи параметра --strategy.
         """
     )
 
     missing_args_message = "Вы должны указать наименование функции."
@@ -354,16 +356,16 @@
     def add_arguments(self, parser):
         """
         Добавление параметров команды
         """
         super().add_arguments(parser)
 
         strategy_help = '\n'.join([
-            f'{strategy.key} - {strategy.title};'
-            for strategy in ImplementationStrategy.get_enum_data().values()
+            f'{strategy["class"].key.upper()} - {strategy["class"].title};'
+            for strategy in self._entity_storage.entities[EntityType.STRATEGY.key].values() if strategy['class'].key
         ])
 
         parser.add_argument(
             '--strategy',
             dest='strategy',
             action='store',
             type=lambda s: str(s).upper(),
@@ -379,15 +381,15 @@
         )
 
         parser.add_argument(
             '--verbose_name',
             dest='function_verbose_name',
             action='store',
             type=str,
-            help='Полное (человекочитаемое) название функции',
+            help='Название функции на русском языке',
             default='Безымянная функция',
         )
 
         parser.add_argument(
             '--is_parameterized',
             dest='is_parameterized',
             action='store',
@@ -460,40 +462,21 @@
 
     def _prepare_strategy_class(self, strategy_key: str):
         """
         Получение стратегии по ключу
         """
         result = None
 
-        entity_storage = EntityStorage()
-        entity_storage.prepare()
-
-        for strategy in entity_storage.entities[EntityType.STRATEGY.key].values():
+        for strategy in self._entity_storage.entities[EntityType.STRATEGY.key].values():
             if strategy['class'].key == strategy_key:
                 result = strategy['class']
                 break
 
         return result
 
-    def _extend_implementation_strategy(self):
-        """
-        Расширение перечисления стратегий реализаций функций.
-        """
-        entity_storage = EntityStorage()
-        entity_storage.prepare()
-
-        strategies = entity_storage.entities[EntityType.STRATEGY.key]
-
-        for strategy in strategies.values():
-            if strategy['class'].key:
-                ImplementationStrategy.extend(
-                    key=strategy['class'].key.upper(),
-                    title=strategy['class'].title,
-                )
-
     def handle(self, **options):
         function_name = options.pop('name')
         target = options.pop('directory')
 
         strategy_key = options.pop('strategy')
 
         strategy_class = self._prepare_strategy_class(strategy_key=strategy_key)
```

### Comparing `function-tools-0.3.8/function_tools/management/strategies.py` & `function-tools-0.3.9/function_tools/management/strategies.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/managers.py` & `function-tools-0.3.9/function_tools/managers.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/migrations/0001_initial.py` & `function-tools-0.3.9/function_tools/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/migrations/0002_registeredfunction_tags.py` & `function-tools-0.3.9/function_tools/migrations/0002_registeredfunction_tags.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/migrations/0003_implementationstrategy.py` & `function-tools-0.3.9/function_tools/migrations/0003_implementationstrategy.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/migrations/0005_auto_20220724_0050.py` & `function-tools-0.3.9/function_tools/migrations/0005_auto_20220724_0050.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/mixins.py` & `function-tools-0.3.9/function_tools/mixins.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/models.py` & `function-tools-0.3.9/function_tools/models.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/presenters.py` & `function-tools-0.3.9/function_tools/presenters.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/results.py` & `function-tools-0.3.9/function_tools/results.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/runners.py` & `function-tools-0.3.9/function_tools/runners.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/storages.py` & `function-tools-0.3.9/function_tools/storages.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,30 +134,15 @@
         try:
             app_module = import_module(application_name)
         except ModuleNotFoundError:
             return
 
         application_path = Path(app_module.__path__[0])
 
-        # Если поиск уже осуществлялся по родительской директории,
-        # то проверку нужно пропустить
-        is_already_checked = False
-
-        for checked_application_path in self._checked_application_paths:
-            try:
-                is_already_checked = application_path.is_relative_to(Path(checked_application_path))
-            # В CI падает с ошибкой 'PosixPath' object has no attribute 'is_relative_to', хотя локально не
-            # воспроизводится
-            except AttributeError:
-                continue
-
-            if is_already_checked:
-                break
-
-        return application_path if not is_already_checked else None
+        return application_path
 
     def _find_application_entities_modules(self, application_name: Union[str, 'AppConfig']):
         """
         Поиск модулей зарегистрированных типов сущностей в приложении.
 
         Args:
             application_name: имя приложения
```

### Comparing `function-tools-0.3.8/function_tools/strategies.py` & `function-tools-0.3.9/function_tools/strategies.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/strings.py` & `function-tools-0.3.9/function_tools/strings.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/types.py` & `function-tools-0.3.9/function_tools/types.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools/utils.py` & `function-tools-0.3.9/function_tools/utils.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/function_tools.egg-info/PKG-INFO` & `function-tools-0.3.9/function_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-tools
-Version: 0.3.8
+Version: 0.3.9
 Summary: Tools for creating functions
 Home-page: https://github.com/sandanilenko/function-tools
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -97,14 +97,21 @@
 Подробная актуальная диаграммка классов представлена на Рисунке 2.
 
 ![Рисунок 2](/docs/source/_static/images/class_diagram.png)
 
 С подробной документацией можно ознакомиться на [function-tools.readthedocs.io](https://function-tools.readthedocs.io/ru/latest/)
 # История изменений
 
+**0.3.9**
+
+- EDUSCHL-19156 Убрана часть кода вызывающая ошибку поиска сущностей, при наличии подключенного приложения, находящегося выше по иерархии, чем, например, функция;
+- EDUSCHL-19156 Добавление описания команды создания Функции;
+- EDUSCHL-19156 Перевод команды создания Функций на использование стратегий из Хранилища;
+- EDUSCHL-19156 Исправление опечаток.
+
 **0.3.8**
 
 - EDUSCHL-18335 Поиск модулей будет осуществляться только в зарегистрированных приложениях без рекурсивного поиска.
 
 **0.3.7**
 
 - EDUSCHL-14355 Добавление on_delete в модель Entity.
```

### Comparing `function-tools-0.3.8/function_tools.egg-info/SOURCES.txt` & `function-tools-0.3.9/function_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.8/setup.py` & `function-tools-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import (
     find_packages,
     setup,
 )
 
 
-__version__ = '0.3.8'
+__version__ = '0.3.9'
 
 
 here = path.abspath(path.dirname(__file__))
 
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
```

