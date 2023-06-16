# Comparing `tmp/garpixcms-4.3.0.tar.gz` & `tmp/garpixcms-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpixcms-4.3.0.tar", last modified: Wed May 31 09:55:41 2023, max compression
+gzip compressed data, was "garpixcms-4.3.1.tar", last modified: Fri Jun 16 08:42:45 2023, max compression
```

## Comparing `garpixcms-4.3.0.tar` & `garpixcms-4.3.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.447478 garpixcms-4.3.0/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-05-31 09:55:41.000000 garpixcms-4.3.0/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-05-31 09:55:41.447286 garpixcms-4.3.0/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.316962 garpixcms-4.3.0/garpixcms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    13564 2023-05-31 09:55:30.000000 garpixcms-4.3.0/garpixcms/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1084 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1207 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/README.rst
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.320778 garpixcms-4.3.0/garpixcms/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      161 2023-04-18 20:28:30.000000 garpixcms-4.3.0/garpixcms/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-04-18 20:28:30.000000 garpixcms-4.3.0/garpixcms/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6796 2023-04-18 20:28:30.000000 garpixcms-4.3.0/garpixcms/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1743 2023-04-18 20:28:31.000000 garpixcms-4.3.0/garpixcms/__pycache__/urls.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.321025 garpixcms-4.3.0/garpixcms/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/admin/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.371236 garpixcms-4.3.0/garpixcms/admin/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      205 2023-04-18 20:28:31.000000 garpixcms-4.3.0/garpixcms/admin/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      487 2023-04-18 20:28:31.000000 garpixcms-4.3.0/garpixcms/admin/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      173 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/admin/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       93 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/apps.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.371658 garpixcms-4.3.0/garpixcms/contexts/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/contexts/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      691 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/contexts/global_context.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.371814 garpixcms-4.3.0/garpixcms/management/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/management/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.372046 garpixcms-4.3.0/garpixcms/management/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:01:00.000000 garpixcms-4.3.0/garpixcms/management/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.372353 garpixcms-4.3.0/garpixcms/management/commands/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/management/commands/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      872 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/management/commands/update_user_module.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.373161 garpixcms-4.3.0/garpixcms/middleware/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/middleware/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.376916 garpixcms-4.3.0/garpixcms/middleware/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:00:43.000000 garpixcms-4.3.0/garpixcms/middleware/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2037 2023-05-10 14:00:43.000000 garpixcms-4.3.0/garpixcms/middleware/__pycache__/locale.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2196 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/middleware/locale.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.377160 garpixcms-4.3.0/garpixcms/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/models/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.377412 garpixcms-4.3.0/garpixcms/models/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      201 2023-04-18 20:28:31.000000 garpixcms-4.3.0/garpixcms/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      818 2023-04-18 20:28:31.000000 garpixcms-4.3.0/garpixcms/models/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      413 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/models/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-05-31 09:46:31.000000 garpixcms-4.3.0/garpixcms/setup.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.298021 garpixcms-4.3.0/garpixcms/static/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.298185 garpixcms-4.3.0/garpixcms/static/admin/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.422064 garpixcms-4.3.0/garpixcms/static/admin/css/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/css/autocomplete.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    22662 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/css/base.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6469 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/css/changelists.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      355 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/css/dashboard.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      423 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/css/fonts.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8370 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/css/forms.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1185 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/css/login.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/css/nav_sidebar.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    18344 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/css/responsive.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1741 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/css/responsive_rtl.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3487 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/css/rtl.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/css/tabbed_translation_fields.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10010 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/css/widgets.css
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.443340 garpixcms-4.3.0/garpixcms/static/admin/img/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      908 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/img/icon-addlink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      825 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/img/icon-changelink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      218 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/img/icon-custom-checked.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      705 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/img/icon-deletelink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      930 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/img/search.svg
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.443592 garpixcms-4.3.0/garpixcms/static/admin/js/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      291 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/static/admin/js/admin.js
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.315368 garpixcms-4.3.0/garpixcms/templates/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.444161 garpixcms-4.3.0/garpixcms/templates/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4421 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/templates/admin/app_list.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4395 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/templates/admin/base.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      809 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/templates/admin/base_site.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.444304 garpixcms-4.3.0/garpixcms/templates/garpixcms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      450 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/templates/garpixcms/base.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.444958 garpixcms-4.3.0/garpixcms/templates/garpixcms/include/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      730 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/templates/garpixcms/include/footer.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      642 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/templates/garpixcms/include/header.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      428 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/templates/garpixcms/include/login.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.445235 garpixcms-4.3.0/garpixcms/templates/garpixcms/menus/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/templates/garpixcms/menus/footer_menu.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/templates/garpixcms/menus/header_menu.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.445782 garpixcms-4.3.0/garpixcms/templates/garpixcms/pages/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      139 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/templates/garpixcms/pages/default.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/templates/garpixcms/pages/home.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      346 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/templates/garpixcms/pages/login.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.446020 garpixcms-4.3.0/garpixcms/translation/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       49 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/translation/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.447019 garpixcms-4.3.0/garpixcms/translation/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      224 2023-04-18 20:28:31.000000 garpixcms-4.3.0/garpixcms/translation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 20:28:31.000000 garpixcms-4.3.0/garpixcms/translation/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      189 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/translation/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1842 2023-04-18 19:40:20.000000 garpixcms-4.3.0/garpixcms/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-31 09:55:41.320266 garpixcms-4.3.0/garpixcms.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-05-31 09:55:41.000000 garpixcms-4.3.0/garpixcms.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2848 2023-05-31 09:55:41.000000 garpixcms-4.3.0/garpixcms.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-31 09:55:41.000000 garpixcms-4.3.0/garpixcms.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-31 09:55:41.000000 garpixcms-4.3.0/garpixcms.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-05-31 09:55:41.000000 garpixcms-4.3.0/garpixcms.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       10 2023-05-31 09:55:41.000000 garpixcms-4.3.0/garpixcms.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-31 09:55:41.447540 garpixcms-4.3.0/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-05-31 09:55:41.000000 garpixcms-4.3.0/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.208536 garpixcms-4.3.1/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-06-16 08:42:45.000000 garpixcms-4.3.1/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-06-16 08:42:45.208373 garpixcms-4.3.1/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.201181 garpixcms-4.3.1/garpixcms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    13630 2023-06-16 08:42:26.000000 garpixcms-4.3.1/garpixcms/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1084 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1207 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/README.rst
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.202276 garpixcms-4.3.1/garpixcms/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      161 2023-04-18 20:28:30.000000 garpixcms-4.3.1/garpixcms/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-04-18 20:28:30.000000 garpixcms-4.3.1/garpixcms/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6796 2023-04-18 20:28:30.000000 garpixcms-4.3.1/garpixcms/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1743 2023-04-18 20:28:31.000000 garpixcms-4.3.1/garpixcms/__pycache__/urls.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.202489 garpixcms-4.3.1/garpixcms/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/admin/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.202714 garpixcms-4.3.1/garpixcms/admin/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      205 2023-04-18 20:28:31.000000 garpixcms-4.3.1/garpixcms/admin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      487 2023-04-18 20:28:31.000000 garpixcms-4.3.1/garpixcms/admin/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      173 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/admin/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       93 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/apps.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.202913 garpixcms-4.3.1/garpixcms/contexts/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/contexts/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      691 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/contexts/global_context.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.203020 garpixcms-4.3.1/garpixcms/management/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/management/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.203118 garpixcms-4.3.1/garpixcms/management/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:01:00.000000 garpixcms-4.3.1/garpixcms/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.203323 garpixcms-4.3.1/garpixcms/management/commands/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/management/commands/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      872 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/management/commands/update_user_module.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.203512 garpixcms-4.3.1/garpixcms/middleware/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/middleware/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.203730 garpixcms-4.3.1/garpixcms/middleware/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:00:43.000000 garpixcms-4.3.1/garpixcms/middleware/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2037 2023-05-10 14:00:43.000000 garpixcms-4.3.1/garpixcms/middleware/__pycache__/locale.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2196 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/middleware/locale.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.203942 garpixcms-4.3.1/garpixcms/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.204157 garpixcms-4.3.1/garpixcms/models/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      201 2023-04-18 20:28:31.000000 garpixcms-4.3.1/garpixcms/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      818 2023-04-18 20:28:31.000000 garpixcms-4.3.1/garpixcms/models/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      413 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/models/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-06-09 06:28:49.000000 garpixcms-4.3.1/garpixcms/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.199264 garpixcms-4.3.1/garpixcms/static/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.199438 garpixcms-4.3.1/garpixcms/static/admin/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.205617 garpixcms-4.3.1/garpixcms/static/admin/css/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/css/autocomplete.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    22662 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/css/base.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6469 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/css/changelists.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      355 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/css/dashboard.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      423 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/css/fonts.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8370 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/css/forms.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1185 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/css/login.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/css/nav_sidebar.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    18344 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/css/responsive.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1741 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/css/responsive_rtl.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3487 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/css/rtl.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/css/tabbed_translation_fields.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10010 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/css/widgets.css
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.206163 garpixcms-4.3.1/garpixcms/static/admin/img/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      908 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/img/icon-addlink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      825 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/img/icon-changelink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      218 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/img/icon-custom-checked.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      705 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/img/icon-deletelink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      930 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/img/search.svg
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.206280 garpixcms-4.3.1/garpixcms/static/admin/js/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      291 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/static/admin/js/admin.js
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.199611 garpixcms-4.3.1/garpixcms/templates/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.206630 garpixcms-4.3.1/garpixcms/templates/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4421 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/templates/admin/app_list.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4395 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/templates/admin/base.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      809 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/templates/admin/base_site.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.206764 garpixcms-4.3.1/garpixcms/templates/garpixcms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      450 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/templates/garpixcms/base.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.207158 garpixcms-4.3.1/garpixcms/templates/garpixcms/include/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      730 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/templates/garpixcms/include/footer.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      642 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/templates/garpixcms/include/header.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      428 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/templates/garpixcms/include/login.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.207428 garpixcms-4.3.1/garpixcms/templates/garpixcms/menus/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/templates/garpixcms/menus/footer_menu.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/templates/garpixcms/menus/header_menu.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.207757 garpixcms-4.3.1/garpixcms/templates/garpixcms/pages/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      139 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/templates/garpixcms/pages/default.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/templates/garpixcms/pages/home.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      346 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/templates/garpixcms/pages/login.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.207972 garpixcms-4.3.1/garpixcms/translation/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       49 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/translation/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.208191 garpixcms-4.3.1/garpixcms/translation/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      224 2023-04-18 20:28:31.000000 garpixcms-4.3.1/garpixcms/translation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 20:28:31.000000 garpixcms-4.3.1/garpixcms/translation/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      189 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/translation/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1842 2023-04-18 19:40:20.000000 garpixcms-4.3.1/garpixcms/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-16 08:42:45.201833 garpixcms-4.3.1/garpixcms.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-06-16 08:42:45.000000 garpixcms-4.3.1/garpixcms.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2848 2023-06-16 08:42:45.000000 garpixcms-4.3.1/garpixcms.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-16 08:42:45.000000 garpixcms-4.3.1/garpixcms.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-16 08:42:45.000000 garpixcms-4.3.1/garpixcms.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-06-16 08:42:45.000000 garpixcms-4.3.1/garpixcms.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       10 2023-06-16 08:42:45.000000 garpixcms-4.3.1/garpixcms.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-06-16 08:42:45.208583 garpixcms-4.3.1/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-06-16 08:42:45.000000 garpixcms-4.3.1/setup.py
```

### Comparing `garpixcms-4.3.0/PKG-INFO` & `garpixcms-4.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpixcms
-Version: 4.3.0
+Version: 4.3.1
 Home-page: https://github.com/garpixcms/garpixcms
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpixcms-4.3.0/garpixcms/CHANGELOG.md` & `garpixcms-4.3.1/garpixcms/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+### 4.3.1 (09.06.2023)
+
+- Upgrade `garpix_user` to version 3.6.1
+
 ### 4.3.0 (31.05.2023)
 
 - Upgrade `garpix_page` to version 2.48.0
 - Upgrade `garpix_user` to version 3.6.0
 - Update documentation
 
 ### 4.2.0 (29.05.2023)
```

### Comparing `garpixcms-4.3.0/garpixcms/CONTRIBUTING.md` & `garpixcms-4.3.1/garpixcms/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/README.rst` & `garpixcms-4.3.1/garpixcms/README.rst`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/__pycache__/settings.cpython-38.pyc` & `garpixcms-4.3.1/garpixcms/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/__pycache__/urls.cpython-38.pyc` & `garpixcms-4.3.1/garpixcms/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/contexts/global_context.py` & `garpixcms-4.3.1/garpixcms/contexts/global_context.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/management/commands/update_user_module.py` & `garpixcms-4.3.1/garpixcms/management/commands/update_user_module.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/middleware/__pycache__/locale.cpython-38.pyc` & `garpixcms-4.3.1/garpixcms/middleware/__pycache__/locale.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/middleware/locale.py` & `garpixcms-4.3.1/garpixcms/middleware/locale.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/models/__pycache__/page.cpython-38.pyc` & `garpixcms-4.3.1/garpixcms/models/__pycache__/page.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/settings.py` & `garpixcms-4.3.1/garpixcms/settings.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/setup.py` & `garpixcms-4.3.1/garpixcms/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpixcms')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpixcms',
-    version='4.3.0',
+    version='4.3.1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpixcms',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -33,15 +33,15 @@
         'Django >= 3.1, < 4',
         'garpix_utils == 1.8.0',
         'garpix_page == 2.48.0',
         'garpix_menu == 1.16.0',
         'eqator == 2.7.0',
         'garpix_auth == 2.3.0',
         'garpix_notify == 5.16.0',
-        'garpix_user == 3.6.0',
+        'garpix_user == 3.6.1',
         'garpix_package == 2.0.1',
         'psycopg2-binary >= 2.8.6',
         'uwsgi >= 2.0.19.1',
         'environs >= 9.3.2',
         'django-ckeditor == 6.3.0',
         'djangorestframework >= 3.12.4',
         'django-cors-headers >= 3.7.0, <= 3.13.0',
```

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/css/autocomplete.css` & `garpixcms-4.3.1/garpixcms/static/admin/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/css/base.css` & `garpixcms-4.3.1/garpixcms/static/admin/css/base.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/css/changelists.css` & `garpixcms-4.3.1/garpixcms/static/admin/css/changelists.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/css/forms.css` & `garpixcms-4.3.1/garpixcms/static/admin/css/forms.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/css/login.css` & `garpixcms-4.3.1/garpixcms/static/admin/css/login.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/css/nav_sidebar.css` & `garpixcms-4.3.1/garpixcms/static/admin/css/nav_sidebar.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/css/responsive.css` & `garpixcms-4.3.1/garpixcms/static/admin/css/responsive.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/css/responsive_rtl.css` & `garpixcms-4.3.1/garpixcms/static/admin/css/responsive_rtl.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/css/rtl.css` & `garpixcms-4.3.1/garpixcms/static/admin/css/rtl.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/css/widgets.css` & `garpixcms-4.3.1/garpixcms/static/admin/css/widgets.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/img/icon-addlink.svg` & `garpixcms-4.3.1/garpixcms/static/admin/img/icon-addlink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/img/icon-changelink.svg` & `garpixcms-4.3.1/garpixcms/static/admin/img/icon-changelink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/img/icon-deletelink.svg` & `garpixcms-4.3.1/garpixcms/static/admin/img/icon-deletelink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/static/admin/img/search.svg` & `garpixcms-4.3.1/garpixcms/static/admin/img/search.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/templates/admin/app_list.html` & `garpixcms-4.3.1/garpixcms/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/templates/admin/base.html` & `garpixcms-4.3.1/garpixcms/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/templates/admin/base_site.html` & `garpixcms-4.3.1/garpixcms/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/templates/garpixcms/include/footer.html` & `garpixcms-4.3.1/garpixcms/templates/garpixcms/include/footer.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/templates/garpixcms/include/header.html` & `garpixcms-4.3.1/garpixcms/templates/garpixcms/include/header.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms/urls.py` & `garpixcms-4.3.1/garpixcms/urls.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/garpixcms.egg-info/PKG-INFO` & `garpixcms-4.3.1/garpixcms.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpixcms
-Version: 4.3.0
+Version: 4.3.1
 Home-page: https://github.com/garpixcms/garpixcms
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpixcms-4.3.0/garpixcms.egg-info/SOURCES.txt` & `garpixcms-4.3.1/garpixcms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpixcms-4.3.0/setup.py` & `garpixcms-4.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpixcms')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpixcms',
-    version='4.3.0',
+    version='4.3.1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpixcms',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -33,15 +33,15 @@
         'Django >= 3.1, < 4',
         'garpix_utils == 1.8.0',
         'garpix_page == 2.48.0',
         'garpix_menu == 1.16.0',
         'eqator == 2.7.0',
         'garpix_auth == 2.3.0',
         'garpix_notify == 5.16.0',
-        'garpix_user == 3.6.0',
+        'garpix_user == 3.6.1',
         'garpix_package == 2.0.1',
         'psycopg2-binary >= 2.8.6',
         'uwsgi >= 2.0.19.1',
         'environs >= 9.3.2',
         'django-ckeditor == 6.3.0',
         'djangorestframework >= 3.12.4',
         'django-cors-headers >= 3.7.0, <= 3.13.0',
```

