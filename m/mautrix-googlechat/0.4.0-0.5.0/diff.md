# Comparing `tmp/mautrix-googlechat-0.4.0.tar.gz` & `tmp/mautrix-googlechat-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mautrix-googlechat-0.4.0.tar", last modified: Tue Nov 15 21:59:31 2022, max compression
+gzip compressed data, was "mautrix-googlechat-0.5.0.tar", last modified: Fri Jun 16 13:05:57 2023, max compression
```

## Comparing `mautrix-googlechat-0.4.0.tar` & `mautrix-googlechat-0.5.0.tar`

### file list

```diff
@@ -1,70 +1,75 @@
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-11-15 21:59:31.332002 mautrix-googlechat-0.4.0/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3665 2022-11-15 15:17:00.000000 mautrix-googlechat-0.4.0/CHANGELOG.md
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    34523 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/LICENSE
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      114 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/MANIFEST.in
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2387 2022-11-15 21:59:31.332002 mautrix-googlechat-0.4.0/PKG-INFO
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1420 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/README.md
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-11-15 21:59:31.324002 mautrix-googlechat-0.4.0/maugclib/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      412 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/maugclib/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     8345 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/maugclib/auth.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    17355 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/maugclib/channel.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    28372 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/maugclib/client.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1798 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/maugclib/event.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      405 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/maugclib/exceptions.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)   877885 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/maugclib/googlechat_pb2.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     7629 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/maugclib/http_utils.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1632 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/maugclib/parsers.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-11-15 21:59:31.328002 mautrix-googlechat-0.4.0/mautrix_googlechat/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       70 2022-11-15 15:16:56.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4159 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/__main__.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-11-15 21:59:31.328002 mautrix-googlechat-0.4.0/mautrix_googlechat/commands/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       24 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/commands/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4744 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/commands/auth.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      284 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/commands/typehint.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3636 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/config.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-11-15 21:59:31.328002 mautrix-googlechat-0.4.0/mautrix_googlechat/db/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      421 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/db/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4823 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/db/message.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4273 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/db/portal.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4125 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/db/puppet.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3541 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/db/reaction.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-11-15 21:59:31.328002 mautrix-googlechat-0.4.0/mautrix_googlechat/db/upgrade/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      174 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/db/upgrade/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3832 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/db/upgrade/v00_latest_revision.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2289 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/db/upgrade/v02_reactions.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1178 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/db/upgrade/v03_store_gc_revision.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1022 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/db/upgrade/v04_store_photo_hash.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3279 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/db/user.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    12955 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/example-config.yaml
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-11-15 21:59:31.328002 mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      152 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     8616 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/from_googlechat.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-11-15 21:59:31.328002 mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/from_matrix/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1640 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/from_matrix/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6250 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/from_matrix/gc_message.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4294 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/from_matrix/parser.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     7615 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/gc_url_preview.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      496 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/util.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1714 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/get_version.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6093 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/matrix.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    60038 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/portal.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    10847 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/puppet.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    23179 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/user.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-11-15 21:59:31.332002 mautrix-googlechat-0.4.0/mautrix_googlechat/util/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/util/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1144 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/util/color_log.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      177 2022-11-15 21:59:31.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/version.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-11-15 21:59:31.332002 mautrix-googlechat-0.4.0/mautrix_googlechat/web/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       39 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/web/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     7689 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/mautrix_googlechat/web/auth.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2022-11-15 21:59:31.328002 mautrix-googlechat-0.4.0/mautrix_googlechat.egg-info/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2387 2022-11-15 21:59:31.000000 mautrix-googlechat-0.4.0/mautrix_googlechat.egg-info/PKG-INFO
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1847 2022-11-15 21:59:31.000000 mautrix-googlechat-0.4.0/mautrix_googlechat.egg-info/SOURCES.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)        1 2022-11-15 21:59:31.000000 mautrix-googlechat-0.4.0/mautrix_googlechat.egg-info/dependency_links.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      406 2022-11-15 21:59:31.000000 mautrix-googlechat-0.4.0/mautrix_googlechat.egg-info/requires.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       28 2022-11-15 21:59:31.000000 mautrix-googlechat-0.4.0/mautrix_googlechat.egg-info/top_level.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      279 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/optional-requirements.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      286 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/pyproject.toml
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      154 2022-11-15 15:16:42.000000 mautrix-googlechat-0.4.0/requirements.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2022-11-15 21:59:31.332002 mautrix-googlechat-0.4.0/setup.cfg
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2283 2022-11-07 15:02:58.000000 mautrix-googlechat-0.4.0/setup.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-06-16 13:05:57.419540 mautrix-googlechat-0.5.0/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4157 2023-06-16 12:55:57.000000 mautrix-googlechat-0.5.0/CHANGELOG.md
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    34523 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/LICENSE
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      114 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/MANIFEST.in
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2350 2023-06-16 13:05:57.419540 mautrix-googlechat-0.5.0/PKG-INFO
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1420 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/README.md
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-06-16 13:05:57.415540 mautrix-googlechat-0.5.0/maugclib/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      560 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/maugclib/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    18836 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/maugclib/channel.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    30874 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/maugclib/client.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1798 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/maugclib/event.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2056 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/maugclib/exceptions.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)   114334 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/maugclib/googlechat_pb2.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     8799 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/maugclib/http_utils.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1632 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/maugclib/parsers.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6744 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/maugclib/pblite.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-06-16 13:05:57.415540 mautrix-googlechat-0.5.0/mautrix_googlechat/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       70 2023-06-16 12:55:57.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4188 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/__main__.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-06-16 13:05:57.415540 mautrix-googlechat-0.5.0/mautrix_googlechat/commands/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       19 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/commands/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3696 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/commands/auth.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      284 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/commands/typehint.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3800 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/config.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-06-16 13:05:57.415540 mautrix-googlechat-0.5.0/mautrix_googlechat/db/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      421 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4823 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/message.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4623 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/portal.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4060 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/puppet.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3541 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/reaction.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-06-16 13:05:57.419540 mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      328 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4043 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/v00_latest_revision.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2289 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/v02_reactions.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1178 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/v03_store_gc_revision.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1022 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/v04_store_photo_hash.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1120 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/v05_rename_thread_columns.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1145 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/v06_space_description.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1093 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/v07_puppet_contact_info_set.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1123 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/v08_web_app_auth.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1030 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/v09_web_app_ua.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3652 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/db/user.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    14437 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/example-config.yaml
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-06-16 13:05:57.419540 mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      152 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     8616 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/from_googlechat.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-06-16 13:05:57.419540 mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/from_matrix/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1640 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/from_matrix/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6519 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/from_matrix/gc_message.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4294 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/from_matrix/parser.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     7615 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/gc_url_preview.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      496 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/util.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1714 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/get_version.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6093 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/matrix.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    66873 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/portal.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    11905 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/puppet.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    27615 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/user.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-06-16 13:05:57.419540 mautrix-googlechat-0.5.0/mautrix_googlechat/util/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/util/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1144 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/util/color_log.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      177 2023-06-16 13:05:57.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/version.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-06-16 13:05:57.419540 mautrix-googlechat-0.5.0/mautrix_googlechat/web/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       39 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/web/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6800 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/mautrix_googlechat/web/auth.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2023-06-16 13:05:57.415540 mautrix-googlechat-0.5.0/mautrix_googlechat.egg-info/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2350 2023-06-16 13:05:57.000000 mautrix-googlechat-0.5.0/mautrix_googlechat.egg-info/PKG-INFO
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2122 2023-06-16 13:05:57.000000 mautrix-googlechat-0.5.0/mautrix_googlechat.egg-info/SOURCES.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        1 2023-06-16 13:05:57.000000 mautrix-googlechat-0.5.0/mautrix_googlechat.egg-info/dependency_links.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      403 2023-06-16 13:05:57.000000 mautrix-googlechat-0.5.0/mautrix_googlechat.egg-info/requires.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       28 2023-06-16 13:05:57.000000 mautrix-googlechat-0.5.0/mautrix_googlechat.egg-info/top_level.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      279 2023-06-15 09:43:17.000000 mautrix-googlechat-0.5.0/optional-requirements.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      286 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/pyproject.toml
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      151 2023-06-16 12:55:56.000000 mautrix-googlechat-0.5.0/requirements.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       38 2023-06-16 13:05:57.419540 mautrix-googlechat-0.5.0/setup.cfg
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2283 2023-05-14 10:31:37.000000 mautrix-googlechat-0.5.0/setup.py
```

### Comparing `mautrix-googlechat-0.4.0/CHANGELOG.md` & `mautrix-googlechat-0.5.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# v0.5.0 (2023-06-16)
+
+* Switched to web app API to make authentication work again.
+  **This will require all users to relogin.**
+* Allowed thread bridging in non-thread-only chats.
+* Improved handling of getting logged out remotely.
+* Added options to automatically ratchet/delete megolm sessions to minimize
+  access to old messages.
+* Added option to not set room name/avatar even in encrypted rooms.
+* Implemented appservice pinging using MSC2659.
+* Updated Docker image to Alpine 3.18.
+
 # v0.4.0 (2022-11-15)
 
 * Added support for bridging room mentions in both directions.
 * Updated formatter to insert Matrix displayname into mentions when bridging
   from Google Chat. This ensures that the Matrix user gets mentioned correctly.
 * Fixed images from Google Chat not being bridged with full resolution.
 * Added SQLite support (thanks to [@durin42] in [#74]).
```

### Comparing `mautrix-googlechat-0.4.0/LICENSE` & `mautrix-googlechat-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/PKG-INFO` & `mautrix-googlechat-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mautrix-googlechat
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Matrix-Google Chat puppeting bridge.
 Home-page: https://github.com/mautrix/googlechat
 Author: Tulir Asokan
 Author-email: tulir@maunium.net
-License: UNKNOWN
 Project-URL: Changelog, https://github.com/mautrix/googlechat/blob/master/CHANGELOG.md
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Communications :: Chat
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -46,9 +44,7 @@
 
 ### Features & Roadmap
 [ROADMAP.md](https://github.com/mautrix/googlechat/blob/master/ROADMAP.md)
 contains a general overview of what is supported by the bridge.
 
 ## Discussion
 Matrix room: [`#googlechat:maunium.net`](https://matrix.to/#/#googlechat:maunium.net)
-
-
```

### Comparing `mautrix-googlechat-0.4.0/README.md` & `mautrix-googlechat-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/maugclib/channel.py` & `mautrix-googlechat-0.5.0/maugclib/channel.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,28 +18,30 @@
 
 from typing import Iterator, NoReturn
 import asyncio
 import base64
 import codecs
 import json
 import logging
+import random
 import re
 import time
 
 import aiohttp
 import async_timeout
 
 from mautrix.util.opt_prometheus import Counter
 
-from . import event, exceptions, googlechat_pb2, http_utils
+from . import event, exceptions, googlechat_pb2, http_utils, pblite
+from .exceptions import SIDExpiringError, SIDInvalidError
 
 logger = logging.getLogger(__name__)
 Utf8IncrementalDecoder = codecs.getincrementaldecoder("utf-8")
 LEN_REGEX = re.compile(r"([0-9]+)\n", re.MULTILINE)
-CHANNEL_URL_BASE = "https://chat.google.com/webchannel/"
+CHANNEL_URL_BASE = "https://chat.google.com/u/0/webchannel/"
 # Long-polling requests send heartbeats every 15-30 seconds, so if we miss two
 # in a row, consider the connection dead.
 PUSH_TIMEOUT = 60
 MAX_READ_BYTES = 1024 * 1024
 
 LONG_POLLING_REQUESTS = Counter(
     name="bridge_gc_started_long_polls",
@@ -52,18 +54,14 @@
 )
 RECEIVED_CHUNKS = Counter(
     name="bridge_gc_received_chunk_bytes",
     documentation="Received chunks from Google Chat long polling",
 )
 
 
-class ChannelSessionError(exceptions.HangupsError):
-    """hangups channel session error"""
-
-
 def _best_effort_decode(data_bytes):
     """Decode as much of data_bytes as possible as UTF-8."""
     decoder = Utf8IncrementalDecoder()
     return decoder.decode(data_bytes)
 
 
 class ChunkParser:
@@ -93,15 +91,14 @@
 
         Note that when encoding a string in UTF-16, Python will prepend a
         byte-order character, so we need to remove the first two bytes.
         """
         self._buf += new_data_bytes
 
         while True:
-
             buf_decoded = _best_effort_decode(self._buf)
             buf_utf16 = buf_decoded.encode("utf-16")[2:]
 
             length_str_match = LEN_REGEX.match(buf_decoded)
             if length_str_match is None:
                 break
             else:
@@ -133,14 +130,29 @@
     Returns SID
     """
     res = json.loads(res)
     sid = res[0][1][1]
     return sid
 
 
+def _unique_id() -> str:
+    def base36(x) -> str:
+        keyspace = "abcdefghijklmnopqrstuvwxyz0123456789"
+
+        encoded = 0
+        quotient = x
+        while quotient != 0:
+            quotient, remainder = divmod(quotient, len(keyspace))
+            encoded = keyspace[remainder] + str(encoded)
+
+        return encoded
+
+    return base36(random.getrandbits(64))
+
+
 class Channel:
     """BrowserChannel client."""
 
     ##########################################################################
     # Public methods
     ##########################################################################
 
@@ -179,15 +191,15 @@
 
         # Discovered parameters:
         self._sid_param = None
         self._csessionid_param = None
 
         self._aid = 0
         self._ofs = 0  # used to track sent events
-        self._rid = 0
+        self._rid = random.randint(10000, 99999)
 
     @property
     def is_connected(self):
         """Whether the channel is currently connected."""
         return self._is_connected
 
     async def listen(self, max_age: float) -> None:
@@ -214,15 +226,15 @@
             skip_backoff = False
 
             # Clear any previous push data, since if there was an error it
             # could contain garbage.
             self._chunk_parser = ChunkParser()
             try:
                 await self._longpoll_request()
-            except ChannelSessionError as err:
+            except SIDExpiringError as err:
                 logger.debug("Long-polling interrupted: %s", err)
 
                 self._csessionid_param = await self._register()
 
                 retries += 1
                 skip_backoff = True
                 continue
@@ -242,84 +254,89 @@
 
             # If the request ended with an error, the client must account for
             # messages being dropped during this time.
 
         logger.error("Ran out of retries for long-polling request")
 
     async def _register(self) -> str | None:
-        # we need to clear our cookies because registering with a valid cookie
-        # invalidates our cookie and doesn't get a new one sent back.
-        self._session.clear_cookies()
+        # Previously we had to clear the cookies as it would cause issues, but
+        # the uri has a query parameter to ignore the COMPASS/dynamite cookie.
         self._sid_param = None
         self._aid = 0
         self._ofs = 0
 
+        # required cookies: COMPASS, SSID, SID, OSID, HSID,
+        # new cookies after login: SIDCC
+
         headers = {"Content-Type": "application/x-protobuf"}
-        res = await self._session.fetch_raw("POST", CHANNEL_URL_BASE + "register", headers=headers)
+        res = await self._session.fetch_raw(
+            "GET", CHANNEL_URL_BASE + "register?ignore_compass_cookie=1", headers=headers
+        )
+
+        body = await res.read()
 
         if res.status != 200:
-            raise exceptions.NetworkError(
-                f"Request return unexpected status: {res.status}: {res.reason}"
+            logger.info(
+                "Register request HTTP %d %s response body: %s", res.status, res.reason, body
+            )
+            raise exceptions.UnexpectedStatusError(
+                f"Register request",
+                res.status,
+                res.reason,
+                body,
             )
-
-        body = await res.read()
 
         morsel = self._session.get_cookie(CHANNEL_URL_BASE, "COMPASS")
         logger.debug("Cookies: %s", self._session._cookie_jar._cookies)
         logger.debug("Register response: %s", body)
         logger.debug("Status: %s", res.status)
         logger.debug("Headers: %s", res.headers)
         if morsel is not None:
-            if morsel.value.startswith("dynamite="):
+            if morsel.value.startswith("dynamite-ui="):
                 logger.info("Registered new channel successfully")
-                return morsel.value[len("dynamite=") :]
+                return morsel.value[len("dynamite-ui=") :]
             else:
                 logger.warning(
-                    "COMPASS cookie doesn't start with dynamite= (value: %s)", morsel.value
+                    "COMPASS cookie doesn't start with dynamite-ui= (value: %s)", morsel.value
                 )
         return None
 
     async def send_stream_event(self, events_request: googlechat_pb2.StreamEventsRequest):
         params = {
             "VER": 8,  # channel protocol version
             "RID": self._rid,  # request identifier
             "t": 1,  # trial
             "SID": self._sid_param,  # session ID
             "AID": self._aid,  # last acknowledged id
-            "CI": 0,  # 0 if streaming/chunked requests should be used
+            # No longer required with the web ui
+            # "CI": 0,  # 0 if streaming/chunked requests should be used
         }
 
         self._rid += 1
 
-        if self._csessionid_param is not None:
-            params["csessionid"] = self._csessionid_param
+        # This doesn't appear to be used at all anymore.
+        # if self._csessionid_param is not None:
+        #     params["csessionid"] = self._csessionid_param
 
         headers = {
             "Content-Type": "application/x-www-form-urlencoded",
         }
 
-        # base64 the raw protobuf
-        b64_bytes = base64.b64encode(events_request.SerializeToString())
-
-        json_body = json.dumps(
-            {
-                "data": b64_bytes.decode("ascii"),
-            }
-        )
-
+        body = pblite.encode(events_request)
+        json_body = json.dumps(body)
         data = {
             "count": 1,
             "ofs": self._ofs,
-            "req0___data__": json_body,
+            "req0_data": json_body,
         }
         self._ofs += 1
 
         res = await self._session.fetch_raw(
             "POST",
-            CHANNEL_URL_BASE + "events_encoded",
+            CHANNEL_URL_BASE + "events",
             headers=headers,
             params=params,
             data=data,
         )
 
         return res
 
@@ -348,97 +365,116 @@
         This method uses keep-alive to make re-opening the request faster, but
         the remote server will set the "Connection: close" header once an hour.
 
         Raises hangups.NetworkError or ChannelSessionError.
         """
         params = {
             "VER": 8,  # channel protocol version
-            "CVER": 22,  # client type
-            "AID": self._aid,
-            "t": 1,  # trial
+            "RID": self._rid,
+            "SID": self._sid_param,
+            "t": 1,  # trial, sometimes seen as 2
+            "zx": _unique_id(),
         }
 
-        self._rid += 1
-
         if self._sid_param is None:
             params.update(
                 {
-                    "$req": "count=0",  # noop request
-                    "RID": "0",
+                    "CVER": 22,
+                    "$req": "count=1&ofs=0&req0_data=%5B%5D",
                     "SID": "null",
-                    "TYPE": "init",  # type of request
                 }
             )
+
+            self._rid += 1
         else:
-            params.update(
-                {
-                    "CI": 0,
-                    "RID": "rpc",
-                    "SID": self._sid_param,
-                    "TYPE": "xmlhttp",
-                }
-            )
+            params.update({"CI": 0, "TYPE": "xmlhttp", "RID": "rpc", "AID": self._aid})
+
+        headers = {
+            "referer": "https://chat.google.com/",
+        }
 
         logger.debug("Opening new long-polling request")
         LONG_POLLING_REQUESTS.inc()
         try:
             res: aiohttp.ClientResponse
             async with self._session.fetch_raw_ctx(
-                "GET", CHANNEL_URL_BASE + "events_encoded", params=params
+                "GET", CHANNEL_URL_BASE + "events", params=params, headers=headers
             ) as res:
                 if res.status != 200:
+                    text = await res.text()
+                    logger.info(
+                        "Long poll HTTP %d %s response body: %s", res.status, res.reason, text
+                    )
+                    LONG_POLLING_ERRORS.labels(reason=f"http {res.status}").inc()
                     if res.status == 400:
-                        text = await res.text()
-                        logger.info("400 %s response text: %s", res.reason, text)
                         if res.reason == "Unknown SID" or "Unknown SID" in text:
                             LONG_POLLING_ERRORS.labels(reason="sid invalid").inc()
-                            raise ChannelSessionError("SID became invalid")
-                    LONG_POLLING_ERRORS.labels(reason=f"http {res.status}").inc()
-                    raise exceptions.NetworkError(
-                        f"Request returned unexpected status: {res.status}: {res.reason}"
+                            raise SIDInvalidError()
+                    raise exceptions.UnexpectedStatusError(
+                        f"Long poll request",
+                        res.status,
+                        res.reason,
+                        text,
                     )
 
                 initial_response = res.headers.get("X-HTTP-Initial-Response", None)
                 if initial_response:
                     sid = _parse_sid_response(initial_response)
                     if self._sid_param != sid:
                         self._sid_param = sid
                         self._aid = 0
                         self._ofs = 0
 
+                        # Tell the server we got the sid. I'm not sure what else
+                        # this could be, but it does seem to be required.
+                        params = {
+                            "VER": 8,
+                            "RID": "rpc",
+                            "SID": self._sid_param,
+                            "AID": self._aid,
+                            "CI": 0,
+                            "TYPE": "xmlhttp",
+                            "zx": _unique_id(),
+                            "t": 1,
+                        }
+
+                        await self._session.fetch_raw(
+                            "GET", CHANNEL_URL_BASE + "events", params=params
+                        )
+
+                        # Finally send the initial ping
                         await self._send_initial_ping()
 
                 while True:
                     async with async_timeout.timeout(PUSH_TIMEOUT):
                         chunk = await res.content.read(MAX_READ_BYTES)
                     if not chunk:
                         break
 
                     await self._on_push_data(chunk)
 
         except asyncio.TimeoutError:
             LONG_POLLING_ERRORS.labels(reason="timeout").inc()
-            raise exceptions.NetworkError("Request timed out")
+            raise exceptions.NetworkError("Long poll request timed out")
         except aiohttp.ServerDisconnectedError as err:
             LONG_POLLING_ERRORS.labels(reason="server disconnected").inc()
             raise exceptions.NetworkError(f"Server disconnected error: {err}")
         except aiohttp.ClientPayloadError:
             LONG_POLLING_ERRORS.labels(reason="sid expiry").inc()
-            raise ChannelSessionError("SID is about to expire")
+            raise SIDExpiringError()
         except aiohttp.ClientError as err:
             LONG_POLLING_ERRORS.labels(reason="connection error").inc()
-            raise exceptions.NetworkError(f"Request connection error: {err}")
+            raise exceptions.NetworkError(f"Long poll request connection error: {err}")
         LONG_POLLING_ERRORS.labels(reason="clean exit").inc()
 
     async def _on_push_data(self, data_bytes: bytes) -> None:
         """Parse push data and trigger events."""
         logger.debug("Received chunk:\n{}".format(data_bytes))
         RECEIVED_CHUNKS.inc(len(data_bytes))
         for chunk in self._chunk_parser.get_chunks(data_bytes):
-
             # Consider the channel connected once the first chunk is received.
             if not self._is_connected:
                 if self._on_connect_called:
                     self._is_connected = True
                     await self.on_reconnect.fire()
                 else:
                     self._on_connect_called = True
```

### Comparing `mautrix-googlechat-0.4.0/maugclib/client.py` & `mautrix-googlechat-0.5.0/maugclib/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,68 @@
 """Abstract class for writing chat clients."""
 
 from __future__ import annotations
 
 from typing import Iterator
+from urllib.parse import urlencode
 import asyncio
 import base64
 import binascii
 import cgi
 import datetime
+import json
 import logging
 import os
 import random
+import re
 
 from google.protobuf import message as proto
 from yarl import URL
 import aiohttp
 
-from . import auth, channel, event, exceptions, googlechat_pb2, http_utils, parsers
+from . import channel, event, exceptions, googlechat_pb2, http_utils, parsers, pblite
 
 logger = logging.getLogger(__name__)
 dl_log = logger.getChild("download")
 UPLOAD_URL = "https://chat.google.com/uploads"
 # API key for `key` parameter (from Hangouts web client)
 API_KEY = "AIzaSyD7InnYR3VKdb4j2rMUEbTCIr2VyEazl6k"
 # Base URL for API requests:
-GC_BASE_URL = "https://chat.google.com"
+GC_BASE_URL = "https://chat.google.com/u/0"
+
+
+wiz_pattern = re.compile(r">window.WIZ_global_data = ({.+?});</script>")
 
 
 class Client:
     """Instant messaging client for Google Chat.
 
     Maintains a connections to the servers, emits events, and accepts commands.
 
     Args:
-        token_manager: (auth.TokenManager): The token manager.
+        cookies: (http_utils.Cookies): The cookies.
         max_retries (int): (optional) Maximum number of connection attempts
             hangups will make before giving up. Defaults to 5.
         retry_backoff_base (int): (optional) The base term for the exponential
             backoff. The following equation is used when calculating the number
             of seconds to wait prior to each retry:
             retry_backoff_base^(# of retries attempted thus far)
             Defaults to 2.
     """
 
     _session: http_utils.Session | None
     _channel: channel.Channel | None
     _listen_future: asyncio.Future | None
 
     def __init__(
-        self, token_manager: auth.TokenManager, max_retries: int = 5, retry_backoff_base: int = 2
+        self,
+        cookies: http_utils.Cookies,
+        user_agent: str | None = None,
+        max_retries: int = 5,
+        retry_backoff_base: int = 2,
     ) -> None:
         self._max_retries = max_retries
         self._retry_backoff_base = retry_backoff_base
 
         self.on_connect = event.Event("Client.on_connect")
         """
         :class:`.Event` fired when the client connects for the first time.
@@ -73,24 +83,26 @@
         """
         :class:`.Event` fired when an update arrives from the server.
 
         Args:
             state_update: A ``StateUpdate`` message.
         """
 
-        self._session = http_utils.Session(token_manager, proxy=os.environ.get("HTTP_PROXY"))
+        self._session = http_utils.Session(
+            cookies, user_agent=user_agent, proxy=os.environ.get("HTTP_PROXY")
+        )
 
         # channel.Channel instance (populated by .connect()):
         self._channel = None
 
         # Future for Channel.listen (populated by .connect()):
         self._listen_future = None
 
         self.gc_request_header = googlechat_pb2.RequestHeader(
-            client_type=googlechat_pb2.RequestHeader.ClientType.IOS,
+            client_type=googlechat_pb2.RequestHeader.ClientType.WEB,
             client_version=2440378181258,
             client_feature_capabilities=googlechat_pb2.ClientFeatureCapabilities(
                 spam_room_invites_level=googlechat_pb2.ClientFeatureCapabilities.FULLY_SUPPORTED,
             ),
         )
 
         # String identifying this client (populated later):
@@ -101,14 +113,27 @@
 
         # Active client management parameters:
         # Time in seconds that the client as last set as active:
         self._last_active_secs = 0.0
         # ActiveClientState enum int value or None:
         self._active_client_state = None
 
+        # requests to /u/0/api have a query parameter named `c` that appears to
+        # be an incrementing counter. It seems to ignore duplicates, but we
+        # keep it around to not stand out.
+        self._api_reqid = 0
+
+        # These are values that need to be acquired from the server via the
+        # check_login() method.
+        self.xsrf_token = None
+
+    @property
+    def cookies(self) -> http_utils.Cookies:
+        return self._session.get_auth_cookies()
+
     ##########################################################################
     # Public methods
     ##########################################################################
 
     async def connect(self, max_age: float) -> None:
         """Establish a connection to the chat server.
 
@@ -439,38 +464,78 @@
                 request_header=self.gc_request_header,
                 state=googlechat_pb2.TYPING if typing else googlechat_pb2.STOPPED,
                 context=context,
             )
         )
         return resp.start_timestamp_usec
 
+    async def refresh_tokens(self):
+        """Makes a request to /mole/world to get some magic values. Right now
+        this is just the xsrf token for api requests, but it could be more
+        at some point. Also if we ever need to go back to the batchexecute
+        api, all of the required values are in this response as well.
+        """
+
+        qs = {
+            "origin": "https://mail.google.com",
+            "shell": "9",
+            "hl": "en",
+            "wfi": "gtn-roster-iframe-id",
+            # TODO: some of these values are passed in via redirect during
+            # login and should probably be used instead of hard coding.
+            "hs": '["h_hs",null,null,[1,0],null,null,"gmail.pinto-server_20230515.06_p0",1,null,[36,35,26,18,24,11,15,14,6],null,null,"3Mu86PSulM4.en..es5",0,null,null,[2]]',
+        }
+        headers = {
+            "authority": "chat.google.com",
+            "refer": "https://mail.google.com/",
+        }
+
+        url = f"{GC_BASE_URL}/mole/world?{urlencode(qs)}"
+
+        res = await self._session.fetch(
+            "GET",
+            url,
+            headers=headers,
+        )
+
+        body = res.body.decode("utf-8")
+        wiz_match = wiz_pattern.search(body)
+        if not wiz_match:
+            raise Exception("Didn't find WIZ_global_data in /mole/world response")
+        try:
+            wiz_data = json.loads(wiz_match.group(1))
+        except json.JSONDecodeError as e:
+            raise Exception("Non-JSON WIZ_global_data in /mole/world response") from e
+        if wiz_data["qwAQke"] == "AccountsSignInUi":
+            raise exceptions.NotLoggedInError("Provided tokens aren't valid")
+        self.xsrf_token = wiz_data["SMqcke"]
+
     ##########################################################################
     # Private methods
     ##########################################################################
 
     async def _on_receive_array(self, array: list) -> None:
         """Parse channel array and call the appropriate events."""
         if array[0] == "noop":
             pass  # This is just a keep-alive, ignore it.
         else:
-            if "data" in array[0]:
-                data = array[0]["data"]
+            data = array[0]
 
-                resp = googlechat_pb2.StreamEventsResponse()
-                resp.ParseFromString(base64.b64decode(data))
+            resp = googlechat_pb2.StreamEventsResponse()
+            pblite.decode(resp, data)
 
-                # An event can have multiple bodies embedded in it. However,
-                # instead of pushing all bodies in the same place, there first
-                # one is a separate field. So to simplify handling, we muck
-                # around with the class by swapping the embedded bodies into
-                # the top level body field and fire the event like it was the
-                # toplevel body.
-                for evt in self.split_event_bodies(resp.event):
-                    logger.debug("Dispatching stream event: %s", evt)
-                    await self.on_stream_event.fire(evt)
+            # An event can have multiple bodies embedded in it. However,
+            # instead of pushing all bodies in the same place, there first
+            # one is a separate field. So to simplify handling, we muck
+            # around with the class by swapping the embedded bodies into
+            # the top level body field and fire the event like it was the
+            # toplevel body.
+            for evt in self.split_event_bodies(resp.event):
+                logger.debug("Dispatching stream event: %s", evt)
+                await self.on_stream_event.fire(evt)
 
     @staticmethod
     def split_event_bodies(evt: googlechat_pb2.Event) -> Iterator[googlechat_pb2.Event]:
         embedded_bodies = evt.bodies
         if len(embedded_bodies) > 0:
             evt.ClearField("bodies")
 
@@ -494,20 +559,27 @@
             endpoint (str): The chat API endpoint to use.
             request_pb: The request body as a Protocol Buffer message.
             response_pb: The response body as a Protocol Buffer message.
 
         Raises:
             NetworkError: If the request fails.
         """
+
+        headers = {}
+        if self.xsrf_token is not None:
+            headers["x-framework-xsrf-token"] = self.xsrf_token
+
         logger.debug("Sending Protocol Buffer request %s:\n%s", endpoint, request_pb)
+        self._api_reqid += 1
         res = await self._base_request(
-            "{}/api/{}?rt=b".format(GC_BASE_URL, endpoint),
+            "{}/api/{}?c={}&rt=b".format(GC_BASE_URL, endpoint, self._api_reqid),
             "application/x-protobuf",  # Request body is Protocol Buffer.
             "proto",  # Response body is Protocol Buffer.
             request_pb.SerializeToString(),
+            headers=headers,
         )
         try:
             response_pb.ParseFromString(res.body)
         except proto.DecodeError as e:
             raise exceptions.NetworkError(
                 "Failed to decode Protocol Buffer response: {}".format(e)
             )
@@ -611,14 +683,15 @@
     ) -> googlechat_pb2.GetSelfUserStatusResponse:
         """Return info about the current user.
 
         Replace get_self_info.
         """
         response = googlechat_pb2.GetSelfUserStatusResponse()
         await self._gc_request("get_self_user_status", get_self_user_status_request, response)
+
         return response
 
     async def proto_get_group(
         self, get_group_request: googlechat_pb2.GetGroupRequest
     ) -> googlechat_pb2.GetGroupResponse:
         """Looks up a group chat"""
         response = googlechat_pb2.GetGroupResponse()
```

### Comparing `mautrix-googlechat-0.4.0/maugclib/event.py` & `mautrix-googlechat-0.5.0/maugclib/event.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/maugclib/http_utils.py` & `mautrix-googlechat-0.5.0/maugclib/http_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,105 @@
 """HTTP request session."""
 from __future__ import annotations
 
-from typing import Any, AsyncIterator, cast
+from typing import Any, AsyncIterator, NamedTuple, cast
 from contextlib import asynccontextmanager
-from http.cookies import Morsel
+from http.cookies import Morsel, SimpleCookie
 import asyncio
-import collections
 import logging
+import re
 
 from yarl import URL
 import aiohttp
 import async_timeout
 
 from . import exceptions
-from .auth import USER_AGENT, TokenManager
 
 logger = logging.getLogger(__name__)
 CONNECT_TIMEOUT = 30
 REQUEST_TIMEOUT = 30
 MAX_RETRIES = 3
 ORIGIN_URL = "https://chat.google.com"
 
-FetchResponse = collections.namedtuple("FetchResponse", ["code", "headers", "body"])
+LATEST_CHROME_VERSION = "114"
+LATEST_FIREFOX_VERSION = "114"
+DEFAULT_USER_AGENT = (
+    f"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) "
+    f"Chrome/{LATEST_CHROME_VERSION}.0.0.0 Safari/537.36"
+)
+chrome_version_regex = re.compile(r"Chrome/\d+\.\d+\.\d+\.\d+")
+firefox_version_regex = re.compile(r"Firefox/\d+.\d+")
+
+
+class FetchResponse(NamedTuple):
+    code: int
+    headers: dict[str, str]
+    body: bytes
+
+
+class Cookies(NamedTuple):
+    compass: str
+    ssid: str
+    sid: str
+    osid: str
+    hsid: str
+
+
+chat_google_com = URL("https://chat.google.com/")
 
 
 class Session:
     """Session for making HTTP requests to Google.
 
     Args:
         cookies (dict): Cookies to authenticate requests with.
         proxy (str): (optional) HTTP proxy URL to use for requests.
     """
 
-    def __init__(self, token_manager: TokenManager, proxy: str = None) -> None:
+    def __init__(self, cookies: Cookies, proxy: str = None, user_agent: str = None) -> None:
         self._proxy = proxy
+
         # The server does not support quoting cookie values (see #498).
         self._cookie_jar = aiohttp.CookieJar(quote_cookie=False)
+        cookie = SimpleCookie()
+        for key, value in cookies._asdict().items():
+            cookie[key.upper()] = value
+            cookie[key.upper()].update({"domain": "chat.google.com", "path": "/"})
+        self._cookie_jar.update_cookies(cookie, chat_google_com)
+
+        if user_agent:
+            user_agent = chrome_version_regex.sub(
+                f"Chrome/{LATEST_CHROME_VERSION}.0.0.0", user_agent
+            )
+            user_agent = firefox_version_regex.sub(
+                f"Firefox/{LATEST_FIREFOX_VERSION}.0", user_agent
+            )
+        else:
+            user_agent = DEFAULT_USER_AGENT
+
         timeout = aiohttp.ClientTimeout(connect=CONNECT_TIMEOUT)
         self._session = aiohttp.ClientSession(
             cookie_jar=self._cookie_jar,
             timeout=timeout,
             trust_env=True,
-            headers={"User-Agent": USER_AGENT},
+            headers={"User-Agent": user_agent},
         )
 
-        self._token_manager = token_manager
+    def get_auth_cookies(self) -> Cookies:
+        vals = {}
+        cookie = self._cookie_jar.filter_cookies(chat_google_com)
+        for field in Cookies._fields:
+            vals[field] = cookie[field.upper()].value
+        return Cookies(**vals)
 
     def get_cookie(self, url: URL | str, name: str) -> Morsel[str]:
         filtered = self._cookie_jar.filter_cookies(url)
 
         return cast(Morsel, filtered.get(name, None))
 
-    def clear_cookies(self) -> None:
-        self._session.cookie_jar.clear()
-
     async def fetch(
         self,
         method: str,
         url: URL | str,
         params: dict[str, str] | None = None,
         headers: dict[str, str] | None = None,
         allow_redirects: bool = True,
@@ -201,15 +243,14 @@
     ):
         # Ensure we don't accidentally send the authorization header to a
         # non-Google domain:
         if not URL(url).host.endswith(".google.com"):
             raise Exception("expected google.com domain")
 
         headers = headers or {}
-        headers["Authorization"] = f"Bearer {await self._token_manager.get()}"
         headers["Connection"] = "Keep-Alive"
         return self._session.request(
             method,
             url,
             params=params,
             headers=headers,
             allow_redirects=allow_redirects,
```

### Comparing `mautrix-googlechat-0.4.0/maugclib/parsers.py` & `mautrix-googlechat-0.5.0/maugclib/parsers.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/__main__.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from .version import linkified_version, version
 from .web import GoogleChatAuthServer
 
 
 class GoogleChatBridge(Bridge):
     name = "mautrix-googlechat"
     module = "mautrix_googlechat"
+    beeper_service_name = "googlechat"
+    beeper_network_name = "googlechat"
     command = "python -m mautrix-googlechat"
     description = "A Matrix-Google Chat puppeting bridge."
     repo_url = "https://github.com/mautrix/googlechat"
     version = version
     markdown_version = linkified_version
     config_class = Config
     matrix_class = MatrixHandler
@@ -51,15 +53,14 @@
         super().prepare_db()
         init_db(self.db)
 
     def prepare_bridge(self) -> None:
         super().prepare_bridge()
         self.auth_server = GoogleChatAuthServer(
             self.config["bridge.provisioning.shared_secret"],
-            self.config["hangouts.device_name"],
         )
         self.az.app.add_subapp("/login", self.auth_server.legacy_app)
         self.az.app.add_subapp(self.config["bridge.provisioning.prefix"], self.auth_server.app)
 
     async def resend_bridge_info(self) -> None:
         self.config["bridge.resend_bridge_info"] = False
         self.config.save()
```

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/config.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mautrix-googlechat - A Matrix-Google Chat puppeting bridge
-# Copyright (C) 2022 Tulir Asokan
+# Copyright (C) 2023 Tulir Asokan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -21,16 +21,14 @@
 
 class Config(BaseBridgeConfig):
     def do_update(self, helper: ConfigUpdateHelper) -> None:
         super().do_update(helper)
 
         copy, copy_dict, base = helper
 
-        copy("hangouts.device_name")
-
         copy("metrics.enabled")
         copy("metrics.listen_port")
 
         copy("bridge.username_template")
         copy("bridge.displayname_template")
         copy("bridge.command_prefix")
 
@@ -57,14 +55,17 @@
         copy("bridge.backfill.initial_nonthread_limit")
         copy("bridge.backfill.missed_event_limit")
         copy("bridge.backfill.missed_event_page_size")
         copy("bridge.backfill.disable_notifications")
         copy("bridge.resend_bridge_info")
         copy("bridge.unimportant_bridge_notices")
         copy("bridge.disable_bridge_notices")
+        copy("bridge.private_chat_portal_meta")
+        if base["bridge.private_chat_portal_meta"] not in ("default", "always", "never"):
+            base["bridge.private_chat_portal_meta"] = "default"
 
         copy("bridge.provisioning.prefix")
         if "bridge.web.auth.shared_secret" in self:
             base["bridge.provisioning.shared_secret"] = self["bridge.web.auth.shared_secret"]
         if self["bridge.provisioning.shared_secret"] == "generate":
             base["bridge.provisioning.shared_secret"] = self._new_token()
         else:
```

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/db/message.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/db/message.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/db/portal.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/db/portal.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,29 +32,32 @@
 
     gcid: str
     gc_receiver: str
     other_user_id: str | None
     mxid: RoomID | None
     name: str | None
     avatar_mxc: ContentURI | None
+    description: str | None
     name_set: bool
     avatar_set: bool
+    description_set: bool
     encrypted: bool
     revision: int | None
-    is_threaded: bool | None
+    threads_only: bool | None
+    threads_enabled: bool | None
 
     @classmethod
     def _from_row(cls, row: Record | None) -> Portal | None:
         if row is None:
             return None
         return cls(**row)
 
     columns = (
-        "gcid, gc_receiver, other_user_id, mxid, name, avatar_mxc, "
-        "name_set, avatar_set, encrypted, revision, is_threaded"
+        "gcid, gc_receiver, other_user_id, mxid, name, avatar_mxc, description, "
+        "name_set, avatar_set, description_set, encrypted, revision, threads_only, threads_enabled"
     )
 
     @classmethod
     async def get_by_gcid(cls, gcid: str, gc_receiver: str) -> Portal | None:
         q = f"SELECT {cls.columns} FROM portal WHERE gcid=$1 AND gc_receiver=$2"
         row = await cls.db.fetchrow(q, gcid, gc_receiver)
         return cls._from_row(row)
@@ -82,39 +85,47 @@
         return (
             self.gcid,
             self.gc_receiver,
             self.other_user_id,
             self.mxid,
             self.name,
             self.avatar_mxc,
+            self.description,
             self.name_set,
             self.avatar_set,
+            self.description_set,
             self.encrypted,
             self.revision,
-            self.is_threaded,
+            self.threads_only,
+            self.threads_enabled,
         )
 
     async def insert(self) -> None:
-        q = (
-            "INSERT INTO portal (gcid, gc_receiver, other_user_id, mxid, name, avatar_mxc, "
-            "                    name_set, avatar_set, encrypted, revision, is_threaded) "
-            "VALUES ($1, $2, $3, $4, $5, $6, $7, $8, $9, $10, $11)"
+        q = """
+        INSERT INTO portal (
+            gcid, gc_receiver, other_user_id, mxid, name, avatar_mxc, description,
+            name_set, avatar_set, description_set, encrypted,
+            revision, threads_only, threads_enabled
         )
+        VALUES ($1, $2, $3, $4, $5, $6, $7, $8, $9, $10, $11, $12, $13, $14)
+        """
         await self.db.execute(q, *self._values)
 
     async def delete(self) -> None:
         q = "DELETE FROM portal WHERE gcid=$1 AND gc_receiver=$2"
         await self.db.execute(q, self.gcid, self.gc_receiver)
 
     async def save(self) -> None:
-        q = (
-            "UPDATE portal SET other_user_id=$3, mxid=$4, name=$5, avatar_mxc=$6, name_set=$7, "
-            "                  avatar_set=$8, encrypted=$9, revision=$10, is_threaded=$11 "
-            "WHERE gcid=$1 AND gc_receiver=$2"
-        )
+        q = """
+        UPDATE portal
+        SET other_user_id=$3, mxid=$4, name=$5, avatar_mxc=$6, description=$7,
+            name_set=$8, avatar_set=$9, description_set=$10, encrypted=$11,
+            revision=$12, threads_only=$13, threads_enabled=$14
+        WHERE gcid=$1 AND gc_receiver=$2
+        """
         await self.db.execute(q, *self._values)
 
     async def set_revision(self, revision: int) -> None:
         if self.revision and self.revision >= revision > 0:
             return
         self.revision = revision
         q = (
```

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/db/puppet.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/db/puppet.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     gcid: str
     name: str | None
     photo_id: str | None
     photo_mxc: ContentURI | None
     photo_hash: str | None
     name_set: bool
     avatar_set: bool
+    contact_info_set: bool
     is_registered: bool
 
     custom_mxid: UserID | None
     access_token: str | None
     next_batch: SyncToken | None
     base_url: URL | None
 
@@ -50,15 +51,15 @@
         if row is None:
             return None
         data = {**row}
         base_url = data.pop("base_url", None)
         return cls(**data, base_url=URL(base_url) if base_url else None)
 
     columns = (
-        "gcid, name, photo_id, photo_mxc, name_set, avatar_set, is_registered, "
+        "gcid, name, photo_id, photo_mxc, name_set, avatar_set, contact_info_set, is_registered, "
         "custom_mxid, access_token, next_batch, base_url, photo_hash"
     )
 
     @classmethod
     async def get_by_gcid(cls, gcid: str) -> Puppet | None:
         q = f"SELECT {cls.columns} FROM puppet WHERE gcid=$1"
         row = await cls.db.fetchrow(q, gcid)
@@ -87,35 +88,36 @@
         return (
             self.gcid,
             self.name,
             self.photo_id,
             self.photo_mxc,
             self.name_set,
             self.avatar_set,
+            self.contact_info_set,
             self.is_registered,
             self.custom_mxid,
             self.access_token,
             self.next_batch,
             str(self.base_url) if self.base_url else None,
             self.photo_hash,
         )
 
     async def insert(self) -> None:
-        q = (
-            "INSERT INTO puppet (gcid, name, photo_id, photo_mxc, name_set, avatar_set, "
-            "                    is_registered, custom_mxid, access_token, next_batch, base_url, photo_hash) "
-            "VALUES ($1, $2, $3, $4, $5, $6, $7, $8, $9, $10, $11, $12)"
-        )
+        q = f"""
+            INSERT INTO puppet ({self.columns})
+            VALUES ($1, $2, $3, $4, $5, $6, $7, $8, $9, $10, $11, $12, $13)
+        """
         await self.db.execute(q, *self._values)
 
     async def delete(self) -> None:
         q = "DELETE FROM puppet WHERE gcid=$1"
         await self.db.execute(q, self.gcid)
 
     async def save(self) -> None:
-        q = (
-            "UPDATE puppet SET name=$2, photo_id=$3, photo_mxc=$4, name_set=$5, avatar_set=$6, "
-            "                  is_registered=$7, custom_mxid=$8, access_token=$9, next_batch=$10,"
-            "                  base_url=$11, photo_hash=$12 "
-            "WHERE gcid=$1"
-        )
+        q = """
+            UPDATE puppet
+            SET name=$2, photo_id=$3, photo_mxc=$4, name_set=$5, avatar_set=$6,
+                contact_info_set=$7, is_registered=$8, custom_mxid=$9, access_token=$10,
+                next_batch=$11, base_url=$12, photo_hash=$13
+            WHERE gcid=$1
+        """
         await self.db.execute(q, *self._values)
```

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/db/reaction.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/db/reaction.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/db/upgrade/v00_latest_revision.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/v00_latest_revision.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,38 +14,42 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from mautrix.util.async_db import Connection
 
 from . import upgrade_table
 
 
-@upgrade_table.register(description="Latest revision", upgrades_to=4)
+@upgrade_table.register(description="Latest revision", upgrades_to=9)
 async def upgrade_latest(conn: Connection) -> None:
     await conn.execute(
         """CREATE TABLE "user" (
-            mxid          TEXT PRIMARY KEY,
-            gcid          TEXT UNIQUE,
-            refresh_token TEXT,
-            notice_room   TEXT,
-            revision      BIGINT
+            mxid        TEXT PRIMARY KEY,
+            gcid        TEXT UNIQUE,
+            cookies     TEXT,
+            user_agent  TEXT,
+            notice_room TEXT,
+            revision    BIGINT
         )"""
     )
     await conn.execute(
         """CREATE TABLE portal (
             gcid          TEXT,
             gc_receiver   TEXT,
             other_user_id TEXT,
             mxid          TEXT UNIQUE,
             name          TEXT,
             avatar_mxc    TEXT,
+            description   TEXT,
             name_set      BOOLEAN NOT NULL DEFAULT false,
             avatar_set    BOOLEAN NOT NULL DEFAULT false,
+            description_set BOOLEAN NOT NULL DEFAULT false,
             encrypted     BOOLEAN NOT NULL DEFAULT false,
             revision      BIGINT,
-            is_threaded   BOOLEAN,
+            threads_only  BOOLEAN,
+            threads_enabled BOOLEAN,
             PRIMARY KEY (gcid, gc_receiver)
         )"""
     )
     await conn.execute(
         """CREATE TABLE puppet (
             gcid       TEXT PRIMARY KEY,
             name       TEXT,
@@ -53,14 +57,16 @@
             photo_mxc  TEXT,
             photo_hash TEXT,
 
             name_set      BOOLEAN NOT NULL DEFAULT false,
             avatar_set    BOOLEAN NOT NULL DEFAULT false,
             is_registered BOOLEAN NOT NULL DEFAULT false,
 
+            contact_info_set BOOLEAN NOT NULL DEFAULT false,
+
             custom_mxid  TEXT,
             access_token TEXT,
             next_batch   TEXT,
             base_url     TEXT
         )"""
     )
     await conn.execute(
```

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/db/upgrade/v02_reactions.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/v02_reactions.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/db/upgrade/v03_store_gc_revision.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/v03_store_gc_revision.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/db/upgrade/v04_store_photo_hash.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/db/upgrade/v04_store_photo_hash.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/db/user.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/db/user.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mautrix-googlechat - A Matrix-Google Chat puppeting bridge
-# Copyright (C) 2022 Tulir Asokan
+# Copyright (C) 2023 Tulir Asokan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,84 +12,95 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, ClassVar
+import json
 
 from asyncpg import Record
 from attr import dataclass
 
+from maugclib import Cookies
 from mautrix.types import RoomID, UserID
 from mautrix.util.async_db import Database
 
 fake_db = Database.create("") if TYPE_CHECKING else None
 
 
 @dataclass
 class User:
     db: ClassVar[Database] = fake_db
 
     mxid: UserID
     gcid: str | None
-    refresh_token: str | None
+    cookies: Cookies | None
+    user_agent: str | None
     notice_room: RoomID | None
     revision: int | None
 
     @classmethod
     def _from_row(cls, row: Record | None) -> User | None:
         if row is None:
             return None
-        return cls(**row)
+        data = {**row}
+        cookies_raw = data.pop("cookies")
+        cookies = Cookies(**json.loads(cookies_raw)) if cookies_raw else None
+        return cls(**data, cookies=cookies)
 
     @classmethod
     async def all_logged_in(cls) -> list[User]:
         q = (
-            'SELECT mxid, gcid, refresh_token, notice_room, revision FROM "user" '
-            "WHERE refresh_token IS NOT NULL"
+            'SELECT mxid, gcid, cookies, user_agent, notice_room, revision FROM "user" '
+            "WHERE cookies IS NOT NULL"
         )
         rows = await cls.db.fetch(q)
         return [cls._from_row(row) for row in rows]
 
     @classmethod
     async def get_by_gcid(cls, gcid: str) -> User | None:
-        q = 'SELECT mxid, gcid, refresh_token, notice_room, revision FROM "user" WHERE gcid=$1'
+        q = """
+        SELECT mxid, gcid, cookies, user_agent, notice_room, revision FROM "user" WHERE gcid=$1
+        """
         row = await cls.db.fetchrow(q, gcid)
         return cls._from_row(row)
 
     @classmethod
     async def get_by_mxid(cls, mxid: UserID) -> User | None:
-        q = 'SELECT mxid, gcid, refresh_token, notice_room, revision FROM "user" WHERE mxid=$1'
+        q = """
+        SELECT mxid, gcid, cookies, user_agent, notice_room, revision FROM "user" WHERE mxid=$1
+        """
         row = await cls.db.fetchrow(q, mxid)
         return cls._from_row(row)
 
     @property
     def _values(self):
         return (
             self.mxid,
             self.gcid,
-            self.refresh_token,
+            json.dumps(self.cookies._asdict()) if self.cookies else None,
+            self.user_agent,
             self.notice_room,
             self.revision,
         )
 
     async def insert(self) -> None:
         q = (
-            'INSERT INTO "user" (mxid, gcid, refresh_token, notice_room, revision) '
-            "VALUES ($1, $2, $3, $4, $5)"
+            'INSERT INTO "user" (mxid, gcid, cookies, user_agent, notice_room, revision) '
+            "VALUES ($1, $2, $3, $4, $5, $6)"
         )
         await self.db.execute(q, *self._values)
 
     async def delete(self) -> None:
         await self.db.execute('DELETE FROM "user" WHERE mxid=$1', self.mxid)
 
     async def save(self) -> None:
         q = (
-            'UPDATE "user" SET gcid=$2, refresh_token=$3, notice_room=$4, revision=$5 '
+            'UPDATE "user" SET gcid=$2, cookies=$3, user_agent=$4, notice_room=$5, revision=$6 '
             "WHERE mxid=$1"
         )
         await self.db.execute(q, *self._values)
 
     async def set_revision(self, revision: int) -> None:
         if self.revision and self.revision >= revision > 0:
             return
```

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/example-config.yaml` & `mautrix-googlechat-0.5.0/mautrix_googlechat/example-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     verify_ssl: true
     # What software is the homeserver running?
     # Standard Matrix homeservers like Synapse, Dendrite and Conduit should just use "standard" here.
     software: standard
     # Number of retries for all HTTP requests if the homeserver isn't reachable.
     http_retry_count: 4
     # The URL to push real-time bridge status to.
-    # If set, the bridge will make POST requests to this URL whenever a user's Google caht connection state changes.
+    # If set, the bridge will make POST requests to this URL whenever a user's Google Chat connection state changes.
     # The bridge will use the appservice as_token to authorize requests.
     status_endpoint: null
     # Endpoint for reporting per-message status.
     message_send_checkpoint_endpoint: null
     # Whether asynchronous uploads via MSC2246 should be enabled for media.
     # Requires a media repo that supports MSC2246.
     async_media: false
@@ -33,15 +33,15 @@
     port: 29320
     # The maximum body size of appservice API requests (from the homeserver) in mebibytes
     # Usually 1 is enough, but on high-traffic bridges you might need to increase this to avoid 413s
     max_body_size: 1
 
     # The full URI to the database. SQLite and Postgres are supported.
     # Format examples:
-    #   SQLite:   sqlite:///filename.db
+    #   SQLite:   sqlite:filename.db
     #   Postgres: postgres://username:password@hostname/dbname
     database: postgres://username:password@hostname/db
     # Additional arguments for asyncpg.create_pool() or sqlite3.connect()
     # https://magicstack.github.io/asyncpg/current/api/index.html#asyncpg.pool.create_pool
     # https://docs.python.org/3/library/sqlite3.html#sqlite3.connect
     # For sqlite, min_size is used as the connection thread pool size and max_size is ignored.
     # Additionally, SQLite supports init_commands as an array of SQL queries to run on connect (e.g. to set PRAGMAs).
@@ -63,19 +63,14 @@
     # You should disable bridge -> sync_with_custom_puppets when this is enabled.
     ephemeral_events: true
 
     # Authentication tokens for AS <-> HS communication. Autogenerated; do not modify.
     as_token: "This value is generated when generating the registration"
     hs_token: "This value is generated when generating the registration"
 
-hangouts:
-    # Device name shown in Google account settings
-    # (probably doesn't actually work anymore)
-    device_name: Mautrix-Google Chat bridge
-
 # Prometheus telemetry config. Requires prometheus-client to be installed.
 metrics:
     enabled: false
     listen_port: 8000
 
 # Manhole config.
 manhole:
@@ -141,14 +136,31 @@
         # Whether to use MSC2409/MSC3202 instead of /sync long polling for receiving encryption-related data.
         appservice: false
         # Require encryption, drop any unencrypted messages.
         require: false
         # Enable key sharing? If enabled, key requests for rooms where users are in will be fulfilled.
         # You must use a client that supports requesting keys from other users to use this feature.
         allow_key_sharing: false
+        # Options for deleting megolm sessions from the bridge.
+        delete_keys:
+            # Beeper-specific: delete outbound sessions when hungryserv confirms
+            # that the user has uploaded the key to key backup.
+            delete_outbound_on_ack: false
+            # Don't store outbound sessions in the inbound table.
+            dont_store_outbound: false
+            # Ratchet megolm sessions forward after decrypting messages.
+            ratchet_on_decrypt: false
+            # Delete fully used keys (index >= max_messages) after decrypting messages.
+            delete_fully_used_on_decrypt: false
+            # Delete previous megolm sessions from same device when receiving a new one.
+            delete_prev_on_new_session: false
+            # Delete megolm sessions received from a device when the device is deleted.
+            delete_on_device_delete: false
+            # Periodically delete megolm sessions when 2x max_age has passed since receiving the session.
+            periodically_delete_expired: false
         # What level of device verification should be required from users?
         #
         # Valid levels:
         #   unverified - Send keys to all device in the room.
         #   cross-signed-untrusted - Require valid cross-signing, but trust all cross-signing keys.
         #   cross-signed-tofu - Require valid cross-signing, trust cross-signing keys on first use (and reject changes).
         #   cross-signed-verified - Require valid cross-signing, plus a valid user signature from the bridge bot.
@@ -176,14 +188,18 @@
             # as the default.
             milliseconds: 604800000
             # The maximum number of messages that should be sent with a given a
             # session before changing it. The Matrix spec recommends 100 as the
             # default.
             messages: 100
 
+            # Disable rotating keys when a user's devices change?
+            # You should not enable this option unless you understand all the implications.
+            disable_device_change_key_rotation: false
+
     # Whether or not the bridge should send a read receipt from the bridge bot when a message has
     # been sent to Google Chat.
     delivery_receipts: false
     # Whether or not delivery errors should be reported as messages in the Matrix room.
     delivery_error_reports: true
     # Whether the bridge should send the message status as a custom com.beeper.message_send_status event.
     message_status_events: false
@@ -214,14 +230,19 @@
     # This field will automatically be changed back to false after it,
     # except if the config file is not writable.
     resend_bridge_info: false
     # Whether or not unimportant bridge notices should be sent to the bridge notice room.
     unimportant_bridge_notices: false
     # Whether or not bridge notices should be disabled entirely.
     disable_bridge_notices: false
+    # Whether to explicitly set the avatar and room name for private chat portal rooms.
+    # If set to `default`, this will be enabled in encrypted rooms and disabled in unencrypted rooms.
+    # If set to `always`, all DM rooms will have explicit names and avatars set.
+    # If set to `never`, DM rooms will never have names and avatars set.
+    private_chat_portal_meta: default
 
     provisioning:
         # Internal prefix in the appservice web server for the login endpoints.
         prefix: /_matrix/provision
         # Shared secret for integration managers such as mautrix-manager.
         # If set to "generate", a random string will be generated on the next startup.
         # If null, integration manager access to the API will not be possible.
```

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/from_googlechat.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/from_googlechat.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/from_matrix/__init__.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/from_matrix/__init__.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/from_matrix/gc_message.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/from_matrix/gc_message.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,7 +158,14 @@
     @property
     def googlechat_entities(self) -> List[googlechat.Annotation]:
         return [
             entity.internal
             for entity in self.entities
             if entity.internal.type != googlechat.ANNOTATION_TYPE_UNKNOWN
         ]
+
+    def format(
+        self, entity_type: GCEntityType, offset: int = None, length: int = None, **kwargs
+    ) -> EntityString:
+        if entity_type == GCEntityType.EMAIL:
+            return self
+        return super().format(entity_type, offset, length, **kwargs)
```

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/from_matrix/parser.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/from_matrix/parser.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/formatter/gc_url_preview.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/formatter/gc_url_preview.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/get_version.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/get_version.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/matrix.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/matrix.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/portal.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/portal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mautrix-googlechat - A Matrix-Google Chat puppeting bridge
-# Copyright (C) 2022 Tulir Asokan
+# Copyright (C) 2023 Tulir Asokan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -11,32 +11,31 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, AsyncIterable, NamedTuple, Union, cast
+from typing import TYPE_CHECKING, Any, AsyncIterable, Literal, NamedTuple, Union, cast
 from collections import deque
 import asyncio
 import mimetypes
 import random
 import time
 
 from yarl import URL
 import aiohttp
 
 from maugclib import FileTooLargeError, googlechat_pb2 as googlechat
 from mautrix.appservice import IntentAPI
 from mautrix.bridge import BasePortal, NotificationDisabler, async_getter_lock
-from mautrix.errors import IntentError, MatrixError, MForbidden
+from mautrix.errors import MatrixError, MForbidden
 from mautrix.types import (
     BeeperMessageStatusEventContent,
     ContentURI,
-    EncryptionAlgorithm,
     EventID,
     EventType,
     ImageInfo,
     MediaMessageEventContent,
     Membership,
     MessageEventContent,
     MessageStatus,
@@ -45,15 +44,15 @@
     PowerLevelStateEventContent,
     RelatesTo,
     RelationType,
     RoomID,
     TextMessageEventContent,
     UserID,
 )
-from mautrix.util import magic, variation_selector
+from mautrix.util import background_task, magic, variation_selector
 from mautrix.util.message_send_checkpoint import MessageSendCheckpointStatus
 from mautrix.util.opt_prometheus import Histogram
 from mautrix.util.simple_lock import SimpleLock
 import maugclib.parsers
 
 from . import formatter as fmt, matrix as m, puppet as p, user as u
 from .config import Config
@@ -93,14 +92,15 @@
 
 class Portal(DBPortal, BasePortal):
     invite_own_puppet_to_pm: bool = False
     by_mxid: dict[RoomID, Portal] = {}
     by_gcid: dict[tuple[str, str], Portal] = {}
     matrix: m.MatrixHandler
     config: Config
+    private_chat_portal_meta: Literal["default", "always", "never"]
 
     _main_intent: IntentAPI | None
     _create_room_lock: asyncio.Lock
     _last_bridged_mxid: EventID | None
     _dedup: deque[str]
     _local_dedup: set[str]
     _send_locks: dict[str, asyncio.Lock]
@@ -115,32 +115,38 @@
         self,
         gcid: str,
         gc_receiver: str,
         other_user_id: str | None = None,
         mxid: RoomID | None = None,
         name: str | None = None,
         avatar_mxc: ContentURI | None = None,
+        description: str | None = None,
         name_set: bool = False,
         avatar_set: bool = False,
+        description_set: bool = False,
         encrypted: bool = False,
         revision: int | None = None,
-        is_threaded: bool | None = None,
+        threads_only: bool | None = None,
+        threads_enabled: bool | None = None,
     ) -> None:
         super().__init__(
             gcid=gcid,
             gc_receiver=gc_receiver,
             other_user_id=other_user_id,
             mxid=mxid,
             name=name,
             avatar_mxc=avatar_mxc,
+            description=description,
             name_set=name_set,
             avatar_set=avatar_set,
+            description_set=description_set,
             encrypted=encrypted,
             revision=revision,
-            is_threaded=is_threaded,
+            threads_only=threads_only,
+            threads_enabled=threads_enabled,
         )
         self.log = self.log.getChild(self.gcid_log)
 
         self._main_intent = None
         self._create_room_lock = asyncio.Lock()
         self._incoming_events = asyncio.Queue()
         self._event_dispatcher_task = None
@@ -158,14 +164,15 @@
     def init_cls(cls, bridge: "GoogleChatBridge") -> None:
         BasePortal.bridge = bridge
         cls.az = bridge.az
         cls.config = bridge.config
         cls.loop = bridge.loop
         cls.matrix = bridge.matrix
         cls.invite_own_puppet_to_pm = cls.config["bridge.invite_own_puppet_to_pm"]
+        cls.private_chat_portal_meta = cls.config["bridge.private_chat_portal_meta"]
         NotificationDisabler.puppet_cls = p.Puppet
         NotificationDisabler.config_enabled = cls.config["bridge.backfill.disable_notifications"]
 
     # region Properties
 
     @property
     def gcid_full(self) -> tuple[str, str]:
@@ -191,14 +198,26 @@
         return self.is_dm and bool(self.other_user_id)
 
     @property
     def is_dm(self) -> bool:
         return self.gcid.startswith("dm:")
 
     @property
+    def is_space(self) -> bool:
+        return self.gcid.startswith("space:")
+
+    @property
+    def set_dm_room_metadata(self) -> bool:
+        return (
+            not self.is_direct
+            or self.private_chat_portal_meta == "always"
+            or (self.encrypted and self.private_chat_portal_meta != "never")
+        )
+
+    @property
     def main_intent(self) -> IntentAPI:
         if not self._main_intent:
             raise ValueError("Portal must be postinit()ed before main_intent can be used")
         return self._main_intent
 
     # endregion
     # region DB conversion
@@ -207,14 +226,15 @@
         if self.mxid:
             await DBMessage.delete_all_by_room(self.mxid)
             await DBReaction.delete_all_by_room(self.mxid)
         self.by_mxid.pop(self.mxid, None)
         self.mxid = None
         self.name_set = False
         self.avatar_set = False
+        self.description_set = False
         await super().save()
 
     # endregion
     # region Chat info updating
 
     async def get_dm_puppet(self) -> p.Puppet | None:
         if not self.is_direct:
@@ -226,41 +246,81 @@
     ) -> ChatInfo:
         if not info or (not self.is_dm and isinstance(info, googlechat.WorldItemLite)):
             info = await source.get_group(
                 self.gcid, (info.group_revision.timestamp if info else self.revision)
             )
 
         changed = False
-        is_threaded = (
-            info if isinstance(info, googlechat.WorldItemLite) else info.group
-        ).HasField("threaded_group")
-        if is_threaded != self.is_threaded:
-            self.is_threaded = is_threaded
+        if isinstance(info, googlechat.WorldItemLite):
+            group_meta = info
+            description = group_meta.group_lite.group_details.description
+        elif isinstance(info, googlechat.GetGroupResponse):
+            group_meta = info.group
+            description = group_meta.group_details.description
+        else:
+            raise RuntimeError(f"Unexpected group metadata type {type(info)} in update_info()")
+        threads_only = group_meta.HasField("threaded_group")
+        if threads_only != self.threads_only:
+            self.threads_only = threads_only
+            changed = True
+        threads_enabled = bool(group_meta.flat_threads_enabled or threads_only)
+        if threads_enabled != self.threads_enabled:
+            self.log.debug(
+                f"{self.gcid}/{self.name} changed threads_enabled "
+                f"from {self.threads_enabled} to {threads_enabled}"
+            )
+            self.threads_enabled = threads_enabled
             changed = True
         changed = await self._update_participants(source, info) or changed
-        changed = await self._update_name(info) or changed
+        changed = await self._update_description(description) or changed
+        changed = await self._update_name_from_info(info) or changed
         if changed:
             await self.save()
             await self.update_bridge_info()
         return info
 
-    async def _update_name(self, info: ChatInfo) -> bool:
+    async def _update_name_from_info(self, info: ChatInfo) -> bool:
         if self.is_direct:
             puppet = await self.get_dm_puppet()
             name = puppet.name
         elif isinstance(info, googlechat.WorldItemLite) and info.HasField("room_name"):
             name = info.room_name
         elif isinstance(info, googlechat.GetGroupResponse) and info.group.HasField("name"):
             name = info.group.name
         else:
             return False
-        if self.name != name:
+        return await self._update_name_direct(name)
+
+    async def _update_name_direct(self, name: str, timestamp: int | None = None) -> bool:
+        if self.name != name or (not self.name_set and self.mxid and self.set_dm_room_metadata):
             self.name = name
-            if self.mxid and (self.encrypted or not self.is_direct):
-                await self.main_intent.set_room_name(self.mxid, self.name)
+            self.name_set = False
+            if self.mxid and self.set_dm_room_metadata:
+                try:
+                    await self.main_intent.set_room_name(self.mxid, self.name, timestamp=timestamp)
+                    self.name_set = True
+                except Exception:
+                    self.log.exception("Failed to update room name")
+            return True
+        return False
+
+    async def _update_description(self, description: str, timestamp: int | None = None) -> bool:
+        if (self.description or "") != description or (
+            not self.description_set and self.mxid and not self.is_direct
+        ):
+            self.description = description
+            self.description_set = False
+            if self.mxid:
+                try:
+                    await self.main_intent.set_room_topic(
+                        self.mxid, self.description, timestamp=timestamp
+                    )
+                    self.description_set = True
+                except Exception:
+                    self.log.exception("Failed to update room topic")
             return True
         return False
 
     def _get_invite_content(self, double_puppet: p.Puppet | None) -> dict[str, Any]:
         invite_content = {}
         if double_puppet:
             invite_content["fi.mau.will_auto_accept"] = True
@@ -290,19 +350,35 @@
             user_ids.remove(source.gcid)
         if self.is_dm and len(user_ids) == 1 and not self.other_user_id:
             self.other_user_id = user_ids[0]
             self._main_intent = (await self.get_dm_puppet()).default_mxid_intent
             await self.save()
         if not self.mxid and not self.is_direct:
             return
+        extra_members = await self.main_intent.get_joined_members(self.mxid) if self.mxid else {}
         users = await source.get_users(user_ids + bots)
-        await asyncio.gather(*[self._update_participant(source, user) for user in users])
+        tasks = []
+        for user in users:
+            puppet: p.Puppet = await p.Puppet.get_by_gcid(user.user_id.id)
+            tasks.append(asyncio.create_task(self._update_participant(source, puppet, user)))
+            extra_members.pop(puppet.intent_for(self).mxid, None)
+        await asyncio.gather(*tasks)
+        for member in extra_members:
+            puppet: p.Puppet = await p.Puppet.get_by_mxid(member)
+            if puppet:
+                try:
+                    await puppet.default_mxid_intent.leave_room(
+                        self.mxid, reason="User is not in group"
+                    )
+                except Exception:
+                    self.log.exception("Failed to leave extra ghost user from room")
 
-    async def _update_participant(self, source: u.User, user: googlechat.User) -> None:
-        puppet: p.Puppet = await p.Puppet.get_by_gcid(user.user_id.id)
+    async def _update_participant(
+        self, source: u.User, puppet: p.Puppet, user: googlechat.User
+    ) -> None:
         await puppet.update_info(source=source, info=user)
         if self.mxid and (not puppet.is_real_user or puppet.gcid != source.gcid):
             await puppet.intent_for(self).ensure_joined(self.mxid, bot=self.main_intent)
 
     # endregion
     # region Backfill
 
@@ -329,49 +405,49 @@
 
     async def _initial_backfill(self, source: u.User) -> int:
         self.log.debug(f"Fetching topics through {source.mxid} for initial backfill")
         req = googlechat.ListTopicsRequest(
             request_header=source.client.gc_request_header,
             page_size_for_topics=(
                 self.config["bridge.backfill.initial_thread_limit"]
-                if self.is_threaded
+                if self.threads_only
                 else self.config["bridge.backfill.initial_nonthread_limit"]
             ),
             group_id=self.gc_group_id,
         )
         resp = await source.client.proto_list_topics(req)
         self.log.debug(
             f"Got {len(resp.topics)} topics from server "
             f"(up to revision {resp.group_revision.timestamp})"
         )
-        if self.is_threaded:
+        if self.threads_only:
             # Store the group revision already now, we can't continue from the middle anyway.
             await self.set_revision(resp.group_revision.timestamp)
         topic: googlechat.Topic
         message_count = 0
         # The reversed list is probably already sorted properly, but re-sort it just in case
         sorted_topics = sorted(reversed(resp.topics), key=lambda topic: topic.sort_time)
         for topic in sorted_topics:
             await self.handle_googlechat_message(source, topic.replies[0])
             message_count += 1
-            if self.is_threaded:
+            if self.threads_only or topic.topic_read_state.thread_created_usec > 0:
                 msg_req = googlechat.ListMessagesRequest(
                     request_header=source.client.gc_request_header,
                     parent_id=googlechat.MessageParentId(topic_id=topic.id),
                     page_size=self.config["bridge.backfill.initial_thread_reply_limit"],
                 )
                 msg_resp = await source.client.proto_list_messages(msg_req)
                 self.log.debug(f"Fetched {len(msg_resp.messages)} replies to {topic.id.topic_id}")
                 for msg in msg_resp.messages:
                     await self.handle_googlechat_message(source, msg)
                     message_count += 1
             else:
                 await self.set_revision(topic.replies[0].create_time)
         self.log.info(f"Initial backfill complete, handled {message_count} messages in total")
-        if not self.is_threaded:
+        if not self.threads_only:
             await self.set_revision(resp.group_revision.timestamp)
         return message_count
 
     async def _catchup_backfill(self, source: u.User, latest_revision: int) -> int:
         if not self.revision:
             self.log.debug("Can't do catch-up backfill on portal with no known last revision")
             return 0
@@ -526,15 +602,16 @@
                 "id": "googlechat",
                 "displayname": "Google Chat",
                 "avatar_url": self.config["appservice.bot_avatar"],
             },
             "channel": {
                 "id": self.gcid,
                 "displayname": self.name,
-                "fi.mau.googlechat.is_threaded": self.is_threaded,
+                "fi.mau.googlechat.threads_only": self.threads_only,
+                "fi.mau.googlechat.threads_enabled": self.threads_enabled,
             },
         }
 
     async def update_bridge_info(self, timestamp: int | None = None) -> None:
         if not self.mxid:
             self.log.debug("Not updating bridge info: no Matrix room created")
             return
@@ -605,22 +682,25 @@
         if not self.config["bridge.federate_rooms"]:
             creation_content["m.federate"] = False
 
         # We lock backfill lock here so any messages that come between the room being created
         # and the initial backfill finishing wouldn't be bridged before the backfill messages.
         with self.backfill_lock:
             self.mxid = await self.main_intent.create_room(
-                name=self.name if self.encrypted or not self.is_direct else None,
+                name=self.name if self.set_dm_room_metadata else None,
+                topic=self.description,
                 is_direct=self.is_direct,
                 initial_state=initial_state,
                 invitees=invites,
                 creation_content=creation_content,
             )
             if not self.mxid:
                 raise Exception("Failed to create room: no mxid returned")
+            self.name_set = bool(self.name) and self.set_dm_room_metadata
+            self.description_set = bool(self.description)
             if self.encrypted and self.matrix.e2ee and self.is_direct:
                 try:
                     await self.az.intent.ensure_joined(self.mxid)
                 except Exception:
                     self.log.warning(f"Failed to add bridge bot to new private chat {self.mxid}")
             await self.save()
             self.log.debug(f"Matrix room created: {self.mxid}")
@@ -802,15 +882,15 @@
         if message.get_edit():
             await self.handle_matrix_edit(sender, message, event_id)
             return
         reply_to = await DBMessage.get_by_mxid(
             message.get_thread_parent() or message.get_reply_to(), self.mxid
         )
         thread_id = (
-            (reply_to.gc_parent_id or reply_to.gcid) if reply_to and self.is_threaded else None
+            (reply_to.gc_parent_id or reply_to.gcid) if reply_to and self.threads_enabled else None
         )
         local_id = f"mautrix-googlechat%{random.randint(0, 0xffffffffffffffff)}"
         self._local_dedup.add(local_id)
 
         # TODO this probably isn't nice for bridging images, it really only needs to lock the
         #      actual message send call and dedup queue append.
         async with self.require_send_lock(sender.gcid):
@@ -854,15 +934,15 @@
             status=MessageSendCheckpointStatus.PERM_FAILURE,
             event_id=event_id,
             room_id=self.mxid,
             event_type=evt_type,
             message_type=msgtype,
             error=reason,
         )
-        asyncio.create_task(self._send_message_status(event_id, NotImplementedError(reason)))
+        background_task.create(self._send_message_status(event_id, NotImplementedError(reason)))
 
     async def _rec_error(
         self,
         user: u.User,
         err: Exception,
         event_id: EventID,
         evt_type: EventType,
@@ -881,15 +961,15 @@
             status=MessageSendCheckpointStatus.PERM_FAILURE,
             event_id=event_id,
             room_id=self.mxid,
             event_type=evt_type,
             message_type=msgtype,
             error=err,
         )
-        asyncio.create_task(self._send_message_status(event_id, err))
+        background_task.create(self._send_message_status(event_id, err))
         if self.config["bridge.delivery_error_reports"]:
             await self._send_message(
                 self.main_intent,
                 TextMessageEventContent(
                     msgtype=MessageType.NOTICE,
                     body=f"\u26a0 Your {type_name} may not have been bridged: {err}",
                 ),
@@ -906,15 +986,15 @@
             status=MessageSendCheckpointStatus.SUCCESS,
             event_id=event_id,
             room_id=self.mxid,
             event_type=evt_type,
             message_type=msgtype,
         )
         await self._send_delivery_receipt(event_id)
-        asyncio.create_task(self._send_message_status(event_id, err=None))
+        background_task.create(self._send_message_status(event_id, err=None))
 
     async def _send_message_status(self, event_id: EventID, err: Exception | None) -> None:
         if not self.config["bridge.message_status_events"]:
             return
         intent = self.az.intent if self.encrypted else self.main_intent
         status = BeeperMessageStatusEventContent(
             network=self.bridge_info_state_key,
@@ -928,15 +1008,14 @@
             status.status = MessageStatus.RETRIABLE
             status.error = str(err)
             if isinstance(err, NotImplementedError):
                 status.reason = MessageStatusReason.UNSUPPORTED
                 status.status = MessageStatus.FAIL
         else:
             status.status = MessageStatus.SUCCESS
-        status.fill_legacy_booleans()
 
         await intent.send_message_event(
             room_id=self.mxid,
             event_type=EventType.BEEPER_MESSAGE_STATUS,
             content=status,
         )
 
@@ -1122,31 +1201,89 @@
         content.set_edit(target.mxid)
         event_id = await self._send_message(
             sender.intent_for(self), content, timestamp=edit_ts // 1000
         )
         self.log.debug("Handled Google Chat edit of %s at %s -> %s", msg_id, edit_ts, event_id)
         await self._send_delivery_receipt(event_id)
 
-    async def handle_googlechat_update(
+    async def handle_googlechat_room_update(
         self, sender: p.Puppet, timestamp: int, update: googlechat.RoomUpdatedMetadata
     ) -> bool:
         if update.HasField("rename_metadata") and update.rename_metadata.new_name:
-            if self.name != update.rename_metadata.new_name:
-                self.name = update.rename_metadata.new_name
-                try:
-                    await sender.intent_for(self).set_room_name(
-                        self.mxid, self.name, timestamp=timestamp
-                    )
-                except (MForbidden, IntentError):
-                    await self.main_intent.set_room_name(self.mxid, self.name, timestamp=timestamp)
+            if await self._update_name_direct(
+                update.rename_metadata.new_name, timestamp=timestamp
+            ):
                 await self.update_bridge_info(timestamp=timestamp)
+                await self.save()
+            return True
+        elif update.HasField("group_details_metadata"):
+            if await self._update_description(
+                update.group_details_metadata.new_group_details.description, timestamp=timestamp
+            ):
+                await self.save()
             return True
         else:
             return False
 
+    async def handle_googlechat_membership_change(
+        self,
+        source: u.User,
+        sender: p.Puppet,
+        update: googlechat.MembershipChangedMetadata,
+    ) -> None:
+        infos = await source.get_users(
+            [member_id.user_id.id for member_id in update.affected_members]
+        )
+        sender_intent = sender.intent_for(self)
+        for member_id, info in zip(update.affected_members, infos):
+            target: p.Puppet = await p.Puppet.get_by_gcid(member_id.user_id.id)
+            target_intent = target.intent_for(self)
+            await target.update_info(source, info)
+            if update.type == googlechat.MembershipChangedMetadata.JOINED:
+                await target_intent.ensure_joined(self.mxid)
+            elif update.type == googlechat.MembershipChangedMetadata.INVITED:
+                try:
+                    await sender_intent.invite_user(self.mxid, target_intent.mxid)
+                except MForbidden:
+                    await self.main_intent.invite_user(
+                        self.mxid, target_intent.mxid, reason=f"Invited by {sender.name}"
+                    )
+            elif update.type in (
+                googlechat.MembershipChangedMetadata.BOT_ADDED,
+                googlechat.MembershipChangedMetadata.ADDED,
+            ):
+                try:
+                    await sender_intent.invite_user(self.mxid, target_intent.mxid)
+                except MForbidden:
+                    pass  # will auto-invite in ensure_joined
+                await target_intent.ensure_joined(self.mxid)
+            elif update.type == googlechat.MembershipChangedMetadata.LEFT:
+                await target_intent.leave_room(self.mxid)
+            elif update.type in (
+                googlechat.MembershipChangedMetadata.REMOVED,
+                googlechat.MembershipChangedMetadata.BOT_REMOVED,
+            ):
+                try:
+                    await sender_intent.kick_user(self.mxid, target_intent.mxid)
+                except MForbidden:
+                    await self.main_intent.kick_user(
+                        self.mxid, target_intent.mxid, reason=f"Removed by {sender.name}"
+                    )
+            elif update.type == googlechat.MembershipChangedMetadata.KICKED_DUE_TO_OTR_CONFLICT:
+                try:
+                    await sender_intent.kick_user(
+                        self.mxid, target_intent.mxid, reason="OTR conflict"
+                    )
+                except MForbidden:
+                    await self.main_intent.kick_user(
+                        self.mxid,
+                        target_intent.mxid,
+                        reason=f"Removed by {sender.name} due to OTR conflict",
+                    )
+
     async def handle_googlechat_message(self, source: u.User, evt: googlechat.Message) -> None:
         sender = await p.Puppet.get_by_gcid(evt.creator.user_id.id)
         msg_id = evt.id.message_id
         async with self.optional_send_lock(sender.gcid):
             if evt.local_id in self._local_dedup:
                 self.log.debug(f"Dropping message {msg_id} (found in local dedup set)")
                 return
@@ -1164,19 +1301,26 @@
                 return
         if not await self._bridge_own_message_pm(source, sender, f"message {msg_id}"):
             return
 
         # Google Chat timestamps are in microseconds, Matrix wants milliseconds
         timestamp = evt.create_time // 1000
 
-        if len(evt.annotations) == 1 and evt.annotations[0].type == googlechat.ROOM_UPDATED:
-            self.log.debug("Handling Google Chat room update message %s", msg_id)
-            if await self.handle_googlechat_update(
-                sender, update=evt.annotations[0].room_updated, timestamp=timestamp
-            ):
+        if evt.message_type == googlechat.Message.SYSTEM_MESSAGE and len(evt.annotations) == 1:
+            self.log.debug("Handling Google Chat update message %s", msg_id)
+            update_type = evt.annotations[0].type
+            if update_type == googlechat.ROOM_UPDATED:
+                if await self.handle_googlechat_room_update(
+                    sender, update=evt.annotations[0].room_updated, timestamp=timestamp
+                ):
+                    return
+            elif update_type == googlechat.MEMBERSHIP_CHANGED:
+                await self.handle_googlechat_membership_change(
+                    source, sender, update=evt.annotations[0].membership_changed
+                )
                 return
         intent = sender.intent_for(self)
         self.log.debug("Handling Google Chat message %s", msg_id)
 
         thread_parent = None
         parent_id = evt.id.parent_id.topic_id.topic_id
         if parent_id:
@@ -1193,16 +1337,16 @@
         # This also adds text to evt.text_body if necessary
         attachment_urls = self._preprocess_annotations(evt)
 
         event_ids: list[tuple[EventID, MessageType]] = []
 
         def _append_event_id(evt_id: EventID, msg_type: MessageType) -> None:
             event_ids.append((evt_id, msg_type))
-            if self.is_threaded:
-                nonlocal thread_parent
+            nonlocal thread_parent
+            if thread_parent or self.threads_only:
                 if not thread_parent:
                     thread_parent = {"thread_parent": evt_id}
                 thread_parent["last_event_in_thread"] = evt_id
 
         if evt.text_body:
             content = await fmt.googlechat_to_matrix(source, evt, self)
             if thread_parent:
@@ -1387,15 +1531,15 @@
             return
         puppet = await p.Puppet.get_by_gcid(sender)
         if self.is_direct and puppet.gcid == source.gcid:
             membership = await self.az.state_store.get_membership(self.mxid, puppet.mxid)
             if membership != Membership.JOIN:
                 return
         await puppet.intent_for(self).set_typing(
-            self.mxid, status == googlechat.TYPING, timeout=6000
+            self.mxid, timeout=6000 if status == googlechat.TYPING else 0
         )
 
     # endregion
     # region Getters
 
     async def postinit(self) -> None:
         self.by_gcid[self.gcid_full] = self
```

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/puppet.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/puppet.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from .db import Puppet as DBPuppet
 
 if TYPE_CHECKING:
     from .__main__ import GoogleChatBridge
 
 
 class Puppet(DBPuppet, BasePuppet):
+    bridge: GoogleChatBridge
     config: Config
     hs_domain: str
     mxid_template: SimpleTemplate[str]
 
     by_gcid: dict[str, Puppet] = {}
     by_custom_mxid: dict[UserID, Puppet] = {}
 
@@ -49,28 +50,30 @@
         self,
         gcid: str,
         name: str | None = None,
         photo_id: str | None = None,
         photo_mxc: ContentURI | None = None,
         name_set: bool = False,
         avatar_set: bool = False,
+        contact_info_set: bool = False,
         is_registered: bool = False,
         custom_mxid: UserID | None = None,
         access_token: str | None = None,
         next_batch: SyncToken | None = None,
         base_url: URL | None = None,
         photo_hash: str | None = None,
     ) -> None:
         super().__init__(
             gcid=gcid,
             name=name,
             photo_id=photo_id,
             photo_mxc=photo_mxc,
             name_set=name_set,
             avatar_set=avatar_set,
+            contact_info_set=contact_info_set,
             is_registered=is_registered,
             custom_mxid=custom_mxid,
             access_token=access_token,
             next_batch=next_batch,
             base_url=base_url,
             photo_hash=photo_hash,
         )
@@ -84,14 +87,15 @@
     def _add_to_cache(self) -> None:
         self.by_gcid[self.gcid] = self
         if self.custom_mxid:
             self.by_custom_mxid[self.custom_mxid] = self
 
     @classmethod
     def init_cls(cls, bridge: "GoogleChatBridge") -> AsyncIterable[Awaitable[None]]:
+        cls.bridge = bridge
         cls.config = bridge.config
         cls.loop = bridge.loop
         cls.mx = bridge.matrix
         cls.az = bridge.az
         cls.hs_domain = cls.config["homeserver"]["domain"]
         cls.mxid_template = SimpleTemplate(
             cls.config["bridge.username_template"],
@@ -108,15 +112,15 @@
         cls.allow_discover_url = cls.config["bridge.double_puppet_allow_discovery"]
         cls.login_shared_secret_map = {
             server: secret.encode("utf-8")
             for server, secret in cls.config["bridge.login_shared_secret_map"].items()
         }
         cls.login_device_name = "Google Chat Bridge"
 
-        return (puppet.start() async for puppet in Puppet.get_all_with_custom_mxid())
+        return (puppet.try_start() async for puppet in Puppet.get_all_with_custom_mxid())
 
     async def default_puppet_should_leave_room(self, room_id: RoomID) -> bool:
         portal = await p.Portal.get_by_mxid(room_id)
         return portal and portal.other_user_id != self.gcid
 
     async def _leave_rooms_with_default_user(self) -> None:
         await super()._leave_rooms_with_default_user()
@@ -139,20 +143,43 @@
     # region User info updating
 
     async def update_info(
         self, source: u.User, info: googlechat.User | None = None, update_avatar: bool = True
     ) -> None:
         if info is None:
             info = (await source.get_users([self.gcid]))[0]
-        changed = await self._update_name(info)
+        changed = await self._update_contact_info(info)
+        changed = await self._update_name(info) or changed
         if update_avatar:
             changed = await self._update_photo(info.avatar_url) or changed
         if changed:
             await self.save()
 
+    async def _update_contact_info(self, info: googlechat.User) -> bool:
+        if not self.bridge.homeserver_software.is_hungry:
+            return False
+
+        if self.contact_info_set:
+            return False
+
+        try:
+            await self.default_mxid_intent.beeper_update_profile(
+                {
+                    "com.beeper.bridge.identifiers": [f"mailto:{info.email}"],
+                    "com.beeper.bridge.remote_id": self.gcid,
+                    "com.beeper.bridge.service": self.bridge.beeper_service_name,
+                    "com.beeper.bridge.network": self.bridge.beeper_network_name,
+                }
+            )
+            self.contact_info_set = True
+        except Exception:
+            self.log.exception("Error updating contact info")
+            self.contact_info_set = False
+        return True
+
     @classmethod
     def get_name_from_info(cls, info: googlechat.User) -> str | None:
         full = info.name
         first = info.first_name
         last = info.last_name
         if not full:
             if info.first_name or info.last_name:
```

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/user.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/user.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mautrix-googlechat - A Matrix-Google Chat puppeting bridge
-# Copyright (C) 2022 Tulir Asokan
+# Copyright (C) 2023 Tulir Asokan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -11,28 +11,31 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, AsyncIterable, Awaitable, Callable, Iterable, cast
+from typing import TYPE_CHECKING, AsyncIterable, Awaitable, Iterable, cast
 import asyncio
 import time
 
 from maugclib import (
     ChannelLifetimeExpired,
     Client,
-    GoogleAuthError,
-    RefreshTokenCache,
-    TokenManager,
+    Cookies,
+    NotLoggedInError,
+    ResponseError,
+    SIDInvalidError,
+    UnexpectedStatusError,
     googlechat_pb2 as googlechat,
 )
 from mautrix.bridge import BaseUser, async_getter_lock
 from mautrix.types import MessageType, RoomID, UserID
+from mautrix.util import background_task
 from mautrix.util.bridge_state import BridgeState, BridgeStateEvent
 from mautrix.util.opt_prometheus import Gauge, Histogram, async_time
 import maugclib.parsers
 
 from . import portal as po, puppet as pu
 from .config import Config
 from .db import User as DBUser
@@ -40,15 +43,14 @@
 if TYPE_CHECKING:
     from .__main__ import GoogleChatBridge
 
 METRIC_SYNC = Histogram("bridge_sync", "calls to sync")
 METRIC_LOGGED_IN = Gauge("bridge_logged_in", "Number of users logged into the bridge")
 METRIC_CONNECTED = Gauge("bridge_connected", "Number of users connected to Google Chat")
 
-
 BridgeState.human_readable_errors.update(
     {"get-self-fail": "Failed to get user info from Google Chat"}
 )
 
 
 class User(DBUser, BaseUser):
     by_mxid: dict[UserID, User] = {}
@@ -65,32 +67,35 @@
     email: str | None
     name_future: asyncio.Future
     connected: bool
     _skip_backoff: bool
     _skip_on_connect: bool
     _prev_sync: float
     periodic_sync_task: asyncio.Task | None
+    conn_task: asyncio.Task | None
 
     groups: dict[str, googlechat.GetGroupResponse]
     groups_lock: asyncio.Lock
     users: dict[str, googlechat.User]
     users_lock: asyncio.Lock
 
     def __init__(
         self,
         mxid: UserID,
         gcid: str | None = None,
         revision: int | None = None,
-        refresh_token: str | None = None,
+        cookies: Cookies | None = None,
+        user_agent: str | None = None,
         notice_room: RoomID | None = None,
     ) -> None:
         super().__init__(
             mxid=mxid,
             gcid=gcid,
-            refresh_token=refresh_token,
+            cookies=cookies,
+            user_agent=user_agent,
             revision=revision,
             notice_room=notice_room,
         )
         BaseUser.__init__(self)
         self._notice_room_lock = asyncio.Lock()
         self.is_whitelisted, self.is_admin, self.level = self.config.get_permissions(mxid)
         self.client = None
@@ -103,14 +108,15 @@
         self._prev_sync = 0
         self.groups = {}
         self.groups_lock = asyncio.Lock()
         self.users = {}
         self.users_lock = asyncio.Lock()
         self._intentional_disconnect = False
         self.periodic_sync_task = None
+        self.conn_task = None
 
     # region Sessions
 
     def _add_to_cache(self) -> None:
         self.by_mxid[self.mxid] = self
         if self.gcid:
             self.by_gcid[self.gcid] = self
@@ -227,59 +233,83 @@
         cls.az = bridge.az
         cls.config = bridge.config
         cls.loop = bridge.loop
         return (user._try_init() async for user in cls.all_logged_in())
 
     async def _try_init(self) -> None:
         try:
-            token_mgr = await TokenManager.from_refresh_token(UserRefreshTokenCache(self))
-        except GoogleAuthError as e:
-            await self.send_bridge_notice(
-                f"Failed to resume session with stored refresh token: {e}",
-                state_event=BridgeStateEvent.BAD_CREDENTIALS,
-                important=True,
-            )
+            await self.connect()
+        except Exception as e:
             self.log.exception("Failed to resume session with stored refresh token")
-            self.refresh_token = None
-            await self.save()
-        else:
-            self.login_complete(token_mgr)
+            if isinstance(e, ResponseError):
+                self.log.debug("Auth error body: %s", e.body)
+            if isinstance(e, UnexpectedStatusError) and e.error_code == "invalid_grant":
+                self.log.info("Resume session error has invalid_grant error code, logging out")
+                await self.logout(is_manual=False, error=e)
+            elif isinstance(e, NotLoggedInError):
+                self.log.info("Resume session error is NotLoggedInError, logging out")
+                await self.logout(is_manual=False)
+            else:
+                await self.send_bridge_notice(
+                    f"Failed to resume session with stored refresh token: {e}",
+                    state_event=BridgeStateEvent.UNKNOWN_ERROR,
+                    important=True,
+                )
+                # TODO retry?
 
-    def login_complete(self, token_manager: TokenManager) -> None:
+    async def connect(self, cookies: Cookies | None = None, get_self: bool = False) -> bool:
         self.log.debug("Running post-login actions")
-        self.client = Client(token_manager, max_retries=3, retry_backoff_base=2)
-        asyncio.create_task(self.start())
+        client = Client(
+            cookies or self.cookies,
+            user_agent=self.user_agent,
+            max_retries=3,
+            retry_backoff_base=2,
+        )
+        await client.refresh_tokens()
+        self.client = client
+        if get_self or not self.gcid:
+            self.log.debug("Fetching own user ID before connecting")
+            try:
+                await self._fetch_own_id()
+            except Exception:
+                self.cookies = None
+                self.client = None
+                await self.save()
+                self.log.exception("Failed to get own info after login")
+                return False
+        client_cookies = self.client.cookies
+        if client_cookies != self.cookies:
+            self.cookies = client_cookies
+            await self.save()
+            self.log.debug("Saved updated auth cookies")
+        self.conn_task = asyncio.create_task(self.start())
         if not self.periodic_sync_task:
             self.periodic_sync_task = asyncio.create_task(self._periodic_sync())
         self.client.on_stream_event.add_observer(self.on_stream_event)
         self.client.on_connect.add_observer(self.on_connect)
         self.client.on_reconnect.add_observer(self.on_reconnect)
         self.client.on_disconnect.add_observer(self.on_disconnect)
-
-    def _in_background(
-        self, method: Callable[[Any], Awaitable[None]]
-    ) -> Callable[[Any], Awaitable[None]]:
-        async def try_proxy(*args, **kwargs) -> None:
-            try:
-                await method(*args, **kwargs)
-            except Exception:
-                self.log.exception("Exception in event handler")
-
-        async def proxy(*args, **kwargs) -> None:
-            asyncio.create_task(try_proxy(*args, **kwargs))
-
-        return proxy
+        return True
 
     async def start(self) -> None:
+        try:
+            await self._start()
+        except Exception:
+            self.log.exception("Fatal error in Google Chat connection")
+
+    async def _start(self) -> None:
         last_disconnection = 0
         backoff = 4
         backoff_reset_in_seconds = 60
         state_event = BridgeStateEvent.TRANSIENT_DISCONNECT
         self._intentional_disconnect = False
         while True:
+            if self._intentional_disconnect:
+                self.log.warning("Client connection already finished, not restarting")
+                return
             try:
                 await self.client.connect(max_age=1.5 * 60 * 60)
                 self._track_metric(METRIC_CONNECTED, False)
                 if self._intentional_disconnect:
                     self.log.info("Client connection finished")
                     return
                 elif self._skip_backoff:
@@ -289,49 +319,107 @@
                 else:
                     self.log.warning("Client connection finished unexpectedly")
                     error_msg = "Client connection finished unexpectedly"
             except ChannelLifetimeExpired:
                 self.log.debug("Client connection was terminated after being alive too long")
                 self._skip_on_connect = True
                 continue
+            except SIDInvalidError:
+                if self._prev_sync + 3 * 60 < time.monotonic():
+                    self.log.debug(
+                        "Client connection was terminated due to invalid SID error, "
+                        "doing small sync to check for missed messages"
+                    )
+                    try:
+                        backfilled_count = await self.sync(limit=3)
+                    except Exception:
+                        self.log.exception("Failed to sync recent chats")
+                        backfilled_count = None
+                    if backfilled_count:
+                        self.log.debug(
+                            f"Sync backfilled {backfilled_count} chats,"
+                            " doing full sync on reconnect"
+                        )
+                    else:
+                        self.log.debug("Sync didn't backfill anything")
+                        self._skip_on_connect = True
+                    continue
+                else:
+                    self.log.warning(
+                        "Client connection was terminated due to invalid SID error, "
+                        "but previous sync was less than 3 minutes ago"
+                    )
+                    error_msg = f"Unknown SID error in Google Chat connection"
             except Exception as e:
                 self._track_metric(METRIC_CONNECTED, False)
                 self.log.exception("Exception in connection")
+                if isinstance(e, ResponseError):
+                    self.log.debug("Response error body: %s", e.body)
+                if isinstance(e, UnexpectedStatusError) and (
+                    e.error_code == "invalid_grant" or e.status == 401
+                ):
+                    self.log.info(
+                        "Connection error has 401 status or invalid_grant error code, logging out"
+                    )
+                    background_task.create(self.logout(is_manual=False, error=e))
+                    return
                 error_msg = f"Exception in Google Chat connection: {e}"
 
             if last_disconnection + backoff_reset_in_seconds < time.time():
                 backoff = 4
                 state_event = BridgeStateEvent.TRANSIENT_DISCONNECT
             else:
                 backoff = int(backoff * 1.5)
                 if backoff > 60:
                     state_event = BridgeStateEvent.UNKNOWN_ERROR
-            await self.send_bridge_notice(
-                error_msg,
-                state_event=state_event,
-                important=state_event == BridgeStateEvent.UNKNOWN_ERROR,
-            )
-            last_disconnection = time.time()
-            self.log.debug(f"Reconnecting in {backoff} seconds")
-            await asyncio.sleep(backoff)
+            try:
+                await self.send_bridge_notice(
+                    error_msg,
+                    state_event=state_event,
+                    important=state_event == BridgeStateEvent.UNKNOWN_ERROR,
+                )
+                last_disconnection = time.time()
+                self.log.debug(f"Reconnecting in {backoff} seconds")
+                await asyncio.sleep(backoff)
+            except asyncio.CancelledError:
+                self.log.debug("Connection task was cancelled while waiting to reconnect")
+                return
+            except Exception:
+                self.log.exception("Error waiting to reconnect")
 
     async def stop(self) -> None:
         if self.client:
             self._intentional_disconnect = True
             self.client.disconnect()
         if self.periodic_sync_task:
             self.periodic_sync_task.cancel()
             self.periodic_sync_task = None
+        if self.conn_task:
+            self.conn_task.cancel()
+            self.conn_task = None
         await self.save()
 
-    async def logout(self) -> None:
+    async def logout(self, is_manual: bool, error: UnexpectedStatusError | None = None) -> None:
+        if self.gcid:
+            if is_manual:
+                await self.push_bridge_state(BridgeStateEvent.LOGGED_OUT)
+            else:
+                message = "Logged out from Google account"
+                if error and isinstance(error, UnexpectedStatusError) and error.error_code:
+                    message += f": {error.error_code}: {error.error_desc}"
+                await self.send_bridge_notice(
+                    message,
+                    state_event=BridgeStateEvent.BAD_CREDENTIALS,
+                    important=True,
+                )
         self._track_metric(METRIC_LOGGED_IN, False)
         self.by_gcid.pop(self.gcid, None)
         self.gcid = None
-        self.refresh_token = None
+        self.cookies = None
+        self.user_agent = None
         await self.stop()
         self.client = None
         self.connected = False
 
         self.users = {}
         self.groups = {}
 
@@ -340,27 +428,32 @@
         if not self.name_future.done():
             self.name_future.set_exception(Exception("logged out"))
         self.name_future = self.loop.create_future()
 
     async def on_connect(self) -> None:
         self.connected = True
         if not self._skip_on_connect:
-            asyncio.create_task(self.on_connect_later())
+            background_task.create(self.on_connect_later())
             await self.send_bridge_notice("Connected to Google Chat")
         else:
             self._skip_on_connect = False
             await self.push_bridge_state(BridgeStateEvent.CONNECTED)
 
+    async def _fetch_own_id(self) -> None:
+        if self.gcid:
+            return
+        info = await self.client.proto_get_self_user_status(
+            googlechat.GetSelfUserStatusRequest(request_header=self.client.gc_request_header)
+        )
+        self.gcid = info.user_status.user_id.id
+        self.by_gcid[self.gcid] = self
+
     async def get_self(self) -> googlechat.User:
         if not self.gcid:
-            info = await self.client.proto_get_self_user_status(
-                googlechat.GetSelfUserStatusRequest(request_header=self.client.gc_request_header)
-            )
-            self.gcid = info.user_status.user_id.id
-            self.by_gcid[self.gcid] = self
+            await self._fetch_own_id()
 
         resp = await self.client.proto_get_members(
             googlechat.GetMembersRequest(
                 request_header=self.client.gc_request_header,
                 member_ids=[
                     googlechat.MemberId(user_id=googlechat.UserId(id=self.gcid)),
                 ],
@@ -371,15 +464,15 @@
         return user
 
     async def get_users(self, ids: Iterable[str]) -> list[googlechat.User]:
         async with self.users_lock:
             req_ids = [
                 googlechat.MemberId(user_id=googlechat.UserId(id=user_id))
                 for user_id in ids
-                if user_id not in self.users
+                if user_id not in self.users and user_id
             ]
             if req_ids:
                 self.log.debug(f"Fetching info of users {[user.user_id.id for user in req_ids]}")
                 resp = await self.client.proto_get_members(
                     googlechat.GetMembersRequest(
                         request_header=self.client.gc_request_header,
                         member_ids=req_ids,
@@ -495,16 +588,27 @@
                     self.log.debug(f"Periodic sync backfilled {backfilled_count} chats")
                     self.reconnect()
                 else:
                     self.log.debug("Periodic sync didn't backfill anything")
             except asyncio.CancelledError:
                 self.log.debug("Periodic sync cancelled")
                 break
-            except Exception:
+            except Exception as e:
                 self.log.exception("Exception in periodic sync")
+                if isinstance(e, ResponseError):
+                    self.log.debug("Response error body: %s", e.body)
+                if isinstance(e, UnexpectedStatusError) and (
+                    e.error_code == "invalid_grant" or e.status == 401
+                ):
+                    self.log.info(
+                        "Periodic sync error has 401 status or invalid_grant error code, "
+                        "logging out"
+                    )
+                    background_task.create(self.logout(is_manual=False, error=e))
+                    return
 
     @async_time(METRIC_SYNC)
     async def sync(self, limit: int | None = None) -> int:
         self._prev_sync = time.monotonic()
         self.log.debug("Fetching first page of the world")
         req = googlechat.PaginatedWorldRequest(
             request_header=self.client.gc_request_header,
@@ -581,23 +685,7 @@
         await self.client.proto_mark_group_read_state(
             googlechat.MarkGroupReadstateRequest(
                 request_header=self.client.gc_request_header,
                 id=maugclib.parsers.group_id_from_id(conversation_id),
                 last_read_time=int((timestamp or (time.time() * 1000)) * 1000),
             )
         )
-
-
-class UserRefreshTokenCache(RefreshTokenCache):
-    user: User
-
-    def __init__(self, user: User) -> None:
-        self.user = user
-
-    async def get(self) -> str:
-        return self.user.refresh_token
-
-    async def set(self, refresh_token: str) -> None:
-        self.user.log.debug("Got new refresh token")
-        self.user.log.trace("New refresh token: %s", refresh_token)
-        self.user.refresh_token = refresh_token
-        await self.user.save()
```

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/util/color_log.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/util/color_log.py`

 * *Files identical despite different names*

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat/web/auth.py` & `mautrix-googlechat-0.5.0/mautrix_googlechat/web/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mautrix-googlechat - A Matrix-Google Chat puppeting bridge
-# Copyright (C) 2022 Tulir Asokan
+# Copyright (C) 2023 Tulir Asokan
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -14,19 +14,19 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from typing import Any
 import asyncio
 import logging
-import urllib.parse
 
 from aiohttp import web
 
-from maugclib.auth import OAUTH2_CLIENT_ID, OAUTH2_SCOPES, GoogleAuthError, TokenManager
+from maugclib import Cookies
+from maugclib.exceptions import NotLoggedInError, ResponseError
 from mautrix.types import UserID
 
 from .. import user as u
 
 
 class ErrorResponse(Exception):
     def __init__(
@@ -53,45 +53,30 @@
 
 
 log = logging.getLogger("mau.gc.auth")
 
 LOGIN_TIMEOUT = 10 * 60
 
 
-def make_login_url(device_name: str) -> str:
-    query = urllib.parse.urlencode(
-        {
-            "scope": "+".join(OAUTH2_SCOPES),
-            "client_id": OAUTH2_CLIENT_ID,
-            "device_name": device_name,
-        },
-        safe="+",
-    )
-    return f"https://accounts.google.com/o/oauth2/programmatic_auth?{query}"
-
-
 class GoogleChatAuthServer:
     app: web.Application
     shared_secret: str | None
-    device_name: str
 
-    def __init__(self, shared_secret: str | None, device_name: str) -> None:
+    def __init__(self, shared_secret: str | None) -> None:
         self.ongoing = {}
-        self.device_name = device_name
         self.shared_secret = shared_secret
 
         self.app = web.Application(middlewares=[error_middleware])
         self.app.router.add_get("/v1/whoami", self.whoami)
         self.app.router.add_post("/v1/login", self.login)
         self.app.router.add_post("/v1/logout", self.logout)
         self.app.router.add_post("/v1/reconnect", self.reconnect)
 
         self.legacy_app = web.Application(middlewares=[error_middleware])
         self.legacy_app.router.add_post("/api/verify", self.verify)
-        self.legacy_app.router.add_post("/api/start", self.start_login)
         self.legacy_app.router.add_post("/api/logout", self.logout)
         self.legacy_app.router.add_post("/api/authorization", self.login)
         self.legacy_app.router.add_post("/api/reconnect", self.reconnect)
         self.legacy_app.router.add_get("/api/whoami", self.whoami)
 
     def verify_token(self, request: web.Request) -> UserID | None:
         try:
@@ -114,15 +99,15 @@
                 "user_id": self.verify_token(request),
             }
         )
 
     async def logout(self, request: web.Request) -> web.Response:
         user_id = self.verify_token(request)
         user = await u.User.get_by_mxid(user_id)
-        await user.logout()
+        await user.logout(is_manual=True)
         return web.json_response({})
 
     async def whoami(self, request: web.Request) -> web.Response:
         user_id = self.verify_token(request)
         user = await u.User.get_by_mxid(user_id)
         return web.json_response(
             {
@@ -141,33 +126,14 @@
 
     async def reconnect(self, request: web.Request) -> web.Response:
         user_id = self.verify_token(request)
         user = await u.User.get_by_mxid(user_id)
         user.reconnect()
         return web.json_response({})
 
-    async def start_login(self, request: web.Request) -> web.Response:
-        user_id = self.verify_token(request)
-        user = await u.User.get_by_mxid(user_id)
-        if user.client:
-            await user.name_future
-            return web.json_response(
-                {
-                    "status": "success",
-                    "name": user.name,
-                    "email": user.email,
-                }
-            )
-        return web.json_response(
-            {
-                "next_step": "authorization",
-                "manual_auth_url": make_login_url(self.device_name),
-            }
-        )
-
     async def login(self, request: web.Request) -> web.Response:
         user_id = self.verify_token(request)
         user = await u.User.get_by_mxid(user_id)
         if user.client:
             await user.name_future
             return web.json_response(
                 {
@@ -176,26 +142,31 @@
                     "email": user.email,
                 }
             )
         data = await request.json()
         if not data:
             raise ErrorResponse(400, "Body is not JSON", "M_NOT_JSON")
         try:
-            auth = data["authorization"]
-        except KeyError:
+            cookies = Cookies(**{k.lower(): v for k, v in data["cookies"].items()})
+        except TypeError:
             raise ErrorResponse(
-                400, "Request body did not contain authorization field", "M_BAD_REQUEST"
+                400, "Request body did not contain the required fields", "M_BAD_REQUEST"
             )
+        user.user_agent = data.get("user_agent", None)
 
-        user.log.debug("Trying to log in with auth code")
+        user.log.debug("Trying to log in with cookies")
         try:
-            token_mgr = await TokenManager.from_authorization_code(
-                auth, u.UserRefreshTokenCache(user)
-            )
-        except GoogleAuthError as e:
+            if not await user.connect(cookies, get_self=True):
+                return web.json_response(
+                    {
+                        "status": "fail",
+                        "error": "Failed to get own info after login",
+                    }
+                )
+        except (ResponseError, NotLoggedInError) as e:
             log.exception(f"Login for {user.mxid} failed")
             return web.json_response(
                 {
                     "status": "fail",
                     "error": str(e),
                 }
             )
@@ -205,15 +176,14 @@
                 {
                     "status": "fail",
                     "error": "internal error",
                 },
                 status=500,
             )
         else:
-            user.login_complete(token_mgr)
             await asyncio.wait_for(asyncio.shield(user.name_future), 20)
             return web.json_response(
                 {
                     "status": "success",
                     "name": user.name,
                     "email": user.email,
                 }
```

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat.egg-info/PKG-INFO` & `mautrix-googlechat-0.5.0/mautrix_googlechat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mautrix-googlechat
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Matrix-Google Chat puppeting bridge.
 Home-page: https://github.com/mautrix/googlechat
 Author: Tulir Asokan
 Author-email: tulir@maunium.net
-License: UNKNOWN
 Project-URL: Changelog, https://github.com/mautrix/googlechat/blob/master/CHANGELOG.md
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Communications :: Chat
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -46,9 +44,7 @@
 
 ### Features & Roadmap
 [ROADMAP.md](https://github.com/mautrix/googlechat/blob/master/ROADMAP.md)
 contains a general overview of what is supported by the bridge.
 
 ## Discussion
 Matrix room: [`#googlechat:maunium.net`](https://matrix.to/#/#googlechat:maunium.net)
-
-
```

### Comparing `mautrix-googlechat-0.4.0/mautrix_googlechat.egg-info/SOURCES.txt` & `mautrix-googlechat-0.5.0/mautrix_googlechat.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 MANIFEST.in
 README.md
 optional-requirements.txt
 pyproject.toml
 requirements.txt
 setup.py
 maugclib/__init__.py
-maugclib/auth.py
 maugclib/channel.py
 maugclib/client.py
 maugclib/event.py
 maugclib/exceptions.py
 maugclib/googlechat_pb2.py
 maugclib/http_utils.py
 maugclib/parsers.py
+maugclib/pblite.py
 mautrix_googlechat/__init__.py
 mautrix_googlechat/__main__.py
 mautrix_googlechat/config.py
 mautrix_googlechat/example-config.yaml
 mautrix_googlechat/get_version.py
 mautrix_googlechat/matrix.py
 mautrix_googlechat/portal.py
@@ -40,14 +40,19 @@
 mautrix_googlechat/db/reaction.py
 mautrix_googlechat/db/user.py
 mautrix_googlechat/db/upgrade/__init__.py
 mautrix_googlechat/db/upgrade/v00_latest_revision.py
 mautrix_googlechat/db/upgrade/v02_reactions.py
 mautrix_googlechat/db/upgrade/v03_store_gc_revision.py
 mautrix_googlechat/db/upgrade/v04_store_photo_hash.py
+mautrix_googlechat/db/upgrade/v05_rename_thread_columns.py
+mautrix_googlechat/db/upgrade/v06_space_description.py
+mautrix_googlechat/db/upgrade/v07_puppet_contact_info_set.py
+mautrix_googlechat/db/upgrade/v08_web_app_auth.py
+mautrix_googlechat/db/upgrade/v09_web_app_ua.py
 mautrix_googlechat/formatter/__init__.py
 mautrix_googlechat/formatter/from_googlechat.py
 mautrix_googlechat/formatter/gc_url_preview.py
 mautrix_googlechat/formatter/util.py
 mautrix_googlechat/formatter/from_matrix/__init__.py
 mautrix_googlechat/formatter/from_matrix/gc_message.py
 mautrix_googlechat/formatter/from_matrix/parser.py
```

### Comparing `mautrix-googlechat-0.4.0/setup.py` & `mautrix-googlechat-0.5.0/setup.py`

 * *Files identical despite different names*

