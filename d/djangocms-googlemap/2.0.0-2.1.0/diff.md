# Comparing `tmp/djangocms-googlemap-2.0.0.tar.gz` & `tmp/djangocms-googlemap-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangocms-googlemap-2.0.0.tar", last modified: Wed Sep  2 13:47:09 2020, max compression
+gzip compressed data, was "djangocms-googlemap-2.1.0.tar", last modified: Fri Jun 16 08:49:36 2023, max compression
```

## Comparing `djangocms-googlemap-2.0.0.tar` & `djangocms-googlemap-2.1.0.tar`

### file list

```diff
@@ -1,344 +1,345 @@
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.935421 djangocms-googlemap-2.0.0/
--rw-r--r--   0 finalangel   (501) staff       (20)     1475 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/LICENSE
--rw-r--r--   0 finalangel   (501) staff       (20)      208 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/MANIFEST.in
--rw-r--r--   0 finalangel   (501) staff       (20)     5928 2020-09-02 13:47:09.934788 djangocms-googlemap-2.0.0/PKG-INFO
--rw-r--r--   0 finalangel   (501) staff       (20)     3793 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/README.rst
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.207842 djangocms-googlemap-2.0.0/djangocms_googlemap/
--rw-r--r--   0 finalangel   (501) staff       (20)       22 2020-09-02 13:47:06.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)     3310 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/cms_plugins.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.185138 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.162949 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/af/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.234883 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/af/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      419 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/af/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4987 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/af/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.163169 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ar/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.236098 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ar/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      616 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     8512 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.163411 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/be/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.243981 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/be/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      558 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/be/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5126 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/be/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.163630 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/bg/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.257324 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/bg/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      534 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5070 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.163871 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/bn/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.264729 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/bn/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      417 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/bn/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4985 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/bn/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.164248 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ca/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.265799 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ca/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      525 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5061 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.164589 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cmn/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.279944 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cmn/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      423 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cmn/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4991 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cmn/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.164937 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cs/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.289319 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cs/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      551 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5087 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.165363 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cy/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.303879 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cy/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      460 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cy/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5028 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cy/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.165690 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/da/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.305137 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/da/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      525 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5061 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.166010 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/de/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.314304 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/de/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)     5939 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     7448 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.166271 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/el/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.329008 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/el/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      532 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5068 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.166534 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/en/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.330588 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/en/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)     5548 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     7022 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.166772 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.338330 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      417 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4985 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.167003 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_AR/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.339850 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      547 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5083 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.167356 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_BO/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.360589 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_BO/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      545 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_BO/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5081 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_BO/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.167602 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_DO/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.380573 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_DO/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      444 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_DO/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5012 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_DO/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.167839 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/et/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.381568 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/et/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      418 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4986 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.168099 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/eu/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.397319 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/eu/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      524 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5060 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.168337 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fa/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.410799 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fa/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      523 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5059 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.170420 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fi/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.419776 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fi/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      525 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5061 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.170697 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fr/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.421265 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fr/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      415 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     6698 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.170960 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ga/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.422692 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ga/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      453 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ga/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5021 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ga/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.171482 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/gl/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.437561 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/gl/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      418 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4986 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.171832 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/gu/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.438927 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/gu/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      418 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/gu/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4986 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/gu/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.172125 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/he/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.446743 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/he/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      531 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5067 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.172365 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hi/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.454550 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hi/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      529 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hi/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5065 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hi/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.172600 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hr/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.467977 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hr/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      600 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5136 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.172838 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hu/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.476152 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hu/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      532 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5068 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.173071 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/id/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.477763 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/id/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      413 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4981 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.173308 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/is/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.497898 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/is/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      549 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/is/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5085 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.173563 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/is_IS/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.498992 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/is_IS/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      457 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/is_IS/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5025 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/is_IS/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.173797 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/it/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.514146 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/it/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      417 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4985 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.174064 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ja/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.535217 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ja/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      524 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5060 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.174311 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ka/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.536873 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ka/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      411 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ka/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4979 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ka/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.174554 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/kk/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.558666 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/kk/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      524 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/kk/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5060 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/kk/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.174791 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/km/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.568268 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/km/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      531 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/km/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5067 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/km/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.175028 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ko/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.576801 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ko/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      409 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4977 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.175271 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ko_KR/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.590675 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      530 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5066 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.175508 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ku_IQ/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.592510 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ku_IQ/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      547 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ku_IQ/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5083 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ku_IQ/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.175744 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/lt/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.594227 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/lt/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      599 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     7510 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.176009 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/lv/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.595789 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/lv/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      452 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/lv/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5020 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.176486 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mn/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.597360 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mn/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      419 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mn/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4987 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mn/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.176785 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mn_MN/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.605211 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mn_MN/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      436 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mn_MN/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5004 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mn_MN/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.177049 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mt/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.606893 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mt/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      490 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mt/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5058 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mt/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.177301 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/nb/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.614905 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/nb/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      536 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5072 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.177551 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/nl/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.616766 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/nl/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      525 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5061 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.177791 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/no/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.618061 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/no/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      528 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/no/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5064 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/no/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.178032 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pl/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.619323 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pl/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      583 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5208 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.178286 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pt/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.620767 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pt/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      528 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5064 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.178642 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pt_BR/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.621906 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      546 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5082 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.178889 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ro/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.623058 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ro/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      567 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5103 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.179124 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ru/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.624767 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ru/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      663 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     9302 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.179358 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sk/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.640067 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sk/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      552 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5088 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.179588 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sl/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.647115 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sl/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      471 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5039 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.179822 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sl_SI/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.661388 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sl_SI/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      596 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sl_SI/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5132 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sl_SI/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.180482 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sq/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.662653 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sq/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      418 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4986 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.180753 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sq_AL/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.664531 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sq_AL/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      434 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sq_AL/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5002 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sq_AL/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.181089 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sr/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.678804 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sr/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      491 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sr/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5059 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.181377 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sr@latin/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.686702 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sr@latin/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      619 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sr@latin/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5155 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sr@latin/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.181655 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sv/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.688725 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sv/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      525 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5061 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.181993 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ta/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.690834 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ta/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      553 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ta/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5089 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ta/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.182295 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/th/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.692736 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/th/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      407 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/th/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4975 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.182537 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/th_TH/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.694308 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/th_TH/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      424 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/th_TH/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4992 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/th_TH/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.182775 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/tlh/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.695655 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/tlh/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      418 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/tlh/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4986 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/tlh/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.183063 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/tr/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.696996 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/tr/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      530 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5066 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.183431 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ug/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.698470 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ug/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      409 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ug/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4977 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ug/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.183713 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/uk/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.705968 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/uk/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      601 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5137 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.183956 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ur/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.707655 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ur/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      414 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ur/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4982 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ur/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.184195 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/vi/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.710174 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/vi/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      413 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4981 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.184499 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/vi_VN/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.711589 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/vi_VN/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      430 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/vi_VN/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4998 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/vi_VN/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.184746 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.712985 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      410 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     4978 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.184989 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh_CN/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.714231 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      534 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5070 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.185230 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh_TW/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.715742 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      535 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     5071 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.828523 djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/
--rw-r--r--   0 finalangel   (501) staff       (20)     3277 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0001_initial.py
--rw-r--r--   0 finalangel   (501) staff       (20)     1239 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0002_auto_20160622_1031.py
--rw-r--r--   0 finalangel   (501) staff       (20)      504 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0003_auto_20160825_1829.py
--rw-r--r--   0 finalangel   (501) staff       (20)    10081 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0004_adapted_fields.py
--rw-r--r--   0 finalangel   (501) staff       (20)     3361 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0005_create_nested_plugins.py
--rw-r--r--   0 finalangel   (501) staff       (20)      965 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0006_remove_fields.py
--rw-r--r--   0 finalangel   (501) staff       (20)      447 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0007_reset_null_values.py
--rw-r--r--   0 finalangel   (501) staff       (20)      437 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0008_removed_null_fields.py
--rw-r--r--   0 finalangel   (501) staff       (20)      791 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0009_googlemapmarker_icon.py
--rw-r--r--   0 finalangel   (501) staff       (20)      778 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0010_auto_20190718_1021.py
--rw-r--r--   0 finalangel   (501) staff       (20)        0 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)     9277 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/models.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.185626 djangocms-googlemap-2.0.0/djangocms_googlemap/static/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.185712 djangocms-googlemap-2.0.0/djangocms_googlemap/static/djangocms_googlemap/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.829080 djangocms-googlemap-2.0.0/djangocms_googlemap/static/djangocms_googlemap/js/
--rw-r--r--   0 finalangel   (501) staff       (20)    12934 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/static/djangocms_googlemap/js/djangocms.googlemap.js
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.186039 djangocms-googlemap-2.0.0/djangocms_googlemap/templates/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.186125 djangocms-googlemap-2.0.0/djangocms_googlemap/templates/djangocms_googlemap/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.865789 djangocms-googlemap-2.0.0/djangocms_googlemap/templates/djangocms_googlemap/default/
--rw-r--r--   0 finalangel   (501) staff       (20)     3827 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/templates/djangocms_googlemap/default/map.html
--rw-r--r--   0 finalangel   (501) staff       (20)      866 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/templates/djangocms_googlemap/default/marker.html
--rw-r--r--   0 finalangel   (501) staff       (20)      492 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/djangocms_googlemap/templates/djangocms_googlemap/default/route.html
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.221423 djangocms-googlemap-2.0.0/djangocms_googlemap.egg-info/
--rw-r--r--   0 finalangel   (501) staff       (20)     5928 2020-09-02 13:47:09.000000 djangocms-googlemap-2.0.0/djangocms_googlemap.egg-info/PKG-INFO
--rw-r--r--   0 finalangel   (501) staff       (20)     9196 2020-09-02 13:47:09.000000 djangocms-googlemap-2.0.0/djangocms_googlemap.egg-info/SOURCES.txt
--rw-r--r--   0 finalangel   (501) staff       (20)        1 2020-09-02 13:47:09.000000 djangocms-googlemap-2.0.0/djangocms_googlemap.egg-info/dependency_links.txt
--rw-r--r--   0 finalangel   (501) staff       (20)        1 2020-09-02 13:47:09.000000 djangocms-googlemap-2.0.0/djangocms_googlemap.egg-info/not-zip-safe
--rw-r--r--   0 finalangel   (501) staff       (20)       34 2020-09-02 13:47:09.000000 djangocms-googlemap-2.0.0/djangocms_googlemap.egg-info/requires.txt
--rw-r--r--   0 finalangel   (501) staff       (20)       26 2020-09-02 13:47:09.000000 djangocms-googlemap-2.0.0/djangocms_googlemap.egg-info/top_level.txt
--rw-r--r--   0 finalangel   (501) staff       (20)       38 2020-09-02 13:47:09.935580 djangocms-googlemap-2.0.0/setup.cfg
--rw-r--r--   0 finalangel   (501) staff       (20)     1591 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/setup.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:47:09.927370 djangocms-googlemap-2.0.0/tests/
--rw-r--r--   0 finalangel   (501) staff       (20)        0 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/tests/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)     3235 2020-08-18 14:02:00.000000 djangocms-googlemap-2.0.0/tests/helpers.py
--rw-r--r--   0 finalangel   (501) staff       (20)      418 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/tests/settings.py
--rw-r--r--   0 finalangel   (501) staff       (20)      885 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/tests/test_migrations.py
--rw-r--r--   0 finalangel   (501) staff       (20)     6685 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/tests/test_models.py
--rw-r--r--   0 finalangel   (501) staff       (20)     3887 2020-09-02 08:31:58.000000 djangocms-googlemap-2.0.0/tests/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.486980 djangocms-googlemap-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-16 08:49:36.486980 djangocms-googlemap-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/cms_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.450980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/af/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/af/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.450980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.450980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/be/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/be/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/be/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/be/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.450980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.450980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/bn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/bn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/bn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.450980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.450980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cmn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cmn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cmn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cmn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cy/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_BO/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_BO/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_BO/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_BO/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_DO/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_DO/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_DO/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_DO/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ga/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ga/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ga/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ga/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/gu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/gu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/gu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/gu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.470980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/is/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/is/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/is/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/is_IS/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/is_IS/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/is_IS/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/is_IS/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.454980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ka/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ka/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/kk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/kk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/kk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/kk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/km/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/km/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/km/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/km/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ku_IQ/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ku_IQ/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ku_IQ/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ku_IQ/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/lv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mn_MN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mn_MN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mn_MN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mn_MN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.474980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/no/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/no/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sl_SI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sl_SI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sl_SI/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sl_SI/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sq_AL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sq_AL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sq_AL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sq_AL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sr@latin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sr@latin/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sr@latin/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sr@latin/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.458980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.478980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.482980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ta/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ta/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.482980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/th/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/th/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/th_TH/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.482980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/th_TH/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/th_TH/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/th_TH/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/tlh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.482980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/tlh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/tlh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/tlh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.482980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ug/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.482980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ug/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ug/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ug/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.482980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.482980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ur/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ur/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.482980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/vi_VN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.482980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/vi_VN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/vi_VN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/vi_VN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.482980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.482980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.482980 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.486980 djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0002_auto_20160622_1031.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0003_auto_20160825_1829.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0004_adapted_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0005_create_nested_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0006_remove_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0007_reset_null_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0008_removed_null_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0009_googlemapmarker_icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0010_auto_20190718_1021.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0011_googlemap_map_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/static/djangocms_googlemap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.486980 djangocms-googlemap-2.1.0/djangocms_googlemap/static/djangocms_googlemap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/static/djangocms_googlemap/js/djangocms.googlemap.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.462980 djangocms-googlemap-2.1.0/djangocms_googlemap/templates/djangocms_googlemap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.486980 djangocms-googlemap-2.1.0/djangocms_googlemap/templates/djangocms_googlemap/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/templates/djangocms_googlemap/default/map.html
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/templates/djangocms_googlemap/default/marker.html
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/djangocms_googlemap/templates/djangocms_googlemap/default/route.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.466980 djangocms-googlemap-2.1.0/djangocms_googlemap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-16 08:49:36.000000 djangocms-googlemap-2.1.0/djangocms_googlemap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-16 08:49:36.000000 djangocms-googlemap-2.1.0/djangocms_googlemap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:49:36.000000 djangocms-googlemap-2.1.0/djangocms_googlemap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:49:36.000000 djangocms-googlemap-2.1.0/djangocms_googlemap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-16 08:49:36.000000 djangocms-googlemap-2.1.0/djangocms_googlemap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 08:49:36.000000 djangocms-googlemap-2.1.0/djangocms_googlemap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:49:36.486980 djangocms-googlemap-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:36.486980 djangocms-googlemap-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-16 08:49:27.000000 djangocms-googlemap-2.1.0/tests/test_plugins.py
```

### Comparing `djangocms-googlemap-2.0.0/LICENSE` & `djangocms-googlemap-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/PKG-INFO` & `djangocms-googlemap-2.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,125 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: djangocms-googlemap
-Version: 2.0.0
+Version: 2.1.0
 Summary: Adds Google Maps plugins to django CMS.
-Home-page: https://github.com/divio/djangocms-googlemap
+Home-page: https://github.com/django-cms/djangocms-googlemap
 Author: Divio AG
 Author-email: info@divio.com
+Maintainer: Django CMS Association and contributors
+Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
-Description: =====================
-        django CMS Google Map
-        =====================
-        
-        |pypi| |build| |coverage|
-        
-        **django CMS Google Map** is a set of plugins for `django CMS <http://django-cms.org>`_
-        that allow you to implement `Google Map <https://developers.google.com/maps/>`_ into your website.
-        
-        This addon is compatible with `Divio Cloud <http://divio.com>`_ and is also available on the
-        `django CMS Marketplace <https://marketplace.django-cms.org/en/addons/browse/djangocms-googlemap/>`_
-        for easy installation.
-        
-        .. image:: preview.gif
-        
-        
-        Contributing
-        ============
-        
-        This is a an open-source project. We'll be delighted to receive your
-        feedback in the form of issues and pull requests. Before submitting your
-        pull request, please review our `contribution guidelines
-        <http://docs.django-cms.org/en/latest/contributing/index.html>`_.
-        
-        We're grateful to all contributors who have helped create and maintain this package.
-        Contributors are listed at the `contributors <https://github.com/divio/djangocms-googlemap/graphs/contributors>`_
-        section.
-        
-        One of the easiest contributions you can make is helping to translate this addon on
-        `Transifex <https://www.transifex.com/projects/p/djangocms-googlemap/>`_.
-        
-        
-        Documentation
-        =============
-        
-        See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-googlemap/blob/master/setup.py>`_
-        file for additional dependencies:
-        
-        |python| |django| |djangocms|
-        
-        * Django Filer 1.7 or higher
-        
-        Make sure `django-filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
-        is installed and configured appropriately.
-        
-        
-        Installation
-        ------------
-        
-        For a manual install:
-        
-        * run ``pip install djangocms-googlemap``
-        * add ``djangocms_googlemap`` to your ``INSTALLED_APPS``
-        * run ``python manage.py migrate djangocms_googlemap``
-        
-        
-        Configuration
-        -------------
-        
-        django CMS Google Map **requires** an
-        `API key from Google <https://developers.google.com/maps/documentation/embed/guide>`_,
-        that needs to be supplied in your Django settings: ::
-        
-            DJANGOCMS_GOOGLEMAP_API_KEY = ''
-        
-        Note that the provided templates are minimal by design. You are encouraged
-        to adapt and override them to your project's requirements. The included
-        demo JavaScript does not require jQuery or any other 3rd party library
-        other than Google Maps own JavaScript, which will be loaded automatically.
-        
-        This addon provides a ``default`` template for all instances. You can provide
-        additional template choices by adding a ``DJANGOCMS_GOOGLEMAP_TEMPLATES``
-        setting::
-        
-            DJANGOCMS_GOOGLEMAP_TEMPLATES = [
-                ('feature', _('Featured Version')),
-            ]
-        
-        You'll need to create the `feature` folder inside ``templates/djangocms_googlemap/``
-        otherwise you will get a *template does not exist* error. You can do this by
-        copying the ``default`` folder inside that directory and renaming it to
-        ``feature``.
-        
-        
-        Running Tests
-        -------------
-        
-        You can run tests by executing::
-        
-            virtualenv env
-            source env/bin/activate
-            pip install -r tests/requirements.txt
-            python setup.py test
-        
-        
-        .. |pypi| image:: https://badge.fury.io/py/djangocms-googlemap.svg
-            :target: http://badge.fury.io/py/djangocms-googlemap
-        .. |build| image:: https://travis-ci.org/divio/djangocms-googlemap.svg?branch=master
-            :target: https://travis-ci.org/divio/djangocms-googlemap
-        .. |coverage| image:: https://codecov.io/gh/divio/djangocms-googlemap/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/divio/djangocms-googlemap
-        
-        .. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
-            :target: https://pypi.org/project/djangocms-googlemap/
-        .. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
-            :target: https://www.djangoproject.com/
-        .. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
-            :target: https://www.django-cms.org/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -134,7 +26,120 @@
 Classifier: Framework :: Django CMS
 Classifier: Framework :: Django CMS :: 3.7
 Classifier: Framework :: Django CMS :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
+
+=====================
+django CMS Google Map
+=====================
+
+|pypi| |build| |coverage|
+
+**django CMS Google Map** is a set of plugins for `django CMS <http://django-cms.org>`_
+that allow you to implement `Google Map <https://developers.google.com/maps/>`_ into your website.
+
+This addon is compatible with `Divio Cloud <http://divio.com>`_ and is also available on the
+`django CMS Marketplace <https://marketplace.django-cms.org/en/addons/browse/djangocms-googlemap/>`_
+for easy installation.
+
+.. image:: preview.gif
+
+
+Contributing
+============
+
+This is a an open-source project. We'll be delighted to receive your
+feedback in the form of issues and pull requests. Before submitting your
+pull request, please review our `contribution guidelines
+<http://docs.django-cms.org/en/latest/contributing/index.html>`_.
+
+We're grateful to all contributors who have helped create and maintain this package.
+Contributors are listed at the `contributors <https://github.com/divio/djangocms-googlemap/graphs/contributors>`_
+section.
+
+One of the easiest contributions you can make is helping to translate this addon on
+`Transifex <https://www.transifex.com/projects/p/djangocms-googlemap/>`_.
+
+
+Documentation
+=============
+
+See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-googlemap/blob/master/setup.py>`_
+file for additional dependencies:
+
+|python| |django| |djangocms|
+
+* Django Filer 1.7 or higher
+
+Make sure `django-filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
+is installed and configured appropriately.
+
+
+Installation
+------------
+
+For a manual install:
+
+* run ``pip install djangocms-googlemap``
+* add ``djangocms_googlemap`` to your ``INSTALLED_APPS``
+* run ``python manage.py migrate djangocms_googlemap``
+
+
+Configuration
+-------------
+
+django CMS Google Map **requires** an
+`API key from Google <https://developers.google.com/maps/documentation/javascript/get-api-key>`_,
+that needs to be supplied in your Django settings: ::
+
+    DJANGOCMS_GOOGLEMAP_API_KEY = ''
+
+Note that the provided templates are minimal by design. You are encouraged
+to adapt and override them to your project's requirements. The included
+demo JavaScript does not require jQuery or any other 3rd party library
+other than Google Maps own Maps JavaScript API, which will be loaded automatically.
+
+This addon provides a ``default`` template for all instances. You can provide
+additional template choices by adding a ``DJANGOCMS_GOOGLEMAP_TEMPLATES``
+setting::
+
+    DJANGOCMS_GOOGLEMAP_TEMPLATES = [
+        ('feature', _('Featured Version')),
+    ]
+
+You'll need to create the `feature` folder inside ``templates/djangocms_googlemap/``
+otherwise you will get a *template does not exist* error. You can do this by
+copying the ``default`` folder inside that directory and renaming it to
+``feature``.
+
+For more details on customizing maps see Google `Maps JavaScript API <https://developers.google.com/maps/documentation/javascript/overview>`_
+documentation, as well as default templates in ``templates/djangocms_googlemap/default`` of
+**django CMS Google Map** plugin for options supported by this plugin.
+
+Running Tests
+-------------
+
+You can run tests by executing::
+
+    virtualenv env
+    source env/bin/activate
+    pip install -r tests/requirements.txt
+    python setup.py test
+
+
+.. |pypi| image:: https://badge.fury.io/py/djangocms-googlemap.svg
+    :target: http://badge.fury.io/py/djangocms-googlemap
+.. |build| image:: https://travis-ci.org/divio/djangocms-googlemap.svg?branch=master
+    :target: https://travis-ci.org/divio/djangocms-googlemap
+.. |coverage| image:: https://codecov.io/gh/divio/djangocms-googlemap/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/divio/djangocms-googlemap
+
+.. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
+    :target: https://pypi.org/project/djangocms-googlemap/
+.. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
+    :target: https://www.djangoproject.com/
+.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
+    :target: https://www.django-cms.org/
```

### Comparing `djangocms-googlemap-2.0.0/README.rst` & `djangocms-googlemap-2.1.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -54,37 +54,40 @@
 * run ``python manage.py migrate djangocms_googlemap``
 
 
 Configuration
 -------------
 
 django CMS Google Map **requires** an
-`API key from Google <https://developers.google.com/maps/documentation/embed/guide>`_,
+`API key from Google <https://developers.google.com/maps/documentation/javascript/get-api-key>`_,
 that needs to be supplied in your Django settings: ::
 
     DJANGOCMS_GOOGLEMAP_API_KEY = ''
 
 Note that the provided templates are minimal by design. You are encouraged
 to adapt and override them to your project's requirements. The included
 demo JavaScript does not require jQuery or any other 3rd party library
-other than Google Maps own JavaScript, which will be loaded automatically.
+other than Google Maps own Maps JavaScript API, which will be loaded automatically.
 
 This addon provides a ``default`` template for all instances. You can provide
 additional template choices by adding a ``DJANGOCMS_GOOGLEMAP_TEMPLATES``
 setting::
 
     DJANGOCMS_GOOGLEMAP_TEMPLATES = [
         ('feature', _('Featured Version')),
     ]
 
 You'll need to create the `feature` folder inside ``templates/djangocms_googlemap/``
 otherwise you will get a *template does not exist* error. You can do this by
 copying the ``default`` folder inside that directory and renaming it to
 ``feature``.
 
+For more details on customizing maps see Google `Maps JavaScript API <https://developers.google.com/maps/documentation/javascript/overview>`_
+documentation, as well as default templates in ``templates/djangocms_googlemap/default`` of
+**django CMS Google Map** plugin for options supported by this plugin.
 
 Running Tests
 -------------
 
 You can run tests by executing::
 
     virtualenv env
```

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/cms_plugins.py` & `djangocms-googlemap-2.1.0/djangocms_googlemap/cms_plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             )
         }),
         (_('Advanced settings'), {
             'classes': ('collapse',),
             'fields': (
                 'template',
                 ('lat', 'lng',),
+                'map_id',
                 'style',
             )
         }),
         (_('Control settings'), {
             'classes': ('collapse',),
             'fields': (
                 ('zoom', 'map_type_control',),
```

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/af/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/af/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ar/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ar/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/be/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/be/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/be/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/be/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/bg/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/bg/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/bn/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/bn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ca/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ca/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cmn/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cmn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cs/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cs/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/cy/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/cy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/da/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/da/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/de/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/de/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/el/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/el/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/en/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/en/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_AR/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_AR/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_BO/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_BO/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_BO/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_BO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/es_DO/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/es_DO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/et/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/eu/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/eu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/eu/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fa/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fa/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fi/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fi/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/fr/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ga/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ga/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/gl/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/gu/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/gu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/he/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/he/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hi/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hi/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hr/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hr/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hu/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/hu/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/id/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/is/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/is/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/is/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/is_IS/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/is_IS/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/it/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ja/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ja/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ka/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/kk/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/kk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/kk/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/kk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/km/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/km/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/km/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/km/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ko/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ko_KR/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ko_KR/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ku_IQ/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ku_IQ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ku_IQ/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ku_IQ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/lt/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/lt/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/lv/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mn/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mn_MN/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mn_MN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/mt/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/mt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/nb/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/nb/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/nl/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/nl/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/no/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/no/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/no/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/no/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pl/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pl/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pt/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pt/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pt_BR/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/pt_BR/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ro/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ro/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ru/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ru/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sk/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sk/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sl/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sl_SI/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sl_SI/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sl_SI/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sl_SI/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sq/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sq_AL/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sq_AL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sr/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sr@latin/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sr@latin/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sr@latin/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sr@latin/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sv/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/sv/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ta/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ta/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ta/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ta/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/th/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/th/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/th_TH/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/th_TH/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/tlh/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/tlh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/tr/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/tr/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ug/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ug/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/uk/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/uk/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/ur/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/ur/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/vi/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/vi_VN/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/vi_VN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh_CN/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh_CN/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh_TW/LC_MESSAGES/django.mo` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/locale/zh_TW/LC_MESSAGES/django.po` & `djangocms-googlemap-2.1.0/djangocms_googlemap/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0001_initial.py` & `djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0002_auto_20160622_1031.py` & `djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0002_auto_20160622_1031.py`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0004_adapted_fields.py` & `djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0004_adapted_fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0005_create_nested_plugins.py` & `djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0005_create_nested_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.db import migrations, models
 
 
 def add_plugin(apps, plugin_type, plugin_model, language, placeholder, parent, **data):  # pragma: no cover
     from cms.models import CMSPlugin
+
     from treebeard.mp_tree import MP_AddChildHandler
 
     # This is a CMSPlugin instance which represents the model's
     # current state for the current migration
     plugin = apps.get_model('cms', 'CMSPlugin')(
         parent=parent,
         placeholder=placeholder,
```

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0006_remove_fields.py` & `djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0006_remove_fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0009_googlemapmarker_icon.py` & `djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0009_googlemapmarker_icon.py`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/migrations/0010_auto_20190718_1021.py` & `djangocms-googlemap-2.1.0/djangocms_googlemap/migrations/0010_auto_20190718_1021.py`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/models.py` & `djangocms-googlemap-2.1.0/djangocms_googlemap/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,21 @@
     )
     style = models.TextField(
         verbose_name=_('Map styling'),
         blank=True,
         help_text=_('Provide a valid (escaped) JSON configuration. See '
                     'http://developers.google.com/maps/documentation/javascript/styling'),
     )
+    map_id = models.CharField(
+        verbose_name=_('Map ID'),
+        max_length=32,
+        blank=True,
+        help_text=_('Map ID of Cloud-based maps styling. See '
+                    'https://developers.google.com/maps/documentation/cloud-customization/overview'),
+    )
     lat = models.FloatField(
         verbose_name=_('Latitude (lat)'),
         null=True,
         blank=True,
         help_text=_('Default Geographical latitude in degrees (e.g. "46.947973").'),
     )
     lng = models.FloatField(
```

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/static/djangocms_googlemap/js/djangocms.googlemap.js` & `djangocms-googlemap-2.1.0/djangocms_googlemap/static/djangocms_googlemap/js/djangocms.googlemap.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -40,14 +40,15 @@
         function GoogleMapConstructor(container) {
             this.container = container;
             this.markers = [];
             this.bounds = new google.maps.LatLngBounds();
             this.settings = {
                 zoom: parseInt(getAttr(container, 'zoom')),
                 styles: JSON.parse(getAttr(container, 'style') || false),
+                mapId: getAttr(container, 'map-id'),
                 zoomControl: getAttr(container, 'zoom-control'),
                 streetViewControl: getAttr(container, 'street-view-control'),
                 rotateControl: getAttr(container, 'rotate-control'),
                 scaleControl: getAttr(container, 'scale-control'),
                 fullscreenControl: getAttr(container, 'fullscreen-control'),
                 panControl: getAttr(container, 'pan-control'),
                 disableDoubleClickZoom: getAttr(container, 'double-click-zoom') === false,
@@ -313,14 +314,18 @@
             if (!container.hasChildNodes()) {
                 new GoogleMap(element);
             }
         }, this);
 
     }
 
+    // make sure callback function is updated in 'djangocms_googlemap' namespace
+    window.djangocms_googlemap = window.djangocms_googlemap || {};
+    window.djangocms_googlemap.InitMap = InitMap;
+
     // make sure google maps is loaded after our dom is ready
     window.addEventListener('load', function() {
         InitMap();
     });
 
     if (window.CMS !== undefined) {
         CMS.$(window).on('cms-content-refresh', function() {
```

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/templates/djangocms_googlemap/default/map.html` & `djangocms-googlemap-2.1.0/djangocms_googlemap/templates/djangocms_googlemap/default/map.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 {% load i18n static sekizai_tags cms_tags %}
+{% get_current_language as LANGUAGE_CODE %}
 
 <div class="djangocms-googlemap js-djangocms-googlemap"
     data-zoom="{{ instance.zoom }}"
     data-style="{{ instance.style }}"
+    data-map-id="{{ instance.map_id }}"
     data-lat="{{ instance.lat|stringformat:"f" }}"
     data-lng="{{ instance.lng|stringformat:"f" }}"
     data-zoom-control="{{ instance.zoom_control|lower }}"
     data-street-view-control="{{ instance.street_view_control|lower }}"
     data-rotate-control="{{ instance.rotate_control|lower }}"
     data-scale-control="{{ instance.scale_control|lower }}"
     data-fullscreen-control="{{ instance.fullscreen_control|lower }}"
@@ -50,15 +52,16 @@
 {% comment %}
 cms_js_classes are for injecting and executing javascript code properly,
 when the plugin is added to a page for the first time
 {% endcomment %}
 {% with cms_js_classes="cms-execute-js-to-render cms-trigger-event-window-load" %}
     {% addtoblock "js" %}
         {% spaceless %}
-            <script src="https://maps.googleapis.com/maps/api/js{% if googlemap_key %}?key={{ googlemap_key }}{% endif %}"
+            <script>var djangocms_googlemap = window.djangocms_googlemap || { InitMap: function(){} };</script>
+            <script src="https://maps.googleapis.com/maps/api/js?callback=djangocms_googlemap.InitMap&language={{ LANGUAGE_CODE }}{% if googlemap_key %}&key={{ googlemap_key }}{% endif %}"
                 {% if request.toolbar and request.toolbar.edit_mode_active or request.toolbar and request.toolbar.edit_mode %}
                     class="{{cms_js_classes}}"
                 {% endif %}
             async defer>
             </script>
         {% endspaceless %}
     {% endaddtoblock %}
@@ -79,14 +82,15 @@
     {{ googlemap_key }}
 
     {{ instance.title }}
     {{ instance.width }}
     {{ instance.height }}
     {{ instance.zoom }}
     {{ instance.style }}
+    {{ instance.map_id }}
 
     {{ instance.map_type_control }}
     {{ instance.zoom_control }}
     {{ instance.street_view_control }}
     {{ instance.rotate_control }}
     {{ instance.scale_control }}
     {{ instance.fullscreen_control }}
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-{% load i18n static sekizai_tags cms_tags %}
+{% load i18n static sekizai_tags cms_tags %} {% get_current_language as
+LANGUAGE_CODE %}
  }}" data-lng="{{Â instance.lng|stringformat:"f" }}" data-zoom-control="{
 { instance.zoom_control|lower }}" data-street-view-control="{
 { instance.street_view_control|lower }}" data-rotate-control="{
 { instance.rotate_control|lower }}" data-scale-control="{
 { instance.scale_control|lower }}" data-fullscreen-control="{
 { instance.fullscreen_control|lower }}" data-pan-control="{
 { instance.pan_control|lower }}" data-double-click-zoom="{
@@ -19,23 +20,24 @@
 examples {% endcomment %} {% if request.toolbar and
 request.toolbar.edit_mode_active or request.toolbar and
 request.toolbar.edit_mode %} {% addtoblock "css" %}
  {% endaddtoblock %} {% endif %} {% comment %} cms_js_classes are for injecting
 and executing javascript code properly, when the plugin is added to a page for
 the first time {% endcomment %} {% with cms_js_classes="cms-execute-js-to-
 render cms-trigger-event-window-load" %} {% addtoblock "js" %} {% spaceless %}
+
 % if request.toolbar and request.toolbar.edit_mode_active or request.toolbar
 and request.toolbar.edit_mode %} class="{{cms_js_classes}}" {% endif %} async
 defer>
 {% endspaceless %} {% endaddtoblock %} {% addtoblock "js" %} {% spaceless %}
 % if request.toolbar and request.toolbar.edit_mode_active or request.toolbar
 and request.toolbar.edit_mode %} class="{{cms_js_classes}}" {% endif %} async
 defer>
 {% endspaceless %} {% endaddtoblock %} {% endwith %} {% comment %} {
 { googlemap_key }} {{Â instance.title }} {{Â instance.width }} {
 {Â instance.height }} {{Â instance.zoom }} {{Â instance.style }} {
-{Â instance.map_type_control }} {{Â instance.zoom_control }} {
-{Â instance.street_view_control }} {{Â instance.rotate_control }} {
+{ instance.map_id }} {{Â instance.map_type_control }} {{Â instance.zoom_control
+}} {{Â instance.street_view_control }} {{Â instance.rotate_control }} {
 {Â instance.scale_control }} {{Â instance.fullscreen_control }} {
 {Â instance.pan_control }} {{Â instance.double_click_zoom }} {
 {Â instance.draggable }} {{Â instance.keyboard_shortcuts }} {
 {Â instance.scrollwheel }} {% endcomment %}
```

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap/templates/djangocms_googlemap/default/marker.html` & `djangocms-googlemap-2.1.0/djangocms_googlemap/templates/djangocms_googlemap/default/marker.html`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap.egg-info/PKG-INFO` & `djangocms-googlemap-2.1.0/djangocms_googlemap.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,125 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: djangocms-googlemap
-Version: 2.0.0
+Version: 2.1.0
 Summary: Adds Google Maps plugins to django CMS.
-Home-page: https://github.com/divio/djangocms-googlemap
+Home-page: https://github.com/django-cms/djangocms-googlemap
 Author: Divio AG
 Author-email: info@divio.com
+Maintainer: Django CMS Association and contributors
+Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
-Description: =====================
-        django CMS Google Map
-        =====================
-        
-        |pypi| |build| |coverage|
-        
-        **django CMS Google Map** is a set of plugins for `django CMS <http://django-cms.org>`_
-        that allow you to implement `Google Map <https://developers.google.com/maps/>`_ into your website.
-        
-        This addon is compatible with `Divio Cloud <http://divio.com>`_ and is also available on the
-        `django CMS Marketplace <https://marketplace.django-cms.org/en/addons/browse/djangocms-googlemap/>`_
-        for easy installation.
-        
-        .. image:: preview.gif
-        
-        
-        Contributing
-        ============
-        
-        This is a an open-source project. We'll be delighted to receive your
-        feedback in the form of issues and pull requests. Before submitting your
-        pull request, please review our `contribution guidelines
-        <http://docs.django-cms.org/en/latest/contributing/index.html>`_.
-        
-        We're grateful to all contributors who have helped create and maintain this package.
-        Contributors are listed at the `contributors <https://github.com/divio/djangocms-googlemap/graphs/contributors>`_
-        section.
-        
-        One of the easiest contributions you can make is helping to translate this addon on
-        `Transifex <https://www.transifex.com/projects/p/djangocms-googlemap/>`_.
-        
-        
-        Documentation
-        =============
-        
-        See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-googlemap/blob/master/setup.py>`_
-        file for additional dependencies:
-        
-        |python| |django| |djangocms|
-        
-        * Django Filer 1.7 or higher
-        
-        Make sure `django-filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
-        is installed and configured appropriately.
-        
-        
-        Installation
-        ------------
-        
-        For a manual install:
-        
-        * run ``pip install djangocms-googlemap``
-        * add ``djangocms_googlemap`` to your ``INSTALLED_APPS``
-        * run ``python manage.py migrate djangocms_googlemap``
-        
-        
-        Configuration
-        -------------
-        
-        django CMS Google Map **requires** an
-        `API key from Google <https://developers.google.com/maps/documentation/embed/guide>`_,
-        that needs to be supplied in your Django settings: ::
-        
-            DJANGOCMS_GOOGLEMAP_API_KEY = ''
-        
-        Note that the provided templates are minimal by design. You are encouraged
-        to adapt and override them to your project's requirements. The included
-        demo JavaScript does not require jQuery or any other 3rd party library
-        other than Google Maps own JavaScript, which will be loaded automatically.
-        
-        This addon provides a ``default`` template for all instances. You can provide
-        additional template choices by adding a ``DJANGOCMS_GOOGLEMAP_TEMPLATES``
-        setting::
-        
-            DJANGOCMS_GOOGLEMAP_TEMPLATES = [
-                ('feature', _('Featured Version')),
-            ]
-        
-        You'll need to create the `feature` folder inside ``templates/djangocms_googlemap/``
-        otherwise you will get a *template does not exist* error. You can do this by
-        copying the ``default`` folder inside that directory and renaming it to
-        ``feature``.
-        
-        
-        Running Tests
-        -------------
-        
-        You can run tests by executing::
-        
-            virtualenv env
-            source env/bin/activate
-            pip install -r tests/requirements.txt
-            python setup.py test
-        
-        
-        .. |pypi| image:: https://badge.fury.io/py/djangocms-googlemap.svg
-            :target: http://badge.fury.io/py/djangocms-googlemap
-        .. |build| image:: https://travis-ci.org/divio/djangocms-googlemap.svg?branch=master
-            :target: https://travis-ci.org/divio/djangocms-googlemap
-        .. |coverage| image:: https://codecov.io/gh/divio/djangocms-googlemap/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/divio/djangocms-googlemap
-        
-        .. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
-            :target: https://pypi.org/project/djangocms-googlemap/
-        .. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
-            :target: https://www.djangoproject.com/
-        .. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
-            :target: https://www.django-cms.org/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -134,7 +26,120 @@
 Classifier: Framework :: Django CMS
 Classifier: Framework :: Django CMS :: 3.7
 Classifier: Framework :: Django CMS :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
+
+=====================
+django CMS Google Map
+=====================
+
+|pypi| |build| |coverage|
+
+**django CMS Google Map** is a set of plugins for `django CMS <http://django-cms.org>`_
+that allow you to implement `Google Map <https://developers.google.com/maps/>`_ into your website.
+
+This addon is compatible with `Divio Cloud <http://divio.com>`_ and is also available on the
+`django CMS Marketplace <https://marketplace.django-cms.org/en/addons/browse/djangocms-googlemap/>`_
+for easy installation.
+
+.. image:: preview.gif
+
+
+Contributing
+============
+
+This is a an open-source project. We'll be delighted to receive your
+feedback in the form of issues and pull requests. Before submitting your
+pull request, please review our `contribution guidelines
+<http://docs.django-cms.org/en/latest/contributing/index.html>`_.
+
+We're grateful to all contributors who have helped create and maintain this package.
+Contributors are listed at the `contributors <https://github.com/divio/djangocms-googlemap/graphs/contributors>`_
+section.
+
+One of the easiest contributions you can make is helping to translate this addon on
+`Transifex <https://www.transifex.com/projects/p/djangocms-googlemap/>`_.
+
+
+Documentation
+=============
+
+See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-googlemap/blob/master/setup.py>`_
+file for additional dependencies:
+
+|python| |django| |djangocms|
+
+* Django Filer 1.7 or higher
+
+Make sure `django-filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
+is installed and configured appropriately.
+
+
+Installation
+------------
+
+For a manual install:
+
+* run ``pip install djangocms-googlemap``
+* add ``djangocms_googlemap`` to your ``INSTALLED_APPS``
+* run ``python manage.py migrate djangocms_googlemap``
+
+
+Configuration
+-------------
+
+django CMS Google Map **requires** an
+`API key from Google <https://developers.google.com/maps/documentation/javascript/get-api-key>`_,
+that needs to be supplied in your Django settings: ::
+
+    DJANGOCMS_GOOGLEMAP_API_KEY = ''
+
+Note that the provided templates are minimal by design. You are encouraged
+to adapt and override them to your project's requirements. The included
+demo JavaScript does not require jQuery or any other 3rd party library
+other than Google Maps own Maps JavaScript API, which will be loaded automatically.
+
+This addon provides a ``default`` template for all instances. You can provide
+additional template choices by adding a ``DJANGOCMS_GOOGLEMAP_TEMPLATES``
+setting::
+
+    DJANGOCMS_GOOGLEMAP_TEMPLATES = [
+        ('feature', _('Featured Version')),
+    ]
+
+You'll need to create the `feature` folder inside ``templates/djangocms_googlemap/``
+otherwise you will get a *template does not exist* error. You can do this by
+copying the ``default`` folder inside that directory and renaming it to
+``feature``.
+
+For more details on customizing maps see Google `Maps JavaScript API <https://developers.google.com/maps/documentation/javascript/overview>`_
+documentation, as well as default templates in ``templates/djangocms_googlemap/default`` of
+**django CMS Google Map** plugin for options supported by this plugin.
+
+Running Tests
+-------------
+
+You can run tests by executing::
+
+    virtualenv env
+    source env/bin/activate
+    pip install -r tests/requirements.txt
+    python setup.py test
+
+
+.. |pypi| image:: https://badge.fury.io/py/djangocms-googlemap.svg
+    :target: http://badge.fury.io/py/djangocms-googlemap
+.. |build| image:: https://travis-ci.org/divio/djangocms-googlemap.svg?branch=master
+    :target: https://travis-ci.org/divio/djangocms-googlemap
+.. |coverage| image:: https://codecov.io/gh/divio/djangocms-googlemap/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/divio/djangocms-googlemap
+
+.. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
+    :target: https://pypi.org/project/djangocms-googlemap/
+.. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
+    :target: https://www.djangoproject.com/
+.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
+    :target: https://www.django-cms.org/
```

### Comparing `djangocms-googlemap-2.0.0/djangocms_googlemap.egg-info/SOURCES.txt` & `djangocms-googlemap-2.1.0/djangocms_googlemap.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -165,14 +165,15 @@
 djangocms_googlemap/migrations/0004_adapted_fields.py
 djangocms_googlemap/migrations/0005_create_nested_plugins.py
 djangocms_googlemap/migrations/0006_remove_fields.py
 djangocms_googlemap/migrations/0007_reset_null_values.py
 djangocms_googlemap/migrations/0008_removed_null_fields.py
 djangocms_googlemap/migrations/0009_googlemapmarker_icon.py
 djangocms_googlemap/migrations/0010_auto_20190718_1021.py
+djangocms_googlemap/migrations/0011_googlemap_map_id.py
 djangocms_googlemap/migrations/__init__.py
 djangocms_googlemap/static/djangocms_googlemap/js/djangocms.googlemap.js
 djangocms_googlemap/templates/djangocms_googlemap/default/map.html
 djangocms_googlemap/templates/djangocms_googlemap/default/marker.html
 djangocms_googlemap/templates/djangocms_googlemap/default/route.html
 tests/__init__.py
 tests/helpers.py
```

### Comparing `djangocms-googlemap-2.0.0/setup.py` & `djangocms-googlemap-2.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from setuptools import find_packages, setup
 
 from djangocms_googlemap import __version__
 
 
 REQUIREMENTS = [
     'django-cms>=3.7',
-    'django-filer>=1.7'
+    'django-filer>=1.7',
+    'django-treebeard>=4.3,<4.5',
 ]
 
 
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
@@ -37,15 +38,17 @@
 
 
 setup(
     name='djangocms-googlemap',
     version=__version__,
     author='Divio AG',
     author_email='info@divio.com',
-    url='https://github.com/divio/djangocms-googlemap',
+    maintainer='Django CMS Association and contributors',
+    maintainer_email='info@django-cms.org',
+    url='https://github.com/django-cms/djangocms-googlemap',
     license='BSD-3-Clause',
     description='Adds Google Maps plugins to django CMS.',
     long_description=open('README.rst').read(),
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     install_requires=REQUIREMENTS,
```

### Comparing `djangocms-googlemap-2.0.0/tests/helpers.py` & `djangocms-googlemap-2.1.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/tests/test_migrations.py` & `djangocms-googlemap-2.1.0/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/tests/test_models.py` & `djangocms-googlemap-2.1.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-googlemap-2.0.0/tests/test_plugins.py` & `djangocms-googlemap-2.1.0/tests/test_plugins.py`

 * *Files identical despite different names*

