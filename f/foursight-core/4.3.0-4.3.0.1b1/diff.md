# Comparing `tmp/foursight_core-4.3.0.tar.gz` & `tmp/foursight_core-4.3.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.3.0.tar", max compression
+gzip compressed data, was "foursight_core-4.3.0.1b1.tar", max compression
```

## Comparing `foursight_core-4.3.0.tar` & `foursight_core-4.3.0.1b1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-06-15 20:06:13.726802 foursight_core-4.3.0/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/app.py
--rw-r--r--   0        0        0   105128 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     5539 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-06-15 20:06:13.734802 foursight_core-4.3.0/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5408 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6629 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6116 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6189 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3196 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9466 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5164 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    81026 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    34216 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-06-15 20:06:13.738802 foursight_core-4.3.0/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1936472 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-06-15 20:06:13.750802 foursight_core-4.3.0/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1604 2023-06-15 20:06:13.750802 foursight_core-4.3.0/pyproject.toml
--rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 foursight_core-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-16 03:29:30.315199 foursight_core-4.3.0.1b1/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-16 03:29:30.323200 foursight_core-4.3.0.1b1/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-06-16 03:29:30.323200 foursight_core-4.3.0.1b1/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-06-16 03:29:30.323200 foursight_core-4.3.0.1b1/foursight_core/app.py
+-rw-r--r--   0        0        0   105329 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2571 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     5541 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5408 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     6629 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6116 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6189 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3196 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9466 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5164 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    81604 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    34216 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1936472 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6330 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1633 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/pyproject.toml
+-rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 foursight_core-4.3.0.1b1/PKG-INFO
```

### Comparing `foursight_core-4.3.0/LICENSE.txt` & `foursight_core-4.3.0.1b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/abstract_connection.py` & `foursight_core-4.3.0.1b1/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/app_utils.py` & `foursight_core-4.3.0.1b1/foursight_core/app_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1830,14 +1830,20 @@
         queued_uuid = self.sqs.send_sqs_messages(queue, environ, [to_send], uuid=uuid)
         # kick off a single check runner lambda
         if invoke_runner is True:
             self.sqs.invoke_check_runner({'sqs_url': queue.url})
         return queued_uuid
 
     def run_check_runner(self, runner_input, propogate=True):
+        print('xyzzy/run_check_runner/enter')
+        print(type(runner_input))
+        print(runner_input)
+        print(type(propogate))
+        print(propogate)
+        # import pdb ; pdb.set_trace()
         """
         Run logic for a check runner. Used to run checks and actions.
 
         runner_input should be a dict containing one
         key: sqs_url that corresponds to the aws url for the queue.
         This function attempts to recieve one message from the standard SQS queue
         using long polling, checks the run dependencies for that check/action, and then
@@ -1872,15 +1878,15 @@
             MaxNumberOfMessages=1,
             VisibilityTimeout=300,
             WaitTimeSeconds=10
         )
         message = response.get('Messages', [{}])[0]
 
         # TODO/2022-12-01/dmichaels: Issue with check not running because not detecting that
-        # dependency # has already run; for example with expset_opf_unique_files_in_experiments
+        # dependency has already run; for example with expset_opf_unique_files_in_experiments
         # depending on expset_opfsets_unique_titles; seems not checking the result in S3 of the
         # depdendency correctly. This is what seems to be returned here if the check has a dependency, e.g.:
         #
         #   [ "data",
         #     "2022-12-02T12:00:17.345942",
         #     "audit_checks/expset_opf_unique_files_in_experiments",
         #     {"primary": true},
```

### Comparing `foursight_core-4.3.0/foursight_core/buckets.py` & `foursight_core-4.3.0.1b1/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/check_schema.py` & `foursight_core-4.3.0.1b1/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/check_utils.py` & `foursight_core-4.3.0.1b1/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.3.0.1b1/foursight_core/checks/access_key_expiration_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         # 2020-06-13/dmichaels: The actual result returned by the portal for this POST is not what
         # seems to be expected; the access_key_id and secret_access_key are not within the @graph
         # array; but handle both cases just in case; maybe that as an older (or newer) API.
         # access_key_res = post_metadata(access_key_req, 'access-keys', key=connection.ff_keys)['@graph'][0]
         access_key_res = post_metadata(access_key_req, 'access-keys', key=connection.ff_keys)
         access_key_id = access_key_res.get('access_key_id')
         secret_access_key = access_key_res.get('secret_access_key')
-        import pdb ; pdb.set_trace()
+        # import pdb ; pdb.set_trace()
         if not access_key_id or not secret_access_key:
             # We will say these must occur in pairs; both at the top level or both within the @graph array.
             graph_item = access_key_res.get('@graph', [{}])[0]
             access_key_id = graph_item.get('access_key_id')
             secret_access_key = graph_item.get('secret_access_key')
         s3_obj = {'secret': secret_access_key, 'key': access_key_id, 'server': s3.url}
         s3.s3_put_secret(json.dumps(s3_obj), kp_name)
```

### Comparing `foursight_core-4.3.0/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.3.0.1b1/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/checks/ecs_checks.py` & `foursight_core-4.3.0.1b1/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.3.0.1b1/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.3.0.1b1/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.3.0.1b1/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/checks/scaling_checks.py` & `foursight_core-4.3.0.1b1/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/checks/test_checks.py` & `foursight_core-4.3.0.1b1/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/decorators.py` & `foursight_core-4.3.0.1b1/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/deploy.py` & `foursight_core-4.3.0.1b1/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/environment.py` & `foursight_core-4.3.0.1b1/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/es_connection.py` & `foursight_core-4.3.0.1b1/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/exceptions.py` & `foursight_core-4.3.0.1b1/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/fs_connection.py` & `foursight_core-4.3.0.1b1/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/identity.py` & `foursight_core-4.3.0.1b1/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/mapping.json` & `foursight_core-4.3.0.1b1/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/package.py` & `foursight_core-4.3.0.1b1/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/auth.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/auth0_config.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/aws_network.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/aws_s3.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/checks.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/cognito.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/encryption.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/envs.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/gac.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/misc_utils.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/react_api.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/react_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -932,28 +932,34 @@
         check_datetime = datetime.datetime.strptime(uuid, "%Y-%m-%dT%H:%M:%S.%f")
         check_datetime = convert_utc_datetime_to_useastern_datetime_string(check_datetime)
         check_results["timestamp"] = check_datetime
         return self.create_success_response(check_results)
 
     def reactapi_checks_history_uuid(self, request: dict, env: str, check: str, uuid: str) -> Response:
         """
-        Called from react_routes for endpoint: GET /{env}/checks/{check}/{uuid}
+        Called from react_routes for endpoint: GET /{env}/checks/{check}/history/{uuid}
         Returns the check result for the given check (name) and uuid.
         Analogous legacy function is app_utils.view_foursight_check.
         TODO: No need to return array.
         """
         ignored(request)
         body = {}
+        # import pdb ; pdb.set_trace()
         try:
             connection = app.core.init_connection(env)
         except Exception:
             connection = None
         if connection:
             check_result = app.core.CheckResult(connection, check)
             if check_result:
+                # This gets the result from S3, for example:
+                # s3://cgap-kmp-main-foursight-cgap-supertest-results/access_key_status/2023-06-15T10:00:21.205768.json
+                # where access_key_status is the check (name) and 2023-06-15T10:00:21.205768 is the uuid;
+                # and cgap-kmp-main-foursight-cgap-supertest-results is the bucket name which is from our environment.
+                # import pdb ; pdb.set_trace()
                 data = check_result.get_result_by_uuid(uuid)
                 if data is None:
                     # the check hasn't run. Return a placeholder view
                     data = {
                         'name': check,
                         'uuid': uuid,
                         'status': 'ERROR',  # in this case we just queued a check, so ERROR is ok
@@ -1085,14 +1091,15 @@
         """
         Called from react_routes for endpoint: GET /{env}/checks/{check}/run
         The args string, if any, is assumed to be a Base64 encoded JSON object.
         Kicks off a run for the given check (name).
         Arguments (args) for the request are any of:
         - args: Base-64 encode JSON object containing fields/values appropriate for the check run.
         """
+        # import pdb ; pdb.set_trace()
         ignored(request)
         args = base64_decode_to_json(args) if args else None
         # This turns strings into ints/floats/etc appropriately.
         args = app.core.query_params_to_literals(args)
         queued_uuid = app.core.queue_check(env, check, args)
         return self.create_success_response({"check": check, "env": env, "uuid": queued_uuid})
 
@@ -1100,14 +1107,15 @@
         """
         Called from react_routes for endpoint: GET /{env}/checks/action/{action}/run
         The args string, if any, is assumed to be a Base64 encoded JSON object.
         Kicks off a run for the given action (name).
         Arguments (args) for the request are any of:
         - args: Base-64 encode JSON object containing fields/values appropriate for the action run.
         """
+        # import pdb ; pdb.set_trace()
         ignored(request)
         args = base64_decode_to_json(args) if args else {}
         # This turns strings into ints/floats/etc appropriately.
         args = app.core.query_params_to_literals(args)
         queued_uuid = app.core.queue_action(env, action, args)
         return self.create_success_response({"action": action, "env": env, "uuid": queued_uuid})
```

### Comparing `foursight_core-4.3.0/foursight_core/react/api/react_api_base.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/react_routes.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/react_ui.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.3.0.1b1/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/ui/index.html` & `foursight_core-4.3.0.1b1/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.3.0.1b1/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.3.0.1b1/foursight_core/react/ui/static/js/main.js`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/route_prefixes.py` & `foursight_core-4.3.0.1b1/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/routes.py` & `foursight_core-4.3.0.1b1/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/run_result.py` & `foursight_core-4.3.0.1b1/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/s3_connection.py` & `foursight_core-4.3.0.1b1/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/schedule_decorator.py` & `foursight_core-4.3.0.1b1/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.3.0.1b1/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.3.0.1b1/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/sqs_utils.py` & `foursight_core-4.3.0.1b1/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/stage.py` & `foursight_core-4.3.0.1b1/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/templates/base.html` & `foursight_core-4.3.0.1b1/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/templates/header.html` & `foursight_core-4.3.0.1b1/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/templates/history.html` & `foursight_core-4.3.0.1b1/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/templates/info.html` & `foursight_core-4.3.0.1b1/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/templates/unused.html` & `foursight_core-4.3.0.1b1/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/templates/user.html` & `foursight_core-4.3.0.1b1/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/templates/users.html` & `foursight_core-4.3.0.1b1/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/templates/view_checks.html` & `foursight_core-4.3.0.1b1/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/foursight_core/templates/view_groups.html` & `foursight_core-4.3.0.1b1/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0/pyproject.toml` & `foursight_core-4.3.0.1b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.3.0"
+version = "4.3.0.1b1"  # TODO: To become 4.4.0
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.3.0/PKG-INFO` & `foursight_core-4.3.0.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.3.0
+Version: 4.3.0.1b1
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

