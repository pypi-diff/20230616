# Comparing `tmp/pycognaize-1.4.3.tar.gz` & `tmp/pycognaize-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycognaize-1.4.3.tar", last modified: Wed May 31 13:08:29 2023, max compression
+gzip compressed data, was "pycognaize-1.4.6.tar", last modified: Fri Jun 16 09:00:36 2023, max compression
```

## Comparing `pycognaize-1.4.3.tar` & `pycognaize-1.4.6.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.123175 pycognaize-1.4.3/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    31663 2023-05-31 13:07:33.000000 pycognaize-1.4.3/CHANGELOG.md
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    35137 2022-11-15 12:53:10.000000 pycognaize-1.4.3/LICENSE.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    33431 2023-05-31 13:08:29.123175 pycognaize-1.4.3/PKG-INFO
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1310 2023-02-20 13:34:43.000000 pycognaize-1.4.3/README.md
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.119175 pycognaize-1.4.3/pycognaize/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      361 2023-05-31 13:07:33.000000 pycognaize-1.4.3/pycognaize/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      210 2023-04-28 11:57:35.000000 pycognaize-1.4.3/pycognaize/cli.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2168 2023-01-11 08:15:39.000000 pycognaize-1.4.3/pycognaize/clidriver.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.119175 pycognaize-1.4.3/pycognaize/common/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/common/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      968 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/common/classification_labels.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2359 2023-03-07 12:26:57.000000 pycognaize-1.4.3/pycognaize/common/confidence.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1650 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/common/decorators.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5138 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/common/enums.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      394 2022-12-06 11:01:27.000000 pycognaize-1.4.3/pycognaize/common/exceptions.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1750 2022-12-06 11:01:27.000000 pycognaize-1.4.3/pycognaize/common/field_collection.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2352 2022-12-06 11:01:27.000000 pycognaize-1.4.3/pycognaize/common/lazy_dict.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2096 2022-12-06 11:01:27.000000 pycognaize-1.4.3/pycognaize/common/lazy_group_dict.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6826 2023-01-26 10:20:57.000000 pycognaize-1.4.3/pycognaize/common/numeric_parser.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3903 2023-05-04 16:18:45.000000 pycognaize-1.4.3/pycognaize/common/table_utils.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    22777 2023-04-28 14:56:56.000000 pycognaize-1.4.3/pycognaize/common/utils.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      285 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/common/white_pixel.jpeg
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.119175 pycognaize-1.4.3/pycognaize/document/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      129 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/document/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    23788 2023-05-31 09:56:30.000000 pycognaize-1.4.3/pycognaize/document/document.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.123175 pycognaize-1.4.3/pycognaize/document/field/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      674 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3367 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/area_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2818 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/date_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3200 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3996 2023-05-30 15:45:37.000000 pycognaize-1.4.3/pycognaize/document/field/link_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3566 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/numeric_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4437 2023-05-31 13:07:33.000000 pycognaize-1.4.3/pycognaize/document/field/section_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2825 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/span_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5242 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/table_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4051 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/field/text_field.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2904 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/html_info.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    21421 2023-02-20 13:34:43.000000 pycognaize-1.4.3/pycognaize/document/page.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3349 2023-04-28 14:56:56.000000 pycognaize-1.4.3/pycognaize/document/snapshot.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.123175 pycognaize-1.4.3/pycognaize/document/tag/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      116 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/document/tag/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3449 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/document/tag/cell.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6090 2023-05-29 14:26:12.000000 pycognaize-1.4.3/pycognaize/document/tag/extraction_tag.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    14209 2023-05-04 16:18:45.000000 pycognaize-1.4.3/pycognaize/document/tag/html_tag.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2657 2023-05-30 10:47:37.000000 pycognaize-1.4.3/pycognaize/document/tag/section_tag.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1794 2022-12-06 11:01:27.000000 pycognaize-1.4.3/pycognaize/document/tag/span_tag.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     8858 2023-01-27 15:01:05.000000 pycognaize-1.4.3/pycognaize/document/tag/table_tag.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    14977 2023-05-29 14:03:01.000000 pycognaize-1.4.3/pycognaize/document/tag/tag.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2863 2022-11-15 12:53:10.000000 pycognaize-1.4.3/pycognaize/index.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3866 2023-05-29 08:03:29.000000 pycognaize-1.4.3/pycognaize/login.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    21992 2023-05-04 16:18:45.000000 pycognaize-1.4.3/pycognaize/model.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.123175 pycognaize-1.4.3/pycognaize/model_registry/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      133 2023-04-28 11:57:35.000000 pycognaize-1.4.3/pycognaize/model_registry/__init__.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.123175 pycognaize-1.4.3/pycognaize/model_registry/db/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2023-04-28 11:57:35.000000 pycognaize-1.4.3/pycognaize/model_registry/db/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      787 2023-04-28 11:57:35.000000 pycognaize-1.4.3/pycognaize/model_registry/db/models.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      598 2023-04-28 11:57:35.000000 pycognaize-1.4.3/pycognaize/model_registry/login.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     4687 2023-04-28 11:57:35.000000 pycognaize-1.4.3/pycognaize/model_registry/submit.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-31 13:08:29.119175 pycognaize-1.4.3/pycognaize.egg-info/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    33431 2023-05-31 13:08:29.000000 pycognaize-1.4.3/pycognaize.egg-info/PKG-INFO
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1852 2023-05-31 13:08:29.000000 pycognaize-1.4.3/pycognaize.egg-info/SOURCES.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        1 2023-05-31 13:08:29.000000 pycognaize-1.4.3/pycognaize.egg-info/dependency_links.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       53 2023-05-31 13:08:29.000000 pycognaize-1.4.3/pycognaize.egg-info/entry_points.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      160 2023-05-31 13:08:29.000000 pycognaize-1.4.3/pycognaize.egg-info/requires.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       11 2023-05-31 13:08:29.000000 pycognaize-1.4.3/pycognaize.egg-info/top_level.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      896 2023-05-31 13:08:29.123175 pycognaize-1.4.3/setup.cfg
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1005 2023-04-28 11:57:35.000000 pycognaize-1.4.3/setup.py
+drwxrwxr-x   0 silva     (1000) silva     (1000)        0 2023-06-16 09:00:36.581236 pycognaize-1.4.6/
+-rw-rw-r--   0 silva     (1000) silva     (1000)    31908 2023-06-16 08:47:24.000000 pycognaize-1.4.6/CHANGELOG.md
+-rw-rw-r--   0 silva     (1000) silva     (1000)    35137 2023-06-16 08:47:24.000000 pycognaize-1.4.6/LICENSE.txt
+-rw-rw-r--   0 silva     (1000) silva     (1000)    33676 2023-06-16 09:00:36.581236 pycognaize-1.4.6/PKG-INFO
+-rw-rw-r--   0 silva     (1000) silva     (1000)     1310 2023-06-16 08:47:24.000000 pycognaize-1.4.6/README.md
+drwxrwxr-x   0 silva     (1000) silva     (1000)        0 2023-06-16 09:00:36.581236 pycognaize-1.4.6/pycognaize/
+-rw-rw-r--   0 silva     (1000) silva     (1000)      361 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/__init__.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)      210 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/cli.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     2168 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/clidriver.py
+drwxrwxr-x   0 silva     (1000) silva     (1000)        0 2023-06-16 09:00:36.581236 pycognaize-1.4.6/pycognaize/common/
+-rw-rw-r--   0 silva     (1000) silva     (1000)        0 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/__init__.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)      968 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/classification_labels.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)      959 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/cloud_service.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     2359 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/confidence.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     2345 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/decorators.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     5138 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/enums.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)      394 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/exceptions.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     1750 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/field_collection.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     2352 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/lazy_dict.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     2096 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/lazy_group_dict.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     6826 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/numeric_parser.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     3903 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/table_utils.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)    22922 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/utils.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)      285 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/common/white_pixel.jpeg
+drwxrwxr-x   0 silva     (1000) silva     (1000)        0 2023-06-16 09:00:36.581236 pycognaize-1.4.6/pycognaize/document/
+-rw-rw-r--   0 silva     (1000) silva     (1000)      129 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/__init__.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)    23603 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/document.py
+drwxrwxr-x   0 silva     (1000) silva     (1000)        0 2023-06-16 09:00:36.581236 pycognaize-1.4.6/pycognaize/document/field/
+-rw-rw-r--   0 silva     (1000) silva     (1000)      674 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/field/__init__.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     3367 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/field/area_field.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     2818 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/field/date_field.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     3200 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/field/field.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     3988 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/field/link_field.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     3566 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/field/numeric_field.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     4437 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/field/section_field.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     2825 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/field/span_field.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     5242 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/field/table_field.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     4051 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/field/text_field.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     2904 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/html_info.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)    21421 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/page.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     3349 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/snapshot.py
+drwxrwxr-x   0 silva     (1000) silva     (1000)        0 2023-06-16 09:00:36.581236 pycognaize-1.4.6/pycognaize/document/tag/
+-rw-rw-r--   0 silva     (1000) silva     (1000)      116 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/tag/__init__.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     3449 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/tag/cell.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     6090 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/tag/extraction_tag.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)    15408 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/tag/html_tag.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     2657 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/tag/section_tag.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     1794 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/tag/span_tag.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     8858 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/tag/table_tag.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)    14977 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/document/tag/tag.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     2863 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/index.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     4004 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/login.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)    21992 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/model.py
+drwxrwxr-x   0 silva     (1000) silva     (1000)        0 2023-06-16 09:00:36.581236 pycognaize-1.4.6/pycognaize/model_registry/
+-rw-rw-r--   0 silva     (1000) silva     (1000)      133 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/model_registry/__init__.py
+drwxrwxr-x   0 silva     (1000) silva     (1000)        0 2023-06-16 09:00:36.581236 pycognaize-1.4.6/pycognaize/model_registry/db/
+-rw-rw-r--   0 silva     (1000) silva     (1000)        0 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/model_registry/db/__init__.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)      787 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/model_registry/db/models.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)      598 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/model_registry/login.py
+-rw-rw-r--   0 silva     (1000) silva     (1000)     4687 2023-06-16 08:47:24.000000 pycognaize-1.4.6/pycognaize/model_registry/submit.py
+drwxrwxr-x   0 silva     (1000) silva     (1000)        0 2023-06-16 09:00:36.581236 pycognaize-1.4.6/pycognaize.egg-info/
+-rw-rw-r--   0 silva     (1000) silva     (1000)    33676 2023-06-16 09:00:36.000000 pycognaize-1.4.6/pycognaize.egg-info/PKG-INFO
+-rw-rw-r--   0 silva     (1000) silva     (1000)     1887 2023-06-16 09:00:36.000000 pycognaize-1.4.6/pycognaize.egg-info/SOURCES.txt
+-rw-rw-r--   0 silva     (1000) silva     (1000)        1 2023-06-16 09:00:36.000000 pycognaize-1.4.6/pycognaize.egg-info/dependency_links.txt
+-rw-rw-r--   0 silva     (1000) silva     (1000)       53 2023-06-16 09:00:36.000000 pycognaize-1.4.6/pycognaize.egg-info/entry_points.txt
+-rw-rw-r--   0 silva     (1000) silva     (1000)      168 2023-06-16 09:00:36.000000 pycognaize-1.4.6/pycognaize.egg-info/requires.txt
+-rw-rw-r--   0 silva     (1000) silva     (1000)       11 2023-06-16 09:00:36.000000 pycognaize-1.4.6/pycognaize.egg-info/top_level.txt
+-rw-rw-r--   0 silva     (1000) silva     (1000)      905 2023-06-16 09:00:36.581236 pycognaize-1.4.6/setup.cfg
+-rw-rw-r--   0 silva     (1000) silva     (1000)     1005 2023-06-16 08:47:24.000000 pycognaize-1.4.6/setup.py
```

### Comparing `pycognaize-1.4.3/CHANGELOG.md` & `pycognaize-1.4.6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # Changelog
 
 ## [1.4]
 
+### [1.4.6] - 2023-06-15
+- Add replace_nans_with_empty_html_tags functionality in HTMLTableTag build df
+
+### [1.4.5] - 2023-06-12
+- Add relogin when AWS token is expired
+
+### [1.4.4] - 2023-05-31
+- Add `anytree` to setup-requires in `setup.cfg`
+
 ### [1.4.3] - 2023-05-31
-- Fix handling of section field with no tagsc
+- Fix handling of section field with no tags
 
 ### [1.4.2] - 2023-05-30
 - Fix handling of section field value when field does not have tags
 
 ### [1.4.1] - 2023-05-29
 - Add section field and section tag functionality
```

### Comparing `pycognaize-1.4.3/LICENSE.txt` & `pycognaize-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/PKG-INFO` & `pycognaize-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycognaize
-Version: 1.4.3
+Version: 1.4.6
 Home-page: https://github.com/cognaize/pycognaize
 Author: Cognaize
 License: Apache License 2.0
 Project-URL: Source, https://github.com/cognaize/pycognaize
 Project-URL: Reference, https://pycognaize.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/cognaize/pycognaize/blob/master/CHANGELOG.md
 Requires-Python: >= 3.7
@@ -45,16 +45,25 @@
 Have a look at the [quick tutorial](http://pycognaize-docs.com.s3-website.us-east-2.amazonaws.com/tutorials/quick_tutorial.html) 
 for understanding main concepts of the SDK.
 
 # Changelog
 
 ## [1.4]
 
+### [1.4.6] - 2023-06-15
+- Add replace_nans_with_empty_html_tags functionality in HTMLTableTag build df
+
+### [1.4.5] - 2023-06-12
+- Add relogin when AWS token is expired
+
+### [1.4.4] - 2023-05-31
+- Add `anytree` to setup-requires in `setup.cfg`
+
 ### [1.4.3] - 2023-05-31
-- Fix handling of section field with no tagsc
+- Fix handling of section field with no tags
 
 ### [1.4.2] - 2023-05-30
 - Fix handling of section field value when field does not have tags
 
 ### [1.4.1] - 2023-05-29
 - Add section field and section tag functionality
```

### Comparing `pycognaize-1.4.3/README.md` & `pycognaize-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/clidriver.py` & `pycognaize-1.4.6/pycognaize/clidriver.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/common/classification_labels.py` & `pycognaize-1.4.6/pycognaize/common/classification_labels.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/common/confidence.py` & `pycognaize-1.4.6/pycognaize/common/confidence.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/common/decorators.py` & `pycognaize-1.4.6/pycognaize/common/decorators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,37 @@
+import functools
 import warnings
+
+from botocore.exceptions import ClientError
+from cloudstorageio import CloudInterface
+
 import pycognaize
 
 
 def module_not_found(stack_level: int = 2):
     """
     Warns user that function uses a module that is not listed in
     requirements.txt and is not installed in the environment
 
     :param stack_level: stack level of the warning
     :type stack_level: int
     """
+
     def module_not_found_custom(func):
         def wrapper(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except ModuleNotFoundError as e:
                 message = f"Please install module " \
-                          f"{str(e).split(' ')[-1]}. \n"\
+                          f"{str(e).split(' ')[-1]}. \n" \
                           f"It can be found in model-requirements.txt"
                 warnings.warn(message, UserWarning, stacklevel=stack_level)
+
         return wrapper
+
     return module_not_found_custom
 
 
 def soon_be_deprecated(version: str = None, stack_level: int = 2):
     """
     Warns user that the function they use will soon be deprecated.
 
@@ -39,9 +47,34 @@
 
     def soon_be_deprecated_custom(func):
         def wrapper(*args, **kwargs):
             message = f"This function will be deprecated after " \
                       f"version {version}"
             warnings.warn(message, DeprecationWarning, stacklevel=stack_level)
             return func(*args, **kwargs)
+
         return wrapper
+
     return soon_be_deprecated_custom
+
+
+def relogin_if_failed(func):
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except ClientError:
+            login = pycognaize.Login()
+
+            login.relogin()
+
+            cloud_service = args[0]
+
+            cloud_service.ci = CloudInterface(
+                aws_access_key_id=login.aws_access_key,
+                aws_secret_access_key=login.aws_secret_access_key,
+                aws_session_token=login.aws_session_token
+            )
+
+            return func(*args, **kwargs)
+
+    return wrapper
```

### Comparing `pycognaize-1.4.3/pycognaize/common/enums.py` & `pycognaize-1.4.6/pycognaize/common/enums.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/common/field_collection.py` & `pycognaize-1.4.6/pycognaize/common/field_collection.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/common/lazy_dict.py` & `pycognaize-1.4.6/pycognaize/common/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/common/lazy_group_dict.py` & `pycognaize-1.4.6/pycognaize/common/lazy_group_dict.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/common/numeric_parser.py` & `pycognaize-1.4.6/pycognaize/common/numeric_parser.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/common/table_utils.py` & `pycognaize-1.4.6/pycognaize/common/table_utils.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/common/utils.py` & `pycognaize-1.4.6/pycognaize/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
+import hashlib
 import io
+import logging
 import os
 import pathlib
 import re
+from dataclasses import dataclass
+from itertools import groupby
+from typing import Union, List, Optional, Iterable, Dict
 
-import hashlib
-import numpy as np
 import bson
-import logging
-
+import numpy as np
 from PIL import Image
-from itertools import groupby
-from typing import Union, List, Optional, Iterable, Dict
 from bson.json_util import loads as bson_loads
-from dataclasses import dataclass
 from cloudstorageio import CloudInterface
 
-from pycognaize.login import Login
-from pycognaize.common.enums import PythonShellEnum
+from pycognaize.common.cloud_service import CloudService
 from pycognaize.common.decorators import soon_be_deprecated
-
+from pycognaize.common.enums import PythonShellEnum
+from pycognaize.login import Login
 
 REGEX_NO_ALPHANUM_CHARS = re.compile(r'[^a-zA-Z\d)\[\](-.,]')
 
 
 def is_float(str_number: str) -> bool:
     """Check if the string value is a valid number.
         Infinity and NaN are regarded as invalid"""
@@ -201,16 +200,18 @@
     for word in box_coord:
         start_point_xmin = max(0, int(round(word['left'])) - 1)
         start_point_ymin = max(0, int(round(word['top'])) - 1)
 
         end_point_xmax = int(round(word['right'])) + 2
         end_point_ymax = int(round(word['bottom'])) + 2
 
-        cropped_word = b_and_w_image[start_point_ymin:end_point_ymax,
-                                     start_point_xmin:end_point_xmax]
+        cropped_word = b_and_w_image[
+                           start_point_ymin:end_point_ymax,
+                           start_point_xmin:end_point_xmax
+                       ]
 
         vectors_y = np.mean(cropped_word, axis=1)
         min_max_y = np.where((vectors_y != 0) & (vectors_y != 255))
 
         if len(min_max_y[0]) == 0:
             continue
         elif 0 < len(min_max_y[0]) < 3:
@@ -616,25 +617,28 @@
 def convert_tag_coords_to_percentages(tag, w, h) -> dict:
     return dict(left=tag.left * w / 100,
                 right=tag.right * w / 100,
                 top=tag.top * h / 100,
                 bottom=tag.bottom * h / 100)
 
 
-def cloud_interface_login(login_instance: Login) -> CloudInterface:
+def cloud_interface_login(login_instance: Login) -> CloudService:
     """Logs in to cloud interface"""
 
     if login_instance.logged_in:
         ci_instance = CloudInterface(
             aws_access_key_id=login_instance.aws_access_key,
             aws_secret_access_key=login_instance.aws_secret_access_key,
             aws_session_token=login_instance.aws_session_token)
     else:
         ci_instance = CloudInterface()
-    return ci_instance
+
+    cloud_service = CloudService(ci_instance)
+
+    return cloud_service
 
 
 def directory_summary_hash(dirname: str):
     """ Computes hash of directory summary"""
     hash_func = hashlib.md5
 
     if not os.path.isdir(dirname):
```

### Comparing `pycognaize-1.4.3/pycognaize/document/document.py` & `pycognaize-1.4.6/pycognaize/document/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -560,14 +560,7 @@
         raise ValueError(f'Wrong opacity value {opacity}')
     color_dict = {"stroke": getColor(color), "fill": getColor(color)}
     annot = page.add_rect_annot(annot_rect)
     annot.set_colors(color_dict)
     annot.set_opacity(opacity)
     annot.update()
     return doc.write()
-
-if __name__ == '__main__':
-    import json
-    with open('/home/atlantx/Downloads/empty_section_hov (1).json') as f:
-        data = json.load(f)
-
-    doc = Document.from_dict(data, '')
```

### Comparing `pycognaize-1.4.3/pycognaize/document/field/__init__.py` & `pycognaize-1.4.6/pycognaize/document/field/__init__.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/field/area_field.py` & `pycognaize-1.4.6/pycognaize/document/field/area_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/field/date_field.py` & `pycognaize-1.4.6/pycognaize/document/field/date_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/field/field.py` & `pycognaize-1.4.6/pycognaize/document/field/field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/field/link_field.py` & `pycognaize-1.4.6/pycognaize/document/field/link_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 | The latter can have no tags, a single tag or multiple tags.
 
 >>> from pycognaize.document.field.link_field import LinkField
 >>> link_field = LinkField(name='URL', value='https://LinkField')
 >>> link_field.name
 'URL'
 >>> link_field.value
-'https://LinkField'
+'LinkField'
 >>> link_field.tags
 []
 """
 import logging
 from typing import List, Optional, Dict, Type
 
 from pycognaize.common.classification_labels import ClassificationLabels
```

### Comparing `pycognaize-1.4.3/pycognaize/document/field/numeric_field.py` & `pycognaize-1.4.6/pycognaize/document/field/numeric_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/field/section_field.py` & `pycognaize-1.4.6/pycognaize/document/field/section_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/field/span_field.py` & `pycognaize-1.4.6/pycognaize/document/field/span_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/field/table_field.py` & `pycognaize-1.4.6/pycognaize/document/field/table_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/field/text_field.py` & `pycognaize-1.4.6/pycognaize/document/field/text_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/html_info.py` & `pycognaize-1.4.6/pycognaize/document/html_info.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/page.py` & `pycognaize-1.4.6/pycognaize/document/page.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/snapshot.py` & `pycognaize-1.4.6/pycognaize/document/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/tag/cell.py` & `pycognaize-1.4.6/pycognaize/document/tag/cell.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/tag/extraction_tag.py` & `pycognaize-1.4.6/pycognaize/document/tag/extraction_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/tag/html_tag.py` & `pycognaize-1.4.6/pycognaize/document/tag/html_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
-from typing import Optional, List, Union
-
 import bson
 import pandas as pd
+import logging
 
+from typing import Optional, List, Union
 from pycognaize.common.enums import (IqRecipeEnum, XBRLCellEnum,
                                      XBRLTableTagEnum, XBRLTagEnum, ID)
 from pycognaize.document.html_info import HTML
 from pycognaize.document.tag.tag import Tag
 
 
 class HTMLTagABC(Tag, metaclass=abc.ABCMeta):
@@ -203,14 +203,38 @@
                                                xpath=cell_.xpath,
                                                raw_value=cell_.raw_value,
                                                raw_ocr_value=cell_.raw_value,
                                                field_id='',
                                                tag_id=self.tag_id,
                                                row_index=row_index,
                                                col_index=col_index)
+        df = self.replace_nans_with_empty_html_tags(df)
+        return df
+
+    def replace_nans_with_empty_html_tags(self,
+                                          df: pd.DataFrame) -> pd.DataFrame:
+        """
+            Replaces NaN values in a DataFrame with empty HTML tags.
+        """
+        for col in df.columns:
+            for idx in df.index:
+                if pd.isna(df.loc[idx, col]):
+                    logging.warning(
+                        f'Build df issue: Replacing empty cell at {idx, col} '
+                        f'with empty HTMLTag in HTMLTableTag with html id '
+                        f'{self.html_id}')
+                    df.loc[idx, col] = HTMLTag(is_table=False,
+                                               html_id='',
+                                               xpath='',
+                                               raw_value='',
+                                               raw_ocr_value='',
+                                               field_id='',
+                                               tag_id='',
+                                               row_index=idx,
+                                               col_index=col)
         return df
 
 
 class HTMLCell:
     """Represents cell tag for XBRL tables"""
     def __init__(self, row_index: int, col_index: int,
                  col_span: int, row_span: int,
```

### Comparing `pycognaize-1.4.3/pycognaize/document/tag/section_tag.py` & `pycognaize-1.4.6/pycognaize/document/tag/section_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/tag/span_tag.py` & `pycognaize-1.4.6/pycognaize/document/tag/span_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/tag/table_tag.py` & `pycognaize-1.4.6/pycognaize/document/tag/table_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/document/tag/tag.py` & `pycognaize-1.4.6/pycognaize/document/tag/tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/index.py` & `pycognaize-1.4.6/pycognaize/index.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/login.py` & `pycognaize-1.4.6/pycognaize/login.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """This module provides login functionality for downloading snapshots"""
 import os
+
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util import Retry
 
 from pycognaize.common.enums import EnvConfigEnum
 from pycognaize.common.exceptions import ServerAPIException
 
@@ -12,14 +13,16 @@
     """Allows to access the AWS S3 bucket using cognaize credentials"""
     INSTANCE = None
     _access_key = ''
     _secret_access_key = ''
     _session_token = ''
     _snapshot_root = ''
     _logged_in = False
+    _email = ''
+    _password = ''
 
     def __new__(cls) -> 'Login':
         if cls.INSTANCE is None:
             cls.INSTANCE = super().__new__(cls)
         return cls.INSTANCE
 
     @property
@@ -75,33 +78,38 @@
                                                   json=authentication,
                                                   timeout=10)
         except requests.exceptions.ConnectionError:
             raise ServerAPIException(f'Failed connecting to url: {url}')
         except requests.exceptions.Timeout:
             raise ServerAPIException(f'Connection timed out: {url}')
 
-        print(user_credentials_response)
         user_credentials = user_credentials_response.json()
         if user_credentials_response.status_code == 200:
             self._logged_in = True
             self._access_key = user_credentials['credentials']['AccessKeyId']
             self._secret_access_key = \
                 user_credentials['credentials']['SecretAccessKey']
             self._session_token = \
                 user_credentials['credentials']['SessionToken']
             self._snapshot_root = user_credentials['snapshotRoot']
+
+            self._email = email
+            self._password = password
         elif user_credentials_response.status_code == 403:
             raise ServerAPIException("Data download permission error. "
                                      "Please make sure you have access"
                                      " to Snapshots")
         elif user_credentials_response.status_code == 401:
             raise ServerAPIException("Wrong email or password. "
                                      "Please make sure you entered the "
                                      "correct credentials")
         else:
             raise ServerAPIException("Server error. There was a problem "
                                      "with the serve")
 
+    def relogin(self):
+        self.login(self._email, self._password)
+
     @classmethod
     def destroy(cls) -> None:
         """Delete singleton"""
         cls.INSTANCE = None
```

### Comparing `pycognaize-1.4.3/pycognaize/model.py` & `pycognaize-1.4.6/pycognaize/model.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/model_registry/db/models.py` & `pycognaize-1.4.6/pycognaize/model_registry/db/models.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/model_registry/login.py` & `pycognaize-1.4.6/pycognaize/model_registry/login.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize/model_registry/submit.py` & `pycognaize-1.4.6/pycognaize/model_registry/submit.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.4.3/pycognaize.egg-info/PKG-INFO` & `pycognaize-1.4.6/pycognaize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycognaize
-Version: 1.4.3
+Version: 1.4.6
 Home-page: https://github.com/cognaize/pycognaize
 Author: Cognaize
 License: Apache License 2.0
 Project-URL: Source, https://github.com/cognaize/pycognaize
 Project-URL: Reference, https://pycognaize.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/cognaize/pycognaize/blob/master/CHANGELOG.md
 Requires-Python: >= 3.7
@@ -45,16 +45,25 @@
 Have a look at the [quick tutorial](http://pycognaize-docs.com.s3-website.us-east-2.amazonaws.com/tutorials/quick_tutorial.html) 
 for understanding main concepts of the SDK.
 
 # Changelog
 
 ## [1.4]
 
+### [1.4.6] - 2023-06-15
+- Add replace_nans_with_empty_html_tags functionality in HTMLTableTag build df
+
+### [1.4.5] - 2023-06-12
+- Add relogin when AWS token is expired
+
+### [1.4.4] - 2023-05-31
+- Add `anytree` to setup-requires in `setup.cfg`
+
 ### [1.4.3] - 2023-05-31
-- Fix handling of section field with no tagsc
+- Fix handling of section field with no tags
 
 ### [1.4.2] - 2023-05-30
 - Fix handling of section field value when field does not have tags
 
 ### [1.4.1] - 2023-05-29
 - Add section field and section tag functionality
```

### Comparing `pycognaize-1.4.3/pycognaize.egg-info/SOURCES.txt` & `pycognaize-1.4.6/pycognaize.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 pycognaize.egg-info/SOURCES.txt
 pycognaize.egg-info/dependency_links.txt
 pycognaize.egg-info/entry_points.txt
 pycognaize.egg-info/requires.txt
 pycognaize.egg-info/top_level.txt
 pycognaize/common/__init__.py
 pycognaize/common/classification_labels.py
+pycognaize/common/cloud_service.py
 pycognaize/common/confidence.py
 pycognaize/common/decorators.py
 pycognaize/common/enums.py
 pycognaize/common/exceptions.py
 pycognaize/common/field_collection.py
 pycognaize/common/lazy_dict.py
 pycognaize/common/lazy_group_dict.py
```

### Comparing `pycognaize-1.4.3/setup.cfg` & `pycognaize-1.4.6/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 	pymupdf==1.21.1
 	urllib3
 	lxml
 	beautifulsoup4
 	dataclasses; python_version <= '3.6'
 	PyYAML
 	click
+	anytree
 
 [options.packages.find]
 exclude = 
 	pycognaize.temp.*
 	pycognaize.temp
 	pycognaize.tests.*
 	pycognaize.tests
```

### Comparing `pycognaize-1.4.3/setup.py` & `pycognaize-1.4.6/setup.py`

 * *Files identical despite different names*

