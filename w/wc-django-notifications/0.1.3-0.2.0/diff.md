# Comparing `tmp/wc-django-notifications-0.1.3.tar.gz` & `tmp/wc-django-notifications-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-django-notifications-0.1.3.tar", last modified: Fri Apr 14 09:03:50 2023, max compression
+gzip compressed data, was "wc-django-notifications-0.2.0.tar", last modified: Fri Jun 16 13:55:23 2023, max compression
```

## Comparing `wc-django-notifications-0.1.3.tar` & `wc-django-notifications-0.2.0.tar`

### file list

```diff
@@ -1,386 +1,387 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      347 2023-04-14 09:03:30.000000 wc-django-notifications-0.1.3/CHANGELOG.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1079 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/LICENSE
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      159 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/MANIFEST.in
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1310 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/Makefile
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9580 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/PKG-INFO
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     8593 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/README.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/setup.cfg
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1842 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/setup.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      620 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/tox.ini
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wc_django_notifications.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9580 2023-04-14 09:03:50.000000 wc-django-notifications-0.1.3/wc_django_notifications.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9640 2023-04-14 09:03:50.000000 wc-django-notifications-0.1.3/wc_django_notifications.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-04-14 09:03:50.000000 wc-django-notifications-0.1.3/wc_django_notifications.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      288 2023-04-14 09:03:50.000000 wc-django-notifications-0.1.3/wc_django_notifications.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       18 2023-04-14 09:03:50.000000 wc-django-notifications-0.1.3/wc_django_notifications.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      130 2023-04-14 09:02:22.000000 wc-django-notifications-0.1.3/wcd_notifications/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1141 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/admin.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      412 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3338 2023-04-14 08:42:13.000000 wc-django-notifications-0.1.3/wcd_notifications/compat.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      603 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/conf.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/contrib/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/contrib/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       68 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/__init__.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     7064 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/filters.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5209 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/serializers.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4250 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/views.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       46 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/exceptions.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/af/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/af/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/af/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/af/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ar/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      463 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ar/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3446 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ar/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ast/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/ast/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ast/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ast/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/az/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/az/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/az/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/az/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/be/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/be/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/be/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3504 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/be/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/bg/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/bg/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/bg/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/bn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/bn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/bn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/bn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/br/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/br/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      671 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/br/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3663 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/br/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/bs/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/bs/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/bs/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3437 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/bs/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ca/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/ca/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ca/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ca/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/cs/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      460 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/cs/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3443 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/cs/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/cy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/cy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      425 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/cy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3408 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/cy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/da/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/da/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/da/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/da/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/de/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/de/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/dsb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/dsb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/dsb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3415 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/dsb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/el/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/el/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/el/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/el/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/en/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.093330 wc-django-notifications-0.1.3/wcd_notifications/locale/en/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4397 2023-04-06 12:40:13.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/eo/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/eo/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/eo/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/eo/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/es/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/es/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/et/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/et/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/et/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/et/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/eu/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/eu/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/eu/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/eu/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/fa/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/fa/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fa/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3359 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fa/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/fi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/fr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3359 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/fy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/fy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/fy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ga/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ga/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      418 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ga/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3401 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ga/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/gd/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/gd/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      441 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/gd/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3424 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/gd/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/gl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/gl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/gl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/gl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/he/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/he/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/he/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3457 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/he/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/hi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/hi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/hr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/hr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      452 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3435 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/hsb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/hsb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hsb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3415 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hsb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/hu/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/hu/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hu/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hu/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/hy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/hy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/hy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ia/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ia/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ia/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ia/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/id/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/id/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ig/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ig/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ig/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ig/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/io/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/io/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/io/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/io/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/is/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/is/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      402 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/is/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3382 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/is/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/it/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/it/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.085330 wc-django-notifications-0.1.3/wcd_notifications/locale/ja/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ja/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ka/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ka/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ka/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3358 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ka/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/kab/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/kab/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/kab/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/kab/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/kk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/kk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/kk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3358 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/kk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/km/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/km/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/km/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/km/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/kn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/kn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/kn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3359 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/kn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ko/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ko/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ko/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ky/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ky/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ky/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ky/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/lb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/lb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/lb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/lb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/lt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/lt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      511 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/lt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3497 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/lt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/lv/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/lv/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/lv/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3398 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/lv/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/mk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/mk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      410 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/mk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3390 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/mk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ml/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ml/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ml/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ml/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/mn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/mn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/mn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/mn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/mr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/mr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/mr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/mr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ms/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/ms/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ms/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3314 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ms/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/my/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/my/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/my/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/my/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/nb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.097329 wc-django-notifications-0.1.3/wcd_notifications/locale/nb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/nb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/nb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ne/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/ne/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ne/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ne/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/nl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/nl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/nn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/nn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/nn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/nn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/os/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/os/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/os/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/os/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/pa/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/pa/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/pa/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/pa/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/pl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      526 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3512 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/pt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ro/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/ro/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      421 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ro/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3404 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ro/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ru/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4541 2023-04-06 12:40:13.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/sk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/sk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      455 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3438 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/sl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/sl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3415 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/sq/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/sq/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sq/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sq/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/sr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/sr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3437 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/sv/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/sw/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/sw/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sw/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/sw/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ta/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/ta/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ta/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ta/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/te/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/te/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/te/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/te/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/tg/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/tg/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tg/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tg/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/th/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/th/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/th/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/th/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/tk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/tk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/tr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3359 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/tt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/tt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/tt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/udm/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/udm/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/udm/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/udm/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/uk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      602 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4628 2023-04-06 12:40:13.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/ur/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/ur/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ur/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3360 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/ur/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/uz/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/uz/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/uz/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/uz/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.089330 wc-django-notifications-0.1.3/wcd_notifications/locale/vi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/locale/vi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/vi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3353 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/locale/vi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/migrations/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5522 2023-04-14 08:42:40.000000 wc-django-notifications-0.1.3/wcd_notifications/migrations/0001_initial.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/migrations/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/models/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       50 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/models/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9322 2023-04-14 08:13:46.000000 wc-django-notifications-0.1.3/wcd_notifications/models/notifications.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1801 2023-04-14 08:43:15.000000 wc-django-notifications-0.1.3/wcd_notifications/models/stats.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-14 09:03:50.101329 wc-django-notifications-0.1.3/wcd_notifications/services/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/services/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4371 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/services/manager.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2113 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/services/notifier.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      231 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/signals.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      453 2022-12-14 08:36:21.000000 wc-django-notifications-0.1.3/wcd_notifications/subscriptions.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     3927 2023-04-14 08:34:36.000000 wc-django-notifications-0.1.3/wcd_notifications/utils.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      523 2023-06-16 13:54:32.000000 wc-django-notifications-0.2.0/CHANGELOG.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1079 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/LICENSE
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      159 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/MANIFEST.in
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1310 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/Makefile
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9730 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/PKG-INFO
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     8567 2023-06-16 13:50:14.000000 wc-django-notifications-0.2.0/README.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/setup.cfg
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1885 2023-06-16 13:01:55.000000 wc-django-notifications-0.2.0/setup.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      620 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/tox.ini
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wc_django_notifications.egg-info/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9730 2023-06-16 13:55:23.000000 wc-django-notifications-0.2.0/wc_django_notifications.egg-info/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9696 2023-06-16 13:55:23.000000 wc-django-notifications-0.2.0/wc_django_notifications.egg-info/SOURCES.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-06-16 13:55:23.000000 wc-django-notifications-0.2.0/wc_django_notifications.egg-info/dependency_links.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      320 2023-06-16 13:55:23.000000 wc-django-notifications-0.2.0/wc_django_notifications.egg-info/requires.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       18 2023-06-16 13:55:23.000000 wc-django-notifications-0.2.0/wc_django_notifications.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      130 2023-06-16 12:15:26.000000 wc-django-notifications-0.2.0/wcd_notifications/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1350 2023-06-16 13:46:38.000000 wc-django-notifications-0.2.0/wcd_notifications/admin.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      412 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3338 2023-04-14 08:42:13.000000 wc-django-notifications-0.2.0/wcd_notifications/compat.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      603 2023-06-16 12:05:13.000000 wc-django-notifications-0.2.0/wcd_notifications/conf.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/contrib/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/contrib/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       68 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      353 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     7048 2023-06-16 11:45:20.000000 wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/filters.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5207 2023-06-16 11:46:40.000000 wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/serializers.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4067 2023-06-16 12:10:37.000000 wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/views.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       46 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/exceptions.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/af/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/af/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/af/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/af/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/ar/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3556 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/ast/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/ast/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ast/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ast/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/az/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/az/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/az/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/az/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/be/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/be/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/be/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3614 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/be/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/bg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/bg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/bg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/bn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/bn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/bn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/bn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/br/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/br/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      671 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/br/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3773 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/br/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/bs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/bs/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/bs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3547 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/bs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/ca/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/ca/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ca/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ca/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/cs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      460 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3553 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/cy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/cy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      425 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/cy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3518 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/cy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/da/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/da/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/da/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/da/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/de/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/dsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/dsb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/dsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3525 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/dsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/el/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/el/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/el/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/el/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/en/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/eo/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/eo/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/eo/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/eo/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/es/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/et/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/et/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/et/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/et/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/eu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/eu/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/eu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/eu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/fa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/fa/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/fi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/fr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/fy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/fy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/fy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/ga/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/ga/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      418 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ga/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3511 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ga/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.180953 wc-django-notifications-0.2.0/wcd_notifications/locale/gd/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.192952 wc-django-notifications-0.2.0/wcd_notifications/locale/gd/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      441 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/gd/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3534 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/gd/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/gl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/gl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/gl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/gl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/he/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/he/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/he/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3567 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/he/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/hi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/hi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/hr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/hr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      452 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3545 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/hsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/hsb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3525 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/hu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/hu/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/hy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/hy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/hy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ia/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ia/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ia/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ia/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/id/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ig/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ig/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ig/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ig/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/io/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/io/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/io/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/io/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/is/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/is/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      402 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/is/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3492 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/is/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/it/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ja/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ka/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ka/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ka/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3468 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ka/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/kab/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/kab/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/kab/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/kab/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/kk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/kk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/kk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3468 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/kk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/km/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/km/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/km/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/km/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/kn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/kn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/kn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/kn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ko/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ky/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ky/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ky/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ky/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/lb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/lb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/lb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/lb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/lt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/lt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      511 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/lt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3607 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/lt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/lv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/lv/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/lv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3508 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/lv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/mk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/mk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      410 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/mk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3500 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/mk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ml/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/ml/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ml/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ml/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/mn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.196952 wc-django-notifications-0.2.0/wcd_notifications/locale/mn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/mn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/mn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/mr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/mr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/mr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/mr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ms/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/ms/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      337 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ms/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3423 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ms/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/my/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/my/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/my/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/my/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/nb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/nb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/nb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/nb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ne/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/ne/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ne/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ne/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/nl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/nn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/nn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/nn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/nn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/os/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/os/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/os/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/os/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/pa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/pa/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/pa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/pa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/pl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      526 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3622 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/pt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ro/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/ro/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      421 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ro/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3514 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ro/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/ru/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3614 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.184953 wc-django-notifications-0.2.0/wcd_notifications/locale/sk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/sk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      455 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3548 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/sl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/sl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3525 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/sq/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/sq/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sq/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sq/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/sr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/sr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3547 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/sv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/sw/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/sw/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sw/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/sw/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/ta/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/ta/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ta/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ta/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/te/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/te/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/te/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/te/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/tg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/tg/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/th/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.200952 wc-django-notifications-0.2.0/wcd_notifications/locale/th/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/th/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/th/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/tk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/tk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/tr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/tt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/tt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/tt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/udm/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/udm/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/udm/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/udm/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/uk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      602 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3701 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/ur/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/ur/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ur/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3470 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/ur/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/uz/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/uz/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/uz/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/uz/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.188953 wc-django-notifications-0.2.0/wcd_notifications/locale/vi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/locale/vi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2023-06-16 12:14:40.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/vi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3463 2023-06-16 12:14:39.000000 wc-django-notifications-0.2.0/wcd_notifications/locale/vi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/migrations/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5522 2023-04-14 08:42:40.000000 wc-django-notifications-0.2.0/wcd_notifications/migrations/0001_initial.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      928 2023-06-16 11:53:31.000000 wc-django-notifications-0.2.0/wcd_notifications/migrations/0002_auto_20230616_1153.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/migrations/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/models/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       50 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/models/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9341 2023-06-16 12:51:42.000000 wc-django-notifications-0.2.0/wcd_notifications/models/notifications.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1801 2023-04-14 08:43:15.000000 wc-django-notifications-0.2.0/wcd_notifications/models/stats.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-16 13:55:23.204952 wc-django-notifications-0.2.0/wcd_notifications/services/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/services/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4371 2022-12-14 08:36:21.000000 wc-django-notifications-0.2.0/wcd_notifications/services/manager.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2103 2023-06-16 11:47:54.000000 wc-django-notifications-0.2.0/wcd_notifications/services/notifier.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      227 2023-06-16 11:46:27.000000 wc-django-notifications-0.2.0/wcd_notifications/signals.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      449 2023-06-16 11:46:34.000000 wc-django-notifications-0.2.0/wcd_notifications/subscriptions.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     3927 2023-04-14 08:34:36.000000 wc-django-notifications-0.2.0/wcd_notifications/utils.py
```

### Comparing `wc-django-notifications-0.1.3/LICENSE` & `wc-django-notifications-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.3/Makefile` & `wc-django-notifications-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.3/PKG-INFO` & `wc-django-notifications-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-notifications
-Version: 0.1.3
+Version: 0.2.0
 Summary: Modular notifications system for your django applications.
 Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -87,17 +87,17 @@
 ```
 
 Notifications send method has several breakpoints on which you may add additional handlers for a common situations:
 
 1. Each notification separately will run preparation pipeline from `Notification.preparator`. It's an instances of `px_pipline.Filter` so you may add or remove them.
 2. Then preparation pipeline from `settings.PREPARATION_PIPELINE` will be run on all new notification instances.
 3. Notifications will be created.
-4. For each notification `wcd_notifications.signals.notification_sended` will be sent.
-4. For all new notifications `wcd_notifications.signals.notifications_sended` will be sent.
-5. There is already one `wcd_notifications.signals.notifications_sended` signal reciever. It will recollect stats for all the recipients that new notifications has.
+4. For each notification `wcd_notifications.signals.notification_sent` will be sent.
+4. For all new notifications `wcd_notifications.signals.notifications_sent` will be sent.
+5. There is already one `wcd_notifications.signals.notifications_sent` signal reciever. It will recollect stats for all the recipients that new notifications has.
 
 ### Notification state management
 
 You may change flags in three different ways:
 
 - `add` - List of flags to add.
 - `remove` - List of flags to remove.
@@ -137,16 +137,16 @@
 Notification.flags_registry.add(OtherOptions)
 ```
 
 Flags change method also has it's own breakpoints to extend:
 
 1. After all flag changes applied, but not saved pipeline from `settings.CHANGE_FLAG_PIPELINE` runs.
 2. All notification flags changes are saved to database.
-3. Signal `wcd_notifications.signals.notifications_flags_changed` sended.
-3. Signal `wcd_notifications.signals.notifications_updated` sended.
+3. Signal `wcd_notifications.signals.notifications_flags_changed` sent.
+3. Signal `wcd_notifications.signals.notifications_updated` sent.
 
 ### Querying
 
 Notifications queryset has additional methods, for easier querying:
 
 ```python
 from wcd_notifications.models import Notification
@@ -162,16 +162,16 @@
   .recipients([])
   # Actors:
   .actors([])
   # Actions:
   .actions([])
   # Targets:
   .targets([])
-  # To display only already sended messages.
-  .sended(now=None)
+  # To display only already sent messages.
+  .sent(now=None)
 )
 ```
 
 ### Stats
 
 Reading information about notifications state is far more frequent action, that notifications change/sending. So library "caches" state data into database and updates it after any change occured.
 
@@ -251,17 +251,17 @@
 - **targets**: Same as **actors**.
 - **actor_types**: List of types for filter on:
 
   `&actor_types=auth.user,muapp.mymodel&actor_types=otherapp.othermodel` - There can be mutiple same named fields. Comma ',' could be also a separator for multiple values. Or operator used for all identifiers.
 
 - **action_types**: Same as **actor_types**.
 - **target_types**: Same as **actor_types**.
-- **sended_at_before**: Filter by the time >= notification was sended. ISO datetime.
-- **sended_at_after**: Filter by the time <= notification was sended. ISO datetime.
-- **is_sended**: Get only already sended notifications.
+- **sent_at_before**: Filter by the time >= notification was sent. ISO datetime.
+- **sent_at_after**: Filter by the time <= notification was sent. ISO datetime.
+- **is_sent**: Get only already sent notifications.
 - **is_root**: Since notifications are hierarchical you may only need a root notifications.
 - **parents**: List of parent identifiers to filter over:
 
   `&parents=1,2,3&parents=4,6` - There can be mutiple same named fields. Comma ',' could be also a separator for multiple values. Or operator used for all identifiers.
 - **flags**: Filtering over flags is not that simple OR statement.
 
   `&flags=1,2,3&flags=4,6` - Each comma ',' separated list considered as AND comparison. Or operator used between multiple `flags` fields.
@@ -299,14 +299,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.0]
+### Fixed
+- Past form of verb "send" changed everywhere from "sended" to "sent".
+- Removed explicit `pagination_class` from notifications list view.
+- Small fixes.
+
 ## [0.1.3]
 ### Fixed
 - Django 2.2 compatibility.
 
 ## [0.1.1]
 Initial version.
```

### Comparing `wc-django-notifications-0.1.3/README.md` & `wc-django-notifications-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -66,17 +66,17 @@
 ```
 
 Notifications send method has several breakpoints on which you may add additional handlers for a common situations:
 
 1. Each notification separately will run preparation pipeline from `Notification.preparator`. It's an instances of `px_pipline.Filter` so you may add or remove them.
 2. Then preparation pipeline from `settings.PREPARATION_PIPELINE` will be run on all new notification instances.
 3. Notifications will be created.
-4. For each notification `wcd_notifications.signals.notification_sended` will be sent.
-4. For all new notifications `wcd_notifications.signals.notifications_sended` will be sent.
-5. There is already one `wcd_notifications.signals.notifications_sended` signal reciever. It will recollect stats for all the recipients that new notifications has.
+4. For each notification `wcd_notifications.signals.notification_sent` will be sent.
+4. For all new notifications `wcd_notifications.signals.notifications_sent` will be sent.
+5. There is already one `wcd_notifications.signals.notifications_sent` signal reciever. It will recollect stats for all the recipients that new notifications has.
 
 ### Notification state management
 
 You may change flags in three different ways:
 
 - `add` - List of flags to add.
 - `remove` - List of flags to remove.
@@ -116,16 +116,16 @@
 Notification.flags_registry.add(OtherOptions)
 ```
 
 Flags change method also has it's own breakpoints to extend:
 
 1. After all flag changes applied, but not saved pipeline from `settings.CHANGE_FLAG_PIPELINE` runs.
 2. All notification flags changes are saved to database.
-3. Signal `wcd_notifications.signals.notifications_flags_changed` sended.
-3. Signal `wcd_notifications.signals.notifications_updated` sended.
+3. Signal `wcd_notifications.signals.notifications_flags_changed` sent.
+3. Signal `wcd_notifications.signals.notifications_updated` sent.
 
 ### Querying
 
 Notifications queryset has additional methods, for easier querying:
 
 ```python
 from wcd_notifications.models import Notification
@@ -141,16 +141,16 @@
   .recipients([])
   # Actors:
   .actors([])
   # Actions:
   .actions([])
   # Targets:
   .targets([])
-  # To display only already sended messages.
-  .sended(now=None)
+  # To display only already sent messages.
+  .sent(now=None)
 )
 ```
 
 ### Stats
 
 Reading information about notifications state is far more frequent action, that notifications change/sending. So library "caches" state data into database and updates it after any change occured.
 
@@ -230,17 +230,17 @@
 - **targets**: Same as **actors**.
 - **actor_types**: List of types for filter on:
 
   `&actor_types=auth.user,muapp.mymodel&actor_types=otherapp.othermodel` - There can be mutiple same named fields. Comma ',' could be also a separator for multiple values. Or operator used for all identifiers.
 
 - **action_types**: Same as **actor_types**.
 - **target_types**: Same as **actor_types**.
-- **sended_at_before**: Filter by the time >= notification was sended. ISO datetime.
-- **sended_at_after**: Filter by the time <= notification was sended. ISO datetime.
-- **is_sended**: Get only already sended notifications.
+- **sent_at_before**: Filter by the time >= notification was sent. ISO datetime.
+- **sent_at_after**: Filter by the time <= notification was sent. ISO datetime.
+- **is_sent**: Get only already sent notifications.
 - **is_root**: Since notifications are hierarchical you may only need a root notifications.
 - **parents**: List of parent identifiers to filter over:
 
   `&parents=1,2,3&parents=4,6` - There can be mutiple same named fields. Comma ',' could be also a separator for multiple values. Or operator used for all identifiers.
 - **flags**: Filtering over flags is not that simple OR statement.
 
   `&flags=1,2,3&flags=4,6` - Each comma ',' separated list considered as AND comparison. Or operator used between multiple `flags` fields.
```

### Comparing `wc-django-notifications-0.1.3/setup.py` & `wc-django-notifications-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     author='WebCase',
     author_email='info@webcase.studio',
     license='MIT License',
     description='Modular notifications system for your django applications.',
     install_requires=(
         'px-settings>=0.1.3,<0.2.0',
         'px-pipeline>=0.1.2,<0.2.0',
+        'django-prettyjson>=0.4.1,<0.5.0',
     ),
     include_package_data=True,
     extras_require={
         'dev': (
             'pytest>=6.0,<7.0',
             'pytest-watch>=4.2,<5.0',
             'pytest-django>=4.3,<5.0',
```

### Comparing `wc-django-notifications-0.1.3/tox.ini` & `wc-django-notifications-0.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.3/wc_django_notifications.egg-info/PKG-INFO` & `wc-django-notifications-0.2.0/wc_django_notifications.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-notifications
-Version: 0.1.3
+Version: 0.2.0
 Summary: Modular notifications system for your django applications.
 Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -87,17 +87,17 @@
 ```
 
 Notifications send method has several breakpoints on which you may add additional handlers for a common situations:
 
 1. Each notification separately will run preparation pipeline from `Notification.preparator`. It's an instances of `px_pipline.Filter` so you may add or remove them.
 2. Then preparation pipeline from `settings.PREPARATION_PIPELINE` will be run on all new notification instances.
 3. Notifications will be created.
-4. For each notification `wcd_notifications.signals.notification_sended` will be sent.
-4. For all new notifications `wcd_notifications.signals.notifications_sended` will be sent.
-5. There is already one `wcd_notifications.signals.notifications_sended` signal reciever. It will recollect stats for all the recipients that new notifications has.
+4. For each notification `wcd_notifications.signals.notification_sent` will be sent.
+4. For all new notifications `wcd_notifications.signals.notifications_sent` will be sent.
+5. There is already one `wcd_notifications.signals.notifications_sent` signal reciever. It will recollect stats for all the recipients that new notifications has.
 
 ### Notification state management
 
 You may change flags in three different ways:
 
 - `add` - List of flags to add.
 - `remove` - List of flags to remove.
@@ -137,16 +137,16 @@
 Notification.flags_registry.add(OtherOptions)
 ```
 
 Flags change method also has it's own breakpoints to extend:
 
 1. After all flag changes applied, but not saved pipeline from `settings.CHANGE_FLAG_PIPELINE` runs.
 2. All notification flags changes are saved to database.
-3. Signal `wcd_notifications.signals.notifications_flags_changed` sended.
-3. Signal `wcd_notifications.signals.notifications_updated` sended.
+3. Signal `wcd_notifications.signals.notifications_flags_changed` sent.
+3. Signal `wcd_notifications.signals.notifications_updated` sent.
 
 ### Querying
 
 Notifications queryset has additional methods, for easier querying:
 
 ```python
 from wcd_notifications.models import Notification
@@ -162,16 +162,16 @@
   .recipients([])
   # Actors:
   .actors([])
   # Actions:
   .actions([])
   # Targets:
   .targets([])
-  # To display only already sended messages.
-  .sended(now=None)
+  # To display only already sent messages.
+  .sent(now=None)
 )
 ```
 
 ### Stats
 
 Reading information about notifications state is far more frequent action, that notifications change/sending. So library "caches" state data into database and updates it after any change occured.
 
@@ -251,17 +251,17 @@
 - **targets**: Same as **actors**.
 - **actor_types**: List of types for filter on:
 
   `&actor_types=auth.user,muapp.mymodel&actor_types=otherapp.othermodel` - There can be mutiple same named fields. Comma ',' could be also a separator for multiple values. Or operator used for all identifiers.
 
 - **action_types**: Same as **actor_types**.
 - **target_types**: Same as **actor_types**.
-- **sended_at_before**: Filter by the time >= notification was sended. ISO datetime.
-- **sended_at_after**: Filter by the time <= notification was sended. ISO datetime.
-- **is_sended**: Get only already sended notifications.
+- **sent_at_before**: Filter by the time >= notification was sent. ISO datetime.
+- **sent_at_after**: Filter by the time <= notification was sent. ISO datetime.
+- **is_sent**: Get only already sent notifications.
 - **is_root**: Since notifications are hierarchical you may only need a root notifications.
 - **parents**: List of parent identifiers to filter over:
 
   `&parents=1,2,3&parents=4,6` - There can be mutiple same named fields. Comma ',' could be also a separator for multiple values. Or operator used for all identifiers.
 - **flags**: Filtering over flags is not that simple OR statement.
 
   `&flags=1,2,3&flags=4,6` - Each comma ',' separated list considered as AND comparison. Or operator used between multiple `flags` fields.
@@ -299,14 +299,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.0]
+### Fixed
+- Past form of verb "send" changed everywhere from "sended" to "sent".
+- Removed explicit `pagination_class` from notifications list view.
+- Small fixes.
+
 ## [0.1.3]
 ### Fixed
 - Django 2.2 compatibility.
 
 ## [0.1.1]
 Initial version.
```

### Comparing `wc-django-notifications-0.1.3/wc_django_notifications.egg-info/SOURCES.txt` & `wc-django-notifications-0.2.0/wc_django_notifications.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,15 @@
 wcd_notifications/locale/ur/LC_MESSAGES/django.mo
 wcd_notifications/locale/ur/LC_MESSAGES/django.po
 wcd_notifications/locale/uz/LC_MESSAGES/django.mo
 wcd_notifications/locale/uz/LC_MESSAGES/django.po
 wcd_notifications/locale/vi/LC_MESSAGES/django.mo
 wcd_notifications/locale/vi/LC_MESSAGES/django.po
 wcd_notifications/migrations/0001_initial.py
+wcd_notifications/migrations/0002_auto_20230616_1153.py
 wcd_notifications/migrations/__init__.py
 wcd_notifications/models/__init__.py
 wcd_notifications/models/notifications.py
 wcd_notifications/models/stats.py
 wcd_notifications/services/__init__.py
 wcd_notifications/services/manager.py
 wcd_notifications/services/notifier.py
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/compat.py` & `wc-django-notifications-0.2.0/wcd_notifications/compat.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/filters.py` & `wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,39 +198,39 @@
 
 class NotificationsFilterSet(BaseFilterSet):
     actors = GenericKeyMethodFilter(qs_method='actors')
     actions = GenericKeyMethodFilter(qs_method='actions')
     targets = GenericKeyMethodFilter(qs_method='targets')
 
     actor_types = ContentTypeInFilter(field_name='actor_content_type', lookup_expr='in')
-    action_types = ContentTypeInFilter(field_name='actions_content_type', lookup_expr='in')
-    target_types = ContentTypeInFilter(field_name='targets_content_type', lookup_expr='in')
+    action_types = ContentTypeInFilter(field_name='action_content_type', lookup_expr='in')
+    target_types = ContentTypeInFilter(field_name='target_content_type', lookup_expr='in')
 
     parents = NumbersInFilter(field_name='parent_id', lookup_expr='in')
     flags = LookupMultiplicationFilter(field_name='flags', lookup_expr='contains')
 
-    sended_at = filters.IsoDateTimeFromToRangeFilter()
+    sent_at = filters.IsoDateTimeFromToRangeFilter()
 
-    is_sended = filters.BooleanFilter(method='filter_sended')
+    is_sent = filters.BooleanFilter(method='filter_sent')
     is_root = filters.BooleanFilter(method='filter_roots')
 
     class Meta:
         model = Notification
         fields = [
             'ids',
             'actors', 'actions', 'targets',
             'actor_types', 'action_types', 'target_types',
-            'sended_at',
-            'is_sended', 'is_root',
+            'sent_at',
+            'is_sent', 'is_root',
         ]
 
-    def filter_sended(self, qs, value):
+    def filter_sent(self, qs, value):
         if value is not True:
             return qs
 
-        return qs.sended()
+        return qs.sent()
 
     def filter_roots(self, qs, value):
         if value is not True:
             return qs
 
         return qs.filter(parent_id__isnull=True)
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/serializers.py` & `wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     class Meta:
         model = Notification
         fields = (
             'id',
             'recipient', 'actor', 'action', 'target',
             'flags', 'message', 'data',
-            'sended_at', 'created_at',
+            'sent_at', 'created_at',
         )
 
     recipient = serializers.SerializerMethodField()
     actor = serializers.SerializerMethodField()
     action = serializers.SerializerMethodField()
     target = serializers.SerializerMethodField()
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/contrib/drf/views.py` & `wc-django-notifications-0.2.0/wcd_notifications/contrib/drf/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from django.urls import path, include
 
 from rest_framework import status
 from rest_framework.response import Response
 from rest_framework.generics import ListAPIView, GenericAPIView
-from rest_framework.pagination import LimitOffsetPagination
 from django_filters import rest_framework as filters
 
 from wcd_notifications.models import Notification, Stats
 from wcd_notifications.utils import resolve_recipients
 
 from .filters import NotificationsFilterSet
 from .serializers import (
@@ -63,43 +62,40 @@
         )
         .prefetch_related('recipient', 'actor', 'action', 'target')
     )
     filter_backends = (filters.DjangoFilterBackend,)
     filterset_class = NotificationsFilterSet
 
 
+class MultiNotificationsActionView(NotificationsMixin, ActionApiView):
+    def perform_action(self, serializer):
+        queryset = self.filter_queryset(self.get_queryset())
+        serializer.commit(queryset)
+
+
 class FlagsList(ListAPIView):
     serializer_class = FlagReadSerializer
     flags_registry = property(lambda self: Notification.flags_registry)
 
     def list(self, request, *args, **kwargs):
         serializer = self.get_serializer(self.flags_registry.values(), many=True)
         return Response(serializer.data)
 
 
 class NotificationsList(NotificationsMixin, ListAPIView):
     serializer_class = NotificationReadSerializer
-    pagination_class = LimitOffsetPagination
 
 
-class NotificationsClear(NotificationsMixin, ActionApiView):
+class NotificationsClear(MultiNotificationsActionView):
     serializer_class = NotificationClearSerializer
 
-    def perform_action(self, serializer):
-        queryset = self.filter_queryset(self.get_queryset())
-        serializer.commit(queryset)
-
 
-class NotificationsChangeFlags(NotificationsMixin, ActionApiView):
+class NotificationsChangeFlags(MultiNotificationsActionView):
     serializer_class = NotificationChangeFlagSerializer
 
-    def perform_action(self, serializer):
-        queryset = self.filter_queryset(self.get_queryset())
-        serializer.commit(queryset)
-
 
 class StatsList(RecipientsResolverMixin, ListAPIView):
     serializer_class = StatsReadSerializer
     queryset = Stats.objects.all().prefetch_related('recipient')
 
 
 flags_list_view = FlagsList.as_view()
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/af/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ms/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,33 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +41,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ar/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/af/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
-"&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ast/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/be/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,36 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
+"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +44,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/az/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,36 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
+"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +44,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/be/LC_MESSAGES/django.mo` & `wc-django-notifications-0.2.0/wcd_notifications/locale/be/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/be/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/lv/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n"
-"%100>=11 && n%100<=14)? 2 : 3);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : "
+"2);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -38,103 +43,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/bg/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/sk/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +43,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/bn/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/is/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n % 10 != 1 || n % 100 == 11);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/br/LC_MESSAGES/django.mo` & `wc-django-notifications-0.2.0/wcd_notifications/locale/br/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/br/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/br/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,38 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=5; plural=((n%10 == 1) && (n%100 != 11) && (n%100 !"
-"=71) && (n%100 !=91) ? 0 :(n%10 == 2) && (n%100 != 12) && (n%100 !=72) && (n"
-"%100 !=92) ? 1 :(n%10 ==3 || n%10==4 || n%10==9) && (n%100 < 10 || n% 100 > "
-"19) && (n%100 < 70 || n%100 > 79) && (n%100 < 90 || n%100 > 99) ? 2 :(n != 0 "
-"&& n % 1000000 == 0) ? 3 : 4);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"=71) && (n%100 !=91) ? 0 :(n%10 == 2) && (n%100 != 12) && (n%100 !=72) && "
+"(n%100 !=92) ? 1 :(n%10 ==3 || n%10==4 || n%10==9) && (n%100 < 10 || n% 100 "
+"> 19) && (n%100 < 70 || n%100 > 79) && (n%100 < 90 || n%100 > 99) ? 2 :(n != "
+"0 && n % 1000000 == 0) ? 3 : 4);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -40,103 +46,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/bs/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/bs/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +43,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ca/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/uk/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,37 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
+"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
+"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
+"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +45,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/cs/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/gd/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
-"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=4; plural=(n==1 || n==11) ? 0 : (n==2 || n==12) ? 1 : "
+"(n > 2 && n < 20) ? 2 : 3;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +43,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/cy/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ast/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n==2) ? 1 : (n != 8 && n != "
-"11) ? 2 : 3;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/da/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/az/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/de/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/bg/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/dsb/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/mk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || n"
-"%100==4 ? 2 : 3);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n % 10 == 1 && n % 100 != 11) ? 0 : 1;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/el/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/bn/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/en/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ga/LC_MESSAGES/django.po`

 * *Files 24% similar despite different names*

```diff
@@ -4,142 +4,142 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-10 15:02+0200\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=5; plural=(n==1 ? 0 : n==2 ? 1 : n<7 ? 2 : n<11 ? 3 : "
+"4);\n"
 
-#: packages/wc-django-notifications/wcd_notifications/apps.py:10
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:116
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/apps.py:11
+#: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:81
+#: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:82
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:116
+#: wcd_notifications/contrib/drf/filters.py:82
+#: wcd_notifications/contrib/drf/filters.py:116
 msgctxt "wcd_notifications"
 msgid "No such content type exists."
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/serializers.py:120
+#: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:137
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:141
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/eo/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ca/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/es/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/da/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/et/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/de/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/eu/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/el/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/fa/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/en/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/fi/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/eo/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/fr/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/es/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/fy/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/et/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ga/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/eu/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=5; plural=(n==1 ? 0 : n==2 ? 1 : n<7 ? 2 : n<11 ? 3 : "
-"4);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/gd/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/dsb/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1 || n==11) ? 0 : (n==2 || n==12) ? 1 : "
-"(n > 2 && n < 20) ? 2 : 3;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +43,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/gl/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/fa/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/he/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/he/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
 "1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +43,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/hi/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/fi/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/hr/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/sr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +43,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/hsb/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/fr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || n"
-"%100==4 ? 2 : 3);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/hu/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/fy/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/hy/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/gl/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ia/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/hi/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/id/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/hu/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ig/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/hy/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/io/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ia/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/is/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/hsb/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n % 10 != 1 || n % 100 == 11);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +43,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/it/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/io/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ja/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/it/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ka/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ka/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/kab/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/kab/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/kk/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/kk/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/km/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/kn/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/kn/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/lb/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ko/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ml/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ky/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/mn/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/lb/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/mr/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/lt/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/sl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
-"11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
-"1 : n % 1 != 0 ? 2: 3);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -38,103 +43,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/lv/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/nb/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : "
-"2);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/mk/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ne/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n % 10 == 1 && n % 100 != 11) ? 0 : 1;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ml/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/nl/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/mn/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/nn/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/mr/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/os/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ms/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/pa/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/my/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/pt/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/nb/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/sq/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ne/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/sv/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/nl/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/sw/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/nn/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ta/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/os/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/te/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/pa/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/tg/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/pl/LC_MESSAGES/django.mo` & `wc-django-notifications-0.2.0/wcd_notifications/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/pl/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/cs/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n"
-"%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n"
-"%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -38,103 +43,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/pt/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/tk/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ro/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/tr/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
-"2:1));\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ru/LC_MESSAGES/django.mo` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ru/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/pl/LC_MESSAGES/django.po`

 * *Files 19% similar despite different names*

```diff
@@ -4,144 +4,143 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-10 15:02+0200\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n"
-"%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
+"(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
+"n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
-#: packages/wc-django-notifications/wcd_notifications/apps.py:10
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:116
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/apps.py:11
+#: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:81
+#: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:82
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:116
+#: wcd_notifications/contrib/drf/filters.py:82
+#: wcd_notifications/contrib/drf/filters.py:116
 msgctxt "wcd_notifications"
 msgid "No such content type exists."
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/serializers.py:120
+#: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:137
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:141
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/sk/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/lt/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,36 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
-">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
+"11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
+"1 : n % 1 != 0 ? 2: 3);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +44,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/sl/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ur/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || n"
-"%100==4 ? 2 : 3);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/sq/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/id/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/sr/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/cy/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,29 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n==2) ? 1 : (n != 8 && n != "
+"11) ? 2 : 3;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -37,103 +43,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/sv/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ig/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/sw/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ja/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ta/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/km/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/te/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ko/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/tg/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ky/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/th/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/my/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/tk/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/th/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/tr/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/tt/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/tt/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/udm/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/udm/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/uz/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/uk/LC_MESSAGES/django.mo` & `wc-django-notifications-0.2.0/wcd_notifications/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/uk/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/hr/LC_MESSAGES/django.po`

 * *Files 22% similar despite different names*

```diff
@@ -4,145 +4,142 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-10 15:02+0200\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
-"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
-"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
-"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 
-#: packages/wc-django-notifications/wcd_notifications/apps.py:10
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:116
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/apps.py:11
+#: wcd_notifications/contrib/drf/apps.py:11
 msgctxt "wcd_notifications"
 msgid "Notifications DRF"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:81
+#: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:82
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/filters.py:116
+#: wcd_notifications/contrib/drf/filters.py:82
+#: wcd_notifications/contrib/drf/filters.py:116
 msgctxt "wcd_notifications"
 msgid "No such content type exists."
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/contrib/drf/serializers.py:120
+#: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:137
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:141
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: packages/wc-django-notifications/wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/ur/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/vi/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +42,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/uz/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ar/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
+"&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +43,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/locale/vi/LC_MESSAGES/django.po` & `wc-django-notifications-0.2.0/wcd_notifications/locale/ro/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -4,28 +4,35 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-05 13:03+0300\n"
+"POT-Creation-Date: 2023-06-16 15:14+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:116
+"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
+"2:1));\n"
+
+#: wcd_notifications/apps.py:10 wcd_notifications/models/notifications.py:117
 msgctxt "wcd_notifications"
 msgid "Notifications"
 msgstr ""
 
+#: wcd_notifications/contrib/drf/apps.py:11
+msgctxt "wcd_notifications"
+msgid "Notifications DRF"
+msgstr ""
+
 #: wcd_notifications/contrib/drf/filters.py:81
 msgctxt "wcd_notifications"
 msgid "Key is invalid."
 msgstr ""
 
 #: wcd_notifications/contrib/drf/filters.py:82
 #: wcd_notifications/contrib/drf/filters.py:116
@@ -36,103 +43,103 @@
 #: wcd_notifications/contrib/drf/serializers.py:120
 msgctxt "wcd_notifications"
 msgid ""
 "You must pass at least one flag into either `add` or `remove` or `specify` "
 "field."
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:35
+#: wcd_notifications/models/notifications.py:36
 msgctxt "wcd_notifications"
 msgid "Unread"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:36
+#: wcd_notifications/models/notifications.py:37
 msgctxt "wcd_notifications"
 msgid "Read"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:115
+#: wcd_notifications/models/notifications.py:116
 msgctxt "wcd_notifications"
 msgid "Notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:131
+#: wcd_notifications/models/notifications.py:132
 msgctxt "wcd_notifications"
 msgid "Parent notification"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:137
-#: wcd_notifications/models/stats.py:34
+#: wcd_notifications/models/notifications.py:138
+#: wcd_notifications/models/stats.py:35
 msgctxt "wcd_notifications"
 msgid "Recipient: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:141
-#: wcd_notifications/models/stats.py:38
+#: wcd_notifications/models/notifications.py:142
+#: wcd_notifications/models/stats.py:39
 msgctxt "wcd_notifications"
 msgid "Recipient: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:148
+#: wcd_notifications/models/notifications.py:149
 msgctxt "wcd_notifications"
 msgid "Actor: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:152
+#: wcd_notifications/models/notifications.py:153
 msgctxt "wcd_notifications"
 msgid "Actor: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:159
+#: wcd_notifications/models/notifications.py:160
 msgctxt "wcd_notifications"
 msgid "Action: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:163
+#: wcd_notifications/models/notifications.py:164
 msgctxt "wcd_notifications"
 msgid "Action: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:170
+#: wcd_notifications/models/notifications.py:171
 msgctxt "wcd_notifications"
 msgid "Target: Content type"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:174
+#: wcd_notifications/models/notifications.py:175
 msgctxt "wcd_notifications"
 msgid "Target: Id"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:181
+#: wcd_notifications/models/notifications.py:182
 msgctxt "wcd_notifications"
 msgid "Flags"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:185
+#: wcd_notifications/models/notifications.py:186
 msgctxt "wcd_notifications"
 msgid "Message"
 msgstr ""
 
-#: wcd_notifications/models/notifications.py:190
+#: wcd_notifications/models/notifications.py:191
 msgctxt "wcd_notifications"
 msgid "Data"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:23
+#: wcd_notifications/models/stats.py:24
 msgctxt "wcd_notifications"
 msgid "Notification stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:25
+#: wcd_notifications/models/stats.py:26
 msgctxt "wcd_notifications"
 msgid "List of notifications stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:43
+#: wcd_notifications/models/stats.py:44
 msgctxt "wcd_notifications"
 msgid "Flags stats"
 msgstr ""
 
-#: wcd_notifications/models/stats.py:47
+#: wcd_notifications/models/stats.py:48
 msgctxt "wcd_notifications"
 msgid "Total"
 msgstr ""
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/migrations/0001_initial.py` & `wc-django-notifications-0.2.0/wcd_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/models/notifications.py` & `wc-django-notifications-0.2.0/wcd_notifications/models/notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+from json import JSONEncoder
 from typing import Dict, Iterable, List, Optional, Sequence, Tuple, Type, TypedDict
 from itertools import groupby
 from enum import Enum
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.postgres.fields import ArrayField
 from django.contrib.contenttypes.models import ContentType
 from django.utils import timezone
@@ -65,16 +66,16 @@
 
     def actions(self, actions: Sequence[ModelDef]):
         return self.filter(make_generic_Q('action', actions))
 
     def targets(self, targets: Sequence[ModelDef]):
         return self.filter(make_generic_Q('target', targets))
 
-    def sended(self, now: Optional[datetime] = None):
-        return self.filter(sended_at=now if now is not None else timezone.now())
+    def sent(self, now: Optional[datetime] = None):
+        return self.filter(sent_at=now if now is not None else timezone.now())
 
     def collect_total_stats(self) -> Dict[RecipientDef, int]:
         records = (
             self
             .values('recipient_content_type', 'recipient_object_id')
             .order_by()
             .annotate(total=models.Count('pk'))
@@ -111,15 +112,15 @@
     preparator = Filter()
     flags_registry = FlagsRegistry()
     objects = NotificationQuerySet.as_manager()
 
     class Meta:
         verbose_name = pgettext_lazy('wcd_notifications', 'Notification')
         verbose_name_plural = pgettext_lazy('wcd_notifications', 'Notifications')
-        ordering = ('-ordering_field', '-sended_at', '-created_at', '-pk',)
+        ordering = ('-ordering_field', '-sent_at', '-created_at', '-pk',)
         indexes = [
             GinIndex(
                 name='wcdnt_%(class)s_flags',
                 fields=['flags'], opclasses=('gin__int_ops',)
             ),
             BTreeIndex(fields=['recipient_content_type', 'recipient_object_id']),
             BTreeIndex(fields=['actor_content_type', 'actor_object_id']),
@@ -187,15 +188,15 @@
         null=False, blank=False,
     )
 
     data = JSONField(
         verbose_name=pgettext_lazy('wcd_notifications', 'Data'),
         blank=True, null=False, default=dict,
     )
-    sended_at = models.DateTimeField(default=timezone.now, db_index=True)
+    sent_at = models.DateTimeField(default=timezone.now, db_index=True)
     created_at = models.DateTimeField(default=timezone.now, db_index=True)
     ordering_field = models.BigIntegerField(db_index=True, editable=False)
 
     def __str__(self):
         return self.message
 
     def prepare(
@@ -241,15 +242,15 @@
         context['update_field'].append(value)
 
 
 @Notification.preparator.add
 def prepare_ordering(context: dict):
     _set_update_field_context(context, 'ordering_field')
     instance: Notification = context['instance']
-    instance.ordering_field = int(instance.sended_at.timestamp() * 1000)
+    instance.ordering_field = int(instance.sent_at.timestamp() * 1000)
 
     return context
 
 
 @Notification.preparator.add
 def set_readability_state(context: dict):
     instance: Notification = context['instance']
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/models/stats.py` & `wc-django-notifications-0.2.0/wcd_notifications/models/stats.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/services/manager.py` & `wc-django-notifications-0.2.0/wcd_notifications/services/manager.py`

 * *Files identical despite different names*

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/services/notifier.py` & `wc-django-notifications-0.2.0/wcd_notifications/services/notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Optional, Sequence
 from px_pipeline import StraightPipeline
 
 from django.db import models
 from django.utils import timezone
 
 from ..models import Notification
-from ..signals import notification_sended, notifications_sended
+from ..signals import notification_sent, notifications_sent
 from ..conf import settings
 
 
 def send(
     message: str,
     recipients: Sequence[models.Model],
     actor: Optional[models.Model] = None,
@@ -34,15 +34,15 @@
     for recipient in recipients:
         notification = Notification(
             message=message.format(
                 recipient=recipient, actor=actor, action=action, target=target,
                 flags=flags, extra=extra, now=now, actual_now=actual_now,
             ),
             recipient=recipient, actor=actor, action=action, target=target,
-            parent=parent, flags=flags, created_at=now, sended_at=send_at,
+            parent=parent, flags=flags, created_at=now, sent_at=send_at,
             data={'actual_now': actual_now.isoformat(), **extra},
         )
         notification.recipient = recipient
         notification.actor = actor
         notification.action = action
         notification.target = target
         notification.prepare()
@@ -52,12 +52,12 @@
         'instances': notifications,
     })
     notifications = Notification.objects.bulk_create(
         prepared['instances'], batch_size=batch_size,
     )
 
     for notification in notifications:
-        notification_sended.send(Notification, instance=notification)
+        notification_sent.send(Notification, instance=notification)
 
-    notifications_sended.send(Notification, instances=notifications)
+    notifications_sent.send(Notification, instances=notifications)
 
     return notifications
```

### Comparing `wc-django-notifications-0.1.3/wcd_notifications/utils.py` & `wc-django-notifications-0.2.0/wcd_notifications/utils.py`

 * *Files identical despite different names*

