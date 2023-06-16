# Comparing `tmp/trame-client-2.9.1.tar.gz` & `tmp/trame-client-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-client-2.9.1.tar", last modified: Fri Jun 16 21:44:49 2023, max compression
+gzip compressed data, was "trame-client-2.9.2.tar", last modified: Fri Jun 16 21:54:27 2023, max compression
```

## Comparing `trame-client-2.9.1.tar` & `trame-client-2.9.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.272073 trame-client-2.9.1/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-16 21:44:17.000000 trame-client-2.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-16 21:44:17.000000 trame-client-2.9.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3518 2023-06-16 21:44:49.272073 trame-client-2.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2785 2023-06-16 21:44:17.000000 trame-client-2.9.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      842 2023-06-16 21:44:49.272073 trame-client-2.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 21:44:17.000000 trame-client-2.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.264073 trame-client-2.9.1/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.264073 trame-client-2.9.1/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame/modules/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.264073 trame-client-2.9.1/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.264073 trame-client-2.9.1/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      137 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame/widgets/client.py
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame/widgets/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.264073 trame-client-2.9.1/trame_client/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/LICENSE
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.268073 trame-client-2.9.1/trame_client/encoders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/encoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/encoders/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.268073 trame-client-2.9.1/trame_client/module/
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.268073 trame-client-2.9.1/trame_client/module/vue2-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.268073 trame-client-2.9.1/trame_client/module/vue2-www/css/
--rw-r--r--   0 root         (0) root         (0)     1588 2023-06-16 21:44:37.000000 trame-client-2.9.1/trame_client/module/vue2-www/css/app.0b077e70.css
--rw-r--r--   0 root         (0) root         (0)     3963 2023-06-16 21:44:37.000000 trame-client-2.9.1/trame_client/module/vue2-www/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.268073 trame-client-2.9.1/trame_client/module/vue2-www/js/
--rw-r--r--   0 root         (0) root         (0)    23564 2023-06-16 21:44:37.000000 trame-client-2.9.1/trame_client/module/vue2-www/js/app.93852572.js
--rw-r--r--   0 root         (0) root         (0)   170437 2023-06-16 21:44:37.000000 trame-client-2.9.1/trame_client/module/vue2-www/js/chunk-vendors.b42af71c.js
--rw-r--r--   0 root         (0) root         (0)     4506 2023-06-16 21:44:37.000000 trame-client-2.9.1/trame_client/module/vue2-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   107302 2023-06-16 21:44:37.000000 trame-client-2.9.1/trame_client/module/vue2-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/module/vue2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.268073 trame-client-2.9.1/trame_client/module/vue3-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.268073 trame-client-2.9.1/trame_client/module/vue3-www/assets/
--rw-r--r--   0 root         (0) root         (0)   108146 2023-06-16 21:44:44.000000 trame-client-2.9.1/trame_client/module/vue3-www/assets/index-ccad3410.js
--rw-r--r--   0 root         (0) root         (0)     3940 2023-06-16 21:44:44.000000 trame-client-2.9.1/trame_client/module/vue3-www/index.html
--rw-r--r--   0 root         (0) root         (0)     4506 2023-06-16 21:44:44.000000 trame-client-2.9.1/trame_client/module/vue3-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   128872 2023-06-16 21:44:44.000000 trame-client-2.9.1/trame_client/module/vue3-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/module/vue3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.268073 trame-client-2.9.1/trame_client/resources/
--rw-r--r--   0 root         (0) root         (0)     7243 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/resources/attributes.json
--rw-r--r--   0 root         (0) root         (0)        2 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/resources/events.json
--rw-r--r--   0 root         (0) root         (0)      580 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/resources/vue.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.268073 trame-client-2.9.1/trame_client/ui/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5472 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/ui/core.py
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.272073 trame-client-2.9.1/trame_client/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      205 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/utils/defaults.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/utils/testing.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.272073 trame-client-2.9.1/trame_client/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19978 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/widgets/core.py
--rw-r--r--   0 root         (0) root         (0)     3482 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/widgets/generator.py
--rw-r--r--   0 root         (0) root         (0)   193844 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/widgets/html.py
--rw-r--r--   0 root         (0) root         (0)     4670 2023-06-16 21:44:17.000000 trame-client-2.9.1/trame_client/widgets/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:44:49.264073 trame-client-2.9.1/trame_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3518 2023-06-16 21:44:49.000000 trame-client-2.9.1/trame_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1478 2023-06-16 21:44:49.000000 trame-client-2.9.1/trame_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 21:44:49.000000 trame-client-2.9.1/trame_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-16 21:44:49.000000 trame-client-2.9.1/trame_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.478666 trame-client-2.9.2/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-16 21:53:53.000000 trame-client-2.9.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-16 21:53:53.000000 trame-client-2.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-06-16 21:54:27.478666 trame-client-2.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-06-16 21:53:53.000000 trame-client-2.9.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      842 2023-06-16 21:54:27.482666 trame-client-2.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 21:53:53.000000 trame-client-2.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.470666 trame-client-2.9.2/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.470666 trame-client-2.9.2/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/modules/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.470666 trame-client-2.9.2/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.470666 trame-client-2.9.2/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/widgets/client.py
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/widgets/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.470666 trame-client-2.9.2/trame_client/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client/encoders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/encoders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/encoders/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client/module/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client/module/vue2-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client/module/vue2-www/css/
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-16 21:54:15.000000 trame-client-2.9.2/trame_client/module/vue2-www/css/app.0b077e70.css
+-rw-r--r--   0 root         (0) root         (0)     3963 2023-06-16 21:54:15.000000 trame-client-2.9.2/trame_client/module/vue2-www/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client/module/vue2-www/js/
+-rw-r--r--   0 root         (0) root         (0)    23564 2023-06-16 21:54:15.000000 trame-client-2.9.2/trame_client/module/vue2-www/js/app.93852572.js
+-rw-r--r--   0 root         (0) root         (0)   170437 2023-06-16 21:54:15.000000 trame-client-2.9.2/trame_client/module/vue2-www/js/chunk-vendors.b42af71c.js
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-06-16 21:54:15.000000 trame-client-2.9.2/trame_client/module/vue2-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   107302 2023-06-16 21:54:15.000000 trame-client-2.9.2/trame_client/module/vue2-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/module/vue2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client/module/vue3-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.478666 trame-client-2.9.2/trame_client/module/vue3-www/assets/
+-rw-r--r--   0 root         (0) root         (0)   108146 2023-06-16 21:54:22.000000 trame-client-2.9.2/trame_client/module/vue3-www/assets/index-ccad3410.js
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-06-16 21:54:22.000000 trame-client-2.9.2/trame_client/module/vue3-www/index.html
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-06-16 21:54:22.000000 trame-client-2.9.2/trame_client/module/vue3-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   128872 2023-06-16 21:54:22.000000 trame-client-2.9.2/trame_client/module/vue3-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/module/vue3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.478666 trame-client-2.9.2/trame_client/resources/
+-rw-r--r--   0 root         (0) root         (0)     7243 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/resources/attributes.json
+-rw-r--r--   0 root         (0) root         (0)        2 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/resources/events.json
+-rw-r--r--   0 root         (0) root         (0)      580 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/resources/vue.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.478666 trame-client-2.9.2/trame_client/ui/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5472 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/ui/core.py
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.478666 trame-client-2.9.2/trame_client/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      205 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/utils/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/utils/testing.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.478666 trame-client-2.9.2/trame_client/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19978 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/widgets/core.py
+-rw-r--r--   0 root         (0) root         (0)     3482 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/widgets/generator.py
+-rw-r--r--   0 root         (0) root         (0)   193844 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/widgets/html.py
+-rw-r--r--   0 root         (0) root         (0)     4670 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/widgets/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-06-16 21:54:27.000000 trame-client-2.9.2/trame_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-06-16 21:54:27.000000 trame-client-2.9.2/trame_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 21:54:27.000000 trame-client-2.9.2/trame_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-16 21:54:27.000000 trame-client-2.9.2/trame_client.egg-info/top_level.txt
```

### Comparing `trame-client-2.9.1/LICENSE` & `trame-client-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/PKG-INFO` & `trame-client-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 2.9.1
+Version: 2.9.2
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-client-2.9.1/README.rst` & `trame-client-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/setup.cfg` & `trame-client-2.9.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-client
-version = 2.9.1
+version = 2.9.2
 description = Internal client of trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-client-2.9.1/trame_client/LICENSE` & `trame-client-2.9.2/trame_client/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/encoders/numpy.py` & `trame-client-2.9.2/trame_client/encoders/numpy.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/module/vue2-www/css/app.0b077e70.css` & `trame-client-2.9.2/trame_client/module/vue2-www/css/app.0b077e70.css`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/module/vue2-www/index.html` & `trame-client-2.9.2/trame_client/module/vue2-www/index.html`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/module/vue2-www/js/app.93852572.js` & `trame-client-2.9.2/trame_client/module/vue2-www/js/app.93852572.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/module/vue2-www/js/chunk-vendors.b42af71c.js` & `trame-client-2.9.2/trame_client/module/vue2-www/js/chunk-vendors.b42af71c.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/module/vue2-www/logo.png` & `trame-client-2.9.2/trame_client/module/vue2-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/module/vue2-www/vue.global.js` & `trame-client-2.9.2/trame_client/module/vue2-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/module/vue3-www/assets/index-ccad3410.js` & `trame-client-2.9.2/trame_client/module/vue3-www/assets/index-ccad3410.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/module/vue3-www/index.html` & `trame-client-2.9.2/trame_client/module/vue3-www/index.html`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/module/vue3-www/logo.png` & `trame-client-2.9.2/trame_client/module/vue3-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/module/vue3-www/vue.global.js` & `trame-client-2.9.2/trame_client/module/vue3-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/resources/attributes.json` & `trame-client-2.9.2/trame_client/resources/attributes.json`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/resources/vue.json` & `trame-client-2.9.2/trame_client/resources/vue.json`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/ui/core.py` & `trame-client-2.9.2/trame_client/ui/core.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/ui/html.py` & `trame-client-2.9.2/trame_client/ui/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/utils/testing.py` & `trame-client-2.9.2/trame_client/utils/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 def enable_testing(server, *state_monitor):
     server.state.change(*state_monitor)(print_state)
 
     @server.controller.add("on_server_ready")
     def print_server_port(**kwargs):
         print("SERVER_PORT:", server.port, flush=True)
 
+    return server
+
 
 class FixtureHelper:
     def __init__(self, root_path):
         self.root_path = Path(root_path)
 
     def remove_page_urls(self):
         BASE_PATH = self.root_path / "visual_baseline"
```

### Comparing `trame-client-2.9.1/trame_client/utils/version.py` & `trame-client-2.9.2/trame_client/utils/version.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/widgets/core.py` & `trame-client-2.9.2/trame_client/widgets/core.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/widgets/generator.py` & `trame-client-2.9.2/trame_client/widgets/generator.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/widgets/html.py` & `trame-client-2.9.2/trame_client/widgets/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client/widgets/trame.py` & `trame-client-2.9.2/trame_client/widgets/trame.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.1/trame_client.egg-info/PKG-INFO` & `trame-client-2.9.2/trame_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 2.9.1
+Version: 2.9.2
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-client-2.9.1/trame_client.egg-info/SOURCES.txt` & `trame-client-2.9.2/trame_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

