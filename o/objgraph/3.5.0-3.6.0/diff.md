# Comparing `tmp/objgraph-3.5.0.tar.gz` & `tmp/objgraph-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/objgraph-3.5.0.tar", last modified: Sun Oct 11 11:16:05 2020, max compression
+gzip compressed data, was "objgraph-3.6.0.tar", last modified: Fri Jun 16 07:00:52 2023, max compression
```

## Comparing `objgraph-3.5.0.tar` & `objgraph-3.6.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2020-10-11 11:16:05.914251 objgraph-3.5.0/
--rw-rw-r--   0 mg        (1000) mg        (1000)       62 2020-10-08 16:24:49.000000 objgraph-3.5.0/.coveragerc
--rw-rw-r--   0 mg        (1000) mg        (1000)       19 2020-10-08 16:24:49.000000 objgraph-3.5.0/.gitattributes
--rw-rw-r--   0 mg        (1000) mg        (1000)      139 2020-10-08 16:24:49.000000 objgraph-3.5.0/.gitignore
--rw-rw-r--   0 mg        (1000) mg        (1000)      390 2020-10-08 16:41:24.000000 objgraph-3.5.0/.travis.yml
--rw-rw-r--   0 mg        (1000) mg        (1000)     9472 2020-10-11 11:07:03.000000 objgraph-3.5.0/CHANGES.rst
--rw-rw-r--   0 mg        (1000) mg        (1000)     5299 2020-10-08 17:54:11.000000 objgraph-3.5.0/HACKING.rst
--rw-rw-r--   0 mg        (1000) mg        (1000)     1072 2020-10-08 16:24:49.000000 objgraph-3.5.0/LICENSE
--rw-rw-r--   0 mg        (1000) mg        (1000)      408 2020-10-08 16:24:49.000000 objgraph-3.5.0/MANIFEST.in
--rw-rw-r--   0 mg        (1000) mg        (1000)     3352 2020-10-11 11:08:25.000000 objgraph-3.5.0/Makefile
--rw-rw-r--   0 mg        (1000) mg        (1000)    15101 2020-10-11 11:16:05.914251 objgraph-3.5.0/PKG-INFO
--rw-rw-r--   0 mg        (1000) mg        (1000)     2068 2020-10-08 16:24:49.000000 objgraph-3.5.0/README.rst
--rw-rw-r--   0 mg        (1000) mg        (1000)      913 2020-10-08 16:41:24.000000 objgraph-3.5.0/appveyor.yml
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2020-10-11 11:16:05.914251 objgraph-3.5.0/docs/
--rw-rw-r--   0 mg        (1000) mg        (1000)    16030 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/42.png
--rw-rw-r--   0 mg        (1000) mg        (1000)       28 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/CHANGES.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)       28 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/HACKING.txt
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2020-10-11 11:16:05.914251 objgraph-3.5.0/docs/_static/
--rw-rw-r--   0 mg        (1000) mg        (1000)      254 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/_static/mg.css
--rw-rw-r--   0 mg        (1000) mg        (1000)    64453 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/all-the-chars.dot
--rw-rw-r--   0 mg        (1000) mg        (1000)    66114 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/canary-chain.png
--rw-rw-r--   0 mg        (1000) mg        (1000)   109408 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/canary.png
--rw-rw-r--   0 mg        (1000) mg        (1000)    66210 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/chain.png
--rw-rw-r--   0 mg        (1000) mg        (1000)      890 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/chain.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)     9202 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/class-with-finalizers.png
--rw-rw-r--   0 mg        (1000) mg        (1000)     7349 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/conf.py
--rw-rw-r--   0 mg        (1000) mg        (1000)    20411 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/extra-info.png
--rw-rw-r--   0 mg        (1000) mg        (1000)      799 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/extra-info.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)    29549 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/finalizers.png
--rw-rw-r--   0 mg        (1000) mg        (1000)    15272 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/forward-chain.png
--rw-rw-r--   0 mg        (1000) mg        (1000)     1474 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/generator-sample.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)    55647 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/highlight.png
--rw-rw-r--   0 mg        (1000) mg        (1000)      623 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/highlighting.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)     5902 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/index.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)     1685 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/objgraph.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)      426 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/quoting.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)    22199 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/refcounts.png
--rw-rw-r--   0 mg        (1000) mg        (1000)     1385 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/references.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)   169056 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/roots.png
--rw-rw-r--   0 mg        (1000) mg        (1000)    37530 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/sample-backref-graph.png
--rw-rw-r--   0 mg        (1000) mg        (1000)    10906 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/sample-graph.png
--rw-rw-r--   0 mg        (1000) mg        (1000)    14085 2020-10-11 11:15:48.000000 objgraph-3.5.0/docs/too-many.png
--rw-rw-r--   0 mg        (1000) mg        (1000)     1248 2020-10-08 16:24:49.000000 objgraph-3.5.0/docs/uncollectable.txt
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2020-10-11 11:16:05.914251 objgraph-3.5.0/objgraph.egg-info/
--rw-rw-r--   0 mg        (1000) mg        (1000)    15101 2020-10-11 11:16:05.000000 objgraph-3.5.0/objgraph.egg-info/PKG-INFO
--rw-rw-r--   0 mg        (1000) mg        (1000)      942 2020-10-11 11:16:05.000000 objgraph-3.5.0/objgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)        1 2020-10-11 11:16:05.000000 objgraph-3.5.0/objgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)        9 2020-10-11 11:16:05.000000 objgraph-3.5.0/objgraph.egg-info/requires.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)        9 2020-10-11 11:16:05.000000 objgraph-3.5.0/objgraph.egg-info/top_level.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)        1 2020-10-08 16:42:49.000000 objgraph-3.5.0/objgraph.egg-info/zip-safe
--rwxrwxr-x   0 mg        (1000) mg        (1000)    43526 2020-10-11 11:07:15.000000 objgraph-3.5.0/objgraph.py
--rw-rw-r--   0 mg        (1000) mg        (1000)        9 2020-10-08 16:24:49.000000 objgraph-3.5.0/other-requirements.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)     5401 2020-10-11 10:54:04.000000 objgraph-3.5.0/release.mk
--rw-rw-r--   0 mg        (1000) mg        (1000)      277 2020-10-11 11:16:05.914251 objgraph-3.5.0/setup.cfg
--rwxrwxr-x   0 mg        (1000) mg        (1000)     2622 2020-10-08 16:41:24.000000 objgraph-3.5.0/setup.py
--rwxrwxr-x   0 mg        (1000) mg        (1000)    24371 2020-10-08 16:24:49.000000 objgraph-3.5.0/tests.py
--rw-rw-r--   0 mg        (1000) mg        (1000)      604 2020-10-11 11:08:02.000000 objgraph-3.5.0/tox.ini
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2023-06-16 07:00:52.081587 objgraph-3.6.0/
+-rw-rw-r--   0 mg        (1000) mg        (1000)      163 2023-06-16 06:43:01.000000 objgraph-3.6.0/.coveragerc
+-rw-r--r--   0 mg        (1000) mg        (1000)       19 2019-06-13 12:23:07.000000 objgraph-3.6.0/.gitattributes
+-rw-r--r--   0 mg        (1000) mg        (1000)      139 2019-06-13 12:23:07.000000 objgraph-3.6.0/.gitignore
+-rw-rw-r--   0 mg        (1000) mg        (1000)      577 2023-06-07 12:28:26.000000 objgraph-3.6.0/.readthedocs.yaml
+-rw-rw-r--   0 mg        (1000) mg        (1000)     9555 2023-06-16 06:59:13.000000 objgraph-3.6.0/CHANGES.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)     5299 2020-10-24 10:07:07.000000 objgraph-3.6.0/HACKING.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     1072 2019-06-13 12:23:07.000000 objgraph-3.6.0/LICENSE
+-rw-r--r--   0 mg        (1000) mg        (1000)      450 2023-06-07 13:29:01.000000 objgraph-3.6.0/MANIFEST.in
+-rw-rw-r--   0 mg        (1000) mg        (1000)     3352 2023-06-16 06:58:24.000000 objgraph-3.6.0/Makefile
+-rw-rw-r--   0 mg        (1000) mg        (1000)    12200 2023-06-16 07:00:52.081587 objgraph-3.6.0/PKG-INFO
+-rw-rw-r--   0 mg        (1000) mg        (1000)     2093 2020-12-01 07:49:21.000000 objgraph-3.6.0/README.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)      905 2023-06-16 06:43:01.000000 objgraph-3.6.0/appveyor.yml
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2023-06-16 07:00:52.081587 objgraph-3.6.0/docs/
+-rw-rw-r--   0 mg        (1000) mg        (1000)    16557 2023-06-16 07:00:38.000000 objgraph-3.6.0/docs/42.png
+-rw-r--r--   0 mg        (1000) mg        (1000)       28 2019-06-13 12:23:07.000000 objgraph-3.6.0/docs/CHANGES.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)       28 2019-06-13 12:23:07.000000 objgraph-3.6.0/docs/HACKING.txt
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2023-06-16 07:00:52.081587 objgraph-3.6.0/docs/_static/
+-rw-r--r--   0 mg        (1000) mg        (1000)      254 2019-06-13 12:23:07.000000 objgraph-3.6.0/docs/_static/mg.css
+-rw-rw-r--   0 mg        (1000) mg        (1000)    36391 2023-06-16 07:00:43.000000 objgraph-3.6.0/docs/all-the-chars.dot
+-rw-rw-r--   0 mg        (1000) mg        (1000)    47552 2023-06-16 07:00:38.000000 objgraph-3.6.0/docs/canary-chain.png
+-rw-rw-r--   0 mg        (1000) mg        (1000)   177565 2023-06-16 07:00:38.000000 objgraph-3.6.0/docs/canary.png
+-rw-rw-r--   0 mg        (1000) mg        (1000)    66682 2023-06-16 07:00:38.000000 objgraph-3.6.0/docs/chain.png
+-rw-r--r--   0 mg        (1000) mg        (1000)      890 2019-06-13 12:23:07.000000 objgraph-3.6.0/docs/chain.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     9202 2019-06-13 12:23:07.000000 objgraph-3.6.0/docs/class-with-finalizers.png
+-rw-rw-r--   0 mg        (1000) mg        (1000)     7770 2023-06-16 06:53:38.000000 objgraph-3.6.0/docs/conf.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)    19504 2023-06-16 07:00:38.000000 objgraph-3.6.0/docs/extra-info.png
+-rw-r--r--   0 mg        (1000) mg        (1000)      799 2019-06-13 12:23:07.000000 objgraph-3.6.0/docs/extra-info.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)    29549 2019-06-13 12:23:07.000000 objgraph-3.6.0/docs/finalizers.png
+-rw-rw-r--   0 mg        (1000) mg        (1000)    16200 2023-06-16 07:00:38.000000 objgraph-3.6.0/docs/forward-chain.png
+-rw-rw-r--   0 mg        (1000) mg        (1000)     1497 2022-11-28 08:57:09.000000 objgraph-3.6.0/docs/generator-sample.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)    34762 2023-06-16 07:00:38.000000 objgraph-3.6.0/docs/highlight.png
+-rw-rw-r--   0 mg        (1000) mg        (1000)      646 2022-11-28 08:57:09.000000 objgraph-3.6.0/docs/highlighting.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)     5916 2023-06-16 06:57:58.000000 objgraph-3.6.0/docs/index.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     1685 2019-06-13 12:23:07.000000 objgraph-3.6.0/docs/objgraph.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)      426 2019-06-13 12:23:07.000000 objgraph-3.6.0/docs/quoting.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)    40106 2023-06-16 07:00:38.000000 objgraph-3.6.0/docs/refcounts.png
+-rw-r--r--   0 mg        (1000) mg        (1000)     1385 2019-06-13 12:23:07.000000 objgraph-3.6.0/docs/references.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)   253483 2023-06-16 07:00:38.000000 objgraph-3.6.0/docs/roots.png
+-rw-rw-r--   0 mg        (1000) mg        (1000)    47419 2023-06-16 07:00:38.000000 objgraph-3.6.0/docs/sample-backref-graph.png
+-rw-rw-r--   0 mg        (1000) mg        (1000)    11194 2023-06-16 07:00:38.000000 objgraph-3.6.0/docs/sample-graph.png
+-rw-rw-r--   0 mg        (1000) mg        (1000)    14343 2023-06-16 07:00:38.000000 objgraph-3.6.0/docs/too-many.png
+-rw-r--r--   0 mg        (1000) mg        (1000)     1248 2019-06-13 12:23:07.000000 objgraph-3.6.0/docs/uncollectable.txt
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2023-06-16 07:00:52.081587 objgraph-3.6.0/objgraph.egg-info/
+-rw-r--r--   0 mg        (1000) mg        (1000)    12200 2023-06-16 07:00:52.000000 objgraph-3.6.0/objgraph.egg-info/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)      948 2023-06-16 07:00:52.000000 objgraph-3.6.0/objgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-06-16 07:00:52.000000 objgraph-3.6.0/objgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)       28 2023-06-16 07:00:52.000000 objgraph-3.6.0/objgraph.egg-info/requires.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        9 2023-06-16 07:00:52.000000 objgraph-3.6.0/objgraph.egg-info/top_level.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2019-06-13 13:10:01.000000 objgraph-3.6.0/objgraph.egg-info/zip-safe
+-rwxrwxr-x   0 mg        (1000) mg        (1000)    42871 2023-06-16 06:59:13.000000 objgraph-3.6.0/objgraph.py
+-rw-r--r--   0 mg        (1000) mg        (1000)        9 2019-06-13 12:23:07.000000 objgraph-3.6.0/other-requirements.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)     5599 2021-04-19 14:36:29.000000 objgraph-3.6.0/release.mk
+-rw-r--r--   0 mg        (1000) mg        (1000)      278 2023-06-16 07:00:52.081587 objgraph-3.6.0/setup.cfg
+-rwxrwxr-x   0 mg        (1000) mg        (1000)     2837 2023-06-16 06:43:01.000000 objgraph-3.6.0/setup.py
+-rwxrwxr-x   0 mg        (1000) mg        (1000)    23229 2023-06-16 06:43:01.000000 objgraph-3.6.0/tests.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)      974 2023-06-16 06:58:20.000000 objgraph-3.6.0/tox.ini
```

### Comparing `objgraph-3.5.0/CHANGES.rst` & `objgraph-3.6.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 Changes
 =======
 
 .. currentmodule:: objgraph
 
+3.6.0 (2023-06-16)
+------------------
+
+- Add support for Python 3.9, 3.10, and 3.11.
+
+- Drop support for Python 2.7 and 3.6.
+
+
 3.5.0 (2020-10-11)
 ------------------
 
 - Do not require ``mock`` for the test suite on Python 3; use unittest.mock
   instead.
 
 - 100% test coverage for each version of Python rather than combined, using
@@ -123,18 +131,18 @@
 
 2.0.0 (2015-04-18)
 ------------------
 
 - :func:`show_refs` and :func:`show_backrefs` now accept a file-like object
   (via the new ``output`` argument) as an alternative to a filename.
 
-- Made internal helper methods private. This includes :func:`find_chain`,
-  :func:`show_graph`, :func:`obj_node_id`, :func:`obj_label`, :func:`quote`,
-  :func:`long_typename`, :func:`safe_repr`, :func:`short_repr`,
-  :func:`gradient`, :func:`edge_label`, and :func:`_program_in_path`.
+- Made internal helper methods private. This includes ``find_chain``,
+  ``show_graph``, ``obj_node_id``, ``obj_label``, ``quote``,
+  ``long_typename``, ``safe_repr``, ``short_repr``,
+  ``gradient``, ``edge_label``, and ``_program_in_path``.
 
 - Correctly determine the name of old-style classes in :func:`count`,
   :func:`by_type`, and graph drawing functions.
 
   Fixes `issue 16 <https://github.com/mgedmin/objgraph/pull/16>`_.  Contributed
   by Mike Lambert.
```

### Comparing `objgraph-3.5.0/HACKING.rst` & `objgraph-3.6.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `objgraph-3.5.0/LICENSE` & `objgraph-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `objgraph-3.5.0/Makefile` & `objgraph-3.6.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 PYTHON = python3
 
 FILE_WITH_VERSION = objgraph.py
 FILE_WITH_CHANGELOG = CHANGES.rst
 
 VCS_DIFF_IMAGES = git diff docs/*.png
 
-SPHINXOPTS      =
+SPHINXOPTS      = -Wn
 SPHINXBUILD     = sphinx-build
 SPHINXBUILDDIR  = docs/_build
 ALLSPHINXOPTS   = -d $(SPHINXBUILDDIR)/doctrees $(SPHINXOPTS) docs/
 
 
 .PHONY: all
 all:
@@ -38,19 +38,19 @@
 # 'make check' is defined in release.mk and here's how you can override it
 define check_recipe =
 	@$(MAKE) coverage
 endef
 
 .PHONY: coverage
 coverage:                       ##: measure test coverage
-	tox -e coverage2,coverage3
+	tox -e coverage
 
 .PHONY: flake8
 flake8:                         ##: check for style problems
-	flake8
+	tox -e flake8
 
 # Make sure $(VCS_DIFF_IMAGES) can work
 .PHONY: config-imgdiff
 config-imgdiff:
 	@test -z "`git config diff.imgdiff.command`" && git config diff.imgdiff.command 'f() { imgdiff --eog -H $$1 $$2; }; f' || true
 
 .PHONY: imgdiff
```

### Comparing `objgraph-3.5.0/README.rst` & `objgraph-3.6.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Python Object Graphs
 ====================
 
-.. image:: https://travis-ci.org/mgedmin/objgraph.svg?branch=master
-   :target: https://travis-ci.org/mgedmin/objgraph
+.. image:: https://github.com/mgedmin/objgraph/workflows/build/badge.svg?branch=master
+    :target: https://github.com/mgedmin/objgraph/actions
    :alt: Build Status
 
 .. image:: https://ci.appveyor.com/api/projects/status/github/mgedmin/objgraph?branch=master&svg=true
    :target: https://ci.appveyor.com/project/mgedmin/objgraph
    :alt: Build Status (Windows)
 
 .. image:: https://coveralls.io/repos/mgedmin/objgraph/badge.svg?branch=master
```

### Comparing `objgraph-3.5.0/appveyor.yml` & `objgraph-3.6.0/appveyor.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 version: build-{build}-{branch}
 
 environment:
   matrix:
     # https://www.appveyor.com/docs/installed-software#python lists available
     # versions
-    - PYTHON: "C:\\Python27"
-    - PYTHON: "C:\\Python36"
     - PYTHON: "C:\\Python37"
     - PYTHON: "C:\\Python38"
+    - PYTHON: "C:\\Python39"
+    - PYTHON: "C:\\Python310"
+    - PYTHON: "C:\\Python311"
 
 init:
   - "echo %PYTHON%"
 
 install:
   - ps: |
       if (-not (Test-Path $env:PYTHON)) {
@@ -19,15 +20,14 @@
         .\install_python.ps1
       }
   - ps: if (-not (Test-Path $env:PYTHON)) { throw "No $env:PYTHON" }
   - "set PATH=%PYTHON%;%PYTHON%\\Scripts;%PATH%"
   - python --version
   - pip install -U virtualenv  # upgrade pip in tox's virtualenvs
   - pip install tox
-  - choco install graphviz
-  - "set PATH=c:\\Program Files (x86)\\graphviz2.38\\bin;%PATH%"
+  - choco install graphviz --version=2.38.0.20190211
   - dot -V
 
 build: off
 
 test_script:
   - tox -e py
```

### Comparing `objgraph-3.5.0/docs/chain.txt` & `objgraph-3.6.0/docs/chain.txt`

 * *Files identical despite different names*

### Comparing `objgraph-3.5.0/docs/class-with-finalizers.png` & `objgraph-3.6.0/docs/class-with-finalizers.png`

 * *Files identical despite different names*

### Comparing `objgraph-3.5.0/docs/conf.py` & `objgraph-3.6.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,38 +7,61 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import sys, os
+import io
+import os
+import re
+import sys
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.append(os.path.abspath('..'))
 
+
 def relative(filename):
     here = os.path.dirname('__file__')
     return os.path.join(here, filename)
 
+
+def read(filename):
+    with io.open(relative(filename), encoding='UTF-8') as f:
+        return f.read()
+
+
 def get_version():
-    d = {}
-    exec open(relative('../objgraph.py')).read() in d
-    return d['__version__']
+    r = re.compile('''^__version__ = ["'](.+)["']$''')
+    for line in read('../objgraph.py').splitlines():
+        m = r.match(line)
+        if m:
+            return m.group(1)
+    raise AssertionError('Could not determine version number from objgraph.py')
+
 
 def get_short_version():
     return '.'.join(get_version().split('.')[:2])
 
+
 # -- General configuration -----------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.doctest']
+extensions = [
+    'sphinx.ext.autodoc',
+    'sphinx.ext.doctest',
+    'sphinx.ext.intersphinx',
+]
+
+intersphinx_mapping = {
+    'python': ('https://docs.python.org/3', None),
+}
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.txt'
```

### Comparing `objgraph-3.5.0/docs/extra-info.txt` & `objgraph-3.6.0/docs/extra-info.txt`

 * *Files identical despite different names*

### Comparing `objgraph-3.5.0/docs/finalizers.png` & `objgraph-3.6.0/docs/finalizers.png`

 * *Files identical despite different names*

### Comparing `objgraph-3.5.0/docs/generator-sample.txt` & `objgraph-3.6.0/docs/generator-sample.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
    :scale: 50%
 
 Or we can examine just one of the reference chains leading straight to a module.
 
     >>> objgraph.show_chain(
     ...     objgraph.find_backref_chain(objgraph.by_type('Canary')[0],
     ...                                 objgraph.is_proper_module),
-    ...     filename='canary-chain.png')
+    ...     filename='canary-chain.png') # doctest: +NODES_VARY
     Graph written to ....dot (11 nodes)
     Image generated as canary-chain.png
 
 .. figure:: canary-chain.png
    :alt: [chain of objects from a module to the canary]
    :scale: 50%
```

### Comparing `objgraph-3.5.0/docs/highlighting.txt` & `objgraph-3.6.0/docs/highlighting.txt`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,14 @@
     >>> d = Node(c)
     >>> a.neighbours.append(d)
 
     >>> import objgraph
     >>> objgraph.show_backrefs(a, max_depth=15,
     ...     extra_ignore=[id(locals())],
     ...     highlight=lambda x: isinstance(x, Node),
-    ...     filename='highlight.png')
+    ...     filename='highlight.png') # doctest: +NODES_VARY
     Graph written to ....dot (12 nodes)
     Image generated as highlight.png
 
 .. figure:: highlight.png
    :scale: 50%
```

### Comparing `objgraph-3.5.0/docs/index.txt` & `objgraph-3.6.0/docs/index.txt`

 * *Files 2% similar despite different names*

```diff
@@ -93,39 +93,39 @@
 and see what changes after we call it
 
     >>> computate_something()
     >>> objgraph.show_growth() # doctest: +RANDOM_OUTPUT
     MyBigFatObject        2        +2
     dict                797        +1
 
-It's easy to see :class:`MyBigFatObject` instances that appeared and were
+It's easy to see ``MyBigFatObject`` instances that appeared and were
 not freed.  I can pick one of them at random and trace the reference chain
 back to one of the garbage collector's roots.
 
 For simplicity's sake let's assume all of the roots are modules.  ``objgraph``
 provides a function, :func:`~objgraph.is_proper_module`, to check this. If
 you've any examples where that isn't true, I'd love to hear about them
 (although see :ref:`leaking-objects`).
 
     >>> import random
     >>> objgraph.show_chain(
     ...     objgraph.find_backref_chain(
     ...         random.choice(objgraph.by_type('MyBigFatObject')),
     ...         objgraph.is_proper_module),
-    ...     filename='chain.png')
+    ...     filename='chain.png') # doctest: +NODES_VARY
     Graph written to ...dot (13 nodes)
     Image generated as chain.png
 
 .. figure:: chain.png
    :alt: [chain of references from a module to a MyBigFatObject instance]
    :scale: 50%
 
 It is perhaps surprising to find :mod:`linecache` at the end of that chain
 (apparently :mod:`doctest` monkey-patches it), but the important things --
-:func:`computate_something` and its cache dictionary -- are in there.
+``computate_something`` and its cache dictionary -- are in there.
 
 There are other tools, perhaps better suited for memory leak hunting:
 `heapy <https://pypi.python.org/pypi/guppy>`_,
 `Dozer <https://pypi.python.org/pypi/Dozer>`_.
 
 
 .. _leaking-objects:
```

### Comparing `objgraph-3.5.0/docs/objgraph.txt` & `objgraph-3.6.0/docs/objgraph.txt`

 * *Files identical despite different names*

### Comparing `objgraph-3.5.0/docs/references.txt` & `objgraph-3.6.0/docs/references.txt`

 * *Files identical despite different names*

### Comparing `objgraph-3.5.0/docs/uncollectable.txt` & `objgraph-3.6.0/docs/uncollectable.txt`

 * *Files identical despite different names*

### Comparing `objgraph-3.5.0/objgraph.egg-info/SOURCES.txt` & `objgraph-3.6.0/objgraph.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .coveragerc
 .gitattributes
 .gitignore
-.travis.yml
+.readthedocs.yaml
 CHANGES.rst
 HACKING.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 appveyor.yml
```

### Comparing `objgraph-3.5.0/objgraph.py` & `objgraph-3.6.0/objgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Tools for drawing Python object reference graphs with graphviz.
 
 You can find documentation online at https://mg.pov.lt/objgraph/
 
-Copyright (c) 2008-2017 Marius Gedminas <marius@pov.lt> and contributors
+Copyright (c) 2008-2023 Marius Gedminas <marius@pov.lt> and contributors
 
 Released under the MIT licence.
 """
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
@@ -21,60 +21,34 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-from __future__ import print_function
-
 import codecs
 import collections
 import gc
-import re
 import inspect
-import types
+import itertools
 import operator
 import os
+import re
 import subprocess
-import tempfile
 import sys
-import itertools
-
-try:
-    # Python 2.x compatibility
-    from StringIO import StringIO
-except ImportError:  # pragma: PY3
-    from io import StringIO
-
-try:
-    from types import InstanceType
-except ImportError:  # pragma: PY3
-    # Python 3.x compatibility
-    InstanceType = None
-
+import tempfile
+import types
+from io import StringIO
 
 __author__ = "Marius Gedminas (marius@gedmin.as)"
-__copyright__ = "Copyright (c) 2008-2017 Marius Gedminas and contributors"
+__copyright__ = "Copyright (c) 2008-2023 Marius Gedminas and contributors"
 __license__ = "MIT"
-__version__ = '3.5.0'
-__date__ = '2020-10-11'
-
+__version__ = '3.6.0'
+__date__ = '2023-06-16'
 
-try:
-    basestring
-except NameError:  # pragma: PY3
-    # Python 3.x compatibility
-    basestring = str
-
-try:
-    iteritems = dict.iteritems
-except AttributeError:  # pragma: PY3
-    # Python 3.x compatibility
-    iteritems = dict.items
 
 IS_INTERACTIVE = False
 try:  # pragma: nocover
     import graphviz
     if 'TerminalInteractiveShell' not in get_ipython().__class__.__name__:
         # So far I know two shells where it's inappropriate to use inline
         # graphics, because they're text only:
@@ -302,15 +276,15 @@
 
     .. versionadded:: 3.3.0
 
     """
     gc.collect()
     stats = typestats(shortnames=shortnames, filter=filter)
     deltas = {}
-    for name, count in iteritems(stats):
+    for name, count in stats.items():
         old_count = peak_stats.get(name, 0)
         if count > old_count:
             deltas[name] = count - old_count
             peak_stats[name] = count
     deltas = sorted(deltas.items(), key=operator.itemgetter(1),
                     reverse=True)
     if limit:
@@ -1099,15 +1073,15 @@
     return ('o%d' % id(obj)).replace('-', '_')
 
 
 def _obj_attrs(obj, extra_node_attrs):
     if extra_node_attrs is not None:
         attrs = extra_node_attrs(obj)
         return ", " + ", ".join('%s="%s"' % (name, _quote(value))
-                                for name, value in sorted(iteritems(attrs))
+                                for name, value in sorted(attrs.items())
                                 if value is not None)
     else:
         return ""
 
 
 def _obj_label(obj, extra_info=None, refcounts=False, shortnames=True):
     if shortnames:
@@ -1132,16 +1106,14 @@
              .replace("\"", "\\\"")
              .replace("\n", "\\n")
              .replace("\0", "\\\\0"))
 
 
 def _get_obj_type(obj):
     objtype = type(obj)
-    if type(obj) == InstanceType:  # pragma: PY2 -- no old-style classes on PY3
-        objtype = obj.__class__
     return objtype
 
 
 def _short_typename(obj):
     return _get_obj_type(obj).__name__
 
 
@@ -1164,15 +1136,15 @@
 
 def _name_or_repr(value):
     try:
         result = value.__name__
     except AttributeError:
         result = repr(value)[:40]
 
-    if _isinstance(result, basestring):
+    if _isinstance(result, str):
         return result
     else:
         return repr(value)[:40]
 
 
 def _short_repr(obj):
     if _isinstance(obj, (type, types.ModuleType, types.BuiltinMethodType,
@@ -1230,17 +1202,17 @@
             if target is source.im_func:
                 return ' [label="im_func",weight=10]'
     if _isinstance(source, types.FunctionType):
         for k in dir(source):
             if target is getattr(source, k):
                 return ' [label="%s",weight=10]' % _quote(k)
     if _isinstance(source, dict):
-        for k, v in iteritems(source):
+        for k, v in source.items():
             if v is target:
-                if _isinstance(k, basestring) and _is_identifier(k):
+                if _isinstance(k, str) and _is_identifier(k):
                     return ' [label="%s",weight=2]' % _quote(k)
                 else:
                     if shortnames:
                         tn = _short_typename(k)
                     else:
                         tn = _long_typename(k)
                     return ' [label="%s"]' % _quote(tn + "\n" + _safe_repr(k))
```

### Comparing `objgraph-3.5.0/release.mk` & `objgraph-3.6.0/release.mk`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# release.mk version 2.0 (2020-10-11)
+# release.mk version 2.1 (2021-04-19)
 #
 # Helpful Makefile rules for releasing Python packages.
 # https://github.com/mgedmin/python-project-skel
 
 # You might want to change these
 FILE_WITH_VERSION ?= setup.py
 FILE_WITH_CHANGELOG ?= CHANGES.rst
@@ -138,22 +138,28 @@
 .PHONY: release
 release: releasechecklist do-release    ##: prepare a new PyPI release
 
 .PHONY: do-release
 do-release:
 	$(release_recipe)
 
-ifndef release_recipe
-define release_recipe =
+define default_release_recipe_publish_and_tag =
 	# I'm chicken so I won't actually do these things yet
 	@echo "Please run"
 	@echo
 	@echo "  $(PYPI_PUBLISH)"
 	@echo "  $(VCS_TAG)"
 	@echo
+endef
+define default_release_recipe_increment_and_push =
 	@echo "Please increment the version number in $(FILE_WITH_VERSION)"
 	@echo "and add a new empty entry at the top of the changelog in $(FILE_WITH_CHANGELOG), then"
 	@echo
 	@echo '  $(VCS_COMMIT_AND_PUSH)'
 	@echo
 endef
+ifndef release_recipe
+define release_recipe =
+$(default_release_recipe_publish_and_tag)
+$(default_release_recipe_increment_and_push)
+endef
 endif
```

### Comparing `objgraph-3.5.0/setup.py` & `objgraph-3.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,29 +60,37 @@
 
 setup(
     name='objgraph',
     version=get_version(),
     author='Marius Gedminas',
     author_email='marius@gedmin.as',
     url='https://mg.pov.lt/objgraph/',
+    project_urls={
+        'Source': 'https://github.com/mgedmin/objgraph',
+    },
     license='MIT',
     description='Draws Python object reference graphs with graphviz',
     long_description=get_description(),
+    long_description_content_type='text/x-rst',
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     keywords='object graph visualization graphviz garbage collection',
     py_modules=['objgraph'],
-    install_requires=[
-        'graphviz',  # just for ipython support currently
-    ],
-    tests_require=['mock;python_version=="2.7"'],
+    python_requires=">=3.7",
+    extras_require={
+        'ipython': [
+            'graphviz',  # just for ipython support currently
+        ],
+        'test': [],
+    },
     test_suite='tests.test_suite',
     zip_safe=True,
 )
```

### Comparing `objgraph-3.5.0/tests.py` & `objgraph-3.6.0/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,87 +7,40 @@
 import shutil
 import string
 import sys
 import tempfile
 import textwrap
 import types
 import unittest
+from io import StringIO
+from unittest import mock, skipIf
 
 # setuptools imports `imp`, which triggers a DeprecationWarning starting with
 # Python 3.4 in the middle of my pristine test suite.  But if I do the import
 # upfront, there's no warning.  I cannot explain this, I'm just happy there's
 # no warning.
 import setuptools  # noqa
 
-try:
-    from unittest import mock
-except ImportError:
-    import mock
-
 import objgraph
 
-try:
-    from cStringIO import StringIO
-except ImportError:
-    from io import StringIO
-
-
-try:
-    from unittest import skipIf
-except ImportError:
-    def skipIf(condition, reason):
-        def wrapper(fn):
-            if condition:
-                def empty_test(case):
-                    pass
-                empty_test.__doc__ = '%s skipped because %s' % (
-                    fn.__name__, reason)
-                return empty_test
-            return fn
-        return wrapper
-
 
 def format(text, **kwargs):
     template = string.Template(text)
     return template.substitute(kwargs)
 
 
-class CompatibilityMixin(object):
-
-    # Python 2.7 .. 3.1 has assertRegexpMatches but not assertRegex
-    # Python <= 2.6 has neither
-    # Python >= 3.2 has both and emits deprecation warnings if you use
-    # assertRegexpMatches.
-
-    if not hasattr(unittest.TestCase, 'assertRegex'):
-        if hasattr(unittest.TestCase, 'assertRegexpMatches'):
-            # This is needed for Python 3.1: let's reuse the existing
-            # function because our replacement doesn't work on Python 3
-            assertRegex = unittest.TestCase.assertRegexpMatches
-        else:
-            def assertRegex(self, text, expected_regexp, msg=None):
-                if isinstance(expected_regexp, basestring):  # noqa
-                    expected_regexp = re.compile(expected_regexp)
-                if not expected_regexp.search(text):
-                    msg = msg or "Regexp didn't match"
-                    msg = '%s: %r not found in %r' % (msg,
-                                                      expected_regexp.pattern,
-                                                      text)
-                    raise self.failureException(msg)
-
-
 class GarbageCollectedMixin(object):
     """A mixin for test cases that garbage collects before running."""
 
     def setUp(self):
-        super(GarbageCollectedMixin, self).setUp()
+        super().setUp()
         gc.collect()
 
     def tearDown(self):
-        super(GarbageCollectedMixin, self).tearDown()
+        super().tearDown()
         gc.enable()
 
 
 class CaptureMixin(object):
     """A mixing that captures sys.stdout"""
 
     def setUp(self):
@@ -374,22 +327,21 @@
 
 
 def doctest_get_new_ids_prints():
     """Test for get_new_ids()
 
         >>> _ = objgraph.get_new_ids(limit=0)
         >>> _ = objgraph.get_new_ids(limit=0)
-        >>> a = [0, 1, 2]  # noqa
-        >>> b = [3, 4, 5]  # noqa
+        >>> a = [[] for n in range(10)]  # noqa
         >>> _ = objgraph.get_new_ids(limit=1)
         ... # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
         ========================================================
         Type      Old_ids  Current_ids      New_ids Count_Deltas
         ========================================================
-        list          ...          ...          ...           +2
+        list          ...          ...          ...          +11
         ========================================================
 
     """
 
 
 class ByTypeTest(GarbageCollectedMixin, unittest.TestCase):
     """Tests for the by_test function."""
@@ -418,15 +370,14 @@
         a = [0, 1, 2]
         new_ids = objgraph.get_new_ids(limit=0)
         new_lists = objgraph.at_addrs(new_ids['list'])
         self.assertIn(a, new_lists)
 
 
 class StringRepresentationTest(GarbageCollectedMixin,
-                               CompatibilityMixin,
                                unittest.TestCase):
     """Tests for the string representation of objects and edges."""
 
     def test_obj_label_long_type_name(self):
         x = type('MyClass', (), {'__module__': 'mymodule'})()
 
         self.assertRegex(
@@ -500,24 +451,40 @@
     def test_short_repr_unbound_method(self):
         class MyClass(object):
             def a_method(self):
                 pass
 
         self.assertEqual('a_method', objgraph._short_repr(MyClass.a_method))
 
+    def test_short_repr_frame(self):
+        frame = sys._getframe()
+        # we're calling _short_repr() 6 lines down from here
+        lineno = frame.f_lineno + 6
+        # Python >= 3.9 uses absolute filenames
+        expected = {
+            'tests.py:%d' % lineno,
+            '%s:%d' % (os.path.abspath('tests.py'), lineno),
+        }
+        self.assertIn(objgraph._short_repr(frame), expected)
+
     def test_gradient_empty(self):
         self.assertEqual((0.1, 0.2, 0.3),
                          objgraph._gradient((0.1, 0.2, 0.3),
                                             (0.2, 0.3, 0.4), 0, 0))
 
     def test_edge_label_frame_locals(self):
         frame = sys._getframe()
         self.assertEqual(' [label="f_locals",weight=10]',
                          objgraph._edge_label(frame, frame.f_locals))
 
+    def test_edge_label_frame_globals(self):
+        frame = sys._getframe()
+        self.assertEqual(' [label="f_globals",weight=10]',
+                         objgraph._edge_label(frame, frame.f_globals))
+
     @skipIf(sys.version_info[0] > 2, "Python 3 has no unbound methods")
     def test_edge_label_unbound_method(self):
         class MyClass(object):
             def a_method(self):
                 pass
         self.assertEqual(' [label="__func__",weight=10]',
                          objgraph._edge_label(MyClass.a_method,
```

