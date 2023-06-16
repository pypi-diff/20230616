# Comparing `tmp/plone.outputfilters-5.0.2.tar.gz` & `tmp/plone.outputfilters-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.outputfilters-5.0.2.tar", last modified: Thu Apr 13 23:39:56 2023, max compression
+gzip compressed data, was "plone.outputfilters-5.0.3.tar", last modified: Fri Jun 16 16:59:00 2023, max compression
```

## Comparing `plone.outputfilters-5.0.2.tar` & `plone.outputfilters-5.0.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.098176 plone.outputfilters-5.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)     8768 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      162 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    16041 2023-04-13 23:39:56.098310 plone.outputfilters-5.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.086078 plone.outputfilters-5.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      736 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.086334 plone.outputfilters-5.0.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.091596 plone.outputfilters-5.0.2/plone/outputfilters/
--rw-r--r--   0 maurits    (501) staff       (20)     2752 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      252 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.093166 plone.outputfilters-5.0.2/plone/outputfilters/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      240 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/browser/captioned_image.pt
--rw-r--r--   0 maurits    (501) staff       (20)      326 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/browser/captioned_image.py
--rw-r--r--   0 maurits    (501) staff       (20)      472 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2267 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/browser/resolveuid.py
--rw-r--r--   0 maurits    (501) staff       (20)      788 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.094547 plone.outputfilters-5.0.2/plone/outputfilters/filters/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/filters/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      865 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/filters/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      373 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/filters/example.py
--rw-r--r--   0 maurits    (501) staff       (20)     1721 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/filters/picture_variants.py
--rw-r--r--   0 maurits    (501) staff       (20)    13893 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/filters/resolveuid_and_caption.py
--rw-r--r--   0 maurits    (501) staff       (20)      744 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      229 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/mimetype.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.082955 plone.outputfilters-5.0.2/plone/outputfilters/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.094963 plone.outputfilters-5.0.2/plone/outputfilters/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/profiles/default/plone.outputfilters.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2902 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1604 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.097051 plone.outputfilters-5.0.2/plone/outputfilters/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    19200 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/image.jpg
--rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/test_apply_filters.py
--rw-r--r--   0 maurits    (501) staff       (20)      787 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/test_docs.py
--rw-r--r--   0 maurits    (501) staff       (20)    11184 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/test_picture_variants.py
--rw-r--r--   0 maurits    (501) staff       (20)    27220 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/test_resolveuid_and_caption.py
--rw-r--r--   0 maurits    (501) staff       (20)     2240 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/tests/test_transforms.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.097948 plone.outputfilters-5.0.2/plone/outputfilters/transforms/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/transforms/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1210 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/transforms/html_to_plone_outputfilters_html.py
--rw-r--r--   0 maurits    (501) staff       (20)      920 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone/outputfilters/transforms/plone_outputfilters_html_to_html.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:39:56.089336 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    16041 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1718 2023-04-13 23:39:56.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      325 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/plone.outputfilters.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1717 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-13 23:39:56.098760 plone.outputfilters-5.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2533 2023-04-13 23:39:55.000000 plone.outputfilters-5.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.796342 plone.outputfilters-5.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)     8920 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      162 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    16193 2023-06-16 16:59:00.796514 plone.outputfilters-5.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.783681 plone.outputfilters-5.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      736 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.783992 plone.outputfilters-5.0.3/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.789606 plone.outputfilters-5.0.3/plone/outputfilters/
+-rw-r--r--   0 maurits    (501) staff       (20)     2752 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      252 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.791051 plone.outputfilters-5.0.3/plone/outputfilters/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      240 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/browser/captioned_image.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      326 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/browser/captioned_image.py
+-rw-r--r--   0 maurits    (501) staff       (20)      472 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2283 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/browser/resolveuid.py
+-rw-r--r--   0 maurits    (501) staff       (20)      788 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.792611 plone.outputfilters-5.0.3/plone/outputfilters/filters/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/filters/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      865 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/filters/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      373 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/filters/example.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1721 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/filters/picture_variants.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13893 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/filters/resolveuid_and_caption.py
+-rw-r--r--   0 maurits    (501) staff       (20)      744 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      229 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/mimetype.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.779625 plone.outputfilters-5.0.3/plone/outputfilters/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.793070 plone.outputfilters-5.0.3/plone/outputfilters/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/profiles/default/plone.outputfilters.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2902 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1604 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.795135 plone.outputfilters-5.0.3/plone/outputfilters/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    19200 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/image.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/test_apply_filters.py
+-rw-r--r--   0 maurits    (501) staff       (20)      787 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/test_docs.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11184 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/test_picture_variants.py
+-rw-r--r--   0 maurits    (501) staff       (20)    27360 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/test_resolveuid_and_caption.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2240 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/test_transforms.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.796110 plone.outputfilters-5.0.3/plone/outputfilters/transforms/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/transforms/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1210 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/transforms/html_to_plone_outputfilters_html.py
+-rw-r--r--   0 maurits    (501) staff       (20)      920 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/transforms/plone_outputfilters_html_to_html.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.786839 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    16193 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1718 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      325 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1717 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-06-16 16:59:00.797095 plone.outputfilters-5.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2533 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/setup.py
```

### Comparing `plone.outputfilters-5.0.2/CHANGES.rst` & `plone.outputfilters-5.0.3/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.3 (2023-06-16)
+------------------
+
+Bug fixes:
+
+
+- Return a 404 Not Found response if the resolveuid view is called with no uuid. @davisagli (#43)
+
+
 5.0.2 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.outputfilters-5.0.2/PKG-INFO` & `plone.outputfilters-5.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.outputfilters
-Version: 5.0.2
+Version: 5.0.3
 Summary: Transformations applied to HTML in Plone text fields as they are rendered
 Home-page: http://github.com/plone/plone.outputfilters
 Author: David Glick, Plone Foundation
 Author-email: davidglick@groundwire.org
 License: GPL
 Keywords: plone transform filter uid caption
 Classifier: Development Status :: 5 - Production/Stable
@@ -218,14 +218,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.3 (2023-06-16)
+------------------
+
+Bug fixes:
+
+
+- Return a 404 Not Found response if the resolveuid view is called with no uuid. @davisagli (#43)
+
+
 5.0.2 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.outputfilters-5.0.2/README.rst` & `plone.outputfilters-5.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/docs/LICENSE.GPL` & `plone.outputfilters-5.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/docs/LICENSE.txt` & `plone.outputfilters-5.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/README.rst` & `plone.outputfilters-5.0.3/plone/outputfilters/README.rst`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/browser/resolveuid.py` & `plone.outputfilters-5.0.3/plone/outputfilters/browser/resolveuid.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     return uuid
 
 
 @implementer(IPublishTraverse)
 class ResolveUIDView(BrowserView):
     """Resolve a URL like /resolveuid/<uuid> to a normalized URL."""
 
+    uuid = None
     subpath = None
 
     def publishTraverse(self, request, name):
         self.uuid = name
         traverse_subpath = self.request["TraversalRequestNameStack"]
         if traverse_subpath:
             traverse_subpath = list(traverse_subpath)
```

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/configure.zcml` & `plone.outputfilters-5.0.3/plone/outputfilters/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/filters/configure.zcml` & `plone.outputfilters-5.0.3/plone/outputfilters/filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/filters/picture_variants.py` & `plone.outputfilters-5.0.3/plone/outputfilters/filters/picture_variants.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/filters/resolveuid_and_caption.py` & `plone.outputfilters-5.0.3/plone/outputfilters/filters/resolveuid_and_caption.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/interfaces.py` & `plone.outputfilters-5.0.3/plone/outputfilters/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/setuphandlers.py` & `plone.outputfilters-5.0.3/plone/outputfilters/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/testing.py` & `plone.outputfilters-5.0.3/plone/outputfilters/testing.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/tests/image.jpg` & `plone.outputfilters-5.0.3/plone/outputfilters/tests/image.jpg`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/tests/test_apply_filters.py` & `plone.outputfilters-5.0.3/plone/outputfilters/tests/test_apply_filters.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/tests/test_docs.py` & `plone.outputfilters-5.0.3/plone/outputfilters/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/tests/test_picture_variants.py` & `plone.outputfilters-5.0.3/plone/outputfilters/tests/test_picture_variants.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/tests/test_resolveuid_and_caption.py` & `plone.outputfilters-5.0.3/plone/outputfilters/tests/test_resolveuid_and_caption.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,14 +295,18 @@
         self.assertEqual(301, res.status)
         self.assertEqual("http://nohost/plone/image.jpg", res.headers["location"])
 
     def test_resolveuid_view_bad_uuid(self):
         res = self.publish("/plone/resolveuid/BOGUS")
         self.assertEqual(404, res.status)
 
+    def test_resolveuid_view_missing_uuid(self):
+        res = self.publish("/plone/resolveuid")
+        self.assertEqual(404, res.status)
+
     def test_resolveuid_view_subpath(self):
         res = self.publish("/plone/resolveuid/%s/image_thumb" % self.UID)
         self.assertEqual(301, res.status)
         self.assertEqual(
             "http://nohost/plone/image.jpg/image_thumb", res.headers["location"]
         )
```

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/tests/test_transforms.py` & `plone.outputfilters-5.0.3/plone/outputfilters/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/transforms/html_to_plone_outputfilters_html.py` & `plone.outputfilters-5.0.3/plone/outputfilters/transforms/html_to_plone_outputfilters_html.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone/outputfilters/transforms/plone_outputfilters_html_to_html.py` & `plone.outputfilters-5.0.3/plone/outputfilters/transforms/plone_outputfilters_html_to_html.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/plone.outputfilters.egg-info/PKG-INFO` & `plone.outputfilters-5.0.3/plone.outputfilters.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.outputfilters
-Version: 5.0.2
+Version: 5.0.3
 Summary: Transformations applied to HTML in Plone text fields as they are rendered
 Home-page: http://github.com/plone/plone.outputfilters
 Author: David Glick, Plone Foundation
 Author-email: davidglick@groundwire.org
 License: GPL
 Keywords: plone transform filter uid caption
 Classifier: Development Status :: 5 - Production/Stable
@@ -218,14 +218,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.3 (2023-06-16)
+------------------
+
+Bug fixes:
+
+
+- Return a 404 Not Found response if the resolveuid view is called with no uuid. @davisagli (#43)
+
+
 5.0.2 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.outputfilters-5.0.2/plone.outputfilters.egg-info/SOURCES.txt` & `plone.outputfilters-5.0.3/plone.outputfilters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/pyproject.toml` & `plone.outputfilters-5.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.2/setup.py` & `plone.outputfilters-5.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 import os
 
 
-version = "5.0.2"
+version = "5.0.3"
 
 
 def read(filename):
     with open(filename) as myfile:
         try:
             return myfile.read()
         except UnicodeDecodeError:
```

