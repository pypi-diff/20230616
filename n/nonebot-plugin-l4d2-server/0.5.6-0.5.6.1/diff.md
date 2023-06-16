# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.6.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.6.1.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.6.tar` & `nonebot_plugin_l4d2_server-0.5.6.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-06-14 12:38:37.817076 nonebot_plugin_l4d2_server-0.5.6/LICENSE
--rw-r--r--   0        0        0    11703 2023-06-14 12:38:37.817076 nonebot_plugin_l4d2_server-0.5.6/README.md
--rw-r--r--   0        0        0    17650 2023-06-14 12:38:37.821076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-06-14 12:38:37.821076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-06-14 12:38:37.821076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     8734 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-06-14 12:38:37.825076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1906 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1860 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     2688 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4148 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1073 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7415 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3735 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10855 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4113 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1175 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1434 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     9342 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     5753 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     8928 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14781 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1475 2023-06-14 12:38:37.829076 nonebot_plugin_l4d2_server-0.5.6/pyproject.toml
--rw-r--r--   0        0        0    13527 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-16 10:04:39.997589 nonebot_plugin_l4d2_server-0.5.6.1/LICENSE
+-rw-r--r--   0        0        0     5683 2023-06-16 10:04:39.997589 nonebot_plugin_l4d2_server-0.5.6.1/README.md
+-rw-r--r--   0        0        0    16994 2023-06-16 10:04:40.001589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-06-16 10:04:40.001589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-06-16 10:04:40.001589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     8734 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1714 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1860 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     2688 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4148 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1073 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-06-16 10:04:40.005589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7415 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3735 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10855 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4113 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1175 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1434 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     9342 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     5813 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2133 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     8928 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14650 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1477 2023-06-16 10:04:40.009589 nonebot_plugin_l4d2_server-0.5.6.1/pyproject.toml
+-rw-r--r--   0        0        0     7509 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.6.1/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6/LICENSE` & `nonebot_plugin_l4d2_server-0.5.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 driver = get_driver()
 
 
 __version__ = "0.5.6"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
-    usage='求生服务器操作指令',
+    usage="""
+    查询：【关键词】([序号])
+    """,
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_l4d2_server",
     supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
@@ -64,15 +66,15 @@
 
 @up.handle()
 async def _(matcher:Matcher,event: NoticeEvent):
     args = event.dict()
     if args['notice_type'] != 'offline_file':
         matcher.set_arg('txt',args)
         return
-    l4_file_path = l4_config.l4_ipall[CHECK_FILE]['location']
+    l4_file_path = l4_config.l4_ipall[l4_config.l4_number]['location']
     map_path = Path(l4_file_path, vpk_path)
     # 检查下载路径是否存在
     if not Path(l4_file_path).exists():
         await matcher.finish("你填写的路径不存在辣")
     if not Path(map_path).exists():
         await matcher.finish("这个路径并不是求生服务器的路径，请再看看罢")
     url:str = args['file']['url']
@@ -136,15 +138,15 @@
 
     await matcher.finish(mes_list(mes, vpk_files))
 
     
 @find_vpk.handle()
 async def _(bot:Bot,event: MessageEvent,matcher: Matcher):
     name_vpk = []
-    map_path = Path(l4_config.l4_ipall[CHECK_FILE]['location'],vpk_path)
+    map_path = Path(l4_config.l4_ipall[l4_config.l4_number]['location'],vpk_path)
     name_vpk = get_vpk(name_vpk,map_path)
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下vpk文件"
     msg = ''
     msg = mes_list(msg,name_vpk).replace(" ","")
     
     await matcher.finish(mode_txt_to_img(mes,msg))
@@ -153,22 +155,22 @@
 async def _(matcher:Matcher,args:Message = CommandArg()):
     num1 = args.extract_plain_text()
     if num1:
         matcher.set_arg("num",args)
 
 @del_vpk.got("num",prompt="你要删除第几个序号的地图(阿拉伯数字)")
 async def _(matcher: Matcher,tag:int = ArgPlainText("num")):
-    map_path = Path(l4_config.l4_ipall[CHECK_FILE]['location'],vpk_path)
+    map_path = Path(l4_config.l4_ipall[l4_config.l4_number]['location'],vpk_path)
     vpk_name = del_map(tag,map_path)
     await matcher.finish('已删除地图：' + vpk_name)
     
 @rename_vpk.handle()
 async def _(matcher:Matcher,matched: Tuple[int,str, str] = RegexGroup(),):
     num,useless,rename = matched
-    map_path = Path(l4_config.l4_ipall[CHECK_FILE]['location'],vpk_path)
+    map_path = Path(l4_config.l4_ipall[l4_config.l4_number]['location'],vpk_path)
     logger.info('检查是否名字是.vpk后缀')
     if not rename.endswith('.vpk'):
         rename = rename + '.vpk'
     logger.info('尝试改名')
     try:
         map_name = rename_map(num,rename,map_path)
         if map_name:
@@ -219,48 +221,30 @@
     msg = await command_server(tag)
     try:
         await matcher.finish(mode_txt_to_img('服务器返回',msg))
     except:
         await matcher.finish(msg,reply_message = True)
         
 
-# 连续rcon连接
-# @connect_rcon.handle()
-# async def _(State:T_State,args:Message = CommandArg()):
-#     msg = args.extract_plain_text()
-    # client = RCONClient(l4_host[CHECK_FILE], l4_port[CHECK_FILE], l4_rcon[CHECK_FILE])
-    # await client.connect()
-    # State['client'] = client
-#     if msg:
-#         connect_rcon.set_arg(key="prompt",message=args)
-        
-# @connect_rcon.got("prompt", prompt="连接开始...如果需要停止则输入“结束连接”")
-# async def handle_chat(State:T_State,event: MessageEvent, prompt: Message = Arg(), msg: str = ArgPlainText("prompt")):
-    # session_id = event.get_session_id()
-    # client:RCONClient = State['client']
-
-    # await client.close()
-    # await connect_rcon.finish('聊天结束...')
-        
         
 @check_path.handle()
 async def _(matcher:Matcher,args:Message = CommandArg()):
-    global CHECK_FILE
     msg = args.extract_plain_text()
     if msg.startswith('切换'):
         msg_number = int(''.join(msg.replace('切换', ' ').split()))
         if msg_number > len(l4_config.l4_ipall) or msg_number < 0:
             await matcher.send('没有这个序号的路径呐')
         else:
-            CHECK_FILE = msg_number - 1
-            now_path = l4_config.l4_ipall[CHECK_FILE]['location']
-            await matcher.send(f'已经切换路径为\n{str(CHECK_FILE+1)}、{now_path}')
+            l4_config.l4_number = msg_number - 1
+            now_path = l4_config.l4_ipall[l4_config.l4_number]['location']
+            await matcher.send(f'已经切换路径为\n{str(l4_config.l4_number+1)}、{now_path}')
+            config_manager.save()
     else: 
-        now_path = l4_config.l4_ipall[CHECK_FILE]['location']
-        await matcher.send(f'当前的路径为\n{str(CHECK_FILE+1)}、{now_path}')
+        now_path = l4_config.l4_ipall[l4_config.l4_number]['location']
+        await matcher.send(f'当前的路径为\n{str(l4_config.l4_number+1)}、{now_path}')
         
         
 @queries.handle()
 async def _(matcher:Matcher,args:Message = CommandArg()):
     msg = args.extract_plain_text()
     if msg:
         matcher.set_arg("ip",args)
@@ -403,15 +387,15 @@
     file_name:str = str(usr_id) + '.vtf'
     await upload_file(bot, event, img_bytes, file_name)
 
 
 
 @smx_file.handle()
 async def _(matcher:Matcher,):
-    smx_path = Path(l4_config.l4_ipall[CHECK_FILE]['location'],"left4dead2/addons/sourcemod/plugins")
+    smx_path = Path(l4_config.l4_ipall[l4_config.l4_number]['location'],"left4dead2/addons/sourcemod/plugins")
     smx_list = []
     name_smx = get_vpk(smx_list,smx_path,file_=".smx")
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下smx文件"
     msg = ''
     msg = mes_list(msg,name_smx).replace(" ","")
     await matcher.finish(mode_txt_to_img(mes,msg))
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,9 +48,7 @@
         await client.upload(local_path, remote_path)
     elif mode == 'read':
         file = await client.read(remote_path)
         return file
     elif mode == 'del':
         await client.delete(remote_path)
 
-if __name__ == '__main__':
-    asyncio.run(remote(mode='upload',host='106.13.207.45',user='root',password='Taojie@114514',local_path='E:\\zhang\\文件\\login_info.txt',remote_path='/home/'))
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 
 class L4d2Config(BaseModel):
     total_enable: bool = Field(True, alias='是否全局启用求生功能')
     web_username: str = Field('l4d2', alias='后台管理用户名')
     web_password: str = Field('admin', alias='后台管理密码')
     l4_style: str = Field("standard", alias='图片风格')
     l4_image: bool = Field(False , alias='是否启用图片')
-    
     l4_ipall: List[Dict[str,Union[str,int,bool]]] = Field(
         [{
         'id_rank':'1',
         'place': False,
         'location':'C:\\l4d2',
         'host':'127.0.0.1',
         'port':'20715',
@@ -76,14 +75,16 @@
         'port':'20715',
         'rcon':'9191810',
         'account':'root',
         'password':'114514',
         'server_id':'远程地图',
         }],
           alias='l4服务器ip集合')
+    
+    l4_number :int = Field(1,alias='第几个地图路径')
     web_secret_key: str = Field('49c294d32f69b732ef6447c18379451ce1738922a75cd1d4812ef150318a2ed0',
                                 alias='后台管理token密钥')
     l4_master: List[str] = Field(['114514919'], alias='求生地图全局管理员qq')
     # l4_ip:bool = Field(False, alias='查询地图是否显示ip')
     l4_font: str = Field('simsun.ttc', alias='字体')
     l4_only:bool = Field(False, alias='下载地图是是否阻碍其他指令')
     l4_push_interval: int = Field(3, alias='定时任务间隔')
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.6.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,26 +64,24 @@
                                      content='机器人返回图片中文字的字体。')),
         Select(label='图片风格', name='l4_style', value='${l4_style}',source='${l4_styles}',
                   labelRemark=Remark(shape='circle',
                                      content='仅仅是批量查询的风格')),
         Switch(label='是否优先上传地图', name='l4_only', value='${l4_only}', onText='开启', offText='关闭',
                labelRemark=Remark(shape='circle',
                                   content='开启时，上传地图会保证优先级，从而阻碍其他指令')),
-        InputTag(label='查询的远程服务器tag', name='l4_tag', value='${l4_tag}',
-                 enableBatchAdd=True,
-                 placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
-                 labelRemark=Remark(shape='circle',
-                                    content='在这里加入的用户，才能上传地图')),
-        
         InputNumber(label='定时推送间隔（min）', name='l4_push_interval', value='${l4_push_interval}',
                   labelRemark=Remark(shape='circle',
                                      content='设置好后，使用推送服务器定时指令，将以x分钟为间隔推送一次')),
         InputNumber(label='定时推次数', name='l4_push_times', value='${l4_push_times}',
                   labelRemark=Remark(shape='circle',
                                      content='设置好后，将按照推送间隔时间推送x此')),        
+        InputNumber(label='当前路径序号', name='l4_number', value='${l4_number}',
+                  labelRemark=Remark(shape='circle',
+                                     content='如果选定了路径，则上传地图优先传这个路径')),        
+
         InputTag(label='求生上传地图用户', name='l4_master', value='${l4_master}',
                  enableBatchAdd=True,
                  placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
                  labelRemark=Remark(shape='circle',
                                     content='在这里加入的用户，才能上传地图')),
 
     ],
```

#### html2text {}

```diff
@@ -37,29 +37,28 @@
 (shape='circle', content='æºå¨äººè¿åå¾çä¸­æå­çå­ä½ã')), Select
 (label='å¾çé£æ ¼', name='l4_style', value='${l4_style}',source='$
 {l4_styles}', labelRemark=Remark(shape='circle',
 content='ä»ä»æ¯æ¹éæ¥è¯¢çé£æ ¼')), Switch
 (label='æ¯å¦ä¼åä¸ä¼ å°å¾', name='l4_only', value='${l4_only}',
 onText='å¼å¯', offText='å³é­', labelRemark=Remark(shape='circle',
 content='å¼å¯æ¶ï¼ä¸ä¼ å°å¾ä¼ä¿è¯ä¼åçº§ï¼ä»èé»ç¢å¶ä»æä»¤')),
-InputTag(label='æ¥è¯¢çè¿ç¨æå¡å¨tag', name='l4_tag', value='${l4_tag}',
-enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='${total_enable}',
-joinValues=False, extractValue=True, labelRemark=Remark(shape='circle',
-content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')), InputNumber
-(label='å®æ¶æ¨éé´éï¼minï¼', name='l4_push_interval', value='$
-{l4_push_interval}', labelRemark=Remark(shape='circle',
+InputNumber(label='å®æ¶æ¨éé´éï¼minï¼', name='l4_push_interval',
+value='${l4_push_interval}', labelRemark=Remark(shape='circle',
 content='è®¾ç½®å¥½åï¼ä½¿ç¨æ¨éæå¡å¨å®æ¶æä»¤ï¼å°ä»¥xåéä¸ºé´éæ¨éä¸æ¬¡')),
 InputNumber(label='å®æ¶æ¨æ¬¡æ°', name='l4_push_times', value='$
 {l4_push_times}', labelRemark=Remark(shape='circle',
-content='è®¾ç½®å¥½åï¼å°æç§æ¨éé´éæ¶é´æ¨éxæ­¤')), InputTag
-(label='æ±çä¸ä¼ å°å¾ç¨æ·', name='l4_master', value='${l4_master}',
-enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='${total_enable}',
-joinValues=False, extractValue=True, labelRemark=Remark(shape='circle',
-content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')), ], actions=[Action
-(label='ä¿å­', level=LevelEnum.success, type='submit'), Action
+content='è®¾ç½®å¥½åï¼å°æç§æ¨éé´éæ¶é´æ¨éxæ­¤')), InputNumber
+(label='å½åè·¯å¾åºå·', name='l4_number', value='${l4_number}',
+labelRemark=Remark(shape='circle',
+content='å¦æéå®äºè·¯å¾ï¼åä¸ä¼ å°å¾ä¼åä¼ è¿ä¸ªè·¯å¾')),
+InputTag(label='æ±çä¸ä¼ å°å¾ç¨æ·', name='l4_master', value='$
+{l4_master}', enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='$
+{total_enable}', joinValues=False, extractValue=True, labelRemark=Remark
+(shape='circle', content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')), ],
+actions=[Action(label='ä¿å­', level=LevelEnum.success, type='submit'), Action
 (label='éç½®', level=LevelEnum.warning, type='reset')] ) upload_map_form =
 Form( title='å¨å±éç½®', name='global_config', api='post:/l4d2/api/
 l4d2_map_config', body=[ InputText(label='æå¡å¨host', name='web_username',
 value='${web_username}', labelRemark=Remark(shape='circle',
 content='127.0.0.1')), InputPassword(label='æå¡å¨', name='web_password',
 value='${web_password}', labelRemark=Remark(shape='circle',
 content='ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã')), InputText
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.6"
+version = "0.5.6.1"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

