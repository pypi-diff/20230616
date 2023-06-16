# Comparing `tmp/design.plone.ioprenoto-1.0.4.tar.gz` & `tmp/design.plone.ioprenoto-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.ioprenoto-1.0.4.tar", last modified: Wed Jun 14 13:03:41 2023, max compression
+gzip compressed data, was "design.plone.ioprenoto-1.0.5.tar", last modified: Fri Jun 16 08:40:26 2023, max compression
```

## Comparing `design.plone.ioprenoto-1.0.4.tar` & `design.plone.ioprenoto-1.0.5.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.586432 design.plone.ioprenoto-1.0.4/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      555 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/CHANGES.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       58 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/CONTRIBUTORS.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1338 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/DEVELOP.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/LICENSE.GPL
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      662 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/LICENSE.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      116 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/MANIFEST.in
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6154 2023-06-14 13:03:41.586432 design.plone.ioprenoto-1.0.4/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4344 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/README.rst
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.578432 design.plone.ioprenoto-1.0.4/docs/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7986 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/docs/conf.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       89 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/docs/index.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      340 2023-06-14 13:03:41.586432 design.plone.ioprenoto-1.0.4/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2799 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.574432 design.plone.ioprenoto-1.0.4/src/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.578432 design.plone.ioprenoto-1.0.4/src/design/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.578432 design.plone.ioprenoto-1.0.4/src/design/plone/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.578432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      139 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/adapters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/adapters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      562 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/adapters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1015 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/adapters/stringinterp.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/behaviors/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/behaviors/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1392 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/behaviors/additional_fields.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      591 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/behaviors/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      628 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/overrides/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/overrides/.gitkeep
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/static/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/static/.gitkeep
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1530 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/events/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/events/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      431 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/events/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      136 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/events/on_create.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      270 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/README.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1520 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.574432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/en/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1395 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.574432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/it/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1395 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1754 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/update.py
--rwxrwxr-x   0 mauro     (1000) mauro     (1000)      503 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/update.sh
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/permissions.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.574432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      191 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/catalog.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      191 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/metadata.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/registry/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      180 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/registry/main.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      340 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/rolemap.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/types/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      325 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/uninstall/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      132 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      280 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      414 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1685 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2773 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookable_list/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      478 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6155 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookings/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookings/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      354 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      653 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookings/search.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      201 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      794 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/setuphandlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1930 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/testing.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.586432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.586432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/robot/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2019 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/robot/test_example.robot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1231 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2221 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2800 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7008 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2459 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_setup.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4095 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.578432 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6154 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3749 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      127 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       20 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/not-zip-safe
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      281 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/top_level.txt
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.195556 design.plone.ioprenoto-1.0.5/
+-rw-r--r--   0 folix      (503) staff       (20)      658 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/CHANGES.rst
+-rw-r--r--   0 folix      (503) staff       (20)       58 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/CONTRIBUTORS.rst
+-rw-r--r--   0 folix      (503) staff       (20)     1338 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/DEVELOP.rst
+-rw-r--r--   0 folix      (503) staff       (20)      662 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/LICENSE.rst
+-rw-r--r--   0 folix      (503) staff       (20)      116 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/MANIFEST.in
+-rw-r--r--   0 folix      (503) staff       (20)     7910 2023-06-16 08:40:26.195766 design.plone.ioprenoto-1.0.5/PKG-INFO
+-rw-r--r--   0 folix      (503) staff       (20)     4344 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/README.rst
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.172547 design.plone.ioprenoto-1.0.5/docs/
+-rw-r--r--   0 folix      (503) staff       (20)     7986 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/docs/conf.py
+-rw-r--r--   0 folix      (503) staff       (20)       89 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/docs/index.rst
+-rw-r--r--   0 folix      (503) staff       (20)      340 2023-06-16 08:40:26.196451 design.plone.ioprenoto-1.0.5/setup.cfg
+-rw-r--r--   0 folix      (503) staff       (20)     2774 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/setup.py
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.163525 design.plone.ioprenoto-1.0.5/src/
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.172986 design.plone.ioprenoto-1.0.5/src/design/
+-rw-r--r--   0 folix      (503) staff       (20)       80 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/__init__.py
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.176310 design.plone.ioprenoto-1.0.5/src/design/plone/
+-rw-r--r--   0 folix      (503) staff       (20)       80 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/__init__.py
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.178381 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/
+-rw-r--r--   0 folix      (503) staff       (20)      139 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/__init__.py
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.179383 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/adapters/
+-rw-r--r--   0 folix      (503) staff       (20)       24 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/adapters/__init__.py
+-rw-r--r--   0 folix      (503) staff       (20)      562 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/adapters/configure.zcml
+-rw-r--r--   0 folix      (503) staff       (20)     1015 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/adapters/stringinterp.py
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.180399 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/behaviors/
+-rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/behaviors/__init__.py
+-rw-r--r--   0 folix      (503) staff       (20)     1392 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/behaviors/additional_fields.py
+-rw-r--r--   0 folix      (503) staff       (20)      591 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/behaviors/configure.zcml
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.181018 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/browser/
+-rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/browser/__init__.py
+-rw-r--r--   0 folix      (503) staff       (20)      628 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/browser/configure.zcml
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.181378 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/browser/overrides/
+-rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/browser/overrides/.gitkeep
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.181638 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/browser/static/
+-rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/browser/static/.gitkeep
+-rw-r--r--   0 folix      (503) staff       (20)     1530 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/configure.zcml
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.182534 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/events/
+-rw-r--r--   0 folix      (503) staff       (20)       24 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/events/__init__.py
+-rw-r--r--   0 folix      (503) staff       (20)      724 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/events/configure.zcml
+-rw-r--r--   0 folix      (503) staff       (20)     1338 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/events/on_create.py
+-rw-r--r--   0 folix      (503) staff       (20)      270 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/interfaces.py
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.184114 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/
+-rw-r--r--   0 folix      (503) staff       (20)      611 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/README.rst
+-rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/__init__.py
+-rw-r--r--   0 folix      (503) staff       (20)     1520 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.165620 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/en/
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.184542 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
+-rw-r--r--   0 folix      (503) staff       (20)     1395 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.165983 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/it/
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.184937 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/
+-rw-r--r--   0 folix      (503) staff       (20)     1395 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
+-rw-r--r--   0 folix      (503) staff       (20)     1754 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/update.py
+-rwxr-xr-x   0 folix      (503) staff       (20)      503 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/update.sh
+-rw-r--r--   0 folix      (503) staff       (20)      273 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/permissions.zcml
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.166998 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/profiles/
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.186442 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/profiles/default/
+-rw-r--r--   0 folix      (503) staff       (20)      191 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
+-rw-r--r--   0 folix      (503) staff       (20)      105 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/profiles/default/catalog.xml
+-rw-r--r--   0 folix      (503) staff       (20)      191 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/profiles/default/metadata.xml
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.186796 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/profiles/default/registry/
+-rw-r--r--   0 folix      (503) staff       (20)      180 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/profiles/default/registry/main.xml
+-rw-r--r--   0 folix      (503) staff       (20)      340 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/profiles/default/rolemap.xml
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.187152 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/profiles/default/types/
+-rw-r--r--   0 folix      (503) staff       (20)      325 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.187487 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/profiles/uninstall/
+-rw-r--r--   0 folix      (503) staff       (20)      132 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.188094 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/
+-rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/__init__.py
+-rw-r--r--   0 folix      (503) staff       (20)      280 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/configure.zcml
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.188655 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/serializers/
+-rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/serializers/__init__.py
+-rw-r--r--   0 folix      (503) staff       (20)      166 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.189966 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
+-rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
+-rw-r--r--   0 folix      (503) staff       (20)      414 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
+-rw-r--r--   0 folix      (503) staff       (20)     1685 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
+-rw-r--r--   0 folix      (503) staff       (20)     2773 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.190342 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/services/
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.191116 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/services/bookable_list/
+-rw-r--r--   0 folix      (503) staff       (20)      478 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
+-rw-r--r--   0 folix      (503) staff       (20)     6155 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.192096 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/services/bookings/
+-rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/services/bookings/__init__.py
+-rw-r--r--   0 folix      (503) staff       (20)      354 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml
+-rw-r--r--   0 folix      (503) staff       (20)      653 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/services/bookings/search.py
+-rw-r--r--   0 folix      (503) staff       (20)      201 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/services/configure.zcml
+-rw-r--r--   0 folix      (503) staff       (20)      794 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/setuphandlers.py
+-rw-r--r--   0 folix      (503) staff       (20)     2326 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/testing.py
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.194913 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/
+-rw-r--r--   0 folix      (503) staff       (20)        0 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/__init__.py
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.195273 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/robot/
+-rw-r--r--   0 folix      (503) staff       (20)     2019 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/robot/test_example.robot
+-rw-r--r--   0 folix      (503) staff       (20)     1231 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
+-rw-r--r--   0 folix      (503) staff       (20)     2873 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py
+-rw-r--r--   0 folix      (503) staff       (20)     2221 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
+-rw-r--r--   0 folix      (503) staff       (20)     2800 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
+-rw-r--r--   0 folix      (503) staff       (20)     7008 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
+-rw-r--r--   0 folix      (503) staff       (20)     2459 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/test_setup.py
+-rw-r--r--   0 folix      (503) staff       (20)     4095 2023-06-16 08:40:25.000000 design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
+drwxr-xr-x   0 folix      (503) staff       (20)        0 2023-06-16 08:40:26.175994 design.plone.ioprenoto-1.0.5/src/design.plone.ioprenoto.egg-info/
+-rw-r--r--   0 folix      (503) staff       (20)     7910 2023-06-16 08:40:26.000000 design.plone.ioprenoto-1.0.5/src/design.plone.ioprenoto.egg-info/PKG-INFO
+-rw-r--r--   0 folix      (503) staff       (20)     3800 2023-06-16 08:40:26.000000 design.plone.ioprenoto-1.0.5/src/design.plone.ioprenoto.egg-info/SOURCES.txt
+-rw-r--r--   0 folix      (503) staff       (20)        1 2023-06-16 08:40:26.000000 design.plone.ioprenoto-1.0.5/src/design.plone.ioprenoto.egg-info/dependency_links.txt
+-rw-r--r--   0 folix      (503) staff       (20)      147 2023-06-16 08:40:26.000000 design.plone.ioprenoto-1.0.5/src/design.plone.ioprenoto.egg-info/entry_points.txt
+-rw-r--r--   0 folix      (503) staff       (20)       20 2023-06-16 08:40:26.000000 design.plone.ioprenoto-1.0.5/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
+-rw-r--r--   0 folix      (503) staff       (20)        1 2023-06-16 08:40:26.000000 design.plone.ioprenoto-1.0.5/src/design.plone.ioprenoto.egg-info/not-zip-safe
+-rw-r--r--   0 folix      (503) staff       (20)      293 2023-06-16 08:40:26.000000 design.plone.ioprenoto-1.0.5/src/design.plone.ioprenoto.egg-info/requires.txt
+-rw-r--r--   0 folix      (503) staff       (20)        7 2023-06-16 08:40:26.000000 design.plone.ioprenoto-1.0.5/src/design.plone.ioprenoto.egg-info/top_level.txt
```

### Comparing `design.plone.ioprenoto-1.0.4/DEVELOP.rst` & `design.plone.ioprenoto-1.0.5/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/LICENSE.rst` & `design.plone.ioprenoto-1.0.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/README.rst` & `design.plone.ioprenoto-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/docs/conf.py` & `design.plone.ioprenoto-1.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/setup.py` & `design.plone.ioprenoto-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,22 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.ioprenoto",
-    version="1.0.4",
+    version="1.0.5",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
-        "Framework :: Plone :: 5.2",
         "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
@@ -54,15 +53,15 @@
     python_requires=">=3.7",
     install_requires=[
         "setuptools",
         # -*- Extra requirements: -*-
         "z3c.jbot",
         "plone.api>=1.8.4",
         "plone.app.dexterity",
-        "redturtle.prenotazioni",
+        "redturtle.prenotazioni>=2.0.0.dev1",
         "design.plone.policy",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
             # Plone KGS does not use this version, because it would break
             # Remove if your package shall be part of coredev.
```

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/adapters/configure.zcml` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/adapters/stringinterp.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/adapters/stringinterp.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/behaviors/additional_fields.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/behaviors/additional_fields.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/behaviors/configure.zcml` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/configure.zcml` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/configure.zcml` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/README.rst` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/update.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookings/search.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/restapi/services/bookings/search.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/setuphandlers.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/testing.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/testing.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,28 +7,42 @@
 from plone.testing import z2
 
 
 import design.plone.ioprenoto
 import redturtle.prenotazioni
 import collective.contentrules.mailfromfield
 
+try:
+    import design.plone.iocittadino
+
+    iocittadino_installed = True
+except ImportError:
+    iocittadino_installed = False
+
 
 class DesignPloneIoprenotoLayer(DesignPlonePolicyLayer):
     def setUpZope(self, app, configurationContext):
         super().setUpZope(app, configurationContext)
 
         self.loadZCML(package=design.plone.policy)
         self.loadZCML(package=redturtle.prenotazioni)
         self.loadZCML(package=collective.contentrules.mailfromfield)
         self.loadZCML(package=design.plone.ioprenoto)
 
+        if iocittadino_installed:
+            self.loadZCML(package=design.plone.iocittadino)
+
     def setUpPloneSite(self, portal):
         super().setUpPloneSite(portal)
 
         applyProfile(portal, "design.plone.ioprenoto:default")
+        applyProfile(portal, "redturtle.prenotazioni:default")
+
+        # if iocittadino_installed:
+        #     applyProfile(portal, "design.plone.iocittadino:default")
 
 
 DESIGN_PLONE_IOPRENOTO_FIXTURE = DesignPloneIoprenotoLayer()
 
 
 DESIGN_PLONE_IOPRENOTO_INTEGRATION_TESTING = IntegrationTesting(
     bases=(DESIGN_PLONE_IOPRENOTO_FIXTURE,),
```

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/robot/test_example.robot` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_setup.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py` & `design.plone.ioprenoto-1.0.5/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/SOURCES.txt` & `design.plone.ioprenoto-1.0.5/src/design.plone.ioprenoto.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 CHANGES.rst
 CONTRIBUTORS.rst
 DEVELOP.rst
-LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 docs/conf.py
 docs/index.rst
@@ -64,13 +63,14 @@
 src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
 src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
 src/design/plone/ioprenoto/restapi/services/bookings/__init__.py
 src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml
 src/design/plone/ioprenoto/restapi/services/bookings/search.py
 src/design/plone/ioprenoto/tests/__init__.py
 src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
+src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py
 src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
 src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
 src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
 src/design/plone/ioprenoto/tests/test_setup.py
 src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
 src/design/plone/ioprenoto/tests/robot/test_example.robot
```

