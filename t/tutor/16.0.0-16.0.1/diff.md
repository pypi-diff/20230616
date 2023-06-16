# Comparing `tmp/tutor-16.0.0.tar.gz` & `tmp/tutor-16.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-16.0.0.tar", last modified: Wed Jun 14 21:51:28 2023, max compression
+gzip compressed data, was "tutor-16.0.1.tar", last modified: Fri Jun 16 10:12:28 2023, max compression
```

## Comparing `tutor-16.0.0.tar` & `tutor-16.0.1.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.019098 tutor-16.0.0/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-14 21:50:41.000000 tutor-16.0.0/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)      121 2023-06-14 21:50:41.000000 tutor-16.0.0/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     6665 2023-06-14 21:51:28.019098 tutor-16.0.0/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     4745 2023-06-14 21:50:41.000000 tutor-16.0.0/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-14 21:50:41.000000 tutor-16.0.0/pyproject.toml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.985764 tutor-16.0.0/requirements/
--rw-r--r--   0 ci        (1000) ci        (1000)       98 2023-06-14 21:50:41.000000 tutor-16.0.0/requirements/base.in
--rw-r--r--   0 ci        (1000) ci        (1000)      340 2023-06-14 21:50:41.000000 tutor-16.0.0/requirements/plugins.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-14 21:51:28.022431 tutor-16.0.0/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     2506 2023-06-14 21:50:41.000000 tutor-16.0.0/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.989098 tutor-16.0.0/tests/
--rw-r--r--   0 ci        (1000) ci        (1000)     2491 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_bindmount.py
--rw-r--r--   0 ci        (1000) ci        (1000)     4172 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_config.py
--rw-r--r--   0 ci        (1000) ci        (1000)    15898 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_env.py
--rw-r--r--   0 ci        (1000) ci        (1000)     3063 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_plugin_indexes.py
--rw-r--r--   0 ci        (1000) ci        (1000)     8279 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_plugins_v0.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2432 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_serialize.py
--rw-r--r--   0 ci        (1000) ci        (1000)    10669 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_utils.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.992431 tutor-16.0.0/tutor/
--rw-r--r--   0 ci        (1000) ci        (1000)     1159 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2546 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/bindmount.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.995764 tutor-16.0.0/tutor/commands/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/__init__.py
--rwxr-xr-x   0 ci        (1000) ci        (1000)     4485 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/cli.py
--rw-r--r--   0 ci        (1000) ci        (1000)    16737 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/compose.py
--rw-r--r--   0 ci        (1000) ci        (1000)     7317 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/config.py
--rw-r--r--   0 ci        (1000) ci        (1000)      794 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/context.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2240 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/dev.py
--rw-r--r--   0 ci        (1000) ci        (1000)    11658 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/images.py
--rw-r--r--   0 ci        (1000) ci        (1000)    10722 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/jobs.py
--rw-r--r--   0 ci        (1000) ci        (1000)    21033 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/k8s.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1772 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/local.py
--rw-r--r--   0 ci        (1000) ci        (1000)     4446 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/mounts.py
--rw-r--r--   0 ci        (1000) ci        (1000)      741 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/params.py
--rw-r--r--   0 ci        (1000) ci        (1000)    13436 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/plugins.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.999098 tutor-16.0.0/tutor/commands/upgrade/
--rw-r--r--   0 ci        (1000) ci        (1000)      185 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/upgrade/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2082 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/upgrade/common.py
--rw-r--r--   0 ci        (1000) ci        (1000)     6047 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/upgrade/compose.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5685 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/upgrade/k8s.py
--rw-r--r--   0 ci        (1000) ci        (1000)     9685 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.999098 tutor-16.0.0/tutor/core/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/core/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.999098 tutor-16.0.0/tutor/core/hooks/
--rw-r--r--   0 ci        (1000) ci        (1000)      292 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/core/hooks/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5707 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/core/hooks/actions.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2929 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/core/hooks/contexts.py
--rw-r--r--   0 ci        (1000) ci        (1000)     9006 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/core/hooks/filters.py
--rw-r--r--   0 ci        (1000) ci        (1000)      638 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/core/hooks/priorities.py
--rw-r--r--   0 ci        (1000) ci        (1000)    17753 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/env.py
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/exceptions.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1213 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/fmt.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.002431 tutor-16.0.0/tutor/hooks/
--rw-r--r--   0 ci        (1000) ci        (1000)      273 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/hooks/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)    24524 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/hooks/catalog.py
--rw-r--r--   0 ci        (1000) ci        (1000)      571 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/images.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5076 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/interactive.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.002431 tutor-16.0.0/tutor/plugins/
--rw-r--r--   0 ci        (1000) ci        (1000)     3802 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/plugins/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      548 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/plugins/base.py
--rw-r--r--   0 ci        (1000) ci        (1000)     6989 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/plugins/indexes.py
--rw-r--r--   0 ci        (1000) ci        (1000)    15218 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/plugins/v0.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2376 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/plugins/v1.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/py.typed
--rw-r--r--   0 ci        (1000) ci        (1000)     1947 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/serialize.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1385 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/tasks.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.005764 tutor-16.0.0/tutor/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.979097 tutor-16.0.0/tutor/templates/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.005764 tutor-16.0.0/tutor/templates/apps/caddy/
--rw-r--r--   0 ci        (1000) ci        (1000)     1989 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/caddy/Caddyfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.005764 tutor-16.0.0/tutor/templates/apps/openedx/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.005764 tutor-16.0.0/tutor/templates/apps/openedx/config/
--rw-r--r--   0 ci        (1000) ci        (1000)     1542 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/config/cms.env.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1787 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/config/lms.env.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.005764 tutor-16.0.0/tutor/templates/apps/openedx/config/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)      673 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/config/partials/auth.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.979097 tutor-16.0.0/tutor/templates/apps/openedx/settings/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.005764 tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      591 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/development.py
--rw-r--r--   0 ci        (1000) ci        (1000)      529 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/production.py
--rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/test.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.009098 tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1132 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/development.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1039 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/production.py
--rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/test.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.009098 tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)    10001 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_all.py
--rw-r--r--   0 ci        (1000) ci        (1000)      924 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_cms.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1450 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_lms.py
--rw-r--r--   0 ci        (1000) ci        (1000)      105 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_test.py
--rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/uwsgi.ini
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.009098 tutor-16.0.0/tutor/templates/apps/permissions/
--rw-r--r--   0 ci        (1000) ci        (1000)      380 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/permissions/setowners.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.009098 tutor-16.0.0/tutor/templates/apps/redis/
--rw-r--r--   0 ci        (1000) ci        (1000)      854 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/redis/redis.conf
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.982431 tutor-16.0.0/tutor/templates/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/
--rw-r--r--   0 ci        (1000) ci        (1000)    12605 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/bin/
--rwxr-xr-x   0 ci        (1000) ci        (1000)     7042 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/bin/openedx-assets
--rwxr-xr-x   0 ci        (1000) ci        (1000)      116 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/bin/reload-uwsgi
--rw-r--r--   0 ci        (1000) ci        (1000)     2329 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/bin/site-configuration
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/locale/
--rw-r--r--   0 ci        (1000) ci        (1000)      438 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/locale/customlocales.md
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/requirements/
--rw-r--r--   0 ci        (1000) ci        (1000)      305 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/requirements/private-sample.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/revisions.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/settings/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/settings/cms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/cms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      317 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/cms/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/cms/i18n.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/settings/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/lms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      306 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/lms/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/lms/i18n.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)      441 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/partials/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)      420 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/partials/i18n.py
--rw-r--r--   0 ci        (1000) ci        (1000)      262 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/uwsgi.ini
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/themes/
--rw-r--r--   0 ci        (1000) ci        (1000)       75 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/themes/README
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.015764 tutor-16.0.0/tutor/templates/build/permissions/
--rw-r--r--   0 ci        (1000) ci        (1000)      189 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/permissions/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      302 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/permissions/setowner.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.015764 tutor-16.0.0/tutor/templates/config/
--rw-r--r--   0 ci        (1000) ci        (1000)      515 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/config/base.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2610 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/config/defaults.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.015764 tutor-16.0.0/tutor/templates/dev/
--rw-r--r--   0 ci        (1000) ci        (1000)      885 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/dev/docker-compose.jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1395 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/dev/docker-compose.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.982431 tutor-16.0.0/tutor/templates/jobs/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.015764 tutor-16.0.0/tutor/templates/jobs/init/
--rw-r--r--   0 ci        (1000) ci        (1000)      418 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/jobs/init/cms.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1807 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/jobs/init/lms.sh
--rw-r--r--   0 ci        (1000) ci        (1000)      756 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/jobs/init/mounted-edx-platform.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1455 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/jobs/init/mysql.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.019098 tutor-16.0.0/tutor/templates/k8s/
--rw-r--r--   0 ci        (1000) ci        (1000)    13150 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/k8s/deployments.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2090 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/k8s/jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)      125 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/k8s/namespace.yml
--rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/k8s/override.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2358 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/k8s/services.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1428 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/k8s/volumes.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2142 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/kustomization.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.019098 tutor-16.0.0/tutor/templates/local/
--rw-r--r--   0 ci        (1000) ci        (1000)     2185 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/local/docker-compose.jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)      950 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/local/docker-compose.prod.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     6496 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/local/docker-compose.yml
--rw-r--r--   0 ci        (1000) ci        (1000)       19 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/version
--rw-r--r--   0 ci        (1000) ci        (1000)     1327 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/types.py
--rw-r--r--   0 ci        (1000) ci        (1000)    10935 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/utils.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.995764 tutor-16.0.0/tutor.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     6665 2023-06-14 21:51:27.000000 tutor-16.0.0/tutor.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     4098 2023-06-14 21:51:27.000000 tutor-16.0.0/tutor.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-14 21:51:27.000000 tutor-16.0.0/tutor.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-06-14 21:51:27.000000 tutor-16.0.0/tutor.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)      397 2023-06-14 21:51:27.000000 tutor-16.0.0/tutor.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        6 2023-06-14 21:51:27.000000 tutor-16.0.0/tutor.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.341752 tutor-16.0.1/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-16 10:11:27.000000 tutor-16.0.1/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)      121 2023-06-16 10:11:27.000000 tutor-16.0.1/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     6665 2023-06-16 10:12:28.341752 tutor-16.0.1/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     4745 2023-06-16 10:11:27.000000 tutor-16.0.1/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-16 10:11:27.000000 tutor-16.0.1/pyproject.toml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.295085 tutor-16.0.1/requirements/
+-rw-r--r--   0 ci        (1000) ci        (1000)       98 2023-06-16 10:11:27.000000 tutor-16.0.1/requirements/base.in
+-rw-r--r--   0 ci        (1000) ci        (1000)      340 2023-06-16 10:11:27.000000 tutor-16.0.1/requirements/plugins.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-16 10:12:28.341752 tutor-16.0.1/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     2506 2023-06-16 10:11:27.000000 tutor-16.0.1/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.301751 tutor-16.0.1/tests/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2491 2023-06-16 10:11:27.000000 tutor-16.0.1/tests/test_bindmount.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     4172 2023-06-16 10:11:27.000000 tutor-16.0.1/tests/test_config.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15898 2023-06-16 10:11:27.000000 tutor-16.0.1/tests/test_env.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     3063 2023-06-16 10:11:27.000000 tutor-16.0.1/tests/test_plugin_indexes.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     8279 2023-06-16 10:11:27.000000 tutor-16.0.1/tests/test_plugins_v0.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2432 2023-06-16 10:11:27.000000 tutor-16.0.1/tests/test_serialize.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    10669 2023-06-16 10:11:27.000000 tutor-16.0.1/tests/test_utils.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.315085 tutor-16.0.1/tutor/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1159 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2546 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/bindmount.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.321752 tutor-16.0.1/tutor/commands/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/__init__.py
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     4485 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/cli.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    16737 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/compose.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     7317 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/config.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      794 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/context.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2240 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/dev.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    11658 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/images.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    10722 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/jobs.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    21075 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/k8s.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1772 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/local.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     4446 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/mounts.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      741 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/params.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    13436 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/plugins.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.321752 tutor-16.0.1/tutor/commands/upgrade/
+-rw-r--r--   0 ci        (1000) ci        (1000)      185 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/upgrade/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2082 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/upgrade/common.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     6047 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/upgrade/compose.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5685 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/commands/upgrade/k8s.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     9685 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.321752 tutor-16.0.1/tutor/core/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/core/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.325085 tutor-16.0.1/tutor/core/hooks/
+-rw-r--r--   0 ci        (1000) ci        (1000)      292 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/core/hooks/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5707 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/core/hooks/actions.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2929 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/core/hooks/contexts.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     9006 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/core/hooks/filters.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      638 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/core/hooks/priorities.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    17753 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/env.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/exceptions.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1213 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/fmt.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.325085 tutor-16.0.1/tutor/hooks/
+-rw-r--r--   0 ci        (1000) ci        (1000)      273 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/hooks/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    24524 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/hooks/catalog.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      571 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/images.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5076 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/interactive.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.328418 tutor-16.0.1/tutor/plugins/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3802 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/plugins/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      548 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/plugins/base.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     6989 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/plugins/indexes.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15218 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/plugins/v0.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2376 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/plugins/v1.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/py.typed
+-rw-r--r--   0 ci        (1000) ci        (1000)     1947 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/serialize.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1385 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/tasks.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.328418 tutor-16.0.1/tutor/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.285085 tutor-16.0.1/tutor/templates/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.328418 tutor-16.0.1/tutor/templates/apps/caddy/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1989 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/caddy/Caddyfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.328418 tutor-16.0.1/tutor/templates/apps/openedx/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.328418 tutor-16.0.1/tutor/templates/apps/openedx/config/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1542 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/config/cms.env.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1787 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/config/lms.env.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.328418 tutor-16.0.1/tutor/templates/apps/openedx/config/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)      673 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/config/partials/auth.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.285085 tutor-16.0.1/tutor/templates/apps/openedx/settings/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.328418 tutor-16.0.1/tutor/templates/apps/openedx/settings/cms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/settings/cms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      591 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/settings/cms/development.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      529 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/settings/cms/production.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/settings/cms/test.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.331752 tutor-16.0.1/tutor/templates/apps/openedx/settings/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/settings/lms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1132 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/settings/lms/development.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1039 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/settings/lms/production.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/settings/lms/test.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.331752 tutor-16.0.1/tutor/templates/apps/openedx/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)    10001 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/settings/partials/common_all.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      924 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/settings/partials/common_cms.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1450 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/settings/partials/common_lms.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      105 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/settings/partials/common_test.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/openedx/uwsgi.ini
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.331752 tutor-16.0.1/tutor/templates/apps/permissions/
+-rw-r--r--   0 ci        (1000) ci        (1000)      380 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/permissions/setowners.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.331752 tutor-16.0.1/tutor/templates/apps/redis/
+-rw-r--r--   0 ci        (1000) ci        (1000)      854 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/apps/redis/redis.conf
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.288418 tutor-16.0.1/tutor/templates/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.335085 tutor-16.0.1/tutor/templates/build/openedx/
+-rw-r--r--   0 ci        (1000) ci        (1000)    12605 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.335085 tutor-16.0.1/tutor/templates/build/openedx/bin/
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     7042 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/bin/openedx-assets
+-rwxr-xr-x   0 ci        (1000) ci        (1000)      116 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/bin/reload-uwsgi
+-rw-r--r--   0 ci        (1000) ci        (1000)     2329 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/bin/site-configuration
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.335085 tutor-16.0.1/tutor/templates/build/openedx/locale/
+-rw-r--r--   0 ci        (1000) ci        (1000)      438 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/locale/customlocales.md
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.335085 tutor-16.0.1/tutor/templates/build/openedx/requirements/
+-rw-r--r--   0 ci        (1000) ci        (1000)      305 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/requirements/private-sample.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/revisions.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.335085 tutor-16.0.1/tutor/templates/build/openedx/settings/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.335085 tutor-16.0.1/tutor/templates/build/openedx/settings/cms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/settings/cms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      317 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/settings/cms/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/settings/cms/i18n.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.335085 tutor-16.0.1/tutor/templates/build/openedx/settings/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/settings/lms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      306 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/settings/lms/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/settings/lms/i18n.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.338418 tutor-16.0.1/tutor/templates/build/openedx/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)      441 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/settings/partials/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      420 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/settings/partials/i18n.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      262 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/settings/uwsgi.ini
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.338418 tutor-16.0.1/tutor/templates/build/openedx/themes/
+-rw-r--r--   0 ci        (1000) ci        (1000)       75 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/openedx/themes/README
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.338418 tutor-16.0.1/tutor/templates/build/permissions/
+-rw-r--r--   0 ci        (1000) ci        (1000)      189 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/permissions/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      302 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/build/permissions/setowner.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.338418 tutor-16.0.1/tutor/templates/config/
+-rw-r--r--   0 ci        (1000) ci        (1000)      515 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/config/base.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2610 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/config/defaults.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.338418 tutor-16.0.1/tutor/templates/dev/
+-rw-r--r--   0 ci        (1000) ci        (1000)      885 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/dev/docker-compose.jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1395 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/dev/docker-compose.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.291751 tutor-16.0.1/tutor/templates/jobs/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.341752 tutor-16.0.1/tutor/templates/jobs/init/
+-rw-r--r--   0 ci        (1000) ci        (1000)      418 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/jobs/init/cms.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1807 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/jobs/init/lms.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)      756 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/jobs/init/mounted-edx-platform.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1455 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/jobs/init/mysql.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.341752 tutor-16.0.1/tutor/templates/k8s/
+-rw-r--r--   0 ci        (1000) ci        (1000)    13150 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/k8s/deployments.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2090 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/k8s/jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)      125 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/k8s/namespace.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/k8s/override.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2358 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/k8s/services.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1428 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/k8s/volumes.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2142 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/kustomization.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.341752 tutor-16.0.1/tutor/templates/local/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2185 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/local/docker-compose.jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)      950 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/local/docker-compose.prod.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     6496 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/local/docker-compose.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)       19 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/templates/version
+-rw-r--r--   0 ci        (1000) ci        (1000)     1327 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/types.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    10935 2023-06-16 10:11:27.000000 tutor-16.0.1/tutor/utils.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-16 10:12:28.315085 tutor-16.0.1/tutor.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6665 2023-06-16 10:12:28.000000 tutor-16.0.1/tutor.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     4098 2023-06-16 10:12:28.000000 tutor-16.0.1/tutor.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-16 10:12:28.000000 tutor-16.0.1/tutor.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-06-16 10:12:28.000000 tutor-16.0.1/tutor.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)      397 2023-06-16 10:12:28.000000 tutor-16.0.1/tutor.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        6 2023-06-16 10:12:28.000000 tutor-16.0.1/tutor.egg-info/top_level.txt
```

### Comparing `tutor-16.0.0/LICENSE.txt` & `tutor-16.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/PKG-INFO` & `tutor-16.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor
-Version: 16.0.0
+Version: 16.0.1
 Summary: The Docker-based Open edX distribution designed for peace of mind
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.io
 Author-email: contact@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor
```

### Comparing `tutor-16.0.0/README.rst` & `tutor-16.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/setup.py` & `tutor-16.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tests/test_bindmount.py` & `tutor-16.0.1/tests/test_bindmount.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tests/test_config.py` & `tutor-16.0.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tests/test_env.py` & `tutor-16.0.1/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tests/test_plugin_indexes.py` & `tutor-16.0.1/tests/test_plugin_indexes.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tests/test_plugins_v0.py` & `tutor-16.0.1/tests/test_plugins_v0.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tests/test_serialize.py` & `tutor-16.0.1/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tests/test_utils.py` & `tutor-16.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/__about__.py` & `tutor-16.0.1/tutor/__about__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 # Increment this version number to trigger a new release. See
 # docs/tutor.html#versioning for information on the versioning scheme.
-__version__ = "16.0.0"
+__version__ = "16.0.1"
 
 # The version suffix will be appended to the actual version, separated by a
 # dash. Use this suffix to differentiate between the actual released version and
 # the versions from other branches. For instance: set the suffix to "nightly" in
 # the nightly branch.
 # The suffix is cleanly separated from the __version__ in this module to avoid
 # conflicts when merging branches.
```

### Comparing `tutor-16.0.0/tutor/bindmount.py` & `tutor-16.0.1/tutor/bindmount.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/cli.py` & `tutor-16.0.1/tutor/commands/cli.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/compose.py` & `tutor-16.0.1/tutor/commands/compose.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/config.py` & `tutor-16.0.1/tutor/commands/config.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/context.py` & `tutor-16.0.1/tutor/commands/context.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/dev.py` & `tutor-16.0.1/tutor/commands/dev.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/images.py` & `tutor-16.0.1/tutor/commands/images.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/jobs.py` & `tutor-16.0.1/tutor/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/k8s.py` & `tutor-16.0.1/tutor/commands/k8s.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,17 @@
     _instance = None
 
     def __init__(self) -> None:
         # Loading the kubernetes module here to avoid import overhead
         # pylint: disable=import-outside-toplevel
         from kubernetes import client, config
 
-        if os.path.exists(config.kube_config.KUBE_CONFIG_DEFAULT_LOCATION):
+        if os.path.exists(
+            os.path.expanduser(config.kube_config.KUBE_CONFIG_DEFAULT_LOCATION)
+        ):
             # found the kubeconfig file, let's load it!
             config.load_kube_config()
         elif (
             config.incluster_config.SERVICE_HOST_ENV_NAME in os.environ
             and config.incluster_config.SERVICE_PORT_ENV_NAME in os.environ
         ):
             # We are running inside a cluster, let's load the in-cluster configuration.
```

### Comparing `tutor-16.0.0/tutor/commands/local.py` & `tutor-16.0.1/tutor/commands/local.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/mounts.py` & `tutor-16.0.1/tutor/commands/mounts.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/params.py` & `tutor-16.0.1/tutor/commands/params.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/plugins.py` & `tutor-16.0.1/tutor/commands/plugins.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/upgrade/common.py` & `tutor-16.0.1/tutor/commands/upgrade/common.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/upgrade/compose.py` & `tutor-16.0.1/tutor/commands/upgrade/compose.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/commands/upgrade/k8s.py` & `tutor-16.0.1/tutor/commands/upgrade/k8s.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/config.py` & `tutor-16.0.1/tutor/config.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/core/hooks/actions.py` & `tutor-16.0.1/tutor/core/hooks/actions.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/core/hooks/contexts.py` & `tutor-16.0.1/tutor/core/hooks/contexts.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/core/hooks/filters.py` & `tutor-16.0.1/tutor/core/hooks/filters.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/core/hooks/priorities.py` & `tutor-16.0.1/tutor/core/hooks/priorities.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/env.py` & `tutor-16.0.1/tutor/env.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/fmt.py` & `tutor-16.0.1/tutor/fmt.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/hooks/catalog.py` & `tutor-16.0.1/tutor/hooks/catalog.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/images.py` & `tutor-16.0.1/tutor/images.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/interactive.py` & `tutor-16.0.1/tutor/interactive.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/plugins/__init__.py` & `tutor-16.0.1/tutor/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/plugins/base.py` & `tutor-16.0.1/tutor/plugins/base.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/plugins/indexes.py` & `tutor-16.0.1/tutor/plugins/indexes.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/plugins/v0.py` & `tutor-16.0.1/tutor/plugins/v0.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/plugins/v1.py` & `tutor-16.0.1/tutor/plugins/v1.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/serialize.py` & `tutor-16.0.1/tutor/serialize.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/tasks.py` & `tutor-16.0.1/tutor/tasks.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/apps/caddy/Caddyfile` & `tutor-16.0.1/tutor/templates/apps/caddy/Caddyfile`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/apps/openedx/config/cms.env.yml` & `tutor-16.0.1/tutor/templates/apps/openedx/config/cms.env.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/apps/openedx/config/lms.env.yml` & `tutor-16.0.1/tutor/templates/apps/openedx/config/lms.env.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/apps/openedx/config/partials/auth.yml` & `tutor-16.0.1/tutor/templates/apps/openedx/config/partials/auth.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/development.py` & `tutor-16.0.1/tutor/templates/apps/openedx/settings/cms/development.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/production.py` & `tutor-16.0.1/tutor/templates/apps/openedx/settings/cms/production.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/development.py` & `tutor-16.0.1/tutor/templates/apps/openedx/settings/lms/development.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/production.py` & `tutor-16.0.1/tutor/templates/apps/openedx/settings/lms/production.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_all.py` & `tutor-16.0.1/tutor/templates/apps/openedx/settings/partials/common_all.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_cms.py` & `tutor-16.0.1/tutor/templates/apps/openedx/settings/partials/common_cms.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_lms.py` & `tutor-16.0.1/tutor/templates/apps/openedx/settings/partials/common_lms.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/apps/redis/redis.conf` & `tutor-16.0.1/tutor/templates/apps/redis/redis.conf`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/build/openedx/Dockerfile` & `tutor-16.0.1/tutor/templates/build/openedx/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/build/openedx/bin/openedx-assets` & `tutor-16.0.1/tutor/templates/build/openedx/bin/openedx-assets`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/build/openedx/bin/site-configuration` & `tutor-16.0.1/tutor/templates/build/openedx/bin/site-configuration`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/config/base.yml` & `tutor-16.0.1/tutor/templates/config/base.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/config/defaults.yml` & `tutor-16.0.1/tutor/templates/config/defaults.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/dev/docker-compose.jobs.yml` & `tutor-16.0.1/tutor/templates/dev/docker-compose.jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/dev/docker-compose.yml` & `tutor-16.0.1/tutor/templates/dev/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/jobs/init/lms.sh` & `tutor-16.0.1/tutor/templates/jobs/init/lms.sh`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/jobs/init/mounted-edx-platform.sh` & `tutor-16.0.1/tutor/templates/jobs/init/mounted-edx-platform.sh`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/jobs/init/mysql.sh` & `tutor-16.0.1/tutor/templates/jobs/init/mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/k8s/deployments.yml` & `tutor-16.0.1/tutor/templates/k8s/deployments.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/k8s/jobs.yml` & `tutor-16.0.1/tutor/templates/k8s/jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/k8s/services.yml` & `tutor-16.0.1/tutor/templates/k8s/services.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/k8s/volumes.yml` & `tutor-16.0.1/tutor/templates/k8s/volumes.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/kustomization.yml` & `tutor-16.0.1/tutor/templates/kustomization.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/local/docker-compose.jobs.yml` & `tutor-16.0.1/tutor/templates/local/docker-compose.jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/local/docker-compose.prod.yml` & `tutor-16.0.1/tutor/templates/local/docker-compose.prod.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/templates/local/docker-compose.yml` & `tutor-16.0.1/tutor/templates/local/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/types.py` & `tutor-16.0.1/tutor/types.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor/utils.py` & `tutor-16.0.1/tutor/utils.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.0/tutor.egg-info/PKG-INFO` & `tutor-16.0.1/tutor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor
-Version: 16.0.0
+Version: 16.0.1
 Summary: The Docker-based Open edX distribution designed for peace of mind
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.io
 Author-email: contact@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor
```

### Comparing `tutor-16.0.0/tutor.egg-info/SOURCES.txt` & `tutor-16.0.1/tutor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

