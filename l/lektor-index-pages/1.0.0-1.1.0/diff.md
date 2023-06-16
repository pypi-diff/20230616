# Comparing `tmp/lektor-index-pages-1.0.0.tar.gz` & `tmp/lektor_index_pages-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektor-index-pages-1.0.0.tar", last modified: Fri Jan 28 19:05:52 2022, max compression
+gzip compressed data, was "lektor_index_pages-1.1.0.tar", last modified: Fri Jun 16 16:34:31 2023, max compression
```

## Comparing `lektor-index-pages-1.0.0.tar` & `lektor_index_pages-1.1.0.tar`

### file list

```diff
@@ -1,83 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.039795 lektor-index-pages-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.031795 lektor-index-pages-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.035795 lektor-index-pages-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4845 2022-01-28 19:05:52.039795 lektor-index-pages-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2054 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.035795 lektor-index-pages-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/docs/CHANGES.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.035795 lektor-index-pages-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)     2654 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.035795 lektor-index-pages-1.0.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (121)     4505 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/docs/reference/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/docs/reference/templateapi.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/docs/reference/virtualsources.rst
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.035795 lektor-index-pages-1.0.0/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (121)     3309 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/docs/usage/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/docs/usage/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/example.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.035795 lektor-index-pages-1.0.0/lektor_index_pages/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/lektor_index_pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/lektor_index_pages/buildprog.py
--rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/lektor_index_pages/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     9693 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/lektor_index_pages/indexmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4229 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/lektor_index_pages/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)    13011 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/lektor_index_pages/sourceobj.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.035795 lektor-index-pages-1.0.0/lektor_index_pages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4845 2022-01-28 19:05:52.000000 lektor-index-pages-1.0.0/lektor_index_pages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-01-28 19:05:52.000000 lektor-index-pages-1.0.0/lektor_index_pages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-28 19:05:52.000000 lektor-index-pages-1.0.0/lektor_index_pages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-01-28 19:05:52.000000 lektor-index-pages-1.0.0/lektor_index_pages.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-01-28 19:05:52.000000 lektor-index-pages-1.0.0/lektor_index_pages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-01-28 19:05:52.000000 lektor-index-pages-1.0.0/lektor_index_pages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-01-28 19:05:52.039795 lektor-index-pages-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.035795 lektor-index-pages-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.035795 lektor-index-pages-1.0.0/tests/demo-site/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/Test Project.lektorproject
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.031795 lektor-index-pages-1.0.0/tests/demo-site/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.035795 lektor-index-pages-1.0.0/tests/demo-site/assets/static/
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/assets/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.035795 lektor-index-pages-1.0.0/tests/demo-site/configs/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/configs/index-pages.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.035795 lektor-index-pages-1.0.0/tests/demo-site/content/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.039795 lektor-index-pages-1.0.0/tests/demo-site/content/blog/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/content/blog/contents.lr
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.039795 lektor-index-pages-1.0.0/tests/demo-site/content/blog/first-post/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/content/blog/first-post/contents.lr
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.039795 lektor-index-pages-1.0.0/tests/demo-site/content/blog/second-post/
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/content/blog/second-post/contents.lr
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/content/contents.lr
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.039795 lektor-index-pages-1.0.0/tests/demo-site/models/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/models/blog-post.ini
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/models/blog.ini
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/models/page.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.039795 lektor-index-pages-1.0.0/tests/demo-site/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/templates/blog-post.html
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/templates/blog.html
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 19:05:52.039795 lektor-index-pages-1.0.0/tests/demo-site/templates/macros/
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/templates/macros/blog-index.html
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/templates/macros/blog.html
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/templates/macros/pagination.html
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/templates/month-index.html
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/demo-site/templates/year-index.html
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/test_buildprog.py
--rw-r--r--   0 runner    (1001) docker     (121)     2277 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (121)    12715 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/test_indexmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5055 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)    11595 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tests/test_sourceobj.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-01-28 19:05:40.000000 lektor-index-pages-1.0.0/tox.ini
+-rw-r--r--   0        0        0     2277 2023-06-16 16:34:12.566218 lektor_index_pages-1.1.0/CHANGES.md
+-rw-r--r--   0        0        0     1062 2023-06-16 16:34:12.566218 lektor_index_pages-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2186 2023-06-16 16:34:12.566218 lektor_index_pages-1.1.0/README.md
+-rw-r--r--   0        0        0       82 2023-06-16 16:34:12.566218 lektor_index_pages-1.1.0/lektor_index_pages/__init__.py
+-rw-r--r--   0        0        0     2137 2023-06-16 16:34:12.566218 lektor_index_pages-1.1.0/lektor_index_pages/buildprog.py
+-rw-r--r--   0        0        0     3411 2023-06-16 16:34:12.566218 lektor_index_pages-1.1.0/lektor_index_pages/config.py
+-rw-r--r--   0        0        0    11223 2023-06-16 16:34:12.566218 lektor_index_pages-1.1.0/lektor_index_pages/indexmodel.py
+-rw-r--r--   0        0        0     5539 2023-06-16 16:34:12.566218 lektor_index_pages-1.1.0/lektor_index_pages/plugin.py
+-rw-r--r--   0        0        0    15444 2023-06-16 16:34:12.566218 lektor_index_pages-1.1.0/lektor_index_pages/sourceobj.py
+-rw-r--r--   0        0        0      753 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/pdm_build.py
+-rw-r--r--   0        0        0     7139 2023-06-16 16:34:31.222716 lektor_index_pages-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3408 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      154 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/Test Project.lektorproject
+-rw-r--r--   0        0        0      538 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/assets/static/style.css
+-rw-r--r--   0        0        0      445 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/configs/index-pages.ini
+-rw-r--r--   0        0        0       29 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/content/blog/contents.lr
+-rw-r--r--   0        0        0      154 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/content/blog/first-post/contents.lr
+-rw-r--r--   0        0        0      152 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/content/blog/second-post/contents.lr
+-rw-r--r--   0        0        0      172 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/content/contents.lr
+-rw-r--r--   0        0        0      290 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/models/blog-post.ini
+-rw-r--r--   0        0        0      190 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/models/blog.ini
+-rw-r--r--   0        0        0      133 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/models/page.ini
+-rw-r--r--   0        0        0      193 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/templates/blog-post.html
+-rw-r--r--   0        0        0      493 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/templates/blog.html
+-rw-r--r--   0        0        0      706 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/templates/layout.html
+-rw-r--r--   0        0        0      659 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/templates/macros/blog-index.html
+-rw-r--r--   0        0        0      359 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/templates/macros/blog.html
+-rw-r--r--   0        0        0      475 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/templates/macros/pagination.html
+-rw-r--r--   0        0        0      103 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/templates/month-index.html
+-rw-r--r--   0        0        0      154 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/templates/page.html
+-rw-r--r--   0        0        0      288 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/demo-site/templates/year-index.html
+-rw-r--r--   0        0        0     3218 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/test_buildprog.py
+-rw-r--r--   0        0        0     2449 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/test_config.py
+-rw-r--r--   0        0        0     1439 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/test_functional.py
+-rw-r--r--   0        0        0    13242 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/test_indexmodel.py
+-rw-r--r--   0        0        0     5138 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/test_plugin.py
+-rw-r--r--   0        0        0    12027 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tests/test_sourceobj.py
+-rw-r--r--   0        0        0     1332 2023-06-16 16:34:12.570218 lektor_index_pages-1.1.0/tox.ini
+-rw-r--r--   0        0        0     6919 1970-01-01 00:00:00.000000 lektor_index_pages-1.1.0/PKG-INFO
```

### Comparing `lektor-index-pages-1.0.0/CHANGES.md` & `lektor_index_pages-1.1.0/CHANGES.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 ## Changelog
 
+### Release 1.1.0 (2023-06-16)
+
+- Drop support for Lektor 3.2.x
+- Test under python 3.11
+- Add type annotations
+- Convert packaging from setuptools to [PDM]
+- Disuse `pkg_resources` in favor of `importlib.metadata`
+- Add [pre-commit] configuration
+- Run [black] and [reorder-python-imports] on code
+
+[PDM]: https://pdm.fming.dev/latest/
+[pre-commit]: https://pre-commit.com/
+[black]: https://black.readthedocs.io/en/stable/index.html
+[reorder-python-imports]: https://github.com/asottile/reorder-python-imports
+
 ### Release 1.0 (2022-01-28)
 
 - Drop support for python 2.7 and 3.6.
 - Fix deprecation warning from `jinja2`. Jinja2 version 3 is now required.
 
 #### Documentation
```

### Comparing `lektor-index-pages-1.0.0/LICENSE` & `lektor_index_pages-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lektor-index-pages-1.0.0/README.md` & `lektor_index_pages-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Lektor Index Pages Plugin
 
 [![PyPI version](https://img.shields.io/pypi/v/lektor-index-pages.svg)](https://pypi.org/project/lektor-index-pages/)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/lektor-index-pages.svg)](https://pypi.python.org/pypi/lektor-index-pages/)
 [![GitHub license](https://img.shields.io/github/license/dairiki/lektor-index-pages)](https://github.com/dairiki/lektor-index-pages/blob/master/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/lektor-index-pages/badge/?version=latest)](https://lektor-index-pages.readthedocs.io/en/latest/?badge=latest)
 [![GitHub Actions (Tests)](https://github.com/dairiki/lektor-index-pages/workflows/Tests/badge.svg)](https://github.com/dairiki/lektor-index-pages)
-
+[![Trackgit Views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhauro0t5wzkw1d0k5lh)](https://trackgit.com)
 
 This [Lektor][] plugin can be used to generate “index pages” for a
 blog or similar collection of pages.  These index pages list the blog posts
 segregated by some key, with each index page containing only those posts
 which match that key.
 
 Examples of what this can be used for include:
```

### Comparing `lektor-index-pages-1.0.0/lektor_index_pages/buildprog.py` & `lektor_index_pages-1.1.0/lektor_index_pages/buildprog.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 """ Build program for the index pages.
 """
+from __future__ import annotations
+
+from typing import Generator
+from typing import TYPE_CHECKING
 
 from lektor.build_programs import BuildProgram
 from lektor.context import get_ctx
 
+if TYPE_CHECKING:
+    from lektor.builder import Artifact
+    from lektor.sourceobj import SourceObject
+
 
-class IndexBuildProgram(BuildProgram):
-    def produce_artifacts(self):
+class IndexBuildProgram(BuildProgram):  # type: ignore[misc]
+    def produce_artifacts(self) -> None:
         source = self.source
         record = source.record
 
         if source.is_visible:
             pagination_enabled = source.datamodel.pagination_config.enabled
             if not pagination_enabled or source.page_num is not None:
                 artifact_name = source.url_path
-                if artifact_name.endswith('/'):
-                    artifact_name += 'index.html'
+                if artifact_name.endswith("/"):
+                    artifact_name += "index.html"
                 # We don't really depend on record — the index doesn't
                 # change if the parent page contents do.  However, if
                 # no sources are listed here, the index will be pruned
                 # immediately after the build.  I guess this will do.
                 sources = [record.source_filename]
                 self.declare_artifact(artifact_name, sources=sources)
 
-    def build_artifact(self, artifact):
+    def build_artifact(self, artifact: Artifact) -> None:
         config_filename = self.source.datamodel.filename
-        template = self.source._data['_template']
+        template = self.source._data["_template"]
 
         if config_filename is not None:
             ctx = get_ctx()
             if ctx is not None:
                 ctx.record_dependency(config_filename)
 
         artifact.render_template_into(template, this=self.source)
 
-    def iter_child_sources(self):
+    def iter_child_sources(self) -> Generator[SourceObject, None, None]:
         source = self.source
         pagination_config = source.datamodel.pagination_config
 
         if pagination_config.enabled and source.page_num is None:
             num_pages = pagination_config.count_pages(source)
             for page_num in range(1, num_pages + 1):
                 yield source.__for_page__(page_num)
 
-        subindexes = getattr(source, 'subindexes', None)
+        subindexes = getattr(source, "subindexes", None)
         if subindexes is not None:
             yield from subindexes
```

### Comparing `lektor-index-pages-1.0.0/lektor_index_pages/config.py` & `lektor_index_pages-1.1.0/lektor_index_pages/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,95 @@
 """ Configuration and config-related logic.
 
 """
-from itertools import chain
+from __future__ import annotations
 
-from lektorlib.recordcache import get_or_create_virtual
+from itertools import chain
+from typing import Generator
+from typing import Sequence
+from typing import TYPE_CHECKING
 
 from lektor.environment import PRIMARY_ALT
+from lektorlib.recordcache import get_or_create_virtual
 
-from .indexmodel import (
-    VIRTUAL_PATH_PREFIX,
-    index_models_from_ini,
-    )
+from .indexmodel import index_models_from_ini
+from .indexmodel import VIRTUAL_PATH_PREFIX
 from .sourceobj import IndexRoot
 
+if TYPE_CHECKING:
+    from inifile import IniFile
+    from lektor.db import Pad
+    from lektor.db import Record
+    from lektor.environment import Environment
+
+    from .indexmodel import IndexRootModel
+    from .sourceobj import IndexSource
+
 
 class NoSuchIndex(KeyError):
     pass
 
 
 class Config:
-    def __init__(self, index_models):
+    def __init__(self, index_models: dict[str, IndexRootModel]):
         self.index_models = index_models
 
-    def get_index_root(self, index_name, pad, alt=PRIMARY_ALT):
+    def get_index_root(
+        self, index_name: str, pad: Pad, alt: str = PRIMARY_ALT
+    ) -> IndexRoot:
         index_model = self.index_models.get(index_name)
         if index_model is None:
-            raise NoSuchIndex("no index named {!r} is configured"
-                              .format(index_name))
+            raise NoSuchIndex(f"no index named {index_name!r} is configured")
         record = pad.get(index_model.parent_path, alt=alt)
         if record is None:
-            raise NoSuchIndex("no parent record exists at {!r} for index {!r}"
-                              .format(index_model.parent_path, index_name))
+            raise NoSuchIndex(
+                "no parent record exists at "
+                f"{index_model.parent_path!r} for index {index_name!r}"
+            )
         return IndexRoot.get_index(index_model, record)
 
-    def iter_index_roots(self, record):
+    def iter_index_roots(self, record: Record) -> Generator[IndexRoot, None, None]:
         record_path = record.path
         for index_model in self.index_models.values():
             if index_model.parent_path == record_path:
                 yield IndexRoot.get_index(index_model, record)
 
-    def resolve_virtual_path(self, record, pieces):
+    def resolve_virtual_path(
+        self, record: Record, pieces: Sequence[str]
+    ) -> IndexRoot | IndexSource | None:
         # Lektor's Pad.get or Pad.get_virtual does not cache virtual
         # sources, so we need to cache them ourself or things get
         # dreadfully slow.
         #
         # Interestingly, Lektor's RecordCache is perfectly capable of caching
         # virtual source objects, so we will use it...
-        def creator():
+        def creator() -> IndexRoot | IndexSource | None:
             return self._resolve_virtual_path(record, pieces)
-        virtual_path = '/'.join(chain([VIRTUAL_PATH_PREFIX], pieces))
+
+        virtual_path = "/".join(chain([VIRTUAL_PATH_PREFIX], pieces))
         return get_or_create_virtual(record, virtual_path, creator)
 
-    def _resolve_virtual_path(self, record, pieces):
+    def _resolve_virtual_path(
+        self, record: Record, pieces: Sequence[str]
+    ) -> IndexRoot | IndexSource | None:
         index_model = self.index_models.get(pieces[0])
         if index_model and index_model.parent_path == record.path:
             index_root = IndexRoot.get_index(index_model, record)
             return index_root.resolve_virtual_path(pieces[1:])
+        return None
 
-    def resolve_url_path(self, record, url_path):
+    def resolve_url_path(
+        self, record: Record, url_path: Sequence[str]
+    ) -> IndexSource | None:
         for index_root in self.iter_index_roots(record):
             source = index_root.resolve_url_path(url_path)
             if source is not None:
                 return source
+        return None
 
     @classmethod
-    def from_ini(cls, env, inifile):
+    def from_ini(cls, env: Environment, inifile: IniFile) -> Config:
         index_models = {}
         for root_model in index_models_from_ini(env, inifile):
             index_name = root_model.index_name
             index_models[index_name] = root_model
         return cls(dict(index_models))
```

### Comparing `lektor-index-pages-1.0.0/lektor_index_pages/sourceobj.py` & `lektor_index_pages-1.1.0/lektor_index_pages/sourceobj.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,307 +1,369 @@
 """ Virtual source objects for the indexes.
 
 """
+from __future__ import annotations
+
 import hashlib
+import pickle
+import sys
+from collections.abc import Hashable
 from itertools import chain
 from operator import itemgetter
-import pickle
-
-from lektorlib.context import disable_dependency_recording
-from lektorlib.query import PrecomputedQuery
-from lektorlib.recordcache import get_or_create_virtual
-from more_itertools import unique_everseen
+from typing import Any
+from typing import Callable
+from typing import Iterable
+from typing import Sequence
+from typing import TYPE_CHECKING
+from typing import TypeVar
 
 import jinja2
 from lektor.db import _CmpHelper
 from lektor.environment import PRIMARY_ALT
 from lektor.pluginsystem import get_plugin
 from lektor.sourceobj import VirtualSourceObject
 from lektor.utils import build_url
+from lektorlib.context import disable_dependency_recording
+from lektorlib.query import PrecomputedQuery
+from lektorlib.recordcache import get_or_create_virtual
+from more_itertools import unique_everseen
 from werkzeug.utils import cached_property
 
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
+if TYPE_CHECKING:
+    from lektor.builder import PathCache
+    from lektor.db import Record
+    from lektor.pagination import Pagination
+    from .indexmodel import IndexModel
+    from .indexmodel import IndexRootModel
+    from .plugin import Cache
+    from .plugin import IndexPagesPlugin
 
-def get_system_data(model, id_):
+
+_T = TypeVar("_T")
+
+
+def get_system_data(model: IndexModel, id_: str) -> dict[str, Any]:
     jinja_env = model.env.jinja_env
 
     # NB: For any data descriptors in here,
     # IndexSource.__getitem__ will call its __get__
     return {
-        '_id': id_,
-        'key': id_,
-        '_slug': IndexSource._slug,
-        '_path': IndexSource.path,
-        '_gid': IndexSource._gid,
-        '_template': getattr(model, 'template', None),
-
-        '_hidden': IndexSource.is_hidden,
-        '_discoverable': IndexSource.is_discoverable,  # always true
-        '_alt': IndexSource.alt,
+        "_id": id_,
+        "key": id_,
+        "_slug": IndexSource._slug,
+        "_path": IndexSource.path,
+        "_gid": IndexSource._gid,
+        "_template": getattr(model, "template", None),
+        "_hidden": IndexSource.is_hidden,
+        "_discoverable": IndexSource.is_discoverable,  # always true
+        "_alt": IndexSource.alt,
         # There is no source for these — they are virtual
         # So reasonable values seem to be either PRIMARY_ALT or Undefined
-        '_source_alt': PRIMARY_ALT,
-
-        '_model': jinja_env.undefined(
-            "Missing value in field '_model': index is virtual"),
-
-        '_attachment_for': jinja_env.undefined(
-            "Missing value in field '_attachment_for': not an attachment"),
-        '_attachment_type': jinja_env.undefined(
-            "Missing value in field '_attachment_type': not an attachment"),
-        }
-
-
-class IndexBase(VirtualSourceObject):
-
-    def __init__(self, model, parent, id_, children, page_num=None):
+        "_source_alt": PRIMARY_ALT,
+        "_model": jinja_env.undefined(
+            "Missing value in field '_model': index is virtual"
+        ),
+        "_attachment_for": jinja_env.undefined(
+            "Missing value in field '_attachment_for': not an attachment"
+        ),
+        "_attachment_type": jinja_env.undefined(
+            "Missing value in field '_attachment_type': not an attachment"
+        ),
+    }
+
+
+class IndexBase(VirtualSourceObject):  # type: ignore[misc]
+    def __init__(
+        self,
+        model: IndexRootModel | IndexModel,
+        parent: Record | IndexBase,
+        id_: str,
+        children: PrecomputedQuery[Record],
+        page_num: int | None = None,
+    ):
         VirtualSourceObject.__init__(self, parent.record)
         self._model = model
         self._id = id_
         self.children = children
         self.datamodel = model.datamodel
         self.page_num = page_num
         self.virtual_path = model.get_virtual_path(parent, id_, page_num)
 
+    @property
+    def has_subindex(self) -> bool:
+        """True iff this index has a sub-index configured."""
+        return self._model.subindex_model is not None
+
     @cached_property
-    def subindexes(self):
+    def subindexes(self) -> PrecomputedQuery[IndexSource]:
         """A Query containing the indexes.
 
         E.g. at the top level of a date index, this Query might
         iterate over the indexes for each year.
 
         """
-        subindex_ids = self._subindex_ids
+        if not self.has_subindex:
+            raise AttributeError("no sub-index is configured")
         # path without page number
         path = self.__for_page__(None).path
-        return PrecomputedQuery(path, self.pad, subindex_ids, alt=self.alt)
+        return PrecomputedQuery(path, self.pad, self._subindex_ids, alt=self.alt)
 
     @cached_property
-    def _subindex_ids(self):
-        subindex_model = getattr(self._model, 'subindex_model', None)
-        if subindex_model is None:
-            raise AttributeError("sub-indexes are not enabled")
+    def _subindex_ids(self) -> tuple[str, ...]:
+        if self._model.subindex_model is None:
+            raise AttributeError("no sub-index is configured")
+        subindex_model = self._model.subindex_model
 
-        def get_subindex_ids():
+        def get_subindex_ids() -> tuple[str, ...]:
             with disable_dependency_recording():
-                return tuple(unique_everseen(
-                    chain.from_iterable(
-                        map(subindex_model.keys_for_post, self.children))))
+                return tuple(
+                    unique_everseen(
+                        chain.from_iterable(
+                            map(subindex_model.keys_for_post, self.children)
+                        )
+                    )
+                )
 
-        cache_key = 'subindex_ids', self.path
+        cache_key = "subindex_ids", self.path
         return self._get_cache().get_or_create(cache_key, get_subindex_ids)
 
-    def _get_cache(self):
+    def _get_cache(self) -> Cache | DummyCache:
         try:
-            plugin = get_plugin('index-pages', self.pad.env)
+            plugin: IndexPagesPlugin = get_plugin("index-pages", self.pad.env)
         except LookupError:
             return DummyCache()  # testing
         else:
             return plugin.cache
 
     @cached_property
-    def path(self):
+    def path(self) -> str:
         return f"{self.record.path}@{self.virtual_path}"
 
-    def resolve_virtual_path(self, pieces):
+    def resolve_virtual_path(
+        self, pieces: Sequence[str]
+    ) -> IndexRoot | IndexSource | None:
         if not pieces:
             return self
 
-        subindex_model = getattr(self._model, 'subindex_model', None)
-        if subindex_model is not None:
+        if self.has_subindex:
             if pieces[0] in self._subindex_ids:
                 subindex = self._get_subindex(pieces[0])
                 return subindex.resolve_virtual_path(pieces[1:])
 
         return self._model.match_path_pagination(self, pieces)
 
-    def resolve_url_path(self, url_path):
+    def resolve_url_path(self, url_path: Sequence[str]) -> IndexSource | None:
         pagination_config = self.datamodel.pagination_config
 
         if not url_path:
             # resolve to first page rather than unpaginated version
             page_num = 1 if pagination_config.enabled else None
             return self.__for_page__(page_num)
 
-        subindex_model = getattr(self._model, 'subindex_model', None)
-        if subindex_model is not None:
+        if self.has_subindex:
+            subindex: IndexSource
             for subindex in self.subindexes:
-                slug = subindex._slug.split('/')
-                if url_path[:len(slug)] == slug:
-                    return subindex.resolve_url_path(url_path[len(slug):])
+                slug = subindex._slug.split("/")
+                if url_path[: len(slug)] == slug:
+                    return subindex.resolve_url_path(url_path[len(slug) :])
 
         if pagination_config.enabled:
-            return pagination_config.match_pagination(self, url_path)
+            return pagination_config.match_pagination(  # type: ignore[no-any-return]
+                self, url_path
+            )
+
+        return None
+
+    def __for_page__(self, page_num: int | None) -> IndexRoot | IndexSource:
+        raise NotImplementedError()
 
-    def _get_subindex(self, id_, page_num=None):
+    def _get_subindex(self, id_: str, page_num: int | None = None) -> IndexSource:
+        if self._model.subindex_model is None:
+            raise LookupError("no sub-index is configured")
         subindex_model = self._model.subindex_model
 
-        def get_child_ids():
+        def get_child_ids() -> list[str]:
             keys_for_post = subindex_model.keys_for_post
 
-            def match_key(post):
+            def match_key(post: Record) -> bool:
                 return id_ in keys_for_post(post)
 
             children = self.children.filter(match_key)
             # We could just give the subindex the raw query, but if we do,
             # it generates unnecessary dependencies when iterated over in
             # a template.
             #
             # To avoid this, we precompute the list of matching ids (while
             # ignoring any dependencies), and return a custom Query class
             # which will iterate over only those matching children.
             with disable_dependency_recording():
-                return list(map(itemgetter('_id'), children))
+                return list(map(itemgetter("_id"), children))
 
-        cache_key = 'child_ids', self.path, id_
+        cache_key = "child_ids", self.path, id_
         child_ids = self._get_cache().get_or_create(cache_key, get_child_ids)
-        children = PrecomputedQuery(
-            self.children.path, self.pad, child_ids, alt=self.children.alt)
-        return IndexSource.get_index(
-            subindex_model, self, id_, children, page_num)
+        children: PrecomputedQuery[Record] = PrecomputedQuery(
+            self.children.path, self.pad, child_ids, alt=self.children.alt
+        )
+        return IndexSource.get_index(subindex_model, self, id_, children, page_num)
 
     @cached_property
-    def _gid(self):
-        return hashlib.md5(self.path.encode('utf-8')).hexdigest()
+    def _gid(self) -> str:
+        return hashlib.md5(self.path.encode("utf-8")).hexdigest()
 
-    def get_checksum(self, path_cache):
+    def get_checksum(self, path_cache: PathCache) -> str:
         return self._compute_checksum(self._get_checksum_data(path_cache))
 
-    def _get_checksum_data(self, path_cache):
+    def _get_checksum_data(
+        self, path_cache: PathCache
+    ) -> tuple[tuple[str, ...] | str, ...]:
         # Checksum for this virtual source It should change if the
         # composition --- that is the sequence of subindexes or the
         # sequence of childeren (e.g. blog posts) --- changes.
 
+        child_paths: tuple[str, ...] | str
         with disable_dependency_recording():
             if not self.datamodel.pagination_config.enabled:
                 # Normal index page.
                 # We change if the sequence of child identities changes
-                child_paths = [child.path for child in self.children]
+                child_paths = tuple(child.path for child in self.children)
             elif self.page_num is not None:
                 # Pagination is in effect, we change if the sequence of
                 # child identities on this page changes
-                child_paths = [child.path for child in self.pagination.items]
+                child_paths = tuple(child.path for child in self.pagination.items)
             else:
                 # Pagination is in effect, but we're the unpaginated page.
                 # We change if the number of pages changes
                 child_paths = f"NPAGES={self.pagination.pages}"
 
-        subindex_ids = getattr(self, '_subindex_ids', None)
-        if subindex_ids is not None:
+        if self.has_subindex:
             # If we have subindexes the composition of the index
             # also depends on the sequence of subindexes
-            return self.path, child_paths, subindex_ids
+            return self.path, child_paths, self._subindex_ids
         return self.path, child_paths
 
     @staticmethod
-    def _compute_checksum(data):
+    def _compute_checksum(data: tuple[tuple[str, ...] | str, ...]) -> str:
         return hashlib.sha1(pickle.dumps(data, protocol=0)).hexdigest()
 
     # is_discoverable = True (inherited from SourceObject)
     # alt = self.record.alt (inherited from VirtualSourceObject)
 
     # FIXME: to implement?
     # Page
     # has_prev
     # has_next
     # get_siblings
 
-    def __eq__(self, other):
-        if self is other:
-            return True
-        return (self.__class__ == other.__class__
-                and self.path == other.path)
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, IndexBase):
+            return NotImplemented
+        return other.path == self.path and other.__class__ == self.__class__
 
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(self.path)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         # path without page_num
-        bits = ["path={path!r}"]
+        bits = [f"path={self.__for_page__(None).path!r}"]
         if self.alt is not PRIMARY_ALT:
-            bits.append("alt={alt!r}")
+            bits.append(f"alt={self.alt!r}")
         if self.page_num is not None:
-            bits.append("page_num={page_num}")
-        desc = ' '.join(bits).format(
-            path=self.__for_page__(None).path,  # path without page_num
-            alt=self.alt,
-            page_num=self.page_num)
-        return f"<{self.__class__.__name__} {desc}>"
+            bits.append(f"page_num={self.page_num}")
+        return f"<{self.__class__.__name__} {' '.join(bits)}>"
 
 
 class IndexRoot(IndexBase):
-    """Root source node for an index tree.
+    """Root source node for an index tree."""
 
-    """
-    def __init__(self, model, record):
-        IndexBase.__init__(self, model, record,
-                           id_=model.index_name,
-                           children=model.get_items(record))
+    def __init__(self, model: IndexRootModel, record: Record):
+        IndexBase.__init__(
+            self, model, record, id_=model.index_name, children=model.get_items(record)
+        )
 
     @classmethod
-    def get_index(class_, model, record):
-        def creator():
+    def get_index(class_, model: IndexRootModel, record: Record) -> IndexRoot:
+        def creator() -> IndexRoot:
             assert record.record == record
             return class_(model, record)
+
         virtual_path = model.get_virtual_path(record)
         return get_or_create_virtual(record, virtual_path, creator)
 
     @property
-    def _slug(self):
+    def _slug(self) -> None:
         return None
 
     @property
-    def url_path(self):
-        return self.record.url_path
+    def url_path(self) -> str:
+        return self.record.url_path  # type: ignore[no-any-return]
 
-    def __for_page__(self, page_num):
-        """Get source object for a (possibly) different page number.
-        """
+    def __for_page__(self, page_num: int | None) -> IndexRoot:
+        """Get source object for a (possibly) different page number."""
         assert page_num is None
         return self
 
     @property
-    def is_hidden(self):
+    def is_hidden(self) -> Literal[True]:
         # top level of the index trees does not actually produce an artifact
         return True
 
 
 class IndexSource(IndexBase):
-    """Index source node.
+    """Index source node."""
+
+    # override property in parent
+    parent: IndexRoot | IndexSource = None  # type: ignore[assignment]
 
-    """
-    parent = None               # override property in parent
+    _model: IndexModel
 
-    def __init__(self, model, parent, id_, children, page_num=None):
+    def __init__(
+        self,
+        model: IndexModel,
+        parent: IndexRoot | IndexSource,
+        id_: str,
+        children: PrecomputedQuery[Record],
+        page_num: int | None = None,
+    ):
         IndexBase.__init__(self, model, parent, id_, children, page_num)
         self.parent = parent
         self._data = get_system_data(model, id_)
         self._data.update(model.data_descriptors)
 
     @classmethod
-    def get_index(class_, model, parent, id_, children, page_num=None):
-        def creator():
+    def get_index(
+        class_,
+        model: IndexModel,
+        parent: IndexRoot | IndexSource,
+        id_: str,
+        children: PrecomputedQuery[Record],
+        page_num: int | None = None,
+    ) -> IndexSource:
+        def creator() -> IndexSource:
             return class_(model, parent, id_, children, page_num)
+
         virtual_path = model.get_virtual_path(parent, id_, page_num)
         return get_or_create_virtual(parent.record, virtual_path, creator)
 
-    def __contains__(self, name):
+    def __contains__(self, name: str) -> bool:
         return name in self._data and not jinja2.is_undefined(self[name])
 
-    def __getitem__(self, name):
+    def __getitem__(self, name: str) -> Any:
         rv = self._data[name]
-        if hasattr(rv, '__get__'):
+        if hasattr(rv, "__get__"):
             rv = rv.__get__(self)
             self._data[name] = rv
         return rv
 
     @cached_property
-    def pagination(self):
+    def pagination(self) -> Pagination:
         pagination_config = self.datamodel.pagination_config
 
         # XXX: get_pagination_controller raises RuntimeError if
         # pagination is not enabled.  Perhaps AttributeError would be
         # better or maybe an Undefined?  However this is what
         # lektor.db.Page.pagination does, so we’ll stick with it for
         # now.
@@ -319,48 +381,50 @@
         # iterate over self.pagination.items, thus registering all
         # the items on the page as dependencies.  (And if it doesn’t,
         # then they shouldn't needn’t be dependencies.)
         with disable_dependency_recording():
             return pagination_config.get_pagination_controller(self)
 
     @cached_property
-    def _slug(self):
+    def _slug(self) -> str:
         return self._model.get_slug(self)
 
     @property
-    def url_path(self):
+    def url_path(self) -> str:
         datamodel = self.datamodel
         slug = self._slug
         path = [self.parent.url_path, slug]
-        if self.page_num not in (None, 1):
+        if self.page_num is not None and self.page_num != 1:
             assert datamodel.pagination_config.enabled
             path.append(datamodel.pagination_config.url_suffix)
-            path.append(self.page_num)
-        _, _, slug_tail = slug.rstrip('/').rpartition('/')
-        return build_url(path, trailing_slash=('.' not in slug_tail))
+            path.append(f"{self.page_num:d}")
+        _, _, slug_tail = slug.rstrip("/").rpartition("/")
+        return build_url(  # type: ignore[no-any-return]
+            path, trailing_slash=("." not in slug_tail)
+        )
 
-    def __for_page__(self, page_num):
-        """Get source object for a (possibly) different page number.
-        """
+    def __for_page__(self, page_num: int | None) -> IndexSource:
+        """Get source object for a (possibly) different page number."""
         if page_num == self.page_num:
             return self
         return self.get_index(
-            self._model, self.parent, self._id, self.children, page_num)
+            self._model, self.parent, self._id, self.children, page_num
+        )
 
     @property
-    def is_hidden(self):
-        return self.record.is_hidden
+    def is_hidden(self) -> bool:
+        return self.record.is_hidden  # type: ignore[no-any-return]
 
-    def get_sort_key(self, fields):
-        def cmp_val(field):
-            reverse = field.startswith('-')
-            if reverse or field.startswith('+'):
+    def get_sort_key(self, fields: Iterable[str]) -> list[_CmpHelper]:
+        def cmp_val(field: str) -> _CmpHelper:
+            reverse = field.startswith("-")
+            if reverse or field.startswith("+"):
                 field = field[1:]
             value = self[field] if field in self else None
             return _CmpHelper(value, reverse)
 
         return [cmp_val(field) for field in fields]
 
 
 class DummyCache:
-    def get_or_create(self, key, creator):
+    def get_or_create(self, key: Hashable, creator: Callable[[], _T]) -> _T:
         return creator()
```

### Comparing `lektor-index-pages-1.0.0/tests/conftest.py` & `lektor_index_pages-1.1.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,45 @@
-try:
-    from pathlib import Path
-except ImportError:             # pragma: no cover
-    from pathlib2 import Path
+import sys
+from contextlib import ExitStack
+from pathlib import Path
 
-import pkg_resources
-import pytest
-
-from inifile import IniFile
 import lektor.builder
 import lektor.context
 import lektor.datamodel
 import lektor.db
 import lektor.environment
 import lektor.pagination
 import lektor.project
+import pytest
+from inifile import IniFile
+
+if sys.version_info >= (3, 10):
+    from importlib.metadata import distribution
+else:
+    from importlib_metadata import distribution
 
 
 @pytest.fixture(scope="session")
 def my_plugin_id():
-    dist = pkg_resources.get_distribution('lektor_index_pages')
-    prefix = 'lektor-'
-    assert dist.project_name.lower().startswith(prefix)
-    return dist.project_name[len(prefix):]
+    dist = distribution("lektor_index_pages")
+    prefix = "lektor-"
+    assert dist.name.lower().startswith(prefix)
+    return dist.name[len(prefix) :]
 
 
 @pytest.fixture(scope="session")
 def my_plugin_cls(my_plugin_id):
-    dist = pkg_resources.get_distribution('lektor_index_pages')
-    return dist.load_entry_point('lektor.plugins', my_plugin_id)
+    dist = distribution("lektor_index_pages")
+    eps = dist.entry_points.select(group="lektor.plugins")
+    return eps[my_plugin_id].load()
 
 
 @pytest.fixture(scope="session")
 def site_path():
-    return Path(__file__).parent / 'demo-site'
+    return Path(__file__).parent / "demo-site"
 
 
 @pytest.fixture
 def lektor_project(site_path):
     return lektor.project.Project.from_path(str(site_path))
 
 
@@ -53,15 +56,19 @@
 @pytest.fixture
 def lektor_builder(lektor_pad, tmp_path):
     return lektor.builder.Builder(lektor_pad, str(tmp_path / "builder_output"))
 
 
 @pytest.fixture
 def lektor_build_state(lektor_builder):
-    with lektor_builder.new_build_state() as build_state:
+    with ExitStack() as stack:
+        build_state = lektor_builder.new_build_state()
+        if hasattr(build_state, "__enter__"):
+            # Lektor < 3.4
+            build_state = stack.enter_context(build_state)
         yield build_state
 
 
 @pytest.fixture
 def lektor_context(lektor_pad):
     with lektor.context.Context(pad=lektor_pad) as ctx:
         yield ctx
@@ -70,64 +77,63 @@
 @pytest.fixture
 def lektor_alt():
     return lektor.environment.PRIMARY_ALT
 
 
 @pytest.fixture
 def blog_record(lektor_pad, lektor_alt):
-    return lektor_pad.get('/blog', alt=lektor_alt)
+    return lektor_pad.get("/blog", alt=lektor_alt)
 
 
 @pytest.fixture
 def month_index_enabled():
     return False
 
 
 @pytest.fixture
 def pagination_enabled():
     # Set to a positive integer to also set pagination.per_page
     return False
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def junk_ini(tmp_path_factory):
-    return tmp_path_factory.mktemp('junk') / 'junk.ini'
+    return tmp_path_factory.mktemp("junk") / "junk.ini"
 
 
 @pytest.fixture
-def inifile(site_path, junk_ini, my_plugin_id,
-            pagination_enabled, month_index_enabled):
+def inifile(site_path, junk_ini, my_plugin_id, pagination_enabled, month_index_enabled):
     # Make a temporary copy of our .ini file
-    config_name = '%s.ini' % my_plugin_id
-    orig_ini = site_path / 'configs' / config_name
+    config_name = "%s.ini" % my_plugin_id
+    orig_ini = site_path / "configs" / config_name
     inifile = IniFile(str(orig_ini))
     inifile.filename = str(junk_ini)
 
     def yesno(val):
-        return 'yes' if val else 'no'
+        return "yes" if val else "no"
 
-    inifile['pagination.enabled'] = yesno(pagination_enabled)
+    inifile["pagination.enabled"] = yesno(pagination_enabled)
     if not month_index_enabled:
-        del inifile['year-index.subindex']
+        del inifile["year-index.subindex"]
 
     if not isinstance(pagination_enabled, bool):
-        inifile['pagination.per_page'] = pagination_enabled
+        inifile["pagination.per_page"] = pagination_enabled
     return inifile
 
 
 @pytest.fixture
 def plugin(lektor_env, my_plugin_id, my_plugin_cls, inifile):
     # install our plugin
     plugin_controller = lektor_env.plugin_controller
     plugin_controller.instanciate_plugin(my_plugin_id, my_plugin_cls)
 
     # patch in our test inifile
     plugin = lektor_env.plugins[my_plugin_id]
     plugin._inifile = inifile
 
-    plugin_controller.emit('setup-env')
+    plugin_controller.emit("setup-env")
     return plugin
 
 
 @pytest.fixture
 def config(plugin):
     return plugin.read_config()
```

### Comparing `lektor-index-pages-1.0.0/tests/demo-site/assets/static/style.css` & `lektor_index_pages-1.1.0/tests/demo-site/assets/static/style.css`

 * *Files identical despite different names*

### Comparing `lektor-index-pages-1.0.0/tests/demo-site/templates/layout.html` & `lektor_index_pages-1.1.0/tests/demo-site/templates/layout.html`

 * *Files identical despite different names*

### Comparing `lektor-index-pages-1.0.0/tests/demo-site/templates/macros/blog-index.html` & `lektor_index_pages-1.1.0/tests/demo-site/templates/macros/blog-index.html`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,7 @@
             {% endfor %}
           </ul>
         </li>
       {% endfor %}
     </ul>
   {% endif %}
 {% endmacro %}
-
```

### Comparing `lektor-index-pages-1.0.0/tests/test_buildprog.py` & `lektor_index_pages-1.1.0/tests/test_buildprog.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,85 +1,96 @@
+from pathlib import Path
+
 import lektor.context
 import pytest
 
-from .conftest import Path
-
 from lektor_index_pages.buildprog import IndexBuildProgram
 
 
 @pytest.fixture
 def index_root(config, lektor_pad):
-    return config.get_index_root('year-index', lektor_pad)
+    return config.get_index_root("year-index", lektor_pad)
 
 
 class Test_build_index_root:
     @pytest.fixture
     def source(self, index_root):
         return index_root
 
     @pytest.fixture
     def prog(self, source, lektor_build_state):
         return IndexBuildProgram(source, lektor_build_state)
 
     def test_produce_artifacts(self, prog, source, mocker):
         declare_artifact = mocker.patch(
-            'lektor.build_programs.BuildProgram.declare_artifact')
+            "lektor.build_programs.BuildProgram.declare_artifact"
+        )
         prog.produce_artifacts()
         assert not declare_artifact.called
 
     def test_iter_child_sources_pages(self, prog, source):
-        assert [src.path for src in prog.iter_child_sources()] \
-            == ['/blog@index-pages/year-index/2020']
+        assert [src.path for src in prog.iter_child_sources()] == [
+            "/blog@index-pages/year-index/2020"
+        ]
 
 
 class TestIndexBuildProgram:
     @pytest.fixture
     def source(self, index_root):
-        return index_root.resolve_virtual_path(['2020'])
+        return index_root.resolve_virtual_path(["2020"])
 
     @pytest.fixture
     def prog(self, source, lektor_build_state):
         return IndexBuildProgram(source, lektor_build_state)
 
     def test_source_filename(self, source):
         # sanity check
         source_filename = Path(source.record.source_filename)
-        assert source_filename.parts[-2:] == ('blog', 'contents.lr')
+        assert source_filename.parts[-2:] == ("blog", "contents.lr")
 
     def test_produce_artifacts(self, prog, source, mocker):
         source_filename = source.record.source_filename
         declare_artifact = mocker.patch(
-            'lektor.build_programs.BuildProgram.declare_artifact')
+            "lektor.build_programs.BuildProgram.declare_artifact"
+        )
         prog.produce_artifacts()
         assert declare_artifact.called_once_with(
-            '/blog/2020/index.html', sources=[source_filename])
+            "/blog/2020/index.html", sources=[source_filename]
+        )
 
     def test_build_artifact(self, prog, source, mocker):
         template = "year-index.html"
-        artifact = mocker.Mock(name='artifact', spec=('render_template_into',))
+        artifact = mocker.Mock(name="artifact", spec=("render_template_into",))
 
         prog.build_artifact(artifact)
         assert artifact.mock_calls == [
             mocker.call.render_template_into(template, this=source),
-            ]
+        ]
 
-    def test_build_artifact_records_dependency(self, prog, source, inifile,
-                                               mocker):
-        artifact = mocker.Mock(name='artifact')
+    def test_build_artifact_records_dependency(self, prog, source, inifile, mocker):
+        artifact = mocker.Mock(name="artifact")
         with lektor.context.Context(artifact, pad=None) as ctx:
             prog.build_artifact(artifact)
         assert inifile.filename in ctx.referenced_dependencies
 
-    @pytest.mark.parametrize('pagination_enabled', [True])
+    @pytest.mark.parametrize("pagination_enabled", [True])
     def test_iter_child_sources_pages(self, prog, source):
-        assert [src.path for src in prog.iter_child_sources()] \
-            == ['/blog@index-pages/year-index/2020/page/1']
+        assert [src.path for src in prog.iter_child_sources()] == [
+            "/blog@index-pages/year-index/2020/page/1"
+        ]
 
     @pytest.mark.parametrize(
-        'pagination_enabled, month_index_enabled, expected', [
-            (True, False, ['/blog@index-pages/year-index/2020/page/1']),
-            (False, True, ['/blog@index-pages/year-index/2020/04',
-                           '/blog@index-pages/year-index/2020/03']),
-            ]
-        )
+        "pagination_enabled, month_index_enabled, expected",
+        [
+            (True, False, ["/blog@index-pages/year-index/2020/page/1"]),
+            (
+                False,
+                True,
+                [
+                    "/blog@index-pages/year-index/2020/04",
+                    "/blog@index-pages/year-index/2020/03",
+                ],
+            ),
+        ],
+    )
     def test_iter_child_sources(self, prog, expected):
         assert [src.path for src in prog.iter_child_sources()] == expected
```

### Comparing `lektor-index-pages-1.0.0/tests/test_config.py` & `lektor_index_pages-1.1.0/tests/test_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 import pytest
 
-from lektor_index_pages.config import (
-    Config,
-    NoSuchIndex,
-    )
+from lektor_index_pages.config import Config
+from lektor_index_pages.config import NoSuchIndex
 from lektor_index_pages.sourceobj import IndexRoot
 
 
 class TestConfig:
     @pytest.fixture
     def parent_path(self):
-        return '/blog'
+        return "/blog"
 
     @pytest.fixture
     def inifile(self, inifile, parent_path):
-        inifile['year-index.parent_path'] = parent_path
+        inifile["year-index.parent_path"] = parent_path
         return inifile
 
     @pytest.fixture
     def config(self, lektor_env, inifile):
         return Config.from_ini(lektor_env, inifile)
 
     def test_get_index_root(self, config, lektor_pad):
-        root = config.get_index_root('year-index', lektor_pad)
+        root = config.get_index_root("year-index", lektor_pad)
         assert isinstance(root, IndexRoot)
-        assert root._id == 'year-index'
+        assert root._id == "year-index"
 
     def test_get_index_root_fails_if_name_unknown(self, config, lektor_pad):
-        with pytest.raises(NoSuchIndex,
-                           match=r'no index named .* is configured'):
-            config.get_index_root('missing', lektor_pad)
+        with pytest.raises(NoSuchIndex, match=r"no index named .* is configured"):
+            config.get_index_root("missing", lektor_pad)
 
-    @pytest.mark.parametrize('parent_path', ['/missing-parent'])
+    @pytest.mark.parametrize("parent_path", ["/missing-parent"])
     def test_get_index_root_fails_if_parent_unknown(self, config, lektor_pad):
-        with pytest.raises(NoSuchIndex, match=r'no parent .*\bexists'):
-            config.get_index_root('year-index', lektor_pad)
+        with pytest.raises(NoSuchIndex, match=r"no parent .*\bexists"):
+            config.get_index_root("year-index", lektor_pad)
 
     def test_iter_index_roots(self, config, blog_record):
         roots = list(config.iter_index_roots(blog_record))
         assert len(roots) == 1
         assert isinstance(roots[0], IndexRoot)
-        assert roots[0]._id == 'year-index'
+        assert roots[0]._id == "year-index"
 
     def test_resolve_virtual_path(self, config, blog_record):
-        root = config.resolve_virtual_path(blog_record, ['year-index'])
+        root = config.resolve_virtual_path(blog_record, ["year-index"])
         assert isinstance(root, IndexRoot)
 
     def test_resolve_virtual_path_caching(self, config, blog_record):
-        source = config.resolve_virtual_path(blog_record, ['year-index'])
-        assert source._id == 'year-index'
-        reget = config.resolve_virtual_path(blog_record, ['year-index'])
+        source = config.resolve_virtual_path(blog_record, ["year-index"])
+        assert source._id == "year-index"
+        reget = config.resolve_virtual_path(blog_record, ["year-index"])
         assert reget is source
 
     def test_resolve_virtual_path_failure(self, config, blog_record):
-        assert config.resolve_virtual_path(blog_record, ['missing']) is None
+        assert config.resolve_virtual_path(blog_record, ["missing"]) is None
 
-    @pytest.mark.usefixtures('plugin')
+    @pytest.mark.usefixtures("plugin")
     def test_resolve_url_path(self, config, blog_record):
-        year_idx = config.resolve_url_path(blog_record, ['2020'])
-        assert year_idx['year'] == 2020
+        year_idx = config.resolve_url_path(blog_record, ["2020"])
+        assert year_idx["year"] == 2020
+
+    @pytest.mark.usefixtures("plugin")
+    def test_resolve_url_path_failure(self, config, blog_record):
+        assert config.resolve_url_path(blog_record, ["missing"]) is None
```

### Comparing `lektor-index-pages-1.0.0/tests/test_functional.py` & `lektor_index_pages-1.1.0/tests/test_functional.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,50 @@
+import pytest
 from lektor.builder import Builder
 from lektor.db import Database
 from lektor.environment import Environment
 from lektor.project import Project
 from lektor.reporter import CliReporter
-import pytest
 
 
 @pytest.fixture(scope="module")
 def demo_output(site_path, my_plugin_id, my_plugin_cls, tmp_path_factory):
-    """ Build the demo site.
+    """Build the demo site.
 
     Return path to output directory.
 
     """
     project = Project.from_path(str(site_path))
     env = Environment(project, load_plugins=False)
 
     # Load our plugin
     env.plugin_controller.instanciate_plugin(my_plugin_id, my_plugin_cls)
-    env.plugin_controller.emit('setup-env')
+    env.plugin_controller.emit("setup-env")
 
     pad = Database(env).new_pad()
-    output_path = tmp_path_factory.mktemp('demo-site')
+    output_path = tmp_path_factory.mktemp("demo-site")
     builder = Builder(pad, str(output_path))
     with CliReporter(env):
         failures = builder.build_all()
         assert failures == 0
     return output_path
 
 
 def test_year_index(demo_output):
-    year_index_html = demo_output / 'blog/2020/index.html'
+    year_index_html = demo_output / "blog/2020/index.html"
     assert "Blog - 2020" in year_index_html.read_text()
 
 
-@pytest.mark.parametrize("id, expect_text", [
-    ('1999/03', None),
-    ('2020/03', "March 2020"),
-    ('2020/04', "April 2020"),
-    ])
+@pytest.mark.parametrize(
+    "id, expect_text",
+    [
+        ("1999/03", None),
+        ("2020/03", "March 2020"),
+        ("2020/04", "April 2020"),
+    ],
+)
 def test_month_index(demo_output, id, expect_text):
-    month_index_html = demo_output / 'blog' / id / 'index.html'
+    month_index_html = demo_output / "blog" / id / "index.html"
     if expect_text:
         assert expect_text in month_index_html.read_text()
     else:
         assert not month_index_html.exists()
```

### Comparing `lektor-index-pages-1.0.0/tests/test_indexmodel.py` & `lektor_index_pages-1.1.0/tests/test_indexmodel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 import copy
 import datetime
 import inspect
-from operator import attrgetter
 import re
+from operator import attrgetter
 
 import pytest
-
 from inifile import IniFile
 
-from lektor_index_pages.indexmodel import (
-    VIRTUAL_PATH_PREFIX,
-    PaginationConfig,
-    IndexRootModel,
-    IndexModel,
-    ExpressionCompiler,
-    index_models_from_ini,
-    _index_model_from_ini,
-    _field_config_from_ini,
-    _pagination_config_from_ini,
-    )
+from lektor_index_pages.indexmodel import _field_config_from_ini
+from lektor_index_pages.indexmodel import _index_model_from_ini
+from lektor_index_pages.indexmodel import _pagination_config_from_ini
+from lektor_index_pages.indexmodel import ExpressionCompiler
+from lektor_index_pages.indexmodel import index_models_from_ini
+from lektor_index_pages.indexmodel import IndexModel
+from lektor_index_pages.indexmodel import IndexRootModel
+from lektor_index_pages.indexmodel import PaginationConfig
+from lektor_index_pages.indexmodel import VIRTUAL_PATH_PREFIX
 
 
 @pytest.fixture
 def pagination_config(lektor_env, pagination_enabled):
     kw = {}
     if not isinstance(pagination_enabled, bool):
-        kw['per_page'] = int(pagination_enabled)
+        kw["per_page"] = int(pagination_enabled)
         pagination_enabled = bool(pagination_enabled)
 
     return PaginationConfig(lektor_env, enabled=pagination_enabled, **kw)
 
 
 class DummyQuery:
     def __init__(self, count):
@@ -60,81 +57,80 @@
     @pytest.fixture(params=[False, True])
     def source(self, request, lektor_pad):
         if request.param:
             # Dummy virtual source with .__for_page__ method
             return DummyPaginatable()
         else:
             # Concrete record
-            return lektor_pad.get('/blog/first-post')
+            return lektor_pad.get("/blog/first-post")
 
     def test_get_record_for_page(self, pagination_config, source, page_num):
         paginated = pagination_config.get_record_for_page(source, page_num)
-        paginated.page_num == page_num
-        paginated.record is source.record
+        assert paginated.page_num == page_num
+        assert paginated.record is source.record
 
 
 class TestIndexRootModel:
-
     @pytest.fixture
     def items(self):
         return None
 
     @pytest.fixture
     def model(self, lektor_env, items, mocker):
         return IndexRootModel(
             lektor_env,
-            index_name='test-index',
+            index_name="test-index",
             index_model=mocker.sentinel.index_model,
             items=items,
-            config_filename='dummy.ini')
+            config_filename="dummy.ini",
+        )
 
     def test_datamodel(self, model):
         datamodel = model.datamodel
-        assert datamodel.filename == 'dummy.ini'
+        assert datamodel.filename == "dummy.ini"
         assert not datamodel.pagination_config.enabled
 
     def test_get_virtual_path(self, model, mocker):
         parent = mocker.sentinel.parent
-        assert model.get_virtual_path(parent) \
-            == VIRTUAL_PATH_PREFIX + '/test-index'
+        assert model.get_virtual_path(parent) == VIRTUAL_PATH_PREFIX + "/test-index"
 
     def test_match_path_pagination(self, model, mocker):
         source = mocker.sentinel.parent
-        assert model.match_path_pagination(source, ['page', '2']) is None
+        assert model.match_path_pagination(source, ["page", "2"]) is None
 
-    @pytest.mark.parametrize(('items', 'paths'), [
-        (None,
-         ['/blog/second-post', '/blog/first-post']),
-        ("this.children.filter(F._id == 'second-post')",
-         ['/blog/second-post']),
-        ])
+    @pytest.mark.parametrize(
+        ("items", "paths"),
+        [
+            (None, ["/blog/second-post", "/blog/first-post"]),
+            ("this.children.filter(F._id == 'second-post')", ["/blog/second-post"]),
+        ],
+    )
     def test_get_items(self, model, blog_record, paths):
-        assert [post.path for post in model.get_items(blog_record)] \
-            == paths
+        assert [post.path for post in model.get_items(blog_record)] == paths
 
 
 class TestIndexModel:
     @pytest.fixture
     def nchildren(self):
         return 1
 
     @pytest.fixture
     def source(self, nchildren, lektor_pad, lektor_alt):
         source = DummyPaginatable(nchildren=nchildren)
         source.pad, source.alt = lektor_pad, lektor_alt
-        source._id = 'source-id'
+        source._id = "source-id"
         return source
 
     @pytest.fixture
     def blog_post(self, lektor_pad, lektor_alt):
         blog_post = DummyPaginatable()
         blog_post.pad, blog_post.alt = lektor_pad, lektor_alt
         blog_post.pub_date = datetime.date(2020, 3, 21)
-        blog_post.tags = ['tag1', 'tag2']
-        blog_post.funky_tags = ['tag@1', 'täg2']
+        blog_post.tags = ["tag1", "tag2"]
+        blog_post.funky_tags = ["tag@1", "täg2"]
         return blog_post
 
     @pytest.fixture
     def key(self):
         return "item.tags"
 
     @pytest.fixture
@@ -146,167 +142,191 @@
         return None
 
     @pytest.fixture
     def fields(self):
         return None
 
     @pytest.fixture
-    def model(self, lektor_env, mocker,
-              key, template, slug_format, fields, pagination_config):
+    def model(
+        self, lektor_env, mocker, key, template, slug_format, fields, pagination_config
+    ):
         return IndexModel(
             lektor_env,
             key=key,
             template=template,
             slug_format=slug_format,
             fields=fields,
             pagination_config=pagination_config,
             subindex_model=mocker.sentinel.subindex_model,
-            config_filename='dummy.ini')
+            config_filename="dummy.ini",
+            index_name="test",
+        )
 
-    @pytest.mark.parametrize('template, expected', [
-        (None, 'index-pages.html'),
-        ('foo.html', 'foo.html'),
-        ])
+    @pytest.mark.parametrize(
+        "template, expected",
+        [
+            (None, "index-pages.html"),
+            ("foo.html", "foo.html"),
+        ],
+    )
     def test_template(self, model, expected):
         assert model.template == expected
 
     def test_datamodel(self, model, pagination_enabled):
         datamodel = model.datamodel
-        assert datamodel.filename == 'dummy.ini'
+        assert datamodel.filename == "dummy.ini"
         assert datamodel.pagination_config.enabled is bool(pagination_enabled)
 
-    @pytest.mark.parametrize(('parent_path', 'id_', 'page_num', 'expected'), [
-        ('foo', 'bar', None, "foo/bar"),
-        ('foo', 'bar', 42, "foo/bar/page/42"),
-        ])
-    def test_get_virtual_path(self, model,
-                              parent_path, id_, page_num, expected,
-                              mocker):
-        parent = mocker.Mock(name='parent', spec=(),
-                             virtual_path=parent_path,
-                             page_num=None)
+    @pytest.mark.parametrize(
+        ("parent_path", "id_", "page_num", "expected"),
+        [
+            ("foo", "bar", None, "foo/bar"),
+            ("foo", "bar", 42, "foo/bar/page/42"),
+        ],
+    )
+    def test_get_virtual_path(
+        self, model, parent_path, id_, page_num, expected, mocker
+    ):
+        parent = mocker.Mock(
+            name="parent", spec=(), virtual_path=parent_path, page_num=None
+        )
         assert model.get_virtual_path(parent, id_, page_num) == expected
 
     @pytest.mark.parametrize(
-        'pieces, pagination_enabled, nchildren, page_num', [
-            (['page', '1'], True, 10, 1),
-            (['page', '1', 'x'], True, 10, False),
-            (['PAGE', '1'], True, 10, False),
-            (['page', '1'], False, 10, False),
-            (['page', '0'], True, 10, False),
-            (['page', '2'], True, 10, False),  # only one page
-            (['page', '2'], True, 30, 2),
-            ]
-        )
+        "pieces, pagination_enabled, nchildren, page_num",
+        [
+            (["page", "1"], True, 10, 1),
+            (["page", "1", "x"], True, 10, False),
+            (["PAGE", "1"], True, 10, False),
+            (["page", "1"], False, 10, False),
+            (["page", "0"], True, 10, False),
+            (["page", "2"], True, 10, False),  # only one page
+            (["page", "2"], True, 30, 2),
+        ],
+    )
     def test_match_path_pagination(self, model, source, pieces, page_num):
         rv = model.match_path_pagination(source, pieces)
         if page_num is False:
             assert rv is None
         else:
             assert rv.page_num == page_num
             assert rv.record == source.record
 
-    @pytest.mark.parametrize('key, expected', [
-        ("item.tags", ['tag1', 'tag2']),
-        ("'{:04d}'.format(item.pub_date.year)", ['2020']),
-        ("item.funky_tags", ['tag_1', 'täg2']),
-        ])
+    @pytest.mark.parametrize(
+        "key, expected",
+        [
+            ("item.tags", ["tag1", "tag2"]),
+            ("'{:04d}'.format(item.pub_date.year)", ["2020"]),
+            ("item.funky_tags", ["tag_1", "täg2"]),
+        ],
+    )
     def test_keys_for_post(self, model, blog_post, expected):
         assert list(model.keys_for_post(blog_post)) == expected
 
-    @pytest.mark.parametrize('slug_format, expected', [
-        (None, 'source-id'),
-        ("'custom slug/%s'|format(this._id)", 'custom-slug/source-id'),
-        ])
+    @pytest.mark.parametrize(
+        "slug_format, expected",
+        [
+            (None, "source-id"),
+            ("'custom slug/%s'|format(this._id)", "custom-slug/source-id"),
+        ],
+    )
     def test_get_slug(self, model, source, expected):
         assert model.get_slug(source) == expected
 
-    @pytest.mark.parametrize('fields', [
-        [('id_upper', 'this._id.upper()')],
-        ])
+    @pytest.mark.parametrize(
+        "fields",
+        [
+            [("id_upper", "this._id.upper()")],
+        ],
+    )
     def test_data_descriptors(self, model, source):
         data = dict(model.data_descriptors)
-        assert data['id_upper'].__get__(source) == 'SOURCE-ID'
+        assert data["id_upper"].__get__(source) == "SOURCE-ID"
 
 
 class TestExpressionCompiler:
     @pytest.fixture
     def filename(self):
-        return 'config.ini'
+        return "config.ini"
 
     @pytest.fixture
     def section(self):
-        return 'some-section'
+        return "some-section"
 
     @pytest.fixture
     def compiler(self, lektor_env, filename, section):
         return ExpressionCompiler(lektor_env, filename, section)
 
-    @pytest.mark.parametrize('filename', ['config.ini', None])
-    @pytest.mark.parametrize('section', ['section', None])
+    @pytest.mark.parametrize("filename", ["config.ini", None])
+    @pytest.mark.parametrize("section", ["section", None])
     def test_location(self, compiler, filename, section):
         if filename:
-            expect = r'in .*\b%s\b' % re.escape(filename)
+            expect = r"in .*\b%s\b" % re.escape(filename)
             assert re.search(expect, compiler.location)
         if section:
-            expect = r'\[%s\]' % re.escape(section)
+            expect = r"\[%s\]" % re.escape(section)
             assert re.search(expect, compiler.location)
 
     def test_error_report(self, compiler):
-        with pytest.raises(RuntimeError,
-                           match=r'syntax error in config') as excinfo:
-            compiler('test', 'messed up')
-        assert 'messed up' in str(excinfo.value)
+        with pytest.raises(RuntimeError, match=r"syntax error in config") as excinfo:
+            compiler("test", "messed up")
+        assert "messed up" in str(excinfo.value)
 
     def test_call(self, compiler, blog_record):
-        desc = compiler('test', 'this.path')
+        desc = compiler("test", "this.path")
         assert desc.__get__(blog_record) == blog_record.path
 
 
 class IniReaderBase:
     @pytest.fixture
     def inifile(self, test_ini):
         inifile = IniFile(str(test_ini))
-        inifile.filename = '/dev/null'
+        inifile.filename = "/dev/null"
         return inifile
 
 
 class Test_index_models_from_ini(IniReaderBase):
-    @pytest.fixture(scope='session')
+    @pytest.fixture(scope="session")
     def test_ini(self, tmp_path_factory):
-        test_ini = tmp_path_factory.mktemp('imsfi') / 'test.ini'
-        test_ini.write_text(inspect.cleandoc('''
+        test_ini = tmp_path_factory.mktemp("imsfi") / "test.ini"
+        test_ini.write_text(
+            inspect.cleandoc(
+                """
         [index1]
         parent_path = /blog
         key = item.category
 
         [index2]
         key = item.tags
 
         [index3]
         template = tmpl.html
 
         [index4.subindex]
         key = item.tags
-        '''))
+        """
+            )
+        )
         return test_ini
 
     def test(self, lektor_env, inifile):
         models = index_models_from_ini(lektor_env, inifile)
-        assert list(map(attrgetter('parent_path', 'index_name'), models)) == [
-            ('/blog', 'index1'),
-            ('/', 'index2'),
-            ]
+        assert list(map(attrgetter("parent_path", "index_name"), models)) == [
+            ("/blog", "index1"),
+            ("/", "index2"),
+        ]
 
 
 class Test_index_model_from_ini(IniReaderBase):
-    @pytest.fixture(scope='session')
+    @pytest.fixture(scope="session")
     def test_ini(self, tmp_path_factory):
-        test_ini = tmp_path_factory.mktemp('imfi') / 'test.ini'
-        test_ini.write_text(inspect.cleandoc('''
+        test_ini = tmp_path_factory.mktemp("imfi") / "test.ini"
+        test_ini.write_text(
+            inspect.cleandoc(
+                """
         [index1]
         key = item.category
         template = tmpl.html
         subindex = subidx
         slug_format = "c-" ~ this.category
 
         [index1.fields]
@@ -314,89 +334,95 @@
 
         [index1.pagination]
         per_page = 3
 
         [index1.subidx]
         key = item.subcategory
         template = tmpl2.html
-        '''))
+        """
+            )
+        )
         return test_ini
 
     def test(self, lektor_env, inifile):
-        model = _index_model_from_ini(lektor_env, inifile, 'index1')
+        model = _index_model_from_ini(lektor_env, inifile, "index1")
         assert model.key_expr.expr == "item.category"
         assert model.template == "tmpl.html"
         assert model.slug_expr.expr == '"c-" ~ this.category'
         assert model.datamodel.pagination_config.per_page == 3
         assert len(model.data_descriptors) == 1
         assert model.data_descriptors[0][0] == "foo"
 
         assert model.subindex_model.key_expr.expr == "item.subcategory"
         assert model.subindex_model.template == "tmpl2.html"
 
     def test_key_required(self, lektor_env, inifile):
-        del inifile['index1.key']
+        del inifile["index1.key"]
         with pytest.raises(RuntimeError, match="key required"):
-            _index_model_from_ini(lektor_env, inifile, 'index1')
+            _index_model_from_ini(lektor_env, inifile, "index1")
 
 
 class Test_field_config_from_ini(IniReaderBase):
-    @pytest.fixture(scope='session')
+    @pytest.fixture(scope="session")
     def test_ini(self, tmp_path_factory):
-        test_ini = tmp_path_factory.mktemp('acfi') / 'test.ini'
-        test_ini.write_text(inspect.cleandoc('''
+        test_ini = tmp_path_factory.mktemp("acfi") / "test.ini"
+        test_ini.write_text(
+            inspect.cleandoc(
+                """
         [ind1.fields]
         foo = bar
 
         [ind2.fields.this-is-bad]
         foo = bar
-        '''))
+        """
+            )
+        )
         return test_ini
 
     def test(self, inifile):
-        assert _field_config_from_ini(inifile, 'ind1') == {
-            'foo': 'bar',
-            }
+        assert _field_config_from_ini(inifile, "ind1") == {
+            "foo": "bar",
+        }
 
     def test_raises_error(self, inifile):
-        with pytest.raises(RuntimeError,
-                           match=r'should not contain periods'):
-            _field_config_from_ini(inifile, 'ind2')
+        with pytest.raises(RuntimeError, match=r"should not contain periods"):
+            _field_config_from_ini(inifile, "ind2")
 
 
 class Test_pagination_from_ini(IniReaderBase):
-    @pytest.fixture(scope='session')
+    @pytest.fixture(scope="session")
     def test_ini(self, tmp_path_factory):
-        test_ini = tmp_path_factory.mktemp('pfi') / 'test.ini'
-        test_ini.write_text(inspect.cleandoc('''
+        test_ini = tmp_path_factory.mktemp("pfi") / "test.ini"
+        test_ini.write_text(
+            inspect.cleandoc(
+                """
         [pagination]
         per_page = 10
 
         [myindex.pagination]
         enabled = yes
 
         [myindex.subindex.pagination]
         per_page = 5
         url_suffix = pg
-        '''))
+        """
+            )
+        )
         return test_ini
 
     @pytest.fixture
     def pagination_config(self, lektor_env, inifile, index_name):
         return _pagination_config_from_ini(lektor_env, inifile, index_name)
 
-    @pytest.mark.parametrize('index_name, expected', [
-        ('',
-         {'enabled': False, 'per_page': 10, 'url_suffix': 'page'}),
-        ('otherindex',
-         {'enabled': False, 'per_page': 10, 'url_suffix': 'page'}),
-        ('myindex',
-         {'enabled': True, 'per_page': 10, 'url_suffix': 'page'}),
-        ('myindex.subindex',
-         {'enabled': True, 'per_page': 5, 'url_suffix': 'pg'}),
-        ('myindex.other',
-         {'enabled': True, 'per_page': 10, 'url_suffix': 'page'}),
-        ])
-    def test_subindex(self, pagination_config, expected,
-                      index_name, inifile):
+    @pytest.mark.parametrize(
+        "index_name, expected",
+        [
+            ("", {"enabled": False, "per_page": 10, "url_suffix": "page"}),
+            ("otherindex", {"enabled": False, "per_page": 10, "url_suffix": "page"}),
+            ("myindex", {"enabled": True, "per_page": 10, "url_suffix": "page"}),
+            ("myindex.subindex", {"enabled": True, "per_page": 5, "url_suffix": "pg"}),
+            ("myindex.other", {"enabled": True, "per_page": 10, "url_suffix": "page"}),
+        ],
+    )
+    def test_subindex(self, pagination_config, expected, index_name, inifile):
         for key, value in expected.items():
             assert getattr(pagination_config, key) == value
```

### Comparing `lektor-index-pages-1.0.0/tests/test_plugin.py` & `lektor_index_pages-1.1.0/tests/test_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import re
 
-import pytest
-
 import jinja2
+import pytest
 from lektor.db import Query
 from lektor.environment import PRIMARY_ALT
 
 from lektor_index_pages.indexmodel import VIRTUAL_PATH_PREFIX
-from lektor_index_pages.plugin import (
-    Cache,
-    IndexPages,
-    IndexPagesPlugin,
-    )
+from lektor_index_pages.plugin import Cache
+from lektor_index_pages.plugin import IndexPages
+from lektor_index_pages.plugin import IndexPagesPlugin
 from lektor_index_pages.sourceobj import IndexSource
 
 
 @pytest.fixture
 def record(lektor_pad, record_path):
     record = lektor_pad.get(record_path)
     assert record is not None
@@ -24,133 +21,136 @@
 
 class TestCache:
     @pytest.fixture
     def cache(self):
         return Cache()
 
     def test_get_or_create(self, cache, mocker):
-        creator = mocker.Mock(name='creator', spec=())
-        assert cache.get_or_create('key', creator) is creator.return_value
-        assert cache.get_or_create('key', creator) is creator.return_value
+        creator = mocker.Mock(name="creator", spec=())
+        assert cache.get_or_create("key", creator) is creator.return_value
+        assert cache.get_or_create("key", creator) is creator.return_value
         assert creator.mock_calls == [mocker.call()]
 
-        assert cache.get_or_create('other', creator) is creator.return_value
+        assert cache.get_or_create("other", creator) is creator.return_value
         assert creator.mock_calls == [mocker.call(), mocker.call()]
 
     def test_clear(self, cache, mocker):
-        creator = mocker.Mock(name='creator', spec=())
-        assert cache.get_or_create('key', creator) is creator.return_value
+        creator = mocker.Mock(name="creator", spec=())
+        assert cache.get_or_create("key", creator) is creator.return_value
         assert creator.mock_calls == [mocker.call()]
 
         cache.clear()
-        assert cache.get_or_create('key', creator) is creator.return_value
+        assert cache.get_or_create("key", creator) is creator.return_value
         assert creator.mock_calls == [mocker.call(), mocker.call()]
 
 
 class TestIndexPagesPlugin:
     @pytest.fixture
     def plugin(self, lektor_env, my_plugin_id):
         return IndexPagesPlugin(lektor_env, my_plugin_id)
 
     def test_config_caching(self, plugin):
         config = plugin.read_config()
         assert plugin.read_config() is config
 
-        plugin.on_before_build_all('builder')
+        plugin.on_before_build_all("builder")
         assert plugin.read_config() is not config
 
     @pytest.fixture
     def generate_index(self, plugin, lektor_env):
         plugin.on_setup_env()
         assert len(lektor_env.custom_generators) == 1
         return lektor_env.custom_generators[0]
 
-    @pytest.mark.parametrize("record_path, expected", [
-        ("/", []),
-        ("/blog", ['/blog@index-pages/year-index']),
-        ])
+    @pytest.mark.parametrize(
+        "record_path, expected",
+        [
+            ("/", []),
+            ("/blog", ["/blog@index-pages/year-index"]),
+        ],
+    )
     def test_generate_index(self, generate_index, record, expected):
         assert [idx.path for idx in generate_index(record)] == expected
 
     def test_skip_build(self, plugin, lektor_env):
-        plugin.on_setup_env(extra_flags={'index-pages': 'skip-build'})
+        plugin.on_setup_env(extra_flags={"index-pages": "skip-build"})
         assert len(lektor_env.custom_generators) == 0
 
     @pytest.fixture
     def resolve_virtual_path(self, plugin, lektor_env):
         plugin.on_setup_env()
         return lektor_env.virtual_sources[VIRTUAL_PATH_PREFIX]
 
     def test_resolve_virtual_path(self, resolve_virtual_path, blog_record):
-        index = resolve_virtual_path(blog_record, ['year-index', '2020'])
-        assert index.path == '/blog@index-pages/year-index/2020'
+        index = resolve_virtual_path(blog_record, ["year-index", "2020"])
+        assert index.path == "/blog@index-pages/year-index/2020"
 
     @pytest.fixture
     def resolve_url(self, plugin, lektor_env):
         plugin.on_setup_env()
         assert len(lektor_env.custom_url_resolvers) == 1
         return lektor_env.custom_url_resolvers[0]
 
     def test_resolve_url(self, resolve_url, blog_record):
-        index = resolve_url(blog_record, ['2020'])
-        assert index.path == '/blog@index-pages/year-index/2020'
+        index = resolve_url(blog_record, ["2020"])
+        assert index.path == "/blog@index-pages/year-index/2020"
 
     @pytest.fixture
     def jinja_env(self, lektor_env):
         return lektor_env.jinja_env
 
     @pytest.fixture
     def jinja_ctx(self, jinja_env, lektor_pad):
-        return jinja_env.from_string("").new_context({'site': lektor_pad})
+        return jinja_env.from_string("").new_context({"site": lektor_pad})
 
     @pytest.fixture
     def index_pages(self, plugin, jinja_env):
         plugin.on_setup_env()
-        return jinja_env.globals['index_pages']
+        return jinja_env.globals["index_pages"]
 
     def test_index_pages(self, index_pages, jinja_ctx):
-        rv = index_pages(jinja_ctx, 'year-index')
+        rv = index_pages(jinja_ctx, "year-index")
         assert isinstance(rv.indexes, Query)
 
     def test_index_pages_returns_undefined(self, index_pages, jinja_ctx):
-        rv = index_pages(jinja_ctx, 'missing-index')
+        rv = index_pages(jinja_ctx, "missing-index")
         assert jinja2.is_undefined(rv)
 
-    @pytest.mark.parametrize('lektor_pad', [jinja2.Undefined('undefined')])
+    @pytest.mark.parametrize("lektor_pad", [jinja2.Undefined("undefined")])
     def test_index_pages_missing_site(self, index_pages, jinja_ctx):
-        rv = index_pages(jinja_ctx, 'year-index')
+        rv = index_pages(jinja_ctx, "year-index")
         assert jinja2.is_undefined(rv)
 
 
 class TestIndexPages:
     @pytest.fixture
     def alt(self):
         return PRIMARY_ALT
 
     @pytest.fixture
     def index_root(self, config, lektor_pad, alt):
-        return config.get_index_root('year-index', lektor_pad, alt)
+        return config.get_index_root("year-index", lektor_pad, alt)
 
     @pytest.fixture
     def inst(self, index_root):
         return IndexPages(index_root)
 
     def test_indexes(self, inst):
         assert inst.indexes.count() > 0
 
     def test_iter(self, inst):
         first = next(iter(inst), None)
         assert isinstance(first, IndexSource)
-        assert first['year'] == 2020
+        assert first["year"] == 2020
 
     def test_bool(self, inst):
         assert inst
 
     def test_index_name(self, inst):
-        assert inst.index_name == 'year-index'
+        assert inst.index_name == "year-index"
 
     def test_alt(self, inst, alt):
         assert inst.alt == alt
 
-    @pytest.mark.parametrize('alt', [PRIMARY_ALT, 'xx'])
+    @pytest.mark.parametrize("alt", [PRIMARY_ALT, "xx"])
     def test_repr(self, inst):
         assert re.match(r"<index_pages\(u?'year-index'.*\)>", repr(inst))
```

### Comparing `lektor-index-pages-1.0.0/tests/test_sourceobj.py` & `lektor_index_pages-1.1.0/tests/test_sourceobj.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 import copy
 import datetime
 from operator import itemgetter
 
 import pytest
 from lektor.environment import PRIMARY_ALT
 
-from lektor_index_pages.indexmodel import (
-    VIRTUAL_PATH_PREFIX,
-    index_models_from_ini,
-    )
-from lektor_index_pages.sourceobj import (
-    IndexRoot,
-    IndexSource,
-    )
+from lektor_index_pages.indexmodel import index_models_from_ini
+from lektor_index_pages.indexmodel import VIRTUAL_PATH_PREFIX
+from lektor_index_pages.sourceobj import IndexRoot
+from lektor_index_pages.sourceobj import IndexSource
 
 
 @pytest.fixture
 def year_index_slug_format():
     return None
 
 
 @pytest.fixture
-def inifile(inifile, year_index_slug_format,
-            # XXX: not sure why I need to explicitly call these out
-            # They are used by our inherited inifile fixture
-            pagination_enabled, month_index_enabled):
+def inifile(
+    inifile,
+    year_index_slug_format,
+    # XXX: not sure why I need to explicitly call these out
+    # They are used by our inherited inifile fixture
+    pagination_enabled,
+    month_index_enabled,
+):
     if year_index_slug_format is not None:
-        inifile['year-index.slug_format'] = year_index_slug_format
+        inifile["year-index.slug_format"] = year_index_slug_format
     return inifile
 
 
 @pytest.fixture
 def index_root_model(lektor_env, inifile):
-    for model in index_models_from_ini(lektor_env, inifile):
-        break
-    assert model.parent_path == '/blog'
-    assert model.index_name == 'year-index'
+    model = next(iter(index_models_from_ini(lektor_env, inifile)))
+    assert model.parent_path == "/blog"
+    assert model.index_name == "year-index"
     return model
 
 
 @pytest.fixture
 def year_index_model(index_root_model):
     return index_root_model.subindex_model
 
@@ -58,240 +57,259 @@
 
 
 @pytest.fixture
 def year_index(index_root):
     return index_root.subindexes.first()
 
 
-@pytest.fixture(params=['index_root', 'year_index'])
+@pytest.fixture(params=["index_root", "year_index"])
 def index(request, lektor_alt):
     return request.getfixturevalue(request.param)
 
 
-@pytest.mark.usefixtures('plugin')
+@pytest.mark.usefixtures("plugin")
 class TestIndexSource:
     # FIXME: these tests should be reorganized
 
     def test_get_index_root(self, index_root_model, blog_record):
         index_root = IndexRoot.get_index(index_root_model, blog_record)
-        assert index_root.path == '/blog@index-pages/year-index'
+        assert index_root.path == "/blog@index-pages/year-index"
 
         reget = IndexRoot.get_index(index_root_model, blog_record)
         # should return cached value
         assert reget is index_root
 
-    @pytest.mark.parametrize('page_num', [None, 1, 2])
+    @pytest.mark.parametrize("page_num", [None, 1, 2])
     def test_get_index(self, year_index_model, index_root, page_num):
-        id_ = '2020'
+        id_ = "2020"
         children = index_root.children
         year_index = IndexSource.get_index(
-            year_index_model, index_root, id_, children, page_num)
+            year_index_model, index_root, id_, children, page_num
+        )
         assert year_index.page_num == page_num
 
         reget = IndexSource.get_index(
-            year_index_model, index_root, id_, children, page_num)
+            year_index_model, index_root, id_, children, page_num
+        )
         # should return cached value
         assert reget is year_index
 
     def test_parent(self, year_index, index_root):
         assert year_index.parent == index_root
 
     def test_slug(self, index_root, year_index):
         # FIXME: this should be split up
         assert index_root._slug is None
-        assert year_index._slug == '2020'
+        assert year_index._slug == "2020"
 
-    @pytest.mark.parametrize('name, expected', [
-        ('_hidden', True),
-        ('_model', False),      # Undefined
-        ])
+    @pytest.mark.parametrize(
+        "name, expected",
+        [
+            ("_hidden", True),
+            ("_model", False),  # Undefined
+        ],
+    )
     def test_contains(self, year_index, name, expected):
         assert (name in year_index) is expected
 
     def test_getitem(self, year_index):
-        assert year_index['_id'] == '2020'
+        assert year_index["_id"] == "2020"
 
     def test_getitem_with_descriptor(self, year_index):
-        assert year_index['_gid'] == year_index._gid
+        assert year_index["_gid"] == year_index._gid
 
     def test_children(self, index_root, blog_record):
         assert list(index_root.children) == list(blog_record.children)
 
     def test_pagination(self, year_index, blog_record, pagination_enabled):
         if pagination_enabled:
             assert year_index.pagination.total == blog_record.children.count()
         else:
             with pytest.raises(RuntimeError):
                 year_index.pagination
 
     def test_subindexes(self, index, index_root):
         if index is index_root:
-            assert list(map(itemgetter('_id'), index.subindexes)) == ['2020']
+            assert list(map(itemgetter("_id"), index.subindexes)) == ["2020"]
         else:
-            assert not hasattr(index, 'subindexes')
+            assert not hasattr(index, "subindexes")
 
     def test__subindex_ids(self, index_root):
-        assert index_root._subindex_ids == ('2020',)
+        assert index_root._subindex_ids == ("2020",)
+
+    def test__subindex_ids_missing_if_no_subindex(self, year_index):
+        assert not hasattr(year_index, "_subindex_ids")
 
     def test_path(self, index_root):
         assert index_root.path == "/blog@%s/year-index" % VIRTUAL_PATH_PREFIX
 
     def test__gid(self, index_root):
         # md5("/blog@index-pages/year-index")
         assert index_root._gid == "7797910bec275f5dd5e07c6eefb4be4d"
 
-    @pytest.mark.parametrize("year_index_slug_format, expected", [
-        (None, "/blog/2020/"),
-        ("this._id ~ '-html'", "/blog/2020-html/"),
-        ("'{}.html'.format(this._id)", "/blog/2020.html"),
-        ])
+    @pytest.mark.parametrize(
+        "year_index_slug_format, expected",
+        [
+            (None, "/blog/2020/"),
+            ("this._id ~ '-html'", "/blog/2020-html/"),
+            ("'{}.html'.format(this._id)", "/blog/2020.html"),
+        ],
+    )
     def test_url_path(self, year_index, expected):
         assert year_index.url_path == expected
 
-    @pytest.mark.parametrize('pagination_enabled', [True])
+    @pytest.mark.parametrize("pagination_enabled", [True])
     def test_url_path_paginated(self, year_index):
         assert year_index.__for_page__(2).url_path == "/blog/2020/page/2/"
 
-    @pytest.mark.parametrize("path, should_resolve", [
-        ('', 'root'),
-        ('199', False),
-        ('2020', 'year'),
-        ('2020/page', False),
-        ('2020/page/1', 'year-with-page'),
-        ('2020/page/2', False),  # page must be non-empty
-        ('2020/page/1/1', False),
-        ('2020/3', False),
-        ('2020/03', 'month'),
-        ('2019/03', False),
-        ('2020/04/page', False),
-        ('2020/04/page/1', 'month-with-page'),
-        ('2020/05/page/1', False),
-        ('2020/04/page/1/x', False),
-        ])
-    @pytest.mark.parametrize('pagination_enabled', [True, False])
-    @pytest.mark.parametrize('month_index_enabled', [True, False])
-    def test_resolve_virtual_path(self, index_root, path, should_resolve,
-                                  pagination_enabled,
-                                  month_index_enabled):
+    @pytest.mark.parametrize(
+        "path, should_resolve",
+        [
+            ("", "root"),
+            ("199", False),
+            ("2020", "year"),
+            ("2020/page", False),
+            ("2020/page/1", "year-with-page"),
+            ("2020/page/2", False),  # page must be non-empty
+            ("2020/page/1/1", False),
+            ("2020/3", False),
+            ("2020/03", "month"),
+            ("2019/03", False),
+            ("2020/04/page", False),
+            ("2020/04/page/1", "month-with-page"),
+            ("2020/05/page/1", False),
+            ("2020/04/page/1/x", False),
+        ],
+    )
+    @pytest.mark.parametrize("pagination_enabled", [True, False])
+    @pytest.mark.parametrize("month_index_enabled", [True, False])
+    def test_resolve_virtual_path(
+        self, index_root, path, should_resolve, pagination_enabled, month_index_enabled
+    ):
         if should_resolve:
-            flags = should_resolve.split('-')
-            if 'month' in flags and not month_index_enabled:
+            flags = should_resolve.split("-")
+            if "month" in flags and not month_index_enabled:
                 should_resolve = False
-            if 'page' in flags and not pagination_enabled:
+            if "page" in flags and not pagination_enabled:
                 should_resolve = False
 
-        pieces = path.split('/') if path else []
+        pieces = path.split("/") if path else []
         source = index_root.resolve_virtual_path(pieces)
 
         if should_resolve:
-            expected_path = '/'.join(['/blog@index-pages/year-index'] + pieces)
+            expected_path = "/".join(["/blog@index-pages/year-index"] + pieces)
             assert source.path == expected_path
         else:
             assert source is None
 
     @pytest.mark.parametrize(
-        'pagination_enabled, url_path, index_type, path', [
-            (False, '', 'root',
-             '/blog@index-pages/year-index'),
-            (False, 'x', None, None),
-            (False, '2020', 'year',
-             '/blog@index-pages/year-index/2020'),
-            (1, '2020', 'year',
-             '/blog@index-pages/year-index/2020/page/1'),
-            (1, '2020/page', None, None),
-            (1, '2020/page/1', None, None),
-            (1, '2020/page/2', 'year',
-             '/blog@index-pages/year-index/2020/page/2'),
-            (1, '2020/page/3', None, None),
-            (False, '2020/04', 'month',
-             '/blog@index-pages/year-index/2020/04'),
-            (False, '2020/13', None, None),
-            (True, '2020/03', 'month',
-             '/blog@index-pages/year-index/2020/03/page/1'),
-            (False, '2020/02/x', None, None),
-            ])
-    @pytest.mark.parametrize('month_index_enabled', [True, False])
-    def test_resolve_url_path(self, index_root,
-                              url_path, index_type, path,
-                              month_index_enabled):
-        url_path = url_path.split('/') if url_path else []
+        "pagination_enabled, url_path, index_type, path",
+        [
+            (False, "", "root", "/blog@index-pages/year-index"),
+            (False, "x", None, None),
+            (False, "2020", "year", "/blog@index-pages/year-index/2020"),
+            (1, "2020", "year", "/blog@index-pages/year-index/2020/page/1"),
+            (1, "2020/page", None, None),
+            (1, "2020/page/1", None, None),
+            (1, "2020/page/2", "year", "/blog@index-pages/year-index/2020/page/2"),
+            (1, "2020/page/3", None, None),
+            (False, "2020/04", "month", "/blog@index-pages/year-index/2020/04"),
+            (False, "2020/13", None, None),
+            (True, "2020/03", "month", "/blog@index-pages/year-index/2020/03/page/1"),
+            (False, "2020/02/x", None, None),
+        ],
+    )
+    @pytest.mark.parametrize("month_index_enabled", [True, False])
+    def test_resolve_url_path(
+        self, index_root, url_path, index_type, path, month_index_enabled
+    ):
+        url_path = url_path.split("/") if url_path else []
 
         should_resolve = bool(index_type)
-        if not month_index_enabled and index_type == 'month':
+        if not month_index_enabled and index_type == "month":
             should_resolve = False
 
         source = index_root.resolve_url_path(url_path)
 
         if should_resolve:
             assert source.path == path
         else:
             assert source is None
 
-    @pytest.mark.parametrize('page_num', [None, 1, 2])
+    @pytest.mark.parametrize("page_num", [None, 1, 2])
     def test_for_page(self, year_index, page_num):
         paginated = year_index.__for_page__(page_num)
         assert paginated.page_num == page_num
 
-    @pytest.mark.parametrize('month_index_enabled', [True])
+    def test__get_subindex_raises_if_no_subindex(self, year_index):
+        with pytest.raises(LookupError):
+            year_index._get_subindex("1")
+
+    @pytest.mark.parametrize("month_index_enabled", [True])
     def test_get_checksum(self, index):
-        assert index.get_checksum('ignored') \
-            == index._compute_checksum(index._get_checksum_data('ignored'))
+        assert index.get_checksum("ignored") == index._compute_checksum(
+            index._get_checksum_data("ignored")
+        )
 
     def test_get_checksum_data(self, index_root):
-        assert index_root._get_checksum_data('ignored') == (
-            '/blog@index-pages/year-index',
-            ['/blog/second-post', '/blog/first-post'],
-            ('2020',),
-            )
+        assert index_root._get_checksum_data("ignored") == (
+            "/blog@index-pages/year-index",
+            ("/blog/second-post", "/blog/first-post"),
+            ("2020",),
+        )
 
-    @pytest.mark.parametrize('pagination_enabled', [True])
-    @pytest.mark.parametrize('month_index_enabled', [True])
+    @pytest.mark.parametrize("pagination_enabled", [True])
+    @pytest.mark.parametrize("month_index_enabled", [True])
     def test_get_checksum_data_paginated(self, year_index):
-        assert year_index._get_checksum_data('ignored') == (
-            '/blog@index-pages/year-index/2020',
+        assert year_index._get_checksum_data("ignored") == (
+            "/blog@index-pages/year-index/2020",
             "NPAGES=1",
-            ('04', '03'),
-            )
-        assert year_index.__for_page__(1)._get_checksum_data('ignored') == (
-            '/blog@index-pages/year-index/2020/page/1',
-            ['/blog/second-post', '/blog/first-post'],
-            ('04', '03'),
-            )
+            ("04", "03"),
+        )
+        assert year_index.__for_page__(1)._get_checksum_data("ignored") == (
+            "/blog@index-pages/year-index/2020/page/1",
+            ("/blog/second-post", "/blog/first-post"),
+            ("04", "03"),
+        )
 
     def test_get_checksum_data_no_subindexes(self, year_index):
-        assert year_index._get_checksum_data('ignored') == (
-            '/blog@index-pages/year-index/2020',
-            ['/blog/second-post', '/blog/first-post'],
-            )
-
-    @pytest.mark.parametrize('data, checksum', [
-        (("path", ["c1"], ("id")),
-         "e2df3e68cc1a7573ec975aad5b2eb17e1d445165"),
-        ])
+        assert year_index._get_checksum_data("ignored") == (
+            "/blog@index-pages/year-index/2020",
+            ("/blog/second-post", "/blog/first-post"),
+        )
+
+    @pytest.mark.parametrize(
+        "data, checksum",
+        [
+            (("path", ["c1"], ("id")), "e2df3e68cc1a7573ec975aad5b2eb17e1d445165"),
+        ],
+    )
     def test_compute_checksum(self, data, checksum):
         assert IndexSource._compute_checksum(data) == checksum
 
-    @pytest.mark.parametrize('blog_is_hidden', [True, False])
+    @pytest.mark.parametrize("blog_is_hidden", [True, False])
     def test_is_hidden(self, year_index, blog_is_hidden, blog_record):
         if blog_is_hidden:
-            blog_record._data['_hidden'] = True
+            blog_record._data["_hidden"] = True
         assert year_index.is_hidden is blog_is_hidden
 
-    @pytest.mark.parametrize('blog_is_hidden', [True, False])
-    def test_index_root_is_hidden(self, index_root, blog_is_hidden,
-                                  blog_record):
+    @pytest.mark.parametrize("blog_is_hidden", [True, False])
+    def test_index_root_is_hidden(self, index_root, blog_is_hidden, blog_record):
         if blog_is_hidden:
-            blog_record._data['_hidden'] = True
+            blog_record._data["_hidden"] = True
         assert index_root.is_hidden
 
-    @pytest.mark.parametrize("fields, expect_reverse", [
-        (['date', 'non-existing'], False),
-        (['-date', 'non-existing'], True),
-        (['+date', 'non-existing'], False),
-        ])
+    @pytest.mark.parametrize(
+        "fields, expect_reverse",
+        [
+            (["date", "non-existing"], False),
+            (["-date", "non-existing"], True),
+            (["+date", "non-existing"], False),
+        ],
+    )
     def test_get_sort_key(self, year_index, fields, expect_reverse):
         sort_key = year_index.get_sort_key(fields)
         assert len(sort_key) == 2
         assert sort_key[0].value == datetime.date(2020, 1, 1)
         assert sort_key[0].reverse == expect_reverse
         assert sort_key[1].value is None
 
@@ -308,18 +326,24 @@
 
     def test_ne_other(self, year_index):
         other = year_index.__for_page__(1)
         assert year_index != other
         assert not (year_index == other)
         assert hash(year_index) != hash(other)
 
+    def test_ne_non_index(self, index, blog_record):
+        assert index != blog_record
+
     def test_repr(self, year_index):
-        assert repr(year_index) == \
-            "<IndexSource path='/blog@index-pages/year-index/2020'>"
+        assert (
+            repr(year_index) == "<IndexSource path='/blog@index-pages/year-index/2020'>"
+        )
 
     def test_repr_with_page_num(self, year_index):
-        assert repr(year_index.__for_page__(2)) == \
-            "<IndexSource path='/blog@index-pages/year-index/2020' page_num=2>"
+        assert (
+            repr(year_index.__for_page__(2))
+            == "<IndexSource path='/blog@index-pages/year-index/2020' page_num=2>"
+        )
 
-    @pytest.mark.parametrize('lektor_alt', ['xx'])
+    @pytest.mark.parametrize("lektor_alt", ["xx"])
     def test_repr_with_alt(self, index):
         assert repr(index).endswith(" alt='xx'>")
```

### Comparing `lektor-index-pages-1.0.0/tox.ini` & `lektor_index_pages-1.1.0/tox.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,70 @@
 [tox]
-minversion = 3.3
-envlist = {py37,py38,py39,py310}{,-lektor32},lint,docs
+minversion = 4
+envlist =
+    {py37,py38,py39,py310,py311}{,-lektor_pre}
+    cover-{clean,report}
+    lint
+    docs
 isolated_build = true
 
 [gh-actions]
 python =
     3.7: py37
     3.8: py38
     3.9: py39
-    3.10: py310, lint, docs
+    3.10: py310
+    3.11: py311, lint, docs
 
 [testenv]
 deps =
+    coverage[toml]
     pytest
     pytest-mock
     lektor
-    pytest-cov
-setenv =
-    # Prevent parallel pytest-cov runs from clobbering each others
-    # .coverage file
-    COVERAGE_FILE = .coverage.{envname}
+    lektor_pre: lektor>=3.4a0
 commands =
-    pytest --cov=lektor_index_pages {posargs: --cov-fail-under=100 tests}
+    coverage run -m pytest {posargs: tests -ra}
+depends =
+    {py37,py38,py39,py310,py311}: cover-clean
+    cover-report: {py37,py38,py39,py310,py311}{,-lektor_pre}
+
+[testenv:cover-clean]
+deps = coverage[toml]
+skip_install = true
+commands = coverage erase
+
+[testenv:cover-report]
+deps = coverage[toml]
+skip_install = true
+commands =
+    -coverage combine --append
+    coverage html
+    coverage report --fail-under=100 --show-missing
 
 [testenv:lint]
 skip_install = True
 deps =
     build
-    flake8
     twine
-    check-manifest
 commands =
     python -m build --outdir {envtmpdir}/dist {toxinidir}
     twine check {envtmpdir}/dist/*
-    flake8
-    check-manifest
 
 [testenv:docs]
 skip_install = True
 recreate = True
 deps =
     -r {toxinidir}/docs/requirements.txt
 commands =
     sphinx-build -n -b html {toxinidir}/docs {envtmpdir}/html_docs
 
-[pytest]
-addopts =
-    --cov-report=term-missing --cov-report=html
-
 [flake8]
+max-line-length = 88
+extend-ignore = E203
 exclude =
     .tox,
     .git,
     __pycache__,
     .eggs,
     # excludes other virtualenv lib and bin directories
     python*.*, bin
```

