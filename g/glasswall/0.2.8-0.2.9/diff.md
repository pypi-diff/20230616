# Comparing `tmp/glasswall-0.2.8.tar.gz` & `tmp/glasswall-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glasswall-0.2.8.tar", last modified: Wed Sep 29 14:51:33 2021, max compression
+gzip compressed data, was "glasswall-0.2.9.tar", last modified: Fri Oct  1 15:44:21 2021, max compression
```

## Comparing `glasswall-0.2.8.tar` & `glasswall-0.2.9.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.715939 glasswall-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-09-29 14:51:20.000000 glasswall-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15553 2021-09-29 14:51:33.715939 glasswall-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15196 2021-09-29 14:51:20.000000 glasswall-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.707939 glasswall-0.2.8/glasswall/
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.707939 glasswall-0.2.8/glasswall/config/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.707939 glasswall-0.2.8/glasswall/config/creationflags/
--rw-r--r--   0 runner    (1001) docker     (121)      582 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/config/creationflags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.707939 glasswall-0.2.8/glasswall/config/logging/
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/config/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.707939 glasswall-0.2.8/glasswall/config/security_tagging/
--rw-r--r--   0 runner    (1001) docker     (121)      205 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/config/security_tagging/tags_w3schools.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.707939 glasswall-0.2.8/glasswall/config/word_search/
--rw-r--r--   0 runner    (1001) docker     (121)     6180 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/config/word_search/homoglyphs.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.707939 glasswall-0.2.8/glasswall/config/xml/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/config/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/config/xml/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.707939 glasswall-0.2.8/glasswall/content_management/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.707939 glasswall-0.2.8/glasswall/content_management/config_elements/
--rw-r--r--   0 runner    (1001) docker     (121)      805 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/config_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2501 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/config_elements/archiveConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     5710 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/config_elements/config_element.py
--rw-r--r--   0 runner    (1001) docker     (121)     1459 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/config_elements/pdfConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/config_elements/pptConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/config_elements/sysConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/config_elements/textList.py
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/config_elements/textSearchConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/config_elements/tiffConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/config_elements/wordConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/config_elements/xlsConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.707939 glasswall-0.2.8/glasswall/content_management/errors/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      234 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/errors/config_elements.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/errors/policies.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/errors/switches.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.711939 glasswall-0.2.8/glasswall/content_management/policies/
--rw-r--r--   0 runner    (1001) docker     (121)      350 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/policies/archive_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/policies/editor.py
--rw-r--r--   0 runner    (1001) docker     (121)    13106 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/policies/policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/policies/rebuild.py
--rw-r--r--   0 runner    (1001) docker     (121)     4825 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/policies/word_search.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.711939 glasswall-0.2.8/glasswall/content_management/switches/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/switches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7440 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/switches/archive.py
--rw-r--r--   0 runner    (1001) docker     (121)     2771 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/switches/pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/switches/ppt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/switches/switch.py
--rw-r--r--   0 runner    (1001) docker     (121)      640 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/switches/sys.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/switches/tiff.py
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/switches/word.py
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/content_management/switches/xls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.711939 glasswall-0.2.8/glasswall/determine_file_type/
--rw-r--r--   0 runner    (1001) docker     (121)      243 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/determine_file_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/determine_file_type/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)      977 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/determine_file_type/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2213 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/determine_file_type/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4706 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/determine_file_type/successes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.711939 glasswall-0.2.8/glasswall/libraries/
--rw-r--r--   0 runner    (1001) docker     (121)     2391 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.711939 glasswall-0.2.8/glasswall/libraries/archive_manager/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/archive_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    48307 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/archive_manager/archive_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/archive_manager/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/archive_manager/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/archive_manager/successes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.711939 glasswall-0.2.8/glasswall/libraries/editor/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/editor/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)    50905 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/editor/editor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/editor/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/editor/successes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/library.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.711939 glasswall-0.2.8/glasswall/libraries/rebuild/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/rebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/rebuild/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/rebuild/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    44504 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/rebuild/rebuild.py
--rw-r--r--   0 runner    (1001) docker     (121)      374 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/rebuild/successes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.715939 glasswall-0.2.8/glasswall/libraries/security_tagging/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/security_tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      206 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/security_tagging/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/security_tagging/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    11441 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/security_tagging/security_tagging.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/security_tagging/successes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.715939 glasswall-0.2.8/glasswall/libraries/word_search/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/word_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/word_search/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)      346 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/word_search/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/word_search/successes.py
--rw-r--r--   0 runner    (1001) docker     (121)    10251 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/libraries/word_search/word_search.py
--rw-r--r--   0 runner    (1001) docker     (121)    14861 2021-09-29 14:51:20.000000 glasswall-0.2.8/glasswall/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.707939 glasswall-0.2.8/glasswall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15553 2021-09-29 14:51:33.000000 glasswall-0.2.8/glasswall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3657 2021-09-29 14:51:33.000000 glasswall-0.2.8/glasswall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 14:51:33.000000 glasswall-0.2.8/glasswall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-09-29 14:51:33.000000 glasswall-0.2.8/glasswall.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-09-29 14:51:33.715939 glasswall-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      622 2021-09-29 14:51:20.000000 glasswall-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.715939 glasswall-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-09-29 14:51:20.000000 glasswall-0.2.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:33.715939 glasswall-0.2.8/tests/content_management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 14:51:20.000000 glasswall-0.2.8/tests/content_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8572 2021-09-29 14:51:20.000000 glasswall-0.2.8/tests/content_management/test_config_element.py
--rw-r--r--   0 runner    (1001) docker     (121)    26105 2021-09-29 14:51:20.000000 glasswall-0.2.8/tests/content_management/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3042 2021-09-29 14:51:20.000000 glasswall-0.2.8/tests/content_management/test_switch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.449760 glasswall-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2021-10-01 15:44:06.000000 glasswall-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    15553 2021-10-01 15:44:21.449760 glasswall-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    15196 2021-10-01 15:44:06.000000 glasswall-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.433760 glasswall-0.2.9/glasswall/
+-rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.433760 glasswall-0.2.9/glasswall/config/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.433760 glasswall-0.2.9/glasswall/config/creationflags/
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/config/creationflags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.433760 glasswall-0.2.9/glasswall/config/logging/
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/config/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.433760 glasswall-0.2.9/glasswall/config/security_tagging/
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/config/security_tagging/tags_w3schools.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.433760 glasswall-0.2.9/glasswall/config/word_search/
+-rw-r--r--   0 runner    (1001) docker     (121)     6180 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/config/word_search/homoglyphs.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.433760 glasswall-0.2.9/glasswall/config/xml/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/config/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/config/xml/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.433760 glasswall-0.2.9/glasswall/content_management/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.437760 glasswall-0.2.9/glasswall/content_management/config_elements/
+-rw-r--r--   0 runner    (1001) docker     (121)      805 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/config_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2501 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/config_elements/archiveConfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5710 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/config_elements/config_element.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/config_elements/pdfConfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/config_elements/pptConfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/config_elements/sysConfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/config_elements/textList.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2100 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/config_elements/textSearchConfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/config_elements/tiffConfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1508 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/config_elements/wordConfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1505 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/config_elements/xlsConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.437760 glasswall-0.2.9/glasswall/content_management/errors/
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      234 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/errors/config_elements.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/errors/policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/errors/switches.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.437760 glasswall-0.2.9/glasswall/content_management/policies/
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/policies/archive_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1012 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/policies/editor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16041 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/policies/policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1014 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/policies/rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4825 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/policies/word_search.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.441760 glasswall-0.2.9/glasswall/content_management/switches/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/switches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7440 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/switches/archive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2771 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/switches/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2468 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/switches/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1675 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/switches/switch.py
+-rw-r--r--   0 runner    (1001) docker     (121)      640 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/switches/sys.py
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/switches/tiff.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2479 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/switches/word.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2479 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/content_management/switches/xls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.441760 glasswall-0.2.9/glasswall/determine_file_type/
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/determine_file_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/determine_file_type/classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      977 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/determine_file_type/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2213 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/determine_file_type/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4706 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/determine_file_type/successes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.441760 glasswall-0.2.9/glasswall/libraries/
+-rw-r--r--   0 runner    (1001) docker     (121)     2391 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.441760 glasswall-0.2.9/glasswall/libraries/archive_manager/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/archive_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48307 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/archive_manager/archive_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/archive_manager/classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/archive_manager/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/archive_manager/successes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.445760 glasswall-0.2.9/glasswall/libraries/editor/
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/editor/classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50905 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/editor/editor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2023 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/editor/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/editor/successes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1588 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/library.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.445760 glasswall-0.2.9/glasswall/libraries/rebuild/
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/rebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/rebuild/classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4081 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/rebuild/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44504 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/rebuild/rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/rebuild/successes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.445760 glasswall-0.2.9/glasswall/libraries/security_tagging/
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/security_tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/security_tagging/classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/security_tagging/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11441 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/security_tagging/security_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/security_tagging/successes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.445760 glasswall-0.2.9/glasswall/libraries/word_search/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/word_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/word_search/classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/word_search/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/word_search/successes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10251 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/libraries/word_search/word_search.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14861 2021-10-01 15:44:06.000000 glasswall-0.2.9/glasswall/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.433760 glasswall-0.2.9/glasswall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    15553 2021-10-01 15:44:21.000000 glasswall-0.2.9/glasswall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3657 2021-10-01 15:44:21.000000 glasswall-0.2.9/glasswall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-01 15:44:21.000000 glasswall-0.2.9/glasswall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-10-01 15:44:21.000000 glasswall-0.2.9/glasswall.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-10-01 15:44:21.449760 glasswall-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2021-10-01 15:44:06.000000 glasswall-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.445760 glasswall-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-10-01 15:44:06.000000 glasswall-0.2.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:21.445760 glasswall-0.2.9/tests/content_management/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-01 15:44:06.000000 glasswall-0.2.9/tests/content_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8572 2021-10-01 15:44:06.000000 glasswall-0.2.9/tests/content_management/test_config_element.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29371 2021-10-01 15:44:06.000000 glasswall-0.2.9/tests/content_management/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3042 2021-10-01 15:44:06.000000 glasswall-0.2.9/tests/content_management/test_switch.py
```

### Comparing `glasswall-0.2.8/PKG-INFO` & `glasswall-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glasswall
-Version: 0.2.8
+Version: 0.2.9
 Summary: Glasswall Python Wrapper
 Home-page: https://github.com/filetrust/glasswall-python
 Author: AngusWR
 Author-email: aroberts@glasswallsolutions.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `glasswall-0.2.8/README.md` & `glasswall-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/__init__.py` & `glasswall-0.2.9/glasswall/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 import os
 import platform
 import tempfile
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 _OPERATING_SYSTEM = platform.system()
 _PYTHON_VERSION = platform.python_version()
 _ROOT = os.path.dirname(__file__)
 _TEMPDIR = os.path.join(os.environ.get("AGENT_TEMPDIRECTORY", tempfile.gettempdir()), "glasswall")
 
 from glasswall import config, content_management, determine_file_type, utils
```

### Comparing `glasswall-0.2.8/glasswall/config/creationflags/__init__.py` & `glasswall-0.2.9/glasswall/config/creationflags/__init__.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/config/logging/__init__.py` & `glasswall-0.2.9/glasswall/config/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/config/word_search/homoglyphs.json` & `glasswall-0.2.9/glasswall/config/word_search/homoglyphs.json`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/config_elements/__init__.py` & `glasswall-0.2.9/glasswall/content_management/config_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/config_elements/archiveConfig.py` & `glasswall-0.2.9/glasswall/content_management/config_elements/archiveConfig.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/config_elements/config_element.py` & `glasswall-0.2.9/glasswall/content_management/config_elements/config_element.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/config_elements/pdfConfig.py` & `glasswall-0.2.9/glasswall/content_management/config_elements/pdfConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,18 @@
     Args:
         default (str): The default action: allow, disallow, or sanitise.
 
     Key word arguments can be specified to change individual switch values:
     pdfConfig(default="allow", embedded_images="sanitise")
     """
 
-    def __init__(self, default: str = "sanitise", **kwargs):
+    def __init__(self, default: str = "sanitise", attributes: dict = {}, **kwargs):
         self.name = self.__class__.__name__
         self.default = default
+        self.attributes = attributes
         self.switches_module = switches.pdf
         self.default_switches = [
             self.switches_module.acroform(value=default),
             self.switches_module.actions_all(value=default),
             self.switches_module.digital_signatures(value=default),
             self.switches_module.embedded_files(value=default),
             self.switches_module.embedded_images(value=default),
@@ -29,11 +30,12 @@
             self.switches_module.javascript(value=default),
             self.switches_module.metadata(value=default),
         ]
 
         super().__init__(
             name=self.name,
             default=self.default,
+            attributes=self.attributes,
             switches_module=self.switches_module,
             default_switches=self.default_switches,
             config=kwargs
         )
```

### Comparing `glasswall-0.2.8/glasswall/content_management/config_elements/pptConfig.py` & `glasswall-0.2.9/glasswall/content_management/config_elements/pptConfig.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,18 @@
     Args:
         default (str): The default action: allow, disallow, or sanitise.
 
     Key word arguments can be specified to change individual switch values:
     pptConfig(default="allow", embedded_images="sanitise")
     """
 
-    def __init__(self, default: str = "sanitise", **kwargs):
+    def __init__(self, default: str = "sanitise", attributes: dict = {}, **kwargs):
         self.name = self.__class__.__name__
         self.default = default
+        self.attributes = attributes
         self.switches_module = switches.ppt
         self.default_switches = [
             self.switches_module.embedded_files(value=default),
             self.switches_module.embedded_images(value=default),
             self.switches_module.external_hyperlinks(value=default),
             self.switches_module.internal_hyperlinks(value=default),
             self.switches_module.javascript(value=default),
@@ -28,11 +29,12 @@
             self.switches_module.metadata(value=default),
             self.switches_module.review_comments(value=default),
         ]
 
         super().__init__(
             name=self.name,
             default=self.default,
+            attributes=self.attributes,
             switches_module=self.switches_module,
             default_switches=self.default_switches,
             config=kwargs
         )
```

### Comparing `glasswall-0.2.8/glasswall/content_management/config_elements/sysConfig.py` & `glasswall-0.2.9/glasswall/content_management/config_elements/sysConfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 class sysConfig(ConfigElement):
     """ A sysConfig ConfigElement.
 
     Key word arguments can be specified to change individual switch values:
     sysConfig(interchange_type="xml", interchange_pretty="false")
     """
 
-    def __init__(self, **kwargs):
+    def __init__(self, attributes={}, **kwargs):
         self.name = self.__class__.__name__
+        self.attributes = attributes
         self.switches_module = switches.sys
         self.default_switches = [
             self.switches_module.interchange_type(value="sisl"),
             self.switches_module.interchange_pretty(value="false"),
         ]
 
         super().__init__(
             name=self.name,
+            attributes=self.attributes,
             switches_module=self.switches_module,
             default_switches=self.default_switches,
             config=kwargs
         )
```

### Comparing `glasswall-0.2.8/glasswall/content_management/config_elements/textSearchConfig.py` & `glasswall-0.2.9/glasswall/content_management/config_elements/textSearchConfig.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,12 +47,15 @@
 
             # Construct config_element
             config_element = ConfigElement(**textList_dict)
 
             # Append constructed config_element to subelements
             subelements.append(config_element)
 
-        self.subelements = [
-            textList(subelements=subelements)
-        ]
+        if subelements:
+            self.subelements = [
+                textList(subelements=subelements)
+            ]
+        else:
+            self.subelements = []
 
         super().__init__(name=self.name, attributes=self.attributes, subelements=self.subelements)
```

### Comparing `glasswall-0.2.8/glasswall/content_management/config_elements/tiffConfig.py` & `glasswall-0.2.9/glasswall/content_management/config_elements/tiffConfig.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,22 +10,24 @@
     Args:
         default (str): The default action: allow, disallow, or sanitise.
 
     Key word arguments can be specified to change individual switch values:
     tiffConfig(geotiff="sanitise")
     """
 
-    def __init__(self, default: str = "sanitise", **kwargs):
+    def __init__(self, default: str = "sanitise", attributes={}, **kwargs):
         self.name = self.__class__.__name__
         self.default = default
+        self.attributes = attributes
         self.switches_module = switches.tiff
         self.default_switches = [
             self.switches_module.geotiff(value=default),
         ]
 
         super().__init__(
             name=self.name,
             default=self.default,
+            attributes=self.attributes,
             switches_module=self.switches_module,
             default_switches=self.default_switches,
             config=kwargs
         )
```

### Comparing `glasswall-0.2.8/glasswall/content_management/config_elements/wordConfig.py` & `glasswall-0.2.9/glasswall/content_management/config_elements/wordConfig.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,17 +10,18 @@
     Args:
         default (str): The default action: allow, disallow, or sanitise.
 
     Key word arguments can be specified to change individual switch values:
     wordConfig(default="allow", embedded_images="sanitise")
     """
 
-    def __init__(self, default: str = "sanitise", **kwargs):
+    def __init__(self, default: str = "sanitise", attributes: dict = {}, **kwargs):
         self.name = self.__class__.__name__
         self.default = default
+        self.attributes = attributes
         self.switches_module = switches.word
         self.default_switches = [
             self.switches_module.dynamic_data_exchange(value=default),
             self.switches_module.embedded_files(value=default),
             self.switches_module.embedded_images(value=default),
             self.switches_module.external_hyperlinks(value=default),
             self.switches_module.internal_hyperlinks(value=default),
@@ -28,11 +29,12 @@
             self.switches_module.metadata(value=default),
             self.switches_module.review_comments(value=default),
         ]
 
         super().__init__(
             name=self.name,
             default=self.default,
+            attributes=self.attributes,
             switches_module=self.switches_module,
             default_switches=self.default_switches,
             config=kwargs
         )
```

### Comparing `glasswall-0.2.8/glasswall/content_management/config_elements/xlsConfig.py` & `glasswall-0.2.9/glasswall/content_management/config_elements/xlsConfig.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,17 +10,18 @@
     Args:
         default (str): The default action: allow, disallow, or sanitise.
 
     Key word arguments can be specified to change individual switch values:
     xlsConfig(default="allow", embedded_images="sanitise")
     """
 
-    def __init__(self, default: str = "sanitise", **kwargs):
+    def __init__(self, default: str = "sanitise", attributes: dict = {}, **kwargs):
         self.name = self.__class__.__name__
         self.default = default
+        self.attributes = attributes
         self.switches_module = switches.xls
         self.default_switches = [
             self.switches_module.dynamic_data_exchange(value=default),
             self.switches_module.embedded_files(value=default),
             self.switches_module.embedded_images(value=default),
             self.switches_module.external_hyperlinks(value=default),
             self.switches_module.internal_hyperlinks(value=default),
@@ -28,11 +29,12 @@
             self.switches_module.metadata(value=default),
             self.switches_module.review_comments(value=default),
         ]
 
         super().__init__(
             name=self.name,
             default=self.default,
+            attributes=self.attributes,
             switches_module=self.switches_module,
             default_switches=self.default_switches,
             config=kwargs
         )
```

### Comparing `glasswall-0.2.8/glasswall/content_management/policies/archive_manager.py` & `glasswall-0.2.9/glasswall/content_management/policies/archive_manager.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/policies/editor.py` & `glasswall-0.2.9/glasswall/content_management/policies/editor.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/policies/policy.py` & `glasswall-0.2.9/glasswall/content_management/policies/policy.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import glasswall
 from glasswall import utils
 from glasswall.content_management.config_elements.config_element import ConfigElement
 from glasswall.content_management.errors.config_elements import ConfigElementNotFound
 from glasswall.content_management.errors.switches import SwitchNotFound
 from glasswall.content_management.switches.switch import Switch
+from lxml import etree
 
 
 class Policy:
     """ A Content Management Policy made up of a list of ConfigElement instances. """
 
     def __init__(self,
                  config_elements: list = [],
@@ -279,7 +280,62 @@
     def get_switches(dictionary: dict):
         """ Returns switches from arg "dictionary". Switches are key value pairs that do not have a key starting with "@". """
         return {
             k: v
             for k, v in dictionary.items()
             if not k.startswith("@")
         }
+
+    @staticmethod
+    def from_string(string: str):
+        """ Create Policy object from string.
+
+        Args:
+            string (str): A string representation of an xml content management policy, or a file path.
+
+        Returns:
+            new_policy (glasswall.content_management.policies.Policy): A Policy object.
+        """
+        try:
+            string = glasswall.utils.validate_xml(string)
+        except ValueError:
+            raise glasswall.content_management.errors.policies.ContentManagementPolicyError(string)
+
+        config = etree.fromstring(string.encode("utf-8"))
+
+        if config.tag != "config":
+            raise glasswall.content_management.errors.policies.ContentManagementPolicyError(string)
+
+        new_policy = glasswall.content_management.policies.Policy()
+
+        for config_element in config:
+            if hasattr(glasswall.content_management.config_elements, config_element.tag):
+                # Known config element exists, e.g. pdfConfig
+                new_config_element = getattr(glasswall.content_management.config_elements, config_element.tag)(attributes=config_element.attrib)
+            else:
+                # Create custom config element
+                new_config_element = glasswall.content_management.config_elements.ConfigElement(name=config_element.tag, attributes=config_element.attrib)
+
+            for item in config_element:
+                # Add children, e.g. textList has child elements: textItem
+                if item.getchildren():
+                    # if getchildren() then item is a config element, such as textList
+                    textList = glasswall.content_management.config_elements.ConfigElement(name=item.tag, attributes=item.attrib)
+                    for textItem in item.getchildren():
+                        new_textItem = glasswall.content_management.config_elements.ConfigElement(name=textItem.tag, attributes=textItem.attrib)
+                        for switch in textItem:
+                            new_textItem.add_switch(glasswall.content_management.switches.Switch(name=switch.tag, value=switch.text, attributes=switch.attrib))
+                        textList.subelements.append(new_textItem)
+                    new_config_element.subelements.append(textList)
+                    continue
+
+                # if not getchildren() then item is a switch
+                if hasattr(new_config_element.switches_module, item.tag):
+                    # Known switch exists, e.g. pdf.internal_hyperlinks
+                    new_switch = getattr(new_config_element.switches_module, item.tag)(value=item.text)
+                else:
+                    new_switch = glasswall.content_management.switches.Switch(name=item.tag, value=item.text, attributes=item.attrib)
+                new_config_element.add_switch(new_switch)
+
+            new_policy.add_config_element(new_config_element)
+
+        return new_policy
```

### Comparing `glasswall-0.2.8/glasswall/content_management/policies/rebuild.py` & `glasswall-0.2.9/glasswall/content_management/policies/rebuild.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/policies/word_search.py` & `glasswall-0.2.9/glasswall/content_management/policies/word_search.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/switches/archive.py` & `glasswall-0.2.9/glasswall/content_management/switches/archive.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/switches/pdf.py` & `glasswall-0.2.9/glasswall/content_management/switches/pdf.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/switches/ppt.py` & `glasswall-0.2.9/glasswall/content_management/switches/ppt.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/switches/switch.py` & `glasswall-0.2.9/glasswall/content_management/switches/switch.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/switches/sys.py` & `glasswall-0.2.9/glasswall/content_management/switches/sys.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/switches/word.py` & `glasswall-0.2.9/glasswall/content_management/switches/word.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/content_management/switches/xls.py` & `glasswall-0.2.9/glasswall/content_management/switches/xls.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/determine_file_type/errors.py` & `glasswall-0.2.9/glasswall/determine_file_type/errors.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/determine_file_type/helpers.py` & `glasswall-0.2.9/glasswall/determine_file_type/helpers.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/determine_file_type/successes.py` & `glasswall-0.2.9/glasswall/determine_file_type/successes.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/libraries/__init__.py` & `glasswall-0.2.9/glasswall/libraries/__init__.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/libraries/archive_manager/archive_manager.py` & `glasswall-0.2.9/glasswall/libraries/archive_manager/archive_manager.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/libraries/editor/editor.py` & `glasswall-0.2.9/glasswall/libraries/editor/editor.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/libraries/editor/errors.py` & `glasswall-0.2.9/glasswall/libraries/editor/errors.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/libraries/library.py` & `glasswall-0.2.9/glasswall/libraries/library.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/libraries/rebuild/errors.py` & `glasswall-0.2.9/glasswall/libraries/rebuild/errors.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/libraries/rebuild/rebuild.py` & `glasswall-0.2.9/glasswall/libraries/rebuild/rebuild.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/libraries/security_tagging/security_tagging.py` & `glasswall-0.2.9/glasswall/libraries/security_tagging/security_tagging.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/libraries/word_search/word_search.py` & `glasswall-0.2.9/glasswall/libraries/word_search/word_search.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall/utils.py` & `glasswall-0.2.9/glasswall/utils.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/glasswall.egg-info/PKG-INFO` & `glasswall-0.2.9/glasswall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glasswall
-Version: 0.2.8
+Version: 0.2.9
 Summary: Glasswall Python Wrapper
 Home-page: https://github.com/filetrust/glasswall-python
 Author: AngusWR
 Author-email: aroberts@glasswallsolutions.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `glasswall-0.2.8/glasswall.egg-info/SOURCES.txt` & `glasswall-0.2.9/glasswall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/setup.py` & `glasswall-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/tests/content_management/test_config_element.py` & `glasswall-0.2.9/tests/content_management/test_config_element.py`

 * *Files identical despite different names*

### Comparing `glasswall-0.2.8/tests/content_management/test_policy.py` & `glasswall-0.2.9/tests/content_management/test_policy.py`

 * *Files 8% similar despite different names*

```diff
@@ -674,10 +674,88 @@
 
         # textSetting attributes are customisable
         self.assertTrue(policy.textSearchConfig.textList.subelements[0].switches[1].attributes.get("customAttribute") == "customValue")
 
         # replacementChar attribute exists
         self.assertTrue(policy.textSearchConfig.textList.subelements[0].switches[1].attributes.get("replacementChar") == "*")
 
+    def test_policy_from_string___policy_strings_equal(self):
+        policies_to_test = [
+            glasswall.content_management.policies.ArchiveManager(
+                default="sanitise",
+                default_archive_manager="process",
+                config={
+                    "pdfConfig": {"embeddedImages": "disallow"},
+                    "wordConfig": {"embeddedImages": "disallow"},
+                    "archiveConfig": {
+                        "@recursionDepth": "50",
+                        "jpeg": "discard"
+                    }
+                }
+            ),
+            glasswall.content_management.policies.Editor(
+                default="allow",
+                config={
+                    "sysConfig": {
+                        "interchange_type": "sisl",
+                        "interchange_pretty": "true",
+                    },
+                    "xlsConfig": {
+                        "external_hyperlinks": "sanitise",
+                        "internal_hyperlinks": "sanitise",
+                    }
+                },
+            ),
+            glasswall.content_management.policies.Rebuild(
+                default="disallow",
+                config={
+                    "sysConfig": {
+                        "interchange_type": "xml",
+                        "interchange_pretty": "false",
+                    },
+                    "pdfConfig": {
+                        "external_hyperlinks": "sanitise",
+                        "internal_hyperlinks": "sanitise",
+                    }
+                },
+            ),
+            glasswall.content_management.policies.WordSearch(
+                default="allow",
+                config={
+                    "textSearchConfig": {
+                        "@libVersion": "core2",
+                        "textList": [
+                            {"name": "textItem", "switches": [
+                                {"name": "text", "value": "password"},
+                                {"name": "textSetting", "@replacementChar": "*", "value": "redact"},
+                            ]},
+                            {"name": "textItem", "switches": [
+                                {"name": "text", "value": "email"},
+                                {"name": "textSetting", "@replacementChar": "*", "value": "redact"},
+                            ]},
+                        ]
+                    }
+                }
+            ),
+            glasswall.content_management.policies.Policy(
+                config={
+                    "customConfig": {
+                        "customSwitch1": "customValue1",
+                        "customSwitch2": "customValue2",
+                    },
+                    "customConfig2": {
+                        "customSwitch3": "customValue3",
+                    }
+                }
+            )
+        ]
+
+        for policy in policies_to_test:
+            # Create a new Policy object from the using the Policy.from_string method
+            policy_from_string = glasswall.content_management.policies.Policy.from_string(policy.text)
+
+            # The two policies should be equal
+            self.assertTrue(policy.text == policy_from_string.text, msg=f"Policy texts not equal:\n{policy.text}\n{policy_from_string.text}")
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `glasswall-0.2.8/tests/content_management/test_switch.py` & `glasswall-0.2.9/tests/content_management/test_switch.py`

 * *Files identical despite different names*

