# Comparing `tmp/etu-fastapi-frame-1.1.0.tar.gz` & `tmp/etu-fastapi-frame-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etu-fastapi-frame-1.1.0.tar", last modified: Fri Jun 16 06:40:17 2023, max compression
+gzip compressed data, was "etu-fastapi-frame-1.2.0.tar", last modified: Fri Jun 16 07:10:10 2023, max compression
```

## Comparing `etu-fastapi-frame-1.1.0.tar` & `etu-fastapi-frame-1.2.0.tar`

### file list

```diff
@@ -1,126 +1,128 @@
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.232800 etu-fastapi-frame-1.1.0/
--rw-r--r--   0 jieay      (501) staff       (20)     1081 2023-06-01 03:33:58.000000 etu-fastapi-frame-1.1.0/LICENSE
--rw-r--r--   0 jieay      (501) staff       (20)       45 2023-06-16 02:14:01.000000 etu-fastapi-frame-1.1.0/MANIFEST.in
--rw-r--r--   0 jieay      (501) staff       (20)     1768 2023-06-16 06:40:17.232659 etu-fastapi-frame-1.1.0/PKG-INFO
--rw-r--r--   0 jieay      (501) staff       (20)     1007 2023-06-16 03:28:15.000000 etu-fastapi-frame-1.1.0/README.md
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.222190 etu-fastapi-frame-1.1.0/etu_fastapi_frame/
--rw-r--r--   0 jieay      (501) staff       (20)      120 2023-06-16 06:30:07.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/__init__.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.219973 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.220837 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.223430 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/
--rw-r--r--   0 jieay      (501) staff       (20)       43 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/.gitignore
--rw-r--r--   0 jieay      (501) staff       (20)      357 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/Dockerfile
--rw-r--r--   0 jieay      (501) staff       (20)     1333 2023-06-16 03:21:12.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/README.md
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.223898 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/__init__.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.224139 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/__init__.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.224381 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)      415 2023-06-16 06:26:41.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/api.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.224822 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)     1466 2023-06-16 06:22:39.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/demos.py
--rw-r--r--   0 jieay      (501) staff       (20)     4319 2023-06-15 09:59:04.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/login.py
--rw-r--r--   0 jieay      (501) staff       (20)     4984 2023-06-15 10:14:00.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/users.py
--rw-r--r--   0 jieay      (501) staff       (20)     3336 2023-06-15 07:52:36.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/deps.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.225457 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/
--rw-r--r--   0 jieay      (501) staff       (20)      362 2023-06-13 04:05:05.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)     3200 2023-06-15 09:33:18.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/config.py
--rw-r--r--   0 jieay      (501) staff       (20)     2551 2023-06-13 02:01:49.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/log.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.225928 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-09 02:16:03.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)     1398 2023-06-15 09:31:23.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/global_authorized.py
--rw-r--r--   0 jieay      (501) staff       (20)     1905 2023-06-15 05:28:11.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/global_request.py
--rw-r--r--   0 jieay      (501) staff       (20)     1620 2023-06-13 02:00:45.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/log_formatter.py
--rw-r--r--   0 jieay      (501) staff       (20)     1025 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/security.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.226282 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/
--rw-r--r--   0 jieay      (501) staff       (20)     1490 2023-06-13 04:03:00.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)     2193 2023-06-15 09:32:48.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/base.py
--rw-r--r--   0 jieay      (501) staff       (20)     1921 2023-06-15 09:32:40.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/crud_user.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.226827 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)      260 2023-06-08 14:38:15.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/base.py
--rw-r--r--   0 jieay      (501) staff       (20)      387 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/base_class.py
--rw-r--r--   0 jieay      (501) staff       (20)     1080 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/init_db.py
--rw-r--r--   0 jieay      (501) staff       (20)      364 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/session.py
--rw-r--r--   0 jieay      (501) staff       (20)      603 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/initial_data.py
--rw-r--r--   0 jieay      (501) staff       (20)     1522 2023-06-16 04:29:57.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/main.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.227043 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/models/
--rw-r--r--   0 jieay      (501) staff       (20)     1945 2023-06-13 04:03:51.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/models/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)      524 2023-06-15 08:43:54.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/models/user.py
--rw-r--r--   0 jieay      (501) staff       (20)      399 2023-06-09 02:05:19.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/routers.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.227583 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/
--rw-r--r--   0 jieay      (501) staff       (20)     1951 2023-06-16 06:27:16.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)      363 2023-06-16 06:21:17.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/demos.py
--rw-r--r--   0 jieay      (501) staff       (20)      159 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/msg.py
--rw-r--r--   0 jieay      (501) staff       (20)      349 2023-06-15 09:55:12.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/token.py
--rw-r--r--   0 jieay      (501) staff       (20)      836 2023-06-15 08:44:27.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/user.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.227694 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/tests/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/tests/__init__.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.227912 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/utils/
--rw-r--r--   0 jieay      (501) staff       (20)      363 2023-06-13 04:05:53.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/utils/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)     1357 2023-06-15 07:31:12.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/utils/common.py
--rw-r--r--   0 jieay      (501) staff       (20)      478 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/fastapi-all.txt
--rw-r--r--   0 jieay      (501) staff       (20)      204 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/requirements.txt
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.228447 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/
--rw-r--r--   0 jieay      (501) staff       (20)       43 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/.gitignore
--rw-r--r--   0 jieay      (501) staff       (20)      357 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/Dockerfile
--rw-r--r--   0 jieay      (501) staff       (20)     1224 2023-06-16 03:18:51.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/README.md
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.228767 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/__init__.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.228979 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/__init__.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.229194 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)      271 2023-06-13 07:35:17.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/api.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.229528 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)     1466 2023-06-16 06:22:39.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/demos.py
--rw-r--r--   0 jieay      (501) staff       (20)     1645 2023-06-15 05:12:49.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/login.py
--rw-r--r--   0 jieay      (501) staff       (20)     2972 2023-06-15 05:13:52.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/deps.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.230134 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)     1889 2023-06-15 07:25:27.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/config.py
--rw-r--r--   0 jieay      (501) staff       (20)     2551 2023-06-13 02:01:49.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/log.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.230604 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-09 02:16:03.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)     1386 2023-06-15 02:27:17.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/global_authorized.py
--rw-r--r--   0 jieay      (501) staff       (20)     1905 2023-06-15 05:28:11.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/global_request.py
--rw-r--r--   0 jieay      (501) staff       (20)     1620 2023-06-13 02:00:45.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/log_formatter.py
--rw-r--r--   0 jieay      (501) staff       (20)     1175 2023-06-15 04:38:02.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/security.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.231371 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/
--rw-r--r--   0 jieay      (501) staff       (20)       97 2023-06-13 04:17:07.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)      938 2023-06-14 02:58:07.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/base.py
--rw-r--r--   0 jieay      (501) staff       (20)      747 2023-06-15 10:17:29.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/db_user.json
--rw-r--r--   0 jieay      (501) staff       (20)      712 2023-06-15 10:17:00.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/db_user_debug.json
--rw-r--r--   0 jieay      (501) staff       (20)     4802 2023-06-14 07:45:44.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/session.py
--rw-r--r--   0 jieay      (501) staff       (20)      760 2023-06-15 10:17:27.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/sync_org_user.py
--rw-r--r--   0 jieay      (501) staff       (20)      326 2023-06-14 08:14:13.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/user.py
--rw-r--r--   0 jieay      (501) staff       (20)     1725 2023-06-16 04:43:48.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/main.py
--rw-r--r--   0 jieay      (501) staff       (20)      399 2023-06-09 02:06:57.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/routers.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.231918 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/
--rw-r--r--   0 jieay      (501) staff       (20)     1950 2023-06-16 06:21:34.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)      363 2023-06-16 06:21:17.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/demos.py
--rw-r--r--   0 jieay      (501) staff       (20)      159 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/msg.py
--rw-r--r--   0 jieay      (501) staff       (20)      349 2023-06-15 03:01:12.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/token.py
--rw-r--r--   0 jieay      (501) staff       (20)      853 2023-06-14 08:15:41.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/user.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.232021 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/tests/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/tests/__init__.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.232459 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/
--rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/__init__.py
--rw-r--r--   0 jieay      (501) staff       (20)     4903 2023-06-15 10:06:21.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/br_api.py
--rw-r--r--   0 jieay      (501) staff       (20)     1356 2023-06-15 04:54:12.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/common.py
--rw-r--r--   0 jieay      (501) staff       (20)      695 2023-06-15 10:15:07.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/orgauth.py
--rw-r--r--   0 jieay      (501) staff       (20)      478 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/fastapi-all.txt
--rw-r--r--   0 jieay      (501) staff       (20)      127 2023-06-15 07:45:46.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/requirements.txt
--rw-r--r--   0 jieay      (501) staff       (20)     4547 2023-06-16 02:12:46.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame/main.py
-drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 06:40:17.222881 etu-fastapi-frame-1.1.0/etu_fastapi_frame.egg-info/
--rw-r--r--   0 jieay      (501) staff       (20)     1768 2023-06-16 06:40:17.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame.egg-info/PKG-INFO
--rw-r--r--   0 jieay      (501) staff       (20)     5178 2023-06-16 06:40:17.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame.egg-info/SOURCES.txt
--rw-r--r--   0 jieay      (501) staff       (20)        1 2023-06-16 06:40:17.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame.egg-info/dependency_links.txt
--rw-r--r--   0 jieay      (501) staff       (20)       79 2023-06-16 06:40:17.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame.egg-info/entry_points.txt
--rw-r--r--   0 jieay      (501) staff       (20)       18 2023-06-16 06:40:17.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame.egg-info/top_level.txt
--rw-r--r--   0 jieay      (501) staff       (20)        1 2023-06-16 03:38:52.000000 etu-fastapi-frame-1.1.0/etu_fastapi_frame.egg-info/zip-safe
--rw-r--r--   0 jieay      (501) staff       (20)       38 2023-06-16 06:40:17.232841 etu-fastapi-frame-1.1.0/setup.cfg
--rw-r--r--   0 jieay      (501) staff       (20)     1561 2023-06-16 06:29:52.000000 etu-fastapi-frame-1.1.0/setup.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.426234 etu-fastapi-frame-1.2.0/
+-rw-r--r--   0 jieay      (501) staff       (20)     1081 2023-06-01 03:33:58.000000 etu-fastapi-frame-1.2.0/LICENSE
+-rw-r--r--   0 jieay      (501) staff       (20)       45 2023-06-16 02:14:01.000000 etu-fastapi-frame-1.2.0/MANIFEST.in
+-rw-r--r--   0 jieay      (501) staff       (20)     1768 2023-06-16 07:10:10.426081 etu-fastapi-frame-1.2.0/PKG-INFO
+-rw-r--r--   0 jieay      (501) staff       (20)     1007 2023-06-16 03:28:15.000000 etu-fastapi-frame-1.2.0/README.md
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.416020 etu-fastapi-frame-1.2.0/etu_fastapi_frame/
+-rw-r--r--   0 jieay      (501) staff       (20)      120 2023-06-16 07:06:56.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/__init__.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.413807 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.414686 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.417282 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/
+-rw-r--r--   0 jieay      (501) staff       (20)       43 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/.gitignore
+-rw-r--r--   0 jieay      (501) staff       (20)      357 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/Dockerfile
+-rw-r--r--   0 jieay      (501) staff       (20)     1333 2023-06-16 03:21:12.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/README.md
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.417740 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/__init__.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.417961 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/__init__.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.418188 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)      415 2023-06-16 06:26:41.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/api.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.418753 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1466 2023-06-16 06:22:39.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/demos.py
+-rw-r--r--   0 jieay      (501) staff       (20)      358 2023-06-16 07:00:08.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/health.py
+-rw-r--r--   0 jieay      (501) staff       (20)     4319 2023-06-15 09:59:04.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/login.py
+-rw-r--r--   0 jieay      (501) staff       (20)     4984 2023-06-15 10:14:00.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/users.py
+-rw-r--r--   0 jieay      (501) staff       (20)     3361 2023-06-16 07:02:13.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/deps.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.419224 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/
+-rw-r--r--   0 jieay      (501) staff       (20)      362 2023-06-13 04:05:05.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)     3200 2023-06-15 09:33:18.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/config.py
+-rw-r--r--   0 jieay      (501) staff       (20)     2551 2023-06-13 02:01:49.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/log.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.419655 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-09 02:16:03.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1398 2023-06-15 09:31:23.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/global_authorized.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1905 2023-06-15 05:28:11.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/global_request.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1620 2023-06-13 02:00:45.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/log_formatter.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1025 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/security.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.419993 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/
+-rw-r--r--   0 jieay      (501) staff       (20)     1490 2023-06-13 04:03:00.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)     2193 2023-06-15 09:32:48.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/base.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1921 2023-06-15 09:32:40.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/crud_user.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.420537 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)      260 2023-06-08 14:38:15.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/base.py
+-rw-r--r--   0 jieay      (501) staff       (20)      387 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/base_class.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1080 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/init_db.py
+-rw-r--r--   0 jieay      (501) staff       (20)      364 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/session.py
+-rw-r--r--   0 jieay      (501) staff       (20)      603 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/initial_data.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1522 2023-06-16 04:29:57.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/main.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.420748 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/models/
+-rw-r--r--   0 jieay      (501) staff       (20)     1945 2023-06-13 04:03:51.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/models/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)      524 2023-06-15 08:43:54.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/models/user.py
+-rw-r--r--   0 jieay      (501) staff       (20)      465 2023-06-16 07:01:27.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/routers.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.421295 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/
+-rw-r--r--   0 jieay      (501) staff       (20)     1951 2023-06-16 06:27:16.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)      363 2023-06-16 06:21:17.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/demos.py
+-rw-r--r--   0 jieay      (501) staff       (20)      159 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/msg.py
+-rw-r--r--   0 jieay      (501) staff       (20)      349 2023-06-15 09:55:12.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/token.py
+-rw-r--r--   0 jieay      (501) staff       (20)      836 2023-06-15 08:44:27.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/user.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.421401 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/tests/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/tests/__init__.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.421607 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/utils/
+-rw-r--r--   0 jieay      (501) staff       (20)      363 2023-06-13 04:05:53.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/utils/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1357 2023-06-15 07:31:12.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/utils/common.py
+-rw-r--r--   0 jieay      (501) staff       (20)      478 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/fastapi-all.txt
+-rw-r--r--   0 jieay      (501) staff       (20)      204 2023-06-08 14:35:28.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/requirements.txt
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.422134 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/
+-rw-r--r--   0 jieay      (501) staff       (20)       43 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/.gitignore
+-rw-r--r--   0 jieay      (501) staff       (20)      357 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/Dockerfile
+-rw-r--r--   0 jieay      (501) staff       (20)     1224 2023-06-16 03:18:51.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/README.md
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.422447 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/__init__.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.422660 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/__init__.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.422874 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)      271 2023-06-13 07:35:17.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/api.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.423295 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1466 2023-06-16 06:22:39.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/demos.py
+-rw-r--r--   0 jieay      (501) staff       (20)      358 2023-06-16 07:00:08.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/health.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1645 2023-06-15 05:12:49.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/login.py
+-rw-r--r--   0 jieay      (501) staff       (20)     2997 2023-06-16 07:02:36.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/deps.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.423712 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1889 2023-06-15 07:25:27.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/config.py
+-rw-r--r--   0 jieay      (501) staff       (20)     2551 2023-06-13 02:01:49.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/log.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.424134 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-09 02:16:03.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1386 2023-06-15 02:27:17.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/global_authorized.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1905 2023-06-15 05:28:11.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/global_request.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1620 2023-06-13 02:00:45.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/log_formatter.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1175 2023-06-15 04:38:02.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/security.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.424864 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/
+-rw-r--r--   0 jieay      (501) staff       (20)       97 2023-06-13 04:17:07.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)      938 2023-06-14 02:58:07.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/base.py
+-rw-r--r--   0 jieay      (501) staff       (20)      747 2023-06-15 10:17:29.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/db_user.json
+-rw-r--r--   0 jieay      (501) staff       (20)      712 2023-06-15 10:17:00.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/db_user_debug.json
+-rw-r--r--   0 jieay      (501) staff       (20)     4802 2023-06-14 07:45:44.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/session.py
+-rw-r--r--   0 jieay      (501) staff       (20)      760 2023-06-15 10:17:27.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/sync_org_user.py
+-rw-r--r--   0 jieay      (501) staff       (20)      326 2023-06-14 08:14:13.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/user.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1725 2023-06-16 04:43:48.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/main.py
+-rw-r--r--   0 jieay      (501) staff       (20)      465 2023-06-16 07:03:37.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/routers.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.425374 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/
+-rw-r--r--   0 jieay      (501) staff       (20)     1950 2023-06-16 06:21:34.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)      363 2023-06-16 06:21:17.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/demos.py
+-rw-r--r--   0 jieay      (501) staff       (20)      159 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/msg.py
+-rw-r--r--   0 jieay      (501) staff       (20)      349 2023-06-15 03:01:12.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/token.py
+-rw-r--r--   0 jieay      (501) staff       (20)      853 2023-06-14 08:15:41.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/user.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.425479 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/tests/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/tests/__init__.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.425891 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/
+-rw-r--r--   0 jieay      (501) staff       (20)       96 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/__init__.py
+-rw-r--r--   0 jieay      (501) staff       (20)     4903 2023-06-15 10:06:21.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/br_api.py
+-rw-r--r--   0 jieay      (501) staff       (20)     1356 2023-06-15 04:54:12.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/common.py
+-rw-r--r--   0 jieay      (501) staff       (20)      695 2023-06-15 10:15:07.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/orgauth.py
+-rw-r--r--   0 jieay      (501) staff       (20)      478 2023-06-08 14:43:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/fastapi-all.txt
+-rw-r--r--   0 jieay      (501) staff       (20)      127 2023-06-15 07:45:46.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/requirements.txt
+-rw-r--r--   0 jieay      (501) staff       (20)     4547 2023-06-16 02:12:46.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame/main.py
+drwxr-xr-x   0 jieay      (501) staff       (20)        0 2023-06-16 07:10:10.416728 etu-fastapi-frame-1.2.0/etu_fastapi_frame.egg-info/
+-rw-r--r--   0 jieay      (501) staff       (20)     1768 2023-06-16 07:10:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame.egg-info/PKG-INFO
+-rw-r--r--   0 jieay      (501) staff       (20)     5321 2023-06-16 07:10:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame.egg-info/SOURCES.txt
+-rw-r--r--   0 jieay      (501) staff       (20)        1 2023-06-16 07:10:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame.egg-info/dependency_links.txt
+-rw-r--r--   0 jieay      (501) staff       (20)       79 2023-06-16 07:10:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame.egg-info/entry_points.txt
+-rw-r--r--   0 jieay      (501) staff       (20)       18 2023-06-16 07:10:10.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame.egg-info/top_level.txt
+-rw-r--r--   0 jieay      (501) staff       (20)        1 2023-06-16 03:38:52.000000 etu-fastapi-frame-1.2.0/etu_fastapi_frame.egg-info/zip-safe
+-rw-r--r--   0 jieay      (501) staff       (20)       38 2023-06-16 07:10:10.426273 etu-fastapi-frame-1.2.0/setup.cfg
+-rw-r--r--   0 jieay      (501) staff       (20)     1561 2023-06-16 07:07:01.000000 etu-fastapi-frame-1.2.0/setup.py
```

### Comparing `etu-fastapi-frame-1.1.0/LICENSE` & `etu-fastapi-frame-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/PKG-INFO` & `etu-fastapi-frame-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etu-fastapi-frame
-Version: 1.1.0
+Version: 1.2.0
 Summary: 将EFF脚手架工具，制作成为pip安装包，以方便使用
 Author: Jieay
 Author-email: 1016900854@qq.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `etu-fastapi-frame-1.1.0/README.md` & `etu-fastapi-frame-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/README.md` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/README.md`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/demos.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/demos.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/login.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/login.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/users.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/deps.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/deps.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     :param url_path: url path
     :return: bool
     """
     white_list_exact = [
         "/openapi.json",
         "/login/access-token",
         "/api/access-token",
+        "/health/check",
     ]
     white_list_prefix = [
         "/docs",
         "/redoc",
     ]
     if url_path in white_list_exact:
         return True
```

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/config.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/config.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/log.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/log.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/global_authorized.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/global_authorized.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/global_request.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/global_request.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/log_formatter.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/log_formatter.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/security.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/security.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/__init__.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/__init__.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/base.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/base.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/crud_user.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/crud/crud_user.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/init_db.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/db/init_db.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/initial_data.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/initial_data.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/main.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/main.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/models/__init__.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/models/__init__.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/models/user.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/models/user.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/__init__.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/user.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/schemas/user.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/utils/common.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/cfg/app/utils/common.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/README.md` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/README.md`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/demos.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/demos.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/login.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/login.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/deps.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/api/deps.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     获取白名单
     :param url_path: url path
     :return: bool
     """
     white_list_exact = [
         "/openapi.json",
         "/api/access-token",
+        "/health/check",
     ]
     white_list_prefix = [
         "/docs",
         "/redoc",
     ]
     if url_path in white_list_exact:
         return True
```

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/config.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/config.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/log.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/log.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/global_authorized.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/global_authorized.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/global_request.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/global_request.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/log_formatter.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/log_formatter.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/security.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/core/security.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/base.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/base.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/db_user.json` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/db_user.json`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/db_user_debug.json` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/db_user_debug.json`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/session.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/session.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/sync_org_user.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/db/sync_org_user.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/main.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/main.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/__init__.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/user.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/schemas/user.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/br_api.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/br_api.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/common.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/common.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/orgauth.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/fastapi/0.95.2/ms/app/utils/orgauth.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame/main.py` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame/main.py`

 * *Files identical despite different names*

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame.egg-info/PKG-INFO` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etu-fastapi-frame
-Version: 1.1.0
+Version: 1.2.0
 Summary: 将EFF脚手架工具，制作成为pip安装包，以方便使用
 Author: Jieay
 Author-email: 1016900854@qq.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `etu-fastapi-frame-1.1.0/etu_fastapi_frame.egg-info/SOURCES.txt` & `etu-fastapi-frame-1.2.0/etu_fastapi_frame.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/routers.py
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/__init__.py
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/deps.py
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/__init__.py
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/api.py
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/__init__.py
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/demos.py
+etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/health.py
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/login.py
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/api/api_v1/endpoints/users.py
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/__init__.py
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/config.py
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/log.py
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/security.py
 etu_fastapi_frame/fastapi/0.95.2/cfg/app/core/middleware/__init__.py
@@ -63,14 +64,15 @@
 etu_fastapi_frame/fastapi/0.95.2/ms/app/routers.py
 etu_fastapi_frame/fastapi/0.95.2/ms/app/api/__init__.py
 etu_fastapi_frame/fastapi/0.95.2/ms/app/api/deps.py
 etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/__init__.py
 etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/api.py
 etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/__init__.py
 etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/demos.py
+etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/health.py
 etu_fastapi_frame/fastapi/0.95.2/ms/app/api/api_v1/endpoints/login.py
 etu_fastapi_frame/fastapi/0.95.2/ms/app/core/__init__.py
 etu_fastapi_frame/fastapi/0.95.2/ms/app/core/config.py
 etu_fastapi_frame/fastapi/0.95.2/ms/app/core/log.py
 etu_fastapi_frame/fastapi/0.95.2/ms/app/core/security.py
 etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/__init__.py
 etu_fastapi_frame/fastapi/0.95.2/ms/app/core/middleware/global_authorized.py
```

### Comparing `etu-fastapi-frame-1.1.0/setup.py` & `etu-fastapi-frame-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 except ImportError:
     from distutils.core import setup
 import setuptools
 
 
 setup(
     name='etu-fastapi-frame',  # 包的名字
-    version='1.1.0',  # 版本号
+    version='1.2.0',  # 版本号
     author="Jieay",
     author_email="1016900854@qq.com",
     description='将EFF脚手架工具，制作成为pip安装包，以方便使用',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT License',
     packages=setuptools.find_packages(),  # 包需要引用的文件夹
```

