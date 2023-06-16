# Comparing `tmp/foursight_core-4.3.0.1b1.tar.gz` & `tmp/foursight_core-4.3.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.3.0.1b1.tar", max compression
+gzip compressed data, was "foursight_core-4.3.0.1b2.tar", max compression
```

## Comparing `foursight_core-4.3.0.1b1.tar` & `foursight_core-4.3.0.1b2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-06-16 03:29:30.315199 foursight_core-4.3.0.1b1/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-16 03:29:30.323200 foursight_core-4.3.0.1b1/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-06-16 03:29:30.323200 foursight_core-4.3.0.1b1/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-06-16 03:29:30.323200 foursight_core-4.3.0.1b1/foursight_core/app.py
--rw-r--r--   0        0        0   105329 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     5541 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5408 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6629 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6116 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6189 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3196 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9466 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5164 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    81604 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    34216 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-06-16 03:29:30.327200 foursight_core-4.3.0.1b1/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1936472 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-06-16 03:29:30.339200 foursight_core-4.3.0.1b1/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1633 2023-06-16 03:29:30.343201 foursight_core-4.3.0.1b1/pyproject.toml
--rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 foursight_core-4.3.0.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-16 18:59:15.664258 foursight_core-4.3.0.1b2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-16 18:59:15.668258 foursight_core-4.3.0.1b2/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-06-16 18:59:15.668258 foursight_core-4.3.0.1b2/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-06-16 18:59:15.668258 foursight_core-4.3.0.1b2/foursight_core/app.py
+-rw-r--r--   0        0        0   105657 2023-06-16 18:59:15.668258 foursight_core-4.3.0.1b2/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2611 2023-06-16 18:59:15.668258 foursight_core-4.3.0.1b2/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-06-16 18:59:15.668258 foursight_core-4.3.0.1b2/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-06-16 18:59:15.668258 foursight_core-4.3.0.1b2/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-06-16 18:59:15.668258 foursight_core-4.3.0.1b2/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-06-16 18:59:15.668258 foursight_core-4.3.0.1b2/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     5667 2023-06-16 18:59:15.668258 foursight_core-4.3.0.1b2/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-06-16 18:59:15.668258 foursight_core-4.3.0.1b2/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-06-16 18:59:15.668258 foursight_core-4.3.0.1b2/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5408 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     6629 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3093 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6116 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6189 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3196 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9466 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5164 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    81643 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    34216 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-06-16 18:59:15.672258 foursight_core-4.3.0.1b2/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1936472 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/routes.py
+-rw-r--r--   0        0        0    22481 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6389 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5886 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1636 2023-06-16 18:59:15.684258 foursight_core-4.3.0.1b2/pyproject.toml
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 foursight_core-4.3.0.1b2/PKG-INFO
```

### Comparing `foursight_core-4.3.0.1b1/LICENSE.txt` & `foursight_core-4.3.0.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/abstract_connection.py` & `foursight_core-4.3.0.1b2/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/app_utils.py` & `foursight_core-4.3.0.1b2/foursight_core/app_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1864,18 +1864,22 @@
         Args:
             runner_input (dict): body of SQS message
             propogate (bool): if True (default), invoke another check runner lambda
 
         Returns:
             dict: run result if something was run, else None
         """
+        # FYI the runner_input argument is a dict that looks something like this (2023-06-16):
+        # {'sqs_url': 'https://sqs.us-east-1.amazonaws.com/466564410312/foursight-cgap-prod-check_queue'}
+        # and the propogate arguments is a bootstrap.LambdaContext that instance.
         sqs_url = runner_input.get('sqs_url')
         if not sqs_url:
             return
-        client = boto3.client('sqs')
+        client = SQS.get_sqs_boto_client()
+        # import pdb ; pdb.set_trace()
         response = client.receive_message(
             QueueUrl=sqs_url,
             AttributeNames=['MessageGroupId'],
             MaxNumberOfMessages=1,
             VisibilityTimeout=300,
             WaitTimeSeconds=10
         )
```

### Comparing `foursight_core-4.3.0.1b1/foursight_core/buckets.py` & `foursight_core-4.3.0.1b2/foursight_core/buckets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import boto3
 import json
-
+from dcicutils.boto_s3 import boto_s3_client
 from dcicutils.misc_utils import ignored
 
 
 class Buckets(object):
     """create and configure buckets for foursight"""
 
     prefix = 'placeholder_prefix'  # replace w/ e.g. 'foursight-cgap'
@@ -42,23 +42,23 @@
     def es_url(cls, env):
         ignored(env)
         # replace this with the correct url in the child class
         # e.g. "https://search-cgap-testing-6-8-vo4mdkmkshvmyddc65ux7dtaou.us-east-1.es.amazonaws.com"
         return 'https://placeholder_url'
 
     def create_buckets(self):
-        s3 = boto3.client('s3')
+        s3 = boto_s3_client()
         for bucket in self.bucket_names:
             param = {'Bucket': bucket, 'ACL': self.default_acl}
             if self.region != 'us-east-1':
                 param.update({'CreateBucketConfiguration': {'LocationConstraint': self.region}})
             s3.create_bucket(**param)
 
     def configure_env_bucket(self):
-        s3 = boto3.client('s3')
+        s3 = boto_s3_client()
         try:
             s3.head_bucket(self.env_bucket)  # check if bucket exists
         except Exception as e:
             if 'NoSuchBucket' in str(e):
                 print("first create buckets! %s" % str(e))
         for env in self.envs:
             content = {"fourfront": self.ff_url(env),
```

### Comparing `foursight_core-4.3.0.1b1/foursight_core/check_schema.py` & `foursight_core-4.3.0.1b2/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/check_utils.py` & `foursight_core-4.3.0.1b2/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.3.0.1b2/foursight_core/checks/access_key_expiration_detection.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,17 @@
         emit warning and error eventually as it gets closer. Once these keys expire
         (every 90 days), foursight and tibanna will no longer function.
     """
     check = CheckResult(connection, 'access_key_status')
     check.action = 'refresh_access_keys'
     # TOOD: Figure this out ... Seems like, both from this code and what we are seeing in the actual action history,
     # that the refresh action is running everday; we only want to run a refresh if the access is expiring very soon.
-    check.allow_action = True  # always allow refresh
+    # Always allow refresh
+    # TODO: But I think if we do not want the action to run automatically then set check.action to None. 
+    check.allow_action = True
     fs_user_email, fs_user_kp = 'foursight.app@gmail.com', 'access_key_foursight'
     user_props = get_metadata(f'/users/{fs_user_email}?datastore=database', key=connection.ff_keys)
     user_uuid = user_props['uuid']
     access_keys = search_metadata(f'/search/?type=AccessKey&description={fs_user_kp}&user.uuid={user_uuid}'
                                   f'&sort=-date_created', key=connection.ff_keys)
     most_recent_key = access_keys[0]  # should always be present if deploy has run
     # date format: 2022-07-05T01:01:43.498347+00:00 (isoformat)
@@ -37,19 +39,21 @@
         check.brief_output = check.full_output = check.summary
         return check
     elif now > three_weeks_to_expiration:
         check.status = 'WARN'
         check.summary = (f'Application access keys will expire in less than 21 days! Please run'
                          f' the deployment action soon')
         check.brief_output = check.full_output = check.summary
+        check.action = None
         return check
     else:
         check.status = 'PASS'
         check.summary = (f'Application access keys expiration is more than 3 weeks away. All good.'
                          f' Expiration date: {expiration_date}')
+        check.action = None
         return check
 
 
 @action_function()
 def refresh_access_keys(connection, **kwargs):
     """ Triggers a refresh of the 3 admin keys, previously run through the portal """
     action = ActionResult(connection, 'refresh_access_keys')
@@ -74,15 +78,14 @@
         # 2020-06-13/dmichaels: The actual result returned by the portal for this POST is not what
         # seems to be expected; the access_key_id and secret_access_key are not within the @graph
         # array; but handle both cases just in case; maybe that as an older (or newer) API.
         # access_key_res = post_metadata(access_key_req, 'access-keys', key=connection.ff_keys)['@graph'][0]
         access_key_res = post_metadata(access_key_req, 'access-keys', key=connection.ff_keys)
         access_key_id = access_key_res.get('access_key_id')
         secret_access_key = access_key_res.get('secret_access_key')
-        # import pdb ; pdb.set_trace()
         if not access_key_id or not secret_access_key:
             # We will say these must occur in pairs; both at the top level or both within the @graph array.
             graph_item = access_key_res.get('@graph', [{}])[0]
             access_key_id = graph_item.get('access_key_id')
             secret_access_key = graph_item.get('secret_access_key')
         s3_obj = {'secret': secret_access_key, 'key': access_key_id, 'server': s3.url}
         s3.s3_put_secret(json.dumps(s3_obj), kp_name)
```

### Comparing `foursight_core-4.3.0.1b1/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.3.0.1b2/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/checks/ecs_checks.py` & `foursight_core-4.3.0.1b2/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.3.0.1b2/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.3.0.1b2/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.3.0.1b2/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/checks/scaling_checks.py` & `foursight_core-4.3.0.1b2/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/checks/test_checks.py` & `foursight_core-4.3.0.1b2/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/decorators.py` & `foursight_core-4.3.0.1b2/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/deploy.py` & `foursight_core-4.3.0.1b2/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/environment.py` & `foursight_core-4.3.0.1b2/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/es_connection.py` & `foursight_core-4.3.0.1b2/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/exceptions.py` & `foursight_core-4.3.0.1b2/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/fs_connection.py` & `foursight_core-4.3.0.1b2/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/identity.py` & `foursight_core-4.3.0.1b2/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/mapping.json` & `foursight_core-4.3.0.1b2/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/package.py` & `foursight_core-4.3.0.1b2/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/auth.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/auth0_config.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/aws_network.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/aws_s3.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/aws_s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import boto3
 import logging
 from typing import Optional
 from .datetime_utils import convert_utc_datetime_to_useastern_datetime_string
+from dcicutils.boto_s3 import boto_s3_client, boto_s3_resource
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 class AwsS3:
 
     @classmethod
     def get_buckets(cls) -> list:
         results = []
         try:
-            s3 = boto3.resource("s3")
+            s3 = boto_s3_resource()
             results = sorted([bucket.name for bucket in s3.buckets.all()])
         except Exception as e:
             logger.error(f"Exception getting S3 bucket list: {e}")
         return results
 
     @classmethod
     def get_bucket_keys(cls, bucket_name: str) -> list:
         results = []
         try:
-            s3 = boto3.client("s3")
+            s3 = boto_s3_client()
             bucket_keys = s3.list_objects(Bucket=bucket_name)
             if bucket_keys:
                 bucket_keys = bucket_keys.get("Contents")
                 if bucket_keys:
                     for bucket_key in sorted(bucket_keys, key=lambda item: item["Key"]):
                         results.append({
                             "key": bucket_key["Key"],
@@ -50,15 +51,15 @@
         if bucket.endswith("-envs"):
             return True
         return False
 
     @classmethod
     def _get_bucket_key_content_size(cls, bucket_name: str, bucket_key_name) -> int:
         try:
-            s3 = boto3.client('s3')
+            s3 = boto_s3_client()
             response = s3.head_object(Bucket=bucket_name, Key=bucket_key_name)
             size = response['ContentLength']
             return size
         except Exception as e:
             return -1
 
     @classmethod
@@ -73,12 +74,12 @@
 
     @classmethod
     def get_bucket_key_contents(cls, bucket_name: str, bucket_key_name) -> Optional[list]:
         try:
             size = cls._get_bucket_key_content_size(bucket_name, bucket_key_name)
             if size <= 0 or not cls._may_look_at_key_content(bucket_name, bucket_key_name, size):
                 return None
-            s3 = boto3.resource("s3")
+            s3 = boto_s3_resource()
             s3_object = s3.Object(bucket_name, bucket_key_name)
             return s3_object.get()["Body"].read().decode("utf-8")
         except Exception as e:
             logger.error(f"Exception getting S3 key content: {e}")
```

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/checks.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/cognito.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/encryption.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/envs.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/gac.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/misc_utils.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/react_api.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/react_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -937,14 +937,15 @@
     def reactapi_checks_history_uuid(self, request: dict, env: str, check: str, uuid: str) -> Response:
         """
         Called from react_routes for endpoint: GET /{env}/checks/{check}/history/{uuid}
         Returns the check result for the given check (name) and uuid.
         Analogous legacy function is app_utils.view_foursight_check.
         TODO: No need to return array.
         """
+        # import pdb ; pdb.set_trace()
         ignored(request)
         body = {}
         # import pdb ; pdb.set_trace()
         try:
             connection = app.core.init_connection(env)
         except Exception:
             connection = None
```

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/react_api_base.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/react_routes.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/react_ui.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.3.0.1b2/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/ui/index.html` & `foursight_core-4.3.0.1b2/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.3.0.1b2/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.3.0.1b2/foursight_core/react/ui/static/js/main.js`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/route_prefixes.py` & `foursight_core-4.3.0.1b2/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/routes.py` & `foursight_core-4.3.0.1b2/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/run_result.py` & `foursight_core-4.3.0.1b2/foursight_core/run_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,15 @@
         Used to get the uuid, status, and kwargs for a specific check.
         Results are ordered by uuid (timestamped) and sliced from start to limit.
         Probably only called from app_utils.get_foursight_history.
         after_date is an optional datetime object, if provided only the history
         results after that point will be returned.
         Returns a list of lists (inner lists: [status, kwargs])
         """
+        # import pdb ; pdb.set_trace()
         if self.es:
             history, total = self.connections['es'].get_result_history(self.name, start, limit, sort)
 
             def wrapper(obj):
                 filename = obj.get('_id')
                 if filename is None:
                     filename = obj.get('name') + '/' + obj.get('kwargs').get('uuid') + '.json'
```

### Comparing `foursight_core-4.3.0.1b1/foursight_core/s3_connection.py` & `foursight_core-4.3.0.1b2/foursight_core/s3_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 import json
 import boto3
 import datetime
 import logging
 from foursight_core.abstract_connection import AbstractConnection
+from dcicutils.boto_s3 import boto_s3_client, boto_s3_resource
 from dcicutils.misc_utils import full_class_name
 
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 class S3Connection(AbstractConnection):
     def __init__(self, bucket_name):
-        self.client = boto3.client('s3')
-        self.resource = boto3.resource('s3')
+        self.client = boto_s3_client()
+        self.resource = boto_s3_resource()
         self.cw = boto3.client('cloudwatch')  # for s3 bucket stats
         self.bucket = bucket_name
         self.location = 'us-east-1'
         self.encryption = os.environ.get('S3_ENCRYPT_KEY_ID')
         # create the bucket if it doesn't exist
         self.head_info = self.test_connection()
         self.status_code = self.head_info.get('ResponseMetadata', {}).get("HTTPStatusCode", 404)
```

### Comparing `foursight_core-4.3.0.1b1/foursight_core/schedule_decorator.py` & `foursight_core-4.3.0.1b2/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.3.0.1b2/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.3.0.1b2/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/sqs_utils.py` & `foursight_core-4.3.0.1b2/foursight_core/sqs_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 import boto3
-import json
-
 from datetime import datetime
+import json
+import os
 from dcicutils.misc_utils import ignored
 from foursight_core.stage import Stage
 
 
 class SQS(object):
     """
     class SQS is a collection of utils related to Foursight queues
     """
 
     def __init__(self, foursight_prefix):
         self.stage = Stage(foursight_prefix)
 
+    @staticmethod
+    def get_sqs_boto_client():
+        sqs_url_from_env = os.environ.get("SQS_URL")
+        if sqs_url_from_env:
+            return boto3.client("sqs", endpoint_url=sqs_url_from_env)
+        return boto3.client("sqs")
+
+    @staticmethod
+    def get_sqs_boto_resource():
+        sqs_url_from_env = os.environ.get("SQS_URL")
+        if sqs_url_from_env:
+            return boto3.resource("sqs", endpoint_url=sqs_url_from_env)
+        return boto3.resource("sqs")
+
     def invoke_check_runner(self, runner_input):
         """
         Simple function to invoke the next check_runner lambda with runner_input
         (dict containing {'sqs_url': <str>})
         """
         client = boto3.client('lambda')
         # InvocationType='Event' makes asynchronous
@@ -47,15 +61,15 @@
 
         Returns:
             None
         """
         sqs_url = runner_input.get('sqs_url')
         if not sqs_url or not receipt:
             return
-        client = boto3.client('sqs')
+        client = self.get_sqs_boto_client()
         client.delete_message(
             QueueUrl=sqs_url,
             ReceiptHandle=receipt
         )
         if propogate is True:
             self.invoke_check_runner(runner_input)
 
@@ -76,29 +90,29 @@
 
         Returns:
             None
         """
         sqs_url = runner_input.get('sqs_url')
         if not sqs_url or not receipt:
             return
-        client = boto3.client('sqs')
+        client = self.get_sqs_boto_client()
         client.change_message_visibility(
             QueueUrl=sqs_url,
             ReceiptHandle=receipt,
             VisibilityTimeout=15
         )
         if propogate is True:
             self.invoke_check_runner(runner_input)
 
     def get_sqs_queue(self):
         """
         Returns boto3 sqs resource
         """
         queue_name = self.stage.get_queue_name()
-        sqs = boto3.resource('sqs')
+        sqs = self.get_sqs_boto_resource()
         try:
             queue = sqs.get_queue_by_name(QueueName=queue_name)
         except Exception:
             queue = sqs.create_queue(
                 QueueName=queue_name,
                 Attributes={
                     'VisibilityTimeout': '900',
@@ -139,15 +153,15 @@
         """
         Returns a dict of the desired attributes form the queue with given url
         """
         backup = {
             'ApproximateNumberOfMessages': 'ERROR',
             'ApproximateNumberOfMessagesNotVisible': 'ERROR'
         }
-        client = boto3.client('sqs')
+        client = cls.get_sqs_boto_client()
         try:
             result = client.get_queue_attributes(
                 QueueUrl=sqs_url,
                 AttributeNames=[
                     'ApproximateNumberOfMessages',
                     'ApproximateNumberOfMessagesNotVisible'
                 ]
```

### Comparing `foursight_core-4.3.0.1b1/foursight_core/stage.py` & `foursight_core-4.3.0.1b2/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/templates/base.html` & `foursight_core-4.3.0.1b2/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/templates/header.html` & `foursight_core-4.3.0.1b2/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/templates/history.html` & `foursight_core-4.3.0.1b2/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/templates/info.html` & `foursight_core-4.3.0.1b2/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/templates/unused.html` & `foursight_core-4.3.0.1b2/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/templates/user.html` & `foursight_core-4.3.0.1b2/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/templates/users.html` & `foursight_core-4.3.0.1b2/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/templates/view_checks.html` & `foursight_core-4.3.0.1b2/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/foursight_core/templates/view_groups.html` & `foursight_core-4.3.0.1b2/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.1b1/pyproject.toml` & `foursight_core-4.3.0.1b2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.3.0.1b1"  # TODO: To become 4.4.0
+version = "4.3.0.1b2"  # TODO: To become 4.4.0
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.10"
 click = "^7.1.2"
 cron-descriptor = "^1.2.31"
 cryptography = "39.0.2" # Required for AWS Cognito JWT decode (PyJWKClient)
-dcicutils = "^7.5.0"
+dcicutils = "7.5.1.1b1"
 elasticsearch = "7.13.4"
 elasticsearch-dsl = "^7.0.0"
 geocoder = "1.38.1"
 gitpython = "^3.1.2"
 google = "^3.0.0"
 google-auth-oauthlib = "^0.7.0"
 google-api-python-client = "^1.12.5"
```

### Comparing `foursight_core-4.3.0.1b1/PKG-INFO` & `foursight_core-4.3.0.1b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.3.0.1b1
+Version: 4.3.0.1b2
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: cron-descriptor (>=1.2.31,<2.0.0)
 Requires-Dist: cryptography (==39.0.2)
-Requires-Dist: dcicutils (>=7.5.0,<8.0.0)
+Requires-Dist: dcicutils (==7.5.1.1b1)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: google-auth-oauthlib (>=0.7.0,<0.8.0)
```

