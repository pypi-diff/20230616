# Comparing `tmp/django-file-explorer-1.4.0.tar.gz` & `tmp/django-file-explorer-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-file-explorer-1.4.0.tar", last modified: Wed Mar  1 13:00:22 2023, max compression
+gzip compressed data, was "django-file-explorer-1.5.0.tar", last modified: Fri Jun 16 06:18:47 2023, max compression
```

## Comparing `django-file-explorer-1.4.0.tar` & `django-file-explorer-1.5.0.tar`

### file list

```diff
@@ -1,1282 +1,76 @@
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.418985 django-file-explorer-1.4.0/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     5427 2023-03-01 13:00:22.418985 django-file-explorer-1.4.0/PKG-INFO
--rwxrwxr-x   0 sigma     (1000) sigma     (1000)     4471 2023-02-25 08:03:32.000000 django-file-explorer-1.4.0/README.md
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.262985 django-file-explorer-1.4.0/django_file_explorer.egg-info/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     5427 2023-03-01 13:00:22.000000 django-file-explorer-1.4.0/django_file_explorer.egg-info/PKG-INFO
--rw-rw-r--   0 sigma     (1000) sigma     (1000)    84756 2023-03-01 13:00:22.000000 django-file-explorer-1.4.0/django_file_explorer.egg-info/SOURCES.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        1 2023-03-01 13:00:22.000000 django-file-explorer-1.4.0/django_file_explorer.egg-info/dependency_links.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       47 2023-03-01 13:00:22.000000 django-file-explorer-1.4.0/django_file_explorer.egg-info/requires.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       19 2023-03-01 13:00:22.000000 django-file-explorer-1.4.0/django_file_explorer.egg-info/top_level.txt
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.262985 django-file-explorer-1.4.0/explorer/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       21 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1273 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/admin.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      148 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/apps.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.262985 django-file-explorer-1.4.0/explorer/migrations/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      870 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/migrations/0001_initial.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      764 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/migrations/0002_option.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1164 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/migrations/0003_userrole.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      534 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/migrations/0004_auto_20221117_1449.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      373 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/migrations/0005_rename_opertations_userrole_actions.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      818 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/migrations/0006_auto_20230215_1122.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/migrations/__init__.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.262985 django-file-explorer-1.4.0/explorer/models/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       68 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/models/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      872 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/models/action.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1074 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/models/user_role.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      944 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/models/volume.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.258985 django-file-explorer-1.4.0/explorer/static/
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.262985 django-file-explorer-1.4.0/explorer/static/explorer/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      128 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/action.css
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3367 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/action.js
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2383 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/checkbox.js
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      104 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/common.js
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      119 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/icons.css
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       32 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/navigation.css
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1342 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/onload.js
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      360 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/summary.css
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       85 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/volume.css
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1663 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/volume.js
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.262985 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.414985 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/
--rw-r--r--   0 sigma     (1000) sigma     (1000)      168 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/default_file.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      194 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/default_folder.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      314 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/default_folder_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      365 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/default_root_folder.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      485 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/default_root_folder_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1862 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_access.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1549 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_access2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1841 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_actionscript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1805 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_actionscript2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5839 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ada.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      831 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_advpl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1187 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_affectscript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1379 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_affinitydesigner.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1448 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_affinityphoto.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1408 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_affinitypublisher.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      822 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ai.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1491 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ai2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      383 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_al.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      633 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_al_dal.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4913 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_allcontributors.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      487 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_angular.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1368 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ansible.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1407 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_antlr.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1790 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_anyscript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     7102 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_apache.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3644 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_apex.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2303 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_api_extractor.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1037 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_apib.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1035 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_apib2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      240 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_apl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      598 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_applescript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      775 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_appscript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      450 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_appsemble.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      583 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_appveyor.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2178 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_arduino.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      588 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_asciidoc.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1533 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_asp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1381 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_aspx.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1975 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_assembly.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1341 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_astro.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2161 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_astroconfig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2836 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ats.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      537 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_audio.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3946 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_aurelia.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1877 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_autohotkey.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      536 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_autoit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      597 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_avif.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4550 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_avro.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2318 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_awk.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1321 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_aws.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1802 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_azure.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2585 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_azurepipelines.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    17881 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_babel.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2999 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_babel2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      318 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ballerina.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4131 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bat.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1713 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bats.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3537 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bazaar.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      448 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bazel.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      768 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bazel_ignore.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      804 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bazel_version.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2621 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_befunge.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      497 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bicep.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1717 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_biml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1071 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_binary.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      823 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bitbucketpipeline.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1682 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bithound.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1764 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_blade.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      340 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_blitzbasic.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      265 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bolt.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1529 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bosque.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2952 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bower.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2479 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bower2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2641 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_browserslist.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      559 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_buckbuild.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1682 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bun.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    45937 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bundler.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1708 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_bunfig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      707 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_c.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      201 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_c2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1064 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_c3.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2146 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_c_al.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      790 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cabal.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3351 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_caddy.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6813 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cake.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      808 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cakephp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1394 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_capacitor.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    21743 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cargo.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3057 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_casc.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2292 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cddl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    14276 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cert.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2471 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ceylon.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1014 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cf.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2042 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cf2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1718 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cfc.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2809 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cfc2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1910 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cfm.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3189 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cfm2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      436 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cheader.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1870 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_chef.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3683 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_chef_cookbook.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      441 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_circleci.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1531 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_class.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1471 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_clojure.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1922 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_clojurescript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3411 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cloudfoundry.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2134 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cmake.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1812 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cobol.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1012 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_codacy.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      411 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_codeclimate.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1295 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_codecov.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      649 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_codekit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      614 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_codeowners.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1232 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_codeql.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1801 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_coffeelint.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1772 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_coffeescript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      515 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_commitizen.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      900 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_commitlint.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1923 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_compass.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    97096 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_composer.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1103 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_conan.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4065 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_conda.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      937 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_config.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1303 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_confluence.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      797 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_coveralls.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      921 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cpp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      365 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cpp2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1500 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cpp3.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      876 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cppheader.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1591 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_crowdin.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      512 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_crystal.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      735 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_csharp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1319 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_csharp2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      368 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cspell.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1803 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_csproj.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1137 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_css.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3007 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_csscomb.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2658 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_csslint.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2058 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cssmap.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2063 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cucumber.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      945 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cuda.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1277 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cvs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2082 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cypress.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2660 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cypress_spec.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2519 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_cython.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      807 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dal.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1595 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_darcs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      789 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dartlang.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      617 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dartlang_generated.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      617 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dartlang_ignore.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3994 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_datadog.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1089 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_db.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3552 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_delphi.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2640 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_deno.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1145 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dependabot.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      920 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dependencies.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      427 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_devcontainer.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      574 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dhall.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      279 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_diff.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      664 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_django.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3413 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dlang.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5198 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_docker.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2560 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_docker2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4886 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dockertest.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2525 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dockertest2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1033 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_docpad.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4313 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_docz.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6911 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dojo.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      820 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_doppler.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3636 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dotjs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1683 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_doxygen.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      821 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_drawio.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      535 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_drone.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1658 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_drools.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     7180 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dustjs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1365 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dvc.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    10099 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_dylan.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2267 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_earthly.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1116 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_eas-metadata.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      544 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_edge.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      636 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_edge2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5896 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_editorconfig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1556 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_eex.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      924 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ejs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      753 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_elastic.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      971 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_elasticbeanstalk.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3126 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_eleventy.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      475 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_eleventy2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1587 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_elixir.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      508 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_elm.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      714 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_elm2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1856 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_emacs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    43488 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ember.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      568 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ensime.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3804 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_eps.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      227 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_erb.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      478 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_erlang.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      578 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_erlang2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      250 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_esbuild.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      555 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_eslint.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      462 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_eslint2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1287 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_esphome.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1962 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_excel.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1047 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_excel2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1264 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_expo.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      854 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_falcon.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      825 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_fantasticon.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      271 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_fauna.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      667 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_favicon.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      929 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_fbx.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1102 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_firebase.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3325 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_firebasehosting.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1608 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_firestore.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      844 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_fitbit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1777 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_fla.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      975 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_flareact.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      876 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_flash.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      857 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_floobits.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2690 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_flow.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      704 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_flutter.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1780 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_flutter_package.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1550 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_font.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      676 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_formkit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      873 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_fortran.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    13451 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_fossa.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    17560 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_fossil.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      551 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_freemarker.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      332 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_fsharp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      520 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_fsharp2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1356 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_fsproj.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      294 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_fthtml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      756 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_funding.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1331 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_fusebox.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      821 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_galen.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2391 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_galen2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      464 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gamemaker.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      369 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gamemaker2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    18613 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gamemaker81.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      679 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gatsby.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      698 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gcloud.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1703 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gcode.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2152 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gdscript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      401 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_genstat.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      677 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_git.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      660 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_git2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      863 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gitlab.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      919 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gitpod.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    53438 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_glide.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2037 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_glitter.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1703 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_glsl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      588 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_glyphs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    18483 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gnu.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1067 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gnuplot.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2092 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_go.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2097 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_go_aqua.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1993 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_go_black.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2100 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_go_fuchsia.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     9139 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_go_gopher.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2102 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_go_lightblue.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3145 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_go_package.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2083 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_go_white.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2099 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_go_work.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2099 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_go_yellow.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3209 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_goctl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2152 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_godot.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1484 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gradle.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      426 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gradle2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1656 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_graphql.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1920 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_graphql_config.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    15028 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_graphviz.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      838 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_greenkeeper.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1910 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gridsome.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6796 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_groovy.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     7049 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_groovy2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    12136 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_grunt.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5946 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_gulp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     8343 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_haml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1184 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_handlebars.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2267 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_handlebars2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2520 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_harbour.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1783 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_hardhat.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      401 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_hashicorp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      566 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_haskell.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      667 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_haskell2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      833 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_haxe.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2705 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_haxecheckstyle.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    61917 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_haxedevelop.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1079 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_helix.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2412 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_helm.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1323 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_hjson.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1660 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_hlsl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1016 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_homeassistant.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2951 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_horusec.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    15811 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_host.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1017 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_html.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      992 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_htmlhint.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    10464 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_http.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3161 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_hunspell.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1648 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_husky.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1102 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_hy.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1473 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_hygen.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      334 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_hypr.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2340 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_icl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      450 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_idris.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4257 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_idrisbin.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1719 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_idrispkg.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      506 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_image.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      340 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_imba.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      322 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_inc.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1479 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_infopath.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2552 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_informix.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      934 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ini.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2992 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ink.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2575 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_innosetup.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      714 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_io.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3384 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_iodine.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      408 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ionic.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3686 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jake.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1422 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_janet.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1529 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jar.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1514 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jasmine.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1524 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_java.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1137 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jbuilder.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2336 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jekyll.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    17428 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jenkins.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2132 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jest.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2166 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jest_snapshot.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2898 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jinja.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    15795 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jpm.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      685 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      719 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_js_official.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     8371 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jsbeautify.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1508 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jsconfig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      720 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jscpd.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      806 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jshint.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1591 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jsmap.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1616 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_json.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2526 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_json2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3601 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_json5.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1112 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_json_official.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2131 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jsonld.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      981 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jsonnet.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      607 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jsp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2249 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jss.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      779 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_julia.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3149 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_julia2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      688 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_jupyter.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      238 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_k.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      511 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_karma.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    18247 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_key.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      825 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_kitchenci.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      326 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_kite.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1546 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_kivy.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      934 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_kos.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      495 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_kotlin.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1361 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_kusto.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1866 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_latino.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      842 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_layout.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)   219771 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_lerna.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4056 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_less.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1796 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_lex.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    24274 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_license.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1136 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_licensebat.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4135 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_actionscript2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5845 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_ada.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      240 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_apl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    17887 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_babel.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3005 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_babel2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      799 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_cabal.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      447 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_circleci.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3420 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_cloudfoundry.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      850 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_codacy.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      357 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_codeclimate.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      614 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_codeowners.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      943 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_config.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      518 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_crystal.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2094 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_cypress.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2658 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_cypress_spec.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1095 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_db.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2640 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_deno.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      563 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_dhall.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1039 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_docpad.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      541 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_drone.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1156 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_eas-metadata.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3132 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_eleventy.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      475 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_eleventy2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1285 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_esphome.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1223 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_expo.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3309 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_firebasehosting.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1738 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_fla.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1514 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_font.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      354 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_gamemaker2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1052 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_gradle.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      355 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_hashicorp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1308 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_hjson.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      940 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_ini.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      678 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_io.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      691 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1514 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_jsconfig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1597 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_jsmap.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1622 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_json.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3589 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_json5.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2094 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_jsonld.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      332 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_kite.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)   219773 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_lerna.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      892 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_mailing.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      359 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_mdx.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      526 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_mlang.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2476 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_mustache.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1257 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_next.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      855 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_nim.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1258 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_nx.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1711 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_objidconfig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      467 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_openHAB.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1358 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_pcl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      573 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_pnpm.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     9037 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_prettier.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      468 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_prisma.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      599 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_purescript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1621 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_quasar.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      943 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_razzle.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      531 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_rehype.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      731 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_remark.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1373 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_replit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      559 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_retext.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1398 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_rome.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      937 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_rubocop.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3713 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_rust.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4936 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_rust_toolchain.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      430 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_shaderlab.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      742 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_solidity.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1103 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_stylelint.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3095 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_stylus.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1427 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_symfony.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      388 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_systemd.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3038 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_systemverilog.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      430 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_testcafe.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1796 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_testjs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1125 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_tex.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      633 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_todo.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      688 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_toit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      296 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_toml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      478 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_tree.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2317 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_turbo.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4047 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_unibeautify.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1127 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_vash.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      330 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_vsix.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1147 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_vsixmanifest.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1830 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_xfl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1261 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_yaml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      477 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_light_zeit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2784 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_lighthouse.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3175 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_lilypond.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3395 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_lime.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3094 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_lintstagedrc.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1451 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_liquid.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      831 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_lisp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      842 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_livescript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      903 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_lnk.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1324 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_locale.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1185 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_log.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4875 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_lolcode.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6796 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_lsl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4046 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_lua.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1308 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_luau.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1685 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_lync.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      946 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mailing.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1024 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_manifest.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1563 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_manifest_bak.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1105 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_manifest_skip.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      888 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_map.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2400 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mariadb.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      552 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_markdown.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1614 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_markdownlint.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1451 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_markdownlint_ignore.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4924 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_marko.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2625 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_markojs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1988 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_master-co.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1758 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_matlab.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    15037 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_maven.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2094 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_maxscript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3084 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_maya.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      374 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mdx.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     9246 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mediawiki.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3256 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mercurial.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      527 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_meson.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      933 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_meteor.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1138 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mjml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      541 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mlang.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1329 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mocha.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      261 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_modernizr.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1332 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mojolicious.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      430 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_moleculer.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      528 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mondoo.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1922 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mongo.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5152 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_monotone.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1131 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_motif.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1973 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mson.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1203 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mustache.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2454 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_mysql.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1302 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ndst.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1106 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nearly.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2393 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_adapter_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2512 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_adapter_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2396 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_controller_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2515 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_controller_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2397 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_decorator_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2516 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_decorator_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2394 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_filter_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2513 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_filter_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2393 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_gateway_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2512 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_gateway_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2391 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_guard_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2510 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_guard_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2399 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_interceptor_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2518 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_interceptor_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2398 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_middleware_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2517 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_middleware_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2394 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_module_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2513 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_module_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2390 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_pipe_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2509 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_pipe_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2395 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_service_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2514 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nest_service_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1539 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nestjs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3864 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_netlify.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1272 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_next.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1394 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_component_css.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1523 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_component_dart.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1271 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_component_html.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      905 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_component_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1133 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_component_js2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3700 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_component_less.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2678 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_component_sass.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1292 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_component_scss.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1036 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_component_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1433 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_component_ts2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1279 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_controller_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1406 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_controller_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1523 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_directive_dart.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      905 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_directive_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1133 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_directive_js2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1036 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_directive_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1433 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_directive_ts2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1519 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_guard_dart.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      903 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_guard_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1034 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_guard_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1522 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_interceptor_dart.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      908 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_interceptor_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1035 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_interceptor_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1520 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_module_dart.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      902 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_module_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1130 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_module_js2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1033 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_module_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1430 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_module_ts2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1518 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_pipe_dart.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      900 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_pipe_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1128 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_pipe_js2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1031 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_pipe_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1428 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_pipe_ts2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1521 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_routing_dart.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      902 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_routing_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1105 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_routing_js2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1032 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_routing_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1408 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_routing_ts2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1521 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_service_dart.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      903 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_service_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1131 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_service_js2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1034 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_service_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1431 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_service_ts2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1529 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_smart_component_dart.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1067 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_smart_component_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1139 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_smart_component_js2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1326 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_smart_component_ts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1439 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_smart_component_ts2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      786 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ng_tailwind.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      879 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nginx.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      849 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nim.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      995 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nimble.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2916 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ninja.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      988 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nix.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1714 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_njsproj.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      696 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_noc.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1357 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_node.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1412 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_node2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      945 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nodemon.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      383 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_npm.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2057 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nsi.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2336 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nsri-integrity.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1446 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nsri.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      581 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nuget.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1159 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_numpy.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1242 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nunjucks.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      933 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nuxt.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1252 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nx.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     7195 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_nyc.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      996 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_objectivec.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1236 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_objectivecpp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1154 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_objidconfig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5159 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ocaml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2362 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ogone.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1719 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_onenote.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      461 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_openHAB.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2981 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_opencl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2999 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_openscad.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     7252 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_org.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      936 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_outlook.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      914 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ovpn.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1177 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_package.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2305 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_paket.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    22082 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_patch.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1368 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pcl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2061 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pddl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      564 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pddl_happenings.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      326 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pddl_plan.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    42560 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pdf.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3600 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pdf2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1761 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_peeky.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6293 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_perl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2343 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_perl2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    15343 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_perl6.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5366 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pgsql.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1062 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_photoshop.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2519 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_photoshop2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2702 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_php.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    26484 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_php2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1033 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_php3.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2923 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_phpcsfixer.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2030 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_phpstan.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2848 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_phpunit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6302 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_phraseapp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1074 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pine.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1652 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pip.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1545 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pipeline.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     7375 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_plantuml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1298 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_platformio.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2364 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_playwright.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1076 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_plsql.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2014 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_plsql_package.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2006 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_plsql_package_body.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2008 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_plsql_package_header.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2006 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_plsql_package_spec.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3194 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pm2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      555 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pnpm.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    27920 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_poedit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2375 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_poetry.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2278 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_polymer.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2100 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pony.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    23206 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_postcss.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    24112 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_postcssconfig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2266 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_powerpoint.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1180 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_powerpoint2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1683 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_powershell.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3666 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_powershell2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1847 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_powershell_format.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1844 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_powershell_psd.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3686 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_powershell_psd2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1844 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_powershell_psm.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3686 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_powershell_psm2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1843 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_powershell_types.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      396 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_preact.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1061 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_precommit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     8879 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_prettier.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      462 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_prisma.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      767 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_processinglang.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      378 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_procfile.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      580 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_progress.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5808 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_prolog.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      883 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_prometheus.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1130 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_protobuf.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      684 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_protractor.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1379 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_publisher.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6988 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pug.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1430 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pulumi.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      316 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_puppet.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      734 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_purescript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5483 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pyret.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1318 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_python.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2584 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pythowo.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      714 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pytyped.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      636 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_pyup.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      632 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_q.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1657 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_qbs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      924 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_qlikview.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      892 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_qml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      895 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_qmldir.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      910 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_qsharp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1615 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_quasar.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1326 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_r.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      525 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_racket.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6630 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rails.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1721 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rake.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      491 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_raml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1122 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_razor.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      958 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_razzle.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2108 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_reactjs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2114 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_reacttemplate.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2108 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_reactts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      656 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_reason.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2000 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_red.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      666 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_registry.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1023 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rego.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      546 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rehype.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      746 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_remark.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2235 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_renovate.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1373 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_replit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1238 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rescript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1755 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rest.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      574 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_retext.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2980 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rexx.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      502 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_riot.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2975 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rmd.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1054 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_robotframework.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1277 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_robots.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3223 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rollup.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1392 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rome.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3036 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ron.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     7689 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rproj.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2930 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rspec.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1015 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rubocop.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     7553 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ruby.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4236 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rust.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5401 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_rust_toolchain.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      243 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sails.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      935 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_saltstack.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      283 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_san.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1134 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sapphire_framework_cli.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      917 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sas.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3167 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sass.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      548 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sbt.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1566 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_scala.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4195 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_scilab.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1687 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_script.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1295 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_scss.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1235 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_scss2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1645 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sdlang.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      855 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sentry.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2909 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sequelize.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      322 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_serverless.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      424 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_shaderlab.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      446 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_shell.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)   248663 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_shellcheck.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      731 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_shuttle.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      591 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_silverstripe.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2240 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_siyuan.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      868 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sketch.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1214 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_skipper.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2043 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_slang.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      941 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_slashup.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      656 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_slice.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    92505 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_slim.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1951 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sln.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      503 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sln2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    11752 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_smarty.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      327 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_snapcraft.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1311 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_snort.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5777 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_snyk.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1066 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_solidarity.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      636 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_solidity.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1025 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_source.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      283 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_spacengine.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1735 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sparql.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2931 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sqf.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1090 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sql.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1673 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sqlite.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2612 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_squirrel.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    79726 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_sss.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      783 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_stan.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      945 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_stata.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      302 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_stencil.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1004 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_storyboard.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1045 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_storybook.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1738 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_stryker.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2528 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_stylable.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1400 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_style.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6557 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_styled.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1124 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_stylelint.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      756 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_stylish_haskell.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3104 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_stylus.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1689 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_subversion.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1533 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_svelte.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1824 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_svg.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2219 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_swagger.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      873 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_swift.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3172 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_swig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1421 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_symfony.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      382 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_systemd.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     7458 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_systemverilog.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      446 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_t4tt.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      355 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tailwind.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      756 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tauri.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2182 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tcl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      213 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_teal.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1232 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tera.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      562 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_terraform.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1150 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_test.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      424 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_testcafe.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1790 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_testjs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2124 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_testts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1182 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tex.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      626 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_text.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      975 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_textile.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      962 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tfs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1701 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tiltfile.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      648 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_todo.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      688 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_toit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      311 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_toml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6044 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tox.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    17146 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_travis.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      472 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tree.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2152 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tres.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1460 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_truffle.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      620 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_trunk.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2152 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tscn.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1811 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tsconfig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1045 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tsconfig_official.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2611 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tslint.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2353 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tt.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1773 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_ttcn.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      586 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_tuc.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2338 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_turbo.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1133 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_twig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      357 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_typedoc.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1015 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_typescript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1359 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_typescript_official.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1031 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_typescriptdef.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1362 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_typescriptdef_official.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      509 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_typo3.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2711 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_unibeautify.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1933 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_unison.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      752 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_unlicense.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2576 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vagrant.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2012 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vala.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5235 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vanilla_extract.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1968 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vapi.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1090 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vapor.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1121 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vash.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      549 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vb.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2542 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vba.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1123 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vbhtml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1479 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vbproj.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2202 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vcxproj.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      849 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_velocity.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5354 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_verilog.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      560 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vhdl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4261 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_video.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      525 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_view.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    10634 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vim.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1464 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vite.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1188 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vitest.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      470 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vlang.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      227 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_volt.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      797 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vscode-insiders.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      866 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vscode.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      274 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vscode2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      330 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vscode3.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      324 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vsix.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1141 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vsixmanifest.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      360 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vue.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1237 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_vueconfig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      150 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_wallaby.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3781 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_wally.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      470 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_wasm.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2159 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_watchmanconfig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      781 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_webpack.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1361 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_wenyan.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      742 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_wercker.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2024 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_wgsl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2353 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_wikitext.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1951 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_windi.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1500 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_wolfram.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2039 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_word.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1048 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_word2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1284 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_wpml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1944 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_wurst.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1070 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_wxml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1070 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_wxss.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    11825 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_xcode.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1850 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_xfl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2953 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_xib.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1509 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_xliff.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      545 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_xmake.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      378 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_xml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      940 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_xquery.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      378 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_xsl.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2484 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_yacc.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1255 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_yaml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1679 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_yamllint.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      438 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_yandex.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1515 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_yang.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1011 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_yarn.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3151 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_yeoman.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      472 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_zeit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      583 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_zig.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4727 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_zip.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    15657 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/file_type_zip2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1297 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_android.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1427 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_android_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1398 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_api.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1551 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_api_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1456 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_app.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1609 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_app_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    30914 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_arangodb.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    31044 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_arangodb_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1303 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_asset.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1423 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_asset_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      648 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_audio.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      768 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_audio_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4054 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_aurelia.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4174 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_aurelia_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1422 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_aws.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1542 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_aws_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1857 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_azure.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1909 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_azure_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2621 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_azurepipelines.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2683 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_azurepipelines_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1571 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_binary.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1691 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_binary_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      626 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_bloc.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      661 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_bloc_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1384 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_blueprint.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1485 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_blueprint_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      629 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_bot.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      726 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_bot_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2977 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_bower.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3097 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_bower_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      374 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_buildkite.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      418 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_buildkite_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6874 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_cake.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6994 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_cake_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      426 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_certificate.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      520 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_certificate_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1923 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_chef.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2043 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_chef_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      514 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_circleci.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      634 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_circleci_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      399 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_cli.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      443 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_cli_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1765 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_client.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1885 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_client_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2014 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_cmake.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2126 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_cmake_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      780 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_common.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      708 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_common_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4790 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_component.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4910 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_component_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    90378 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_composer.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    90498 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_composer_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1007 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_config.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1127 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_config_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2509 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_controller.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2610 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_controller_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1604 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_coverage.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1724 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_coverage_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1304 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_css.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1424 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_css_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      815 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_cubit.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      844 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_cubit_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2653 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_cypress.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2769 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_cypress_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      587 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_dapr.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      631 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_dapr_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5977 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_datadog.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4198 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_datadog_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1185 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_db.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1305 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_db_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3774 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_debian.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3894 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_debian_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1215 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_dependabot.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1261 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_dependabot_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      530 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_devcontainer.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      574 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_devcontainer_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4132 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_dist.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4252 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_dist_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2780 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_docker.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2900 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_docker_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2724 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_docs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2853 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_docs_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1323 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_e2e.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1380 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_e2e_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1104 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_elasticbeanstalk.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1224 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_elasticbeanstalk_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1730 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_electron.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1776 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_electron_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1369 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_expo.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1445 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_expo_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1077 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_favicon.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1123 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_favicon_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2817 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_flow.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2934 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_flow_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1619 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_fonts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1739 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_fonts_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      895 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_gcp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      996 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_gcp_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      793 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_git.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      913 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_git_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      954 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_github.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      995 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_github_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      967 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_gitlab.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1083 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_gitlab_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1112 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_gradle.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1158 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_gradle_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      965 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_graphql.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1095 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_graphql_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    11963 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_grunt.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    12083 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_grunt_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6252 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_gulp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6353 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_gulp_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1110 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_haxelib.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1230 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_haxelib_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3685 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_helper.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3838 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_helper_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1264 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_hook.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1384 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_hook_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1705 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_husky.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1749 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_husky_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1879 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_idea.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1999 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_idea_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      574 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_images.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      694 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_images_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      700 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_include.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      820 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_include_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      552 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_interfaces.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      593 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_interfaces_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      731 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_ios.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      861 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_ios_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      791 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_js.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      911 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_js_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1685 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_json.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1130 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_json_official.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1172 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_json_official_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1729 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_json_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3572 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_kubernetes.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3692 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_kubernetes_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4028 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_less.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4148 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_less_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1498 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_library.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1618 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_library_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2634 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_cypress.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2750 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_cypress_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1736 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_electron.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1782 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_electron_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1358 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_expo.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1434 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_expo_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1583 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_fonts.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1703 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_fonts_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1118 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_gradle.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1164 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_gradle_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1020 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_meteor.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1140 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_meteor_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2460 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_mysql.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2513 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_mysql_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1530 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_node.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1650 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_node_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1404 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_redux.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1465 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_redux_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1353 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_sass.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1473 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_light_sass_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5381 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_linux.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5482 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_linux_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1390 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_locale.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1510 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_locale_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1446 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_log.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1566 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_log_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1409 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_macos.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1510 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_macos_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2507 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_mariadb.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2613 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_mariadb_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    14953 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_maven.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    15073 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_maven_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     9715 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_memcached.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     9761 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_memcached_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      993 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_meteor.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1113 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_meteor_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1389 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_middleware.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1431 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_middleware_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3397 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_minikube.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3498 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_minikube_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1282 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_mjml.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1402 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_mjml_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1160 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_mock.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1261 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_mock_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1517 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_model.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1637 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_model_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3908 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_module.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     5618 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_module_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2025 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_mongodb.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2082 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_mongodb_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2451 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_mysql.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2507 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_mysql_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1333 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_next.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1368 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_next_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      932 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_nginx.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1052 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_nginx_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3077 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_nix.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3211 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_nix_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1451 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_node.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1571 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_node_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1169 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_notification.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1211 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_notification_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1802 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_nuget.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1922 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_nuget_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1132 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_nuxt.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1120 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_nuxt_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1305 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_package.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1425 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_package_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1123 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_paket.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1242 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_paket_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2746 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_php.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2862 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_php_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1397 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_platformio.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1441 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_platformio_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      461 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_plugin.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      581 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_plugin_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      788 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_prisma.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      897 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_prisma_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      417 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_private.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      553 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_private_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      849 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_public.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1142 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_public_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1443 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_python.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1489 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_python_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3559 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_ravendb.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3679 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_ravendb_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2415 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_redis.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2535 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_redis_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1398 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_redux.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1459 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_redux_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1065 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_route.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1185 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_route_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1374 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_sass.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1494 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_sass_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1785 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_script.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1842 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_script_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6145 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_server.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     6265 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_server_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4286 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_services.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     4330 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_services_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      694 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_shared.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      787 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_shared_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1030 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_src.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1150 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_src_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3449 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_sso.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3493 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_sso_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1121 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_story.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1161 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_story_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1470 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_style.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1590 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_style_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      830 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_tauri.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      950 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_tauri_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      649 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_temp.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      736 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_temp_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      946 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_template.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1066 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_template_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1232 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_test.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1352 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_test_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3403 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_theme.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3437 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_theme_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1771 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_tools.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1891 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_tools_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    16541 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_travis.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)    16661 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_travis_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      810 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_trunk.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      944 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_trunk_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2902 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_typescript.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3022 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_typescript_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2899 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_typings.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1095 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_typings2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1215 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_typings2_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3019 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_typings_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2739 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vagrant.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     2859 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vagrant_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3741 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_video.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     3861 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_video_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      697 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_view.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      817 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_view_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1148 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vs.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      611 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vs2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      731 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vs2_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1192 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vs_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      967 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vscode.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      380 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vscode2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      500 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vscode2_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      615 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vscode3.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      735 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vscode3_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1011 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vscode_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      972 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vscode_test.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      385 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vscode_test2.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      505 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vscode_test2_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      620 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vscode_test3.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      740 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vscode_test3_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1016 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_vscode_test_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      887 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_webpack.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1009 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_webpack_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      366 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_windows.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      467 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_windows_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     9128 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_www.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     9248 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_www_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)      938 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_yarn.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)     1065 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/icons/folder_type_yarn_opened.svg
--rw-r--r--   0 sigma     (1000) sigma     (1000)   204739 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/static/explorer/vs-code-icons/vsicons-icon-theme.json
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.258985 django-file-explorer-1.4.0/explorer/templates/
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.414985 django-file-explorer-1.4.0/explorer/templates/explorer/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1051 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/templates/explorer/about.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2868 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/templates/explorer/base.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      374 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/templates/explorer/error.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     7985 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/templates/explorer/index.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2288 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/templates/explorer/login.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      450 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/templates/explorer/logout.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      331 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/templates/explorer/warning.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       60 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/tests.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      407 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/urls.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.414985 django-file-explorer-1.4.0/explorer/views/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      103 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      835 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/about.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.418985 django-file-explorer-1.4.0/explorer/views/extractor/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/extractor/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3703 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/extractor/location.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1683 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/extractor/request.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1163 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/extractor/user.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.418985 django-file-explorer-1.4.0/explorer/views/logger/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/logger/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3785 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/logger/logger.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1059 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/login.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      542 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/logout.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     4795 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/main.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.418985 django-file-explorer-1.4.0/explorer/views/operations/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/operations/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3595 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/operations/action.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     6689 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/operations/explorer.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2717 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/operations/location.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.418985 django-file-explorer-1.4.0/explorer/views/utils/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/utils/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      605 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/utils/path.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.418985 django-file-explorer-1.4.0/explorer/views/validator/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/validator/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     6065 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/validator/request.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:22.418985 django-file-explorer-1.4.0/explorer/views/vscode_icons/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/vscode_icons/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3176 2023-03-01 13:00:18.000000 django-file-explorer-1.4.0/explorer/views/vscode_icons/vscode.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       38 2023-03-01 13:00:22.418985 django-file-explorer-1.4.0/setup.cfg
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1574 2023-03-01 12:49:17.000000 django-file-explorer-1.4.0/setup.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.990775 django-file-explorer-1.5.0/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     5636 2023-06-16 06:18:47.990775 django-file-explorer-1.5.0/PKG-INFO
+-rwxrwxr-x   0 sigma     (1000) sigma     (1000)     4680 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/README.md
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.986775 django-file-explorer-1.5.0/django_file_explorer.egg-info/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     5636 2023-06-16 06:18:47.000000 django-file-explorer-1.5.0/django_file_explorer.egg-info/PKG-INFO
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1988 2023-06-16 06:18:47.000000 django-file-explorer-1.5.0/django_file_explorer.egg-info/SOURCES.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        1 2023-06-16 06:18:47.000000 django-file-explorer-1.5.0/django_file_explorer.egg-info/dependency_links.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       60 2023-06-16 06:18:47.000000 django-file-explorer-1.5.0/django_file_explorer.egg-info/requires.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       19 2023-06-16 06:18:47.000000 django-file-explorer-1.5.0/django_file_explorer.egg-info/top_level.txt
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.986775 django-file-explorer-1.5.0/explorer/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       21 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1273 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/admin.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      148 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/apps.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.986775 django-file-explorer-1.5.0/explorer/migrations/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      870 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/migrations/0001_initial.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      764 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/migrations/0002_option.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1164 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/migrations/0003_userrole.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      534 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/migrations/0004_auto_20221117_1449.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      373 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/migrations/0005_rename_opertations_userrole_actions.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      818 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/migrations/0006_auto_20230215_1122.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/migrations/__init__.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.986775 django-file-explorer-1.5.0/explorer/models/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       68 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/models/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      872 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/models/action.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1074 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/models/user_role.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      944 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/models/volume.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.982775 django-file-explorer-1.5.0/explorer/static/
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.986775 django-file-explorer-1.5.0/explorer/static/explorer/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      128 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/static/explorer/action.css
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3367 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/static/explorer/action.js
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     2383 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/static/explorer/checkbox.js
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      104 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/static/explorer/common.js
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      119 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/static/explorer/icons.css
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       32 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/static/explorer/navigation.css
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1342 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/static/explorer/onload.js
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      360 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/static/explorer/summary.css
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       85 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/static/explorer/volume.css
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1663 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/static/explorer/volume.js
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.982775 django-file-explorer-1.5.0/explorer/templates/
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.986775 django-file-explorer-1.5.0/explorer/templates/explorer/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1051 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/templates/explorer/about.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     2868 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/templates/explorer/base.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      374 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/templates/explorer/error.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     7985 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/templates/explorer/index.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     2288 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/templates/explorer/login.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      450 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/templates/explorer/logout.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      331 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/templates/explorer/warning.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       60 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/tests.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      407 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/urls.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.990775 django-file-explorer-1.5.0/explorer/views/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      103 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      835 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/about.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.990775 django-file-explorer-1.5.0/explorer/views/extractor/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/extractor/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3703 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/extractor/location.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1683 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/extractor/request.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1163 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/extractor/user.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.990775 django-file-explorer-1.5.0/explorer/views/logger/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/logger/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3785 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/logger/logger.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1059 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/login.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      542 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/logout.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     5657 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/main.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.990775 django-file-explorer-1.5.0/explorer/views/operations/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/operations/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3595 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/operations/action.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     6689 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/operations/explorer.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     2717 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/operations/location.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.990775 django-file-explorer-1.5.0/explorer/views/utils/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/utils/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      605 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/utils/path.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:47.990775 django-file-explorer-1.5.0/explorer/views/validator/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/validator/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     6065 2023-06-16 06:18:44.000000 django-file-explorer-1.5.0/explorer/views/validator/request.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       38 2023-06-16 06:18:47.990775 django-file-explorer-1.5.0/setup.cfg
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1598 2023-06-16 05:35:59.000000 django-file-explorer-1.5.0/setup.py
```

### Comparing `django-file-explorer-1.4.0/PKG-INFO` & `django-file-explorer-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-file-explorer
-Version: 1.4.0
+Version: 1.5.0
 Summary: Django app to explore directory.
 Author: Tahir Rafique
 Author-email: tahirrafiqueasad@gmail.com
 License: MIT
 Keywords: explorer,file explorer,directory explorer,django explorer,location explorer
 Classifier: Framework :: Django :: 3.2
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -150,7 +150,13 @@
 ## Run
 
 Go to explorer url **SERVER:PORT/explorer** and explore the volumes.
 
 ## Author
 
 **Tahir Rafique**
+
+## Releases
+
+| Date      | Version | Summary                                |
+| --------- | ------- | -------------------------------------- |
+| 16-Jun-23 | v1.5.0  | Separating vscode icons from this app. |
```

### Comparing `django-file-explorer-1.4.0/README.md` & `django-file-explorer-1.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -127,7 +127,13 @@
 ## Run
 
 Go to explorer url **SERVER:PORT/explorer** and explore the volumes.
 
 ## Author
 
 **Tahir Rafique**
+
+## Releases
+
+| Date      | Version | Summary                                |
+| --------- | ------- | -------------------------------------- |
+| 16-Jun-23 | v1.5.0  | Separating vscode icons from this app. |
```

### Comparing `django-file-explorer-1.4.0/django_file_explorer.egg-info/PKG-INFO` & `django-file-explorer-1.5.0/django_file_explorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-file-explorer
-Version: 1.4.0
+Version: 1.5.0
 Summary: Django app to explore directory.
 Author: Tahir Rafique
 Author-email: tahirrafiqueasad@gmail.com
 License: MIT
 Keywords: explorer,file explorer,directory explorer,django explorer,location explorer
 Classifier: Framework :: Django :: 3.2
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -150,7 +150,13 @@
 ## Run
 
 Go to explorer url **SERVER:PORT/explorer** and explore the volumes.
 
 ## Author
 
 **Tahir Rafique**
+
+## Releases
+
+| Date      | Version | Summary                                |
+| --------- | ------- | -------------------------------------- |
+| 16-Jun-23 | v1.5.0  | Separating vscode icons from this app. |
```

### Comparing `django-file-explorer-1.4.0/explorer/admin.py` & `django-file-explorer-1.5.0/explorer/admin.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/migrations/0001_initial.py` & `django-file-explorer-1.5.0/explorer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/migrations/0002_option.py` & `django-file-explorer-1.5.0/explorer/migrations/0002_option.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/migrations/0003_userrole.py` & `django-file-explorer-1.5.0/explorer/migrations/0003_userrole.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/migrations/0004_auto_20221117_1449.py` & `django-file-explorer-1.5.0/explorer/migrations/0004_auto_20221117_1449.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/migrations/0006_auto_20230215_1122.py` & `django-file-explorer-1.5.0/explorer/migrations/0006_auto_20230215_1122.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/models/action.py` & `django-file-explorer-1.5.0/explorer/models/action.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/models/user_role.py` & `django-file-explorer-1.5.0/explorer/models/user_role.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/models/volume.py` & `django-file-explorer-1.5.0/explorer/models/volume.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/static/explorer/action.js` & `django-file-explorer-1.5.0/explorer/static/explorer/action.js`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/static/explorer/checkbox.js` & `django-file-explorer-1.5.0/explorer/static/explorer/checkbox.js`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/static/explorer/onload.js` & `django-file-explorer-1.5.0/explorer/static/explorer/onload.js`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/static/explorer/volume.js` & `django-file-explorer-1.5.0/explorer/static/explorer/volume.js`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/templates/explorer/about.html` & `django-file-explorer-1.5.0/explorer/templates/explorer/about.html`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/templates/explorer/base.html` & `django-file-explorer-1.5.0/explorer/templates/explorer/base.html`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/templates/explorer/index.html` & `django-file-explorer-1.5.0/explorer/templates/explorer/index.html`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/templates/explorer/login.html` & `django-file-explorer-1.5.0/explorer/templates/explorer/login.html`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/views/about.py` & `django-file-explorer-1.5.0/explorer/views/about.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/views/extractor/location.py` & `django-file-explorer-1.5.0/explorer/views/extractor/location.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/views/extractor/request.py` & `django-file-explorer-1.5.0/explorer/views/extractor/request.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/views/extractor/user.py` & `django-file-explorer-1.5.0/explorer/views/extractor/user.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/views/logger/logger.py` & `django-file-explorer-1.5.0/explorer/views/logger/logger.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/views/login.py` & `django-file-explorer-1.5.0/explorer/views/login.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/views/logout.py` & `django-file-explorer-1.5.0/explorer/views/logout.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/views/main.py` & `django-file-explorer-1.5.0/explorer/views/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from django import http
 from django.http import FileResponse
 from django.shortcuts import render
 from django.urls import reverse
 from django.views.generic.base import TemplateView
+from django.conf import settings
 
 from .operations.explorer import ExplorerOperations
 from .operations.location import LocationOperations
 from .operations.action import ActionOperations
 from .logger.logger import ExplorerLogger
-from .vscode_icons.vscode import VSCodeIcons
+
 
 class Explorer(TemplateView):
     template_name = 'explorer/index.html'
     http_method_names = ['get', 'post']
     
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
@@ -52,16 +53,15 @@
 
         # GETTING LOATION REATED DATA
         data_list = lo.getData() # Getting location file and dir data.
         summary_data = lo.getDataSummary() # Getting summary data.
         navigation_bar_data = lo.getNavigationBarData() # Getting navigation bar data.
         
         # GETTING ICONS INFORMATION
-        vsi = VSCodeIcons()
-        data_list = vsi.addIconInfo(data_list)
+        data_list = self._addIconInformation(data_list)
 
         # GETTING EXPLORER RELATED DATA
         page_data = xo.getPageData(data_list) # Getting page data.
         pagination_data = xo.getPaginationData(page_data) # Getting pagination data.
         
         # MAKING CONTEXT 
         context = self.get_context_data()
@@ -120,8 +120,36 @@
     
     def _render_error(self, request, message):
         """Rendered error template"""
         return render(request, 'explorer/error.html', {'message': message})
 
     def _render_file(self, request, file_path):
         """Return the file render response."""
-        return FileResponse(open(file_path, 'rb'), as_attachment=False)
+        return FileResponse(open(file_path, 'rb'), as_attachment=False)
+    
+    def _addIconInformation(self, data_list):
+        """Adding icon information if icon package is used."""
+        # IF APP IS NOT USED
+        if not ('vscode_icons' in settings.INSTALLED_APPS):
+            return data_list
+        
+        # LOADING MODULE IF EXISTS
+        try:
+            from vscode_icons.vscode import VSCodeIcons
+            vsi = VSCodeIcons()
+        except:
+            return data_list
+        
+        # UPDATING ICON INFORMATION
+        icon_data = []
+        for data in data_list:
+            # GETTING TYPE AND NAME
+            type = data['type']
+            name = data['name']
+            
+            if type == 'directory':
+                icon_path = vsi.findDirectoryIcon(name)
+            else:
+                icon_path = vsi.findFileIcon(name)
+            data['icon'] = icon_path
+            icon_data.append(data)
+        return data_list
```

### Comparing `django-file-explorer-1.4.0/explorer/views/operations/action.py` & `django-file-explorer-1.5.0/explorer/views/operations/action.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/views/operations/explorer.py` & `django-file-explorer-1.5.0/explorer/views/operations/explorer.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/views/operations/location.py` & `django-file-explorer-1.5.0/explorer/views/operations/location.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/views/utils/path.py` & `django-file-explorer-1.5.0/explorer/views/utils/path.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/explorer/views/validator/request.py` & `django-file-explorer-1.5.0/explorer/views/validator/request.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.4.0/setup.py` & `django-file-explorer-1.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     packages=find_namespace_packages(),
     package_data={
         "": ["*.html", "*.css", "*.js", "*.svg", "*.json"],
     },
     install_requires=[
         'requests',
+        'vscode-icons',
         'django>=3.2.10',
         'psycopg2-binary>=2.9.5'
     ],
 
     keywords=["explorer", "file explorer", "directory explorer", "django explorer", 'location explorer'],
     classifiers=[
         "Framework :: Django :: 3.2",
```

