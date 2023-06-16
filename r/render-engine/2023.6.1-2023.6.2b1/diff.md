# Comparing `tmp/render_engine-2023.6.1.tar.gz` & `tmp/render_engine-2023.6.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine-2023.6.1.tar", last modified: Fri Jun  2 06:02:09 2023, max compression
+gzip compressed data, was "render_engine-2023.6.2b1.tar", last modified: Fri Jun 16 05:36:59 2023, max compression
```

## Comparing `render_engine-2023.6.1.tar` & `render_engine-2023.6.2b1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.176831 render_engine-2023.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.164831 render_engine-2023.6.1/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.164831 render_engine-2023.6.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.devcontainer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.164831 render_engine-2023.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/CONTRIBUTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.164831 render_engine-2023.6.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.164831 render_engine-2023.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.164831 render_engine-2023.6.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 06:01:54.000000 render_engine-2023.6.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-02 06:01:54.000000 render_engine-2023.6.1/Contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-02 06:02:09.176831 render_engine-2023.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-02 06:01:54.000000 render_engine-2023.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-06-02 06:01:54.000000 render_engine-2023.6.1/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.168831 render_engine-2023.6.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.168831 render_engine-2023.6.1/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.168831 render_engine-2023.6.1/docs/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/assets/create-app-help.png
--rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/assets/render-engine-init-help.png
--rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/assets/render-engine-init.png
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/collection.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.168831 render_engine-2023.6.1/docs/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/contributing/pages.md
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/custom_collections.md
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/feeds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.168831 render_engine-2023.6.1/docs/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/getting-started/building-your-site.md
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/getting-started/creating-a-collection.md
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/getting-started/creating-a-page.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/getting-started/creating-your-app.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/getting-started/layout.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/hookspecs.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/page.md
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/parsers.md
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/site.md
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/docs/templates.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 06:01:54.000000 render_engine-2023.6.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-02 06:01:54.000000 render_engine-2023.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-02 06:01:54.000000 render_engine-2023.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 06:02:09.176831 render_engine-2023.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.168831 render_engine-2023.6.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.172831 render_engine-2023.6.1/src/render_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.172831 render_engine-2023.6.1/src/render_engine/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/README_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/base_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.172831 render_engine-2023.6.1/src/render_engine/parsers/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/parsers/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.172831 render_engine-2023.6.1/src/render_engine/render_engine_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/base_collection_path.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/create_app_py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/rss2.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/rss2.0_items.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/sitemap.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/render_engine_templates/sitemap_item.xml
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-02 06:01:54.000000 render_engine-2023.6.1/src/render_engine/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.172831 render_engine-2023.6.1/src/render_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-02 06:02:09.000000 render_engine-2023.6.1/src/render_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-02 06:02:09.000000 render_engine-2023.6.1/src/render_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:02:09.000000 render_engine-2023.6.1/src/render_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-02 06:02:09.000000 render_engine-2023.6.1/src/render_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-02 06:02:09.000000 render_engine-2023.6.1/src/render_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 06:02:09.000000 render_engine-2023.6.1/src/render_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.176831 render_engine-2023.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/create_app_check_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/create_app_check_file_no_site_vars.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.176831 render_engine-2023.6.1/tests/site_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.176831 render_engine-2023.6.1/tests/site_test/blog/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/site_test/blog/test_blog_content.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/site_test/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:02:09.176831 render_engine-2023.6.1/tests/site_test/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/site_test/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_parser_markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-06-02 06:01:54.000000 render_engine-2023.6.1/tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.657572 render_engine-2023.6.2b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.645572 render_engine-2023.6.2b1/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.645572 render_engine-2023.6.2b1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.devcontainer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.649572 render_engine-2023.6.2b1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.github/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.github/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.649572 render_engine-2023.6.2b1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.649572 render_engine-2023.6.2b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.649572 render_engine-2023.6.2b1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/Contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-16 05:36:59.657572 render_engine-2023.6.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.649572 render_engine-2023.6.2b1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.649572 render_engine-2023.6.2b1/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.649572 render_engine-2023.6.2b1/docs/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/assets/create-app-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/assets/render-engine-init-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/assets/render-engine-init.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/collection.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.649572 render_engine-2023.6.2b1/docs/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/contributing/pages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/custom_collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/feeds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.653571 render_engine-2023.6.2b1/docs/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/getting-started/building-your-site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/getting-started/creating-a-collection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/getting-started/creating-a-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/getting-started/creating-your-app.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/getting-started/layout.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/hookspecs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/docs/templates.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 05:36:59.657572 render_engine-2023.6.2b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.653571 render_engine-2023.6.2b1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.653571 render_engine-2023.6.2b1/src/render_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.653571 render_engine-2023.6.2b1/src/render_engine/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/parsers/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/parsers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/parsers/README_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/parsers/base_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.653571 render_engine-2023.6.2b1/src/render_engine/parsers/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/parsers/markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/parsers/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.657572 render_engine-2023.6.2b1/src/render_engine/render_engine_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/render_engine_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/render_engine_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/render_engine_templates/base_collection_path.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/render_engine_templates/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/render_engine_templates/create_app_py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/render_engine_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/render_engine_templates/rss2.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/render_engine_templates/rss2.0_items.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/render_engine_templates/sitemap.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/render_engine_templates/sitemap_item.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/src/render_engine/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.653571 render_engine-2023.6.2b1/src/render_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-16 05:36:59.000000 render_engine-2023.6.2b1/src/render_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-16 05:36:59.000000 render_engine-2023.6.2b1/src/render_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 05:36:59.000000 render_engine-2023.6.2b1/src/render_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-16 05:36:59.000000 render_engine-2023.6.2b1/src/render_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 05:36:59.000000 render_engine-2023.6.2b1/src/render_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 05:36:59.000000 render_engine-2023.6.2b1/src/render_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.657572 render_engine-2023.6.2b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/create_app_check_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/create_app_check_file_no_site_vars.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.657572 render_engine-2023.6.2b1/tests/site_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.657572 render_engine-2023.6.2b1/tests/site_test/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/site_test/blog/test_blog_content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/site_test/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:36:59.657572 render_engine-2023.6.2b1/tests/site_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/site_test/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/test_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/test_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/test_blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/test_create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/test_parser_markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-06-16 05:36:45.000000 render_engine-2023.6.2b1/tests/test_site.py
```

### Comparing `render_engine-2023.6.1/.chglog/CHANGELOG.tpl.md` & `render_engine-2023.6.2b1/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/.devcontainer/devcontainer.json` & `render_engine-2023.6.2b1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/.github/CODE_OF_CONDUCT.md` & `render_engine-2023.6.2b1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/.github/CONTRIBUTION.md` & `render_engine-2023.6.2b1/.github/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/.github/FUNDING.yml` & `render_engine-2023.6.2b1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/.github/LICENSE` & `render_engine-2023.6.2b1/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/.github/dependabot.yml` & `render_engine-2023.6.2b1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/.github/workflows/publish.yml` & `render_engine-2023.6.2b1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/.gitignore` & `render_engine-2023.6.2b1/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/PKG-INFO` & `render_engine-2023.6.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_engine
-Version: 2023.6.1
+Version: 2023.6.2b1
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.6.1/README.md` & `render_engine-2023.6.2b1/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/changelog.md` & `render_engine-2023.6.2b1/changelog.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/archive.md` & `render_engine-2023.6.2b1/docs/docs/archive.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/assets/create-app-help.png` & `render_engine-2023.6.2b1/docs/docs/assets/create-app-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/assets/render-engine-init-help.png` & `render_engine-2023.6.2b1/docs/docs/assets/render-engine-init-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/assets/render-engine-init.png` & `render_engine-2023.6.2b1/docs/docs/assets/render-engine-init.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/cli.md` & `render_engine-2023.6.2b1/docs/docs/cli.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/contributing/pages.md` & `render_engine-2023.6.2b1/docs/docs/contributing/pages.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/custom_collections.md` & `render_engine-2023.6.2b1/docs/docs/custom_collections.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/getting-started/building-your-site.md` & `render_engine-2023.6.2b1/docs/docs/getting-started/building-your-site.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/getting-started/creating-a-collection.md` & `render_engine-2023.6.2b1/docs/docs/getting-started/creating-a-collection.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/getting-started/creating-a-page.md` & `render_engine-2023.6.2b1/docs/docs/getting-started/creating-a-page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/getting-started/installation.md` & `render_engine-2023.6.2b1/docs/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/getting-started/layout.md` & `render_engine-2023.6.2b1/docs/docs/getting-started/layout.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/index.md` & `render_engine-2023.6.2b1/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/page.md` & `render_engine-2023.6.2b1/docs/docs/page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/parsers.md` & `render_engine-2023.6.2b1/docs/docs/parsers.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/docs/templates.md` & `render_engine-2023.6.2b1/docs/docs/templates.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/docs/mkdocs.yml` & `render_engine-2023.6.2b1/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/pyproject.toml` & `render_engine-2023.6.2b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/requirements.txt` & `render_engine-2023.6.2b1/requirements.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/.DS_Store` & `render_engine-2023.6.2b1/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/.DS_Store` & `render_engine-2023.6.2b1/src/render_engine/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/_base_object.py` & `render_engine-2023.6.2b1/src/render_engine/_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/archive.py` & `render_engine-2023.6.2b1/src/render_engine/archive.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/blog.py` & `render_engine-2023.6.2b1/src/render_engine/blog.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/cli.py` & `render_engine-2023.6.2b1/src/render_engine/cli.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/collection.py` & `render_engine-2023.6.2b1/src/render_engine/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         self.has_archive = any(
             [
                 hasattr(self, "archive_template"),
                 getattr(self, "items_per_page", None),
             ]
         )
         self.title = self._title
-
+        
     def iter_content_path(self):
         """Iterate through in the collection's content path."""
 
         return flatten(
             [
                 pathlib.Path(self.content_path).glob(suffix)
                 for suffix in self.include_suffixes
@@ -163,15 +163,15 @@
                 title=self._title,
                 routes=self.routes,
                 archive_index=index,
                 num_archive_pages=num_archive_pages,
             )
 
     @property
-    def _feed(self):
+    def feed(self):
         feed = self.Feed()
         feed.pages = [page for page in self]
         feed.title = getattr(self, "feed_title", self._title)
         feed.slug = self._slug
         feed.Parser = self.PageParser
         return feed
```

### Comparing `render_engine-2023.6.1/src/render_engine/engine.py` & `render_engine-2023.6.2b1/src/render_engine/engine.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 engine = Environment(
     loader=render_engine_templates_loader,
     autoescape=select_autoescape(["xml"]),
     lstrip_blocks=True,
     trim_blocks=True,
 )
 
-
 def to_pub_date(value: datetime):
     """
     Parse information from the given class object.
     """
     return utils.format_datetime(value)
 engine.filters["to_pub_date"] = to_pub_date
 
@@ -49,14 +48,21 @@
 @pass_environment
 def to_absolute(env: Environment, url:str) -> str:
     return urllib.parse.urljoin(env.globals.get('SITE_URL'), url)
 engine.filters["to_absolute"] = to_absolute
 
 
 @pass_environment
+def feed_url(env: Environment, value: str) -> str:
+    """Returns the URL for the collections feed"""
+    routes = env.globals.get("routes")
+    return routes[value].feed.url_for()
+engine.filters["feed_url"] = feed_url
+
+@pass_environment
 def url_for(env: Environment, value: str, page: int=0) -> str:
     """Look for the route in the route_list and return the url for the page."""
     routes = env.globals.get("routes")
     route = value.split(".", maxsplit=1)
 
     if len(route) == 2 and type(route) == list:
         collection, route = route
```

### Comparing `render_engine-2023.6.1/src/render_engine/feeds.py` & `render_engine-2023.6.2b1/src/render_engine/feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/hookspecs.py` & `render_engine-2023.6.2b1/src/render_engine/hookspecs.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/links.py` & `render_engine-2023.6.2b1/src/render_engine/links.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/page.py` & `render_engine-2023.6.2b1/src/render_engine/page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/parsers/.DS_Store` & `render_engine-2023.6.2b1/src/render_engine/parsers/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/parsers/README_TEMPLATE.md` & `render_engine-2023.6.2b1/src/render_engine/parsers/README_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/parsers/base_parsers.py` & `render_engine-2023.6.2b1/src/render_engine/parsers/base_parsers.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/parsers/markdown/README.md` & `render_engine-2023.6.2b1/src/render_engine/parsers/markdown/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/plugins.py` & `render_engine-2023.6.2b1/src/render_engine/plugins.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/render_engine_templates/create_app_py.txt` & `render_engine-2023.6.2b1/src/render_engine/render_engine_templates/create_app_py.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/render_engine_templates/index.html` & `render_engine-2023.6.2b1/src/render_engine/render_engine_templates/index.html`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/render_engine_templates/rss2.0.xml` & `render_engine-2023.6.2b1/src/render_engine/render_engine_templates/rss2.0.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/render_engine_templates/rss2.0_items.xml` & `render_engine-2023.6.2b1/src/render_engine/render_engine_templates/rss2.0_items.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/src/render_engine/site.py` & `render_engine-2023.6.2b1/src/render_engine/site.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         if collection.has_archive:
             for archive in collection.archives:
                 logging.debug("Adding Archive: %s", archive.__class__.__name__)
 
                 self._render_output(collection.routes[0], archive)
 
         if hasattr(collection, "Feed"):
-            self._render_output("./", collection._feed)
+            self._render_output("./", collection.feed)
 
     def _render_full_collection(self, collection: Collection) -> None:
         """Iterate through Pages and Check for Collections and Feeds"""
 
         for entry in collection:
             entry._pm.hook.render_content(Page=entry)
             for route in collection.routes:
@@ -167,15 +167,15 @@
             for archive in collection.archives:
                 logging.debug("Adding Archive: %s", archive.__class__.__name__)
 
                 for route in collection.routes:
                     self._render_output(collection.routes[0], archive)
 
         if hasattr(collection, "Feed"):
-            self._render_output("./", collection._feed)
+            self._render_output("./", collection.feed)
 
     def render(self) -> None:
         """
         Render all pages and collections.
 
         These are pages and collections that have been added to the site using 
         the [`Site.page`][src.render_engine.Site.page]
```

### Comparing `render_engine-2023.6.1/src/render_engine.egg-info/PKG-INFO` & `render_engine-2023.6.2b1/src/render_engine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-engine
-Version: 2023.6.1
+Version: 2023.6.2b1
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.6.1/src/render_engine.egg-info/SOURCES.txt` & `render_engine-2023.6.2b1/src/render_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/tests/conftest.py` & `render_engine-2023.6.2b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/tests/create_app_check_file.txt` & `render_engine-2023.6.2b1/tests/create_app_check_file.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/tests/test_base_object.py` & `render_engine-2023.6.2b1/tests/test_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/tests/test_base_parser.py` & `render_engine-2023.6.2b1/tests/test_base_parser.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/tests/test_collections.py` & `render_engine-2023.6.2b1/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/tests/test_create_app.py` & `render_engine-2023.6.2b1/tests/test_create_app.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/tests/test_feeds.py` & `render_engine-2023.6.2b1/tests/test_feeds.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,39 +35,39 @@
     class TestCollection(Collection):
         feed_title = "Test Feed Title"
         Feed = RSSFeed
         pages = [Page()]
 
     collection = TestCollection()
 
-    assert collection._feed.title == "Test Feed Title"
+    assert collection.feed.title == "Test Feed Title"
 
 
 def test_rss_feed_inherites_from_collection():
     """Test that the feed title is set from the collection"""
 
     class BasicCollection(Collection):
         pages = [Page()]
         archive_template = None
         Feed = RSSFeed
 
     collection = BasicCollection()
 
-    assert collection._feed.title == "BasicCollection"
+    assert collection.feed.title == "BasicCollection"
 
 
 def test_rss_feed_item_url(site):
     """Test that the feed item url is set correctly"""
-    assert "<link>http://localhost:8000/page.html</link>" in site.route_list['testcollection']._feed._render_content(engine=site.engine, SITE_URL="http://localhost:8000")
+    assert "<link>http://localhost:8000/page.html</link>" in site.route_list['testcollection'].feed._render_content(engine=site.engine, SITE_URL="http://localhost:8000")
 
 
 
 def test_rss_feed_item_has_guid(site):
     """Test that the feed item url is set correctly"""
-    assert '<guid isPermaLink="true">http://localhost:8000/page.html</guid>' in site.route_list['testcollection']._feed._render_content(engine=site.engine, SITE_URL="http://localhost:8000")
+    assert '<guid isPermaLink="true">http://localhost:8000/page.html</guid>' in site.route_list['testcollection'].feed._render_content(engine=site.engine, SITE_URL="http://localhost:8000")
 
 
 @pytest.mark.skip("Invalid Test")
 def test_rss_feed_template_with_strictundefined(engine, tmp_path):
     """Test that the RSS feed template works with the StrictUndefined undefined handler."""
     tmp_dir = tmp_path / "content"
     tmp_dir.mkdir()
@@ -76,15 +76,15 @@
 
     class TestCollection(Collection):
         pages = [Page(content_path=file)]
         Feed = RSSFeed
 
     collection = TestCollection()
     engine.undefined = StrictUndefined
-    rendered_content = collection._feed._render_content(
+    rendered_content = collection.feed._render_content(
         engine=engine,
         SITE_TITLE="Test Site Title",
         SITE_URL="http://localhost:8000",
         title="Test Feed Title",
         description="Test Feed Description",
     )
     assert "http://localhost:8000/page.html" in rendered_content
@@ -98,15 +98,15 @@
         date = datetime.datetime(2023, 4, 15, 0, 0, 0, tzinfo=datetime.timezone.utc)   # noqa: UP017
     class TestCollection(Collection):
         Feed = RSSFeed
         pages = [TestPage()]
 
     collection = TestCollection()
 
-    rendered_content = collection._feed._render_content(
+    rendered_content = collection.feed._render_content(
         engine=engine,
         SITE_TITLE="Test Site Title",
         SITE_URL="http://localhost:8000",
         title="Test Feed Title",
         description="Test Feed Description",
     )
```

### Comparing `render_engine-2023.6.1/tests/test_page.py` & `render_engine-2023.6.2b1/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.6.1/tests/test_site.py` & `render_engine-2023.6.2b1/tests/test_site.py`

 * *Files identical despite different names*

