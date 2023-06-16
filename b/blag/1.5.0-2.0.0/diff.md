# Comparing `tmp/blag-1.5.0.tar.gz` & `tmp/blag-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blag-1.5.0.tar", last modified: Sun Apr 16 09:01:18 2023, max compression
+gzip compressed data, was "blag-2.0.0.tar", last modified: Fri Jun 16 21:08:18 2023, max compression
```

## Comparing `blag-1.5.0.tar` & `blag-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,47 @@
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-16 09:01:18.473932 blag-1.5.0/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1072 2021-02-01 20:16:23.000000 blag-1.5.0/LICENSE
--rw-r--r--   0 venthur   (1000) venthur   (1000)     3124 2023-04-16 09:01:18.473932 blag-1.5.0/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1383 2022-07-01 08:26:42.000000 blag-1.5.0/README.md
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-16 09:01:18.473932 blag-1.5.0/blag/
--rw-r--r--   0 venthur   (1000) venthur   (1000)       60 2022-09-01 16:56:08.000000 blag-1.5.0/blag/__init__.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)    12876 2022-09-04 10:57:00.000000 blag-1.5.0/blag/blag.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2624 2022-09-01 16:56:08.000000 blag-1.5.0/blag/devserver.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     3577 2022-09-01 16:56:08.000000 blag-1.5.0/blag/markdown.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1636 2022-09-01 16:56:08.000000 blag-1.5.0/blag/quickstart.py
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-16 09:01:18.473932 blag-1.5.0/blag/templates/
--rw-r--r--   0 venthur   (1000) venthur   (1000)      373 2022-08-06 19:36:01.000000 blag-1.5.0/blag/templates/archive.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      559 2022-08-06 19:36:01.000000 blag-1.5.0/blag/templates/article.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      867 2022-08-06 19:36:01.000000 blag-1.5.0/blag/templates/base.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      120 2021-02-06 13:22:35.000000 blag-1.5.0/blag/templates/page.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      371 2022-08-06 19:36:01.000000 blag-1.5.0/blag/templates/tag.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      245 2021-02-09 20:55:37.000000 blag-1.5.0/blag/templates/tags.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)       22 2023-04-16 08:58:00.000000 blag-1.5.0/blag/version.py
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-16 09:01:18.473932 blag-1.5.0/blag.egg-info/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     3124 2023-04-16 09:01:18.000000 blag-1.5.0/blag.egg-info/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)      594 2023-04-16 09:01:18.000000 blag-1.5.0/blag.egg-info/SOURCES.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)        1 2023-04-16 09:01:18.000000 blag-1.5.0/blag.egg-info/dependency_links.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       40 2023-04-16 09:01:18.000000 blag-1.5.0/blag.egg-info/entry_points.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)      116 2023-04-16 09:01:18.000000 blag-1.5.0/blag.egg-info/requires.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)        5 2023-04-16 09:01:18.000000 blag-1.5.0/blag.egg-info/top_level.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1351 2023-04-16 08:58:00.000000 blag-1.5.0/pyproject.toml
--rw-r--r--   0 venthur   (1000) venthur   (1000)       38 2023-04-16 09:01:18.473932 blag-1.5.0/setup.cfg
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-16 09:01:18.473932 blag-1.5.0/tests/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     8868 2022-09-01 16:56:08.000000 blag-1.5.0/tests/test_blag.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1833 2022-09-01 16:56:08.000000 blag-1.5.0/tests/test_devserver.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2994 2022-09-01 16:56:08.000000 blag-1.5.0/tests/test_markdown.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)      891 2022-09-01 16:56:08.000000 blag-1.5.0/tests/test_quickstart.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1967 2022-09-01 16:56:08.000000 blag-1.5.0/tests/test_templates.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)      167 2022-09-01 16:56:08.000000 blag-1.5.0/tests/test_version.py
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-06-16 21:08:18.680785 blag-2.0.0/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1072 2021-02-01 20:16:23.000000 blag-2.0.0/LICENSE
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     3153 2023-06-16 21:08:18.676785 blag-2.0.0/PKG-INFO
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1412 2023-06-16 20:29:14.000000 blag-2.0.0/README.md
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-06-16 21:08:18.672785 blag-2.0.0/blag/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       60 2022-09-01 16:56:08.000000 blag-2.0.0/blag/__init__.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)    13828 2023-06-16 20:05:45.000000 blag-2.0.0/blag/blag.py
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-06-16 21:08:18.676785 blag-2.0.0/blag/content/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      232 2023-06-16 20:05:45.000000 blag-2.0.0/blag/content/about.md
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1524 2023-06-16 20:05:45.000000 blag-2.0.0/blag/content/hello-world.md
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      197 2023-06-16 20:05:45.000000 blag-2.0.0/blag/content/second-post.md
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1061 2023-06-16 20:05:45.000000 blag-2.0.0/blag/content/testpage.md
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2624 2023-06-16 20:05:45.000000 blag-2.0.0/blag/devserver.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     3577 2023-06-16 20:05:45.000000 blag-2.0.0/blag/markdown.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2407 2023-06-16 20:05:45.000000 blag-2.0.0/blag/quickstart.py
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-06-16 21:08:18.676785 blag-2.0.0/blag/static/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     4048 2023-06-16 20:05:45.000000 blag-2.0.0/blag/static/code-dark.css
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     4036 2023-06-16 20:05:45.000000 blag-2.0.0/blag/static/code-light.css
+-rw-r--r--   0 venthur   (1000) venthur   (1000)    15406 2023-06-16 20:05:45.000000 blag-2.0.0/blag/static/favicon.ico
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2574 2023-06-16 20:05:45.000000 blag-2.0.0/blag/static/style.css
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-06-16 21:08:18.676785 blag-2.0.0/blag/templates/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      449 2023-06-16 20:05:45.000000 blag-2.0.0/blag/templates/archive.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      558 2023-06-16 20:05:45.000000 blag-2.0.0/blag/templates/article.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1520 2023-06-16 20:05:45.000000 blag-2.0.0/blag/templates/base.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      515 2023-06-16 20:05:45.000000 blag-2.0.0/blag/templates/index.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      124 2023-06-16 20:05:45.000000 blag-2.0.0/blag/templates/page.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      493 2023-06-16 20:05:45.000000 blag-2.0.0/blag/templates/tag.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      245 2021-02-09 20:55:37.000000 blag-2.0.0/blag/templates/tags.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       22 2023-06-16 20:33:08.000000 blag-2.0.0/blag/version.py
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-06-16 21:08:18.676785 blag-2.0.0/blag.egg-info/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     3153 2023-06-16 21:08:18.000000 blag-2.0.0/blag.egg-info/PKG-INFO
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      858 2023-06-16 21:08:18.000000 blag-2.0.0/blag.egg-info/SOURCES.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)        1 2023-06-16 21:08:18.000000 blag-2.0.0/blag.egg-info/dependency_links.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       40 2023-06-16 21:08:18.000000 blag-2.0.0/blag.egg-info/entry_points.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      116 2023-06-16 21:08:18.000000 blag-2.0.0/blag.egg-info/requires.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       11 2023-06-16 21:08:18.000000 blag-2.0.0/blag.egg-info/top_level.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1382 2023-06-16 20:05:45.000000 blag-2.0.0/pyproject.toml
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       38 2023-06-16 21:08:18.680785 blag-2.0.0/setup.cfg
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-06-16 21:08:18.676785 blag-2.0.0/tests/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)        0 2021-02-01 20:16:23.000000 blag-2.0.0/tests/__init__.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2262 2023-06-16 20:05:45.000000 blag-2.0.0/tests/conftest.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     9321 2023-06-16 20:05:45.000000 blag-2.0.0/tests/test_blag.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1834 2023-06-16 20:05:45.000000 blag-2.0.0/tests/test_devserver.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2995 2023-06-16 20:05:45.000000 blag-2.0.0/tests/test_markdown.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1233 2023-06-16 20:05:45.000000 blag-2.0.0/tests/test_quickstart.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2461 2023-06-16 20:05:45.000000 blag-2.0.0/tests/test_templates.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      167 2022-09-01 16:56:08.000000 blag-2.0.0/tests/test_version.py
```

### Comparing `blag-1.5.0/LICENSE` & `blag-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blag-1.5.0/PKG-INFO` & `blag-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blag
-Version: 1.5.0
+Version: 2.0.0
 Summary: blog-aware, static site generator
 Author-email: Bastian Venthur <mail@venthur.de>
 License: MIT License
         
         Copyright (c) 2018 Bastian Venthur
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,14 +48,15 @@
 [venthur.de]: https://venthur.de
 [documentation]: https://blag.readthedocs.io/en/latest/
 
 
 ## Features
 
 * Write content in [Markdown][]
+* Good looking default theme
 * Theming support using [Jinja2][] templates
 * Generation of Atom feeds for blog content
 * Fenced code blocks and syntax highlighting using [Pygments][]
 * Integrated devserver
 * Available on [PyPI][]
 
 blag runs on Linux, Mac and Windows and requires Python >= 3.8
```

### Comparing `blag-1.5.0/README.md` & `blag-2.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 [venthur.de]: https://venthur.de
 [documentation]: https://blag.readthedocs.io/en/latest/
 
 
 ## Features
 
 * Write content in [Markdown][]
+* Good looking default theme
 * Theming support using [Jinja2][] templates
 * Generation of Atom feeds for blog content
 * Fenced code blocks and syntax highlighting using [Pygments][]
 * Integrated devserver
 * Available on [PyPI][]
 
 blag runs on Linux, Mac and Windows and requires Python >= 3.8
```

### Comparing `blag-1.5.0/blag/blag.py` & `blag-2.0.0/blag/blag.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,40 +2,36 @@
 
 """blag's core methods.
 
 """
 
 # remove when we don't support py38 anymore
 from __future__ import annotations
-from typing import Any
+
 import argparse
+import configparser
+import logging
 import os
 import shutil
-import logging
-import configparser
 import sys
+from typing import Any
 
-from jinja2 import (
-    Environment,
-    ChoiceLoader,
-    FileSystemLoader,
-    PackageLoader,
-    Template,
-)
 import feedgenerator
+from jinja2 import Environment, FileSystemLoader, Template, TemplateNotFound
 
-from blag.markdown import markdown_factory, convert_markdown
+import blag
 from blag.devserver import serve
-from blag.version import __VERSION__
+from blag.markdown import convert_markdown, markdown_factory
 from blag.quickstart import quickstart
+from blag.version import __VERSION__
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(
     level=logging.INFO,
-    format='%(asctime)s %(levelname)s %(name)s %(message)s',
+    format="%(asctime)s %(levelname)s %(name)s %(message)s",
 )
 
 
 def main(arguments: list[str] | None = None) -> None:
     """Main entrypoint for the CLI.
 
     This method parses the CLI arguments and executes the respective
@@ -66,92 +62,92 @@
     Returns
     -------
     arparse.Namespace
 
     """
     parser = argparse.ArgumentParser()
     parser.add_argument(
-        '--version',
-        action='version',
-        version='%(prog)s ' + __VERSION__,
+        "--version",
+        action="version",
+        version="%(prog)s " + __VERSION__,
     )
     parser.add_argument(
-        '-v',
-        '--verbose',
-        action='store_true',
-        help='Verbose output.',
+        "-v",
+        "--verbose",
+        action="store_true",
+        help="Verbose output.",
     )
 
-    commands = parser.add_subparsers(dest='command')
+    commands = parser.add_subparsers(dest="command")
     commands.required = True
 
     build_parser = commands.add_parser(
-        'build',
-        help='Build website.',
+        "build",
+        help="Build website.",
     )
     build_parser.set_defaults(func=build)
     build_parser.add_argument(
-        '-i',
-        '--input-dir',
-        default='content',
-        help='Input directory (default: content)',
+        "-i",
+        "--input-dir",
+        default="content",
+        help="Input directory (default: content)",
     )
     build_parser.add_argument(
-        '-o',
-        '--output-dir',
-        default='build',
-        help='Ouptut directory (default: build)',
+        "-o",
+        "--output-dir",
+        default="build",
+        help="Ouptut directory (default: build)",
     )
     build_parser.add_argument(
-        '-t',
-        '--template-dir',
-        default='templates',
-        help='Template directory (default: templates)',
+        "-t",
+        "--template-dir",
+        default="templates",
+        help="Template directory (default: templates)",
     )
     build_parser.add_argument(
-        '-s',
-        '--static-dir',
-        default='static',
-        help='Static directory (default: static)',
+        "-s",
+        "--static-dir",
+        default="static",
+        help="Static directory (default: static)",
     )
 
     quickstart_parser = commands.add_parser(
-        'quickstart',
+        "quickstart",
         help="Quickstart blag, creating necessary configuration.",
     )
     quickstart_parser.set_defaults(func=quickstart)
 
     serve_parser = commands.add_parser(
-        'serve',
+        "serve",
         help="Start development server.",
     )
     serve_parser.set_defaults(func=serve)
     serve_parser.add_argument(
-        '-i',
-        '--input-dir',
-        default='content',
-        help='Input directory (default: content)',
+        "-i",
+        "--input-dir",
+        default="content",
+        help="Input directory (default: content)",
     )
     serve_parser.add_argument(
-        '-o',
-        '--output-dir',
-        default='build',
-        help='Ouptut directory (default: build)',
+        "-o",
+        "--output-dir",
+        default="build",
+        help="Ouptut directory (default: build)",
     )
     serve_parser.add_argument(
-        '-t',
-        '--template-dir',
-        default='templates',
-        help='Template directory (default: templates)',
+        "-t",
+        "--template-dir",
+        default="templates",
+        help="Template directory (default: templates)",
     )
     serve_parser.add_argument(
-        '-s',
-        '--static-dir',
-        default='static',
-        help='Static directory (default: static)',
+        "-s",
+        "--static-dir",
+        default="static",
+        help="Static directory (default: static)",
     )
 
     return parser.parse_args(args)
 
 
 def get_config(configfile: str) -> configparser.SectionProxy:
     """Load site configuration from configfile.
@@ -166,57 +162,50 @@
     -------
     configparser.SectionProxy
 
     """
     config = configparser.ConfigParser()
     config.read(configfile)
     # check for the mandatory options
-    for value in 'base_url', 'title', 'description', 'author':
+    for value in "base_url", "title", "description", "author":
         try:
-            config['main'][value]
+            config["main"][value]
         except Exception:
-            print(f'{value} is missing in {configfile}!')
+            print(f"{value} is missing in {configfile}!")
             sys.exit(1)
 
-    if not config['main']['base_url'].endswith('/'):
-        logger.warning('base_url does not end with a slash, adding it.')
-        config['main']['base_url'] += '/'
+    if not config["main"]["base_url"].endswith("/"):
+        logger.warning("base_url does not end with a slash, adding it.")
+        config["main"]["base_url"] += "/"
 
-    return config['main']
+    return config["main"]
 
 
 def environment_factory(
-    template_dir: str | None = None,
+    template_dir: str,
     globals_: dict[str, object] | None = None,
 ) -> Environment:
     """Environment factory.
 
-    Creates a Jinja2 Environment with the default templates and
-    additional templates from `template_dir` loaded. If `globals` are
-    provided, they are attached to the environment and thus available to
-    all contexts.
+    Creates a Jinja2 Environment with the templates from `template_dir` loaded.
+    If `globals` are provided, they are attached to the environment and thus
+    available to all contexts.
 
     Parameters
     ----------
     template_dir
         directory containing the templates
     globals_
 
     Returns
     -------
     jinja2.Environment
 
     """
-    # first we try the custom templates, and fall back the ones provided
-    # by blag
-    loaders: list[FileSystemLoader | PackageLoader] = []
-    if template_dir:
-        loaders.append(FileSystemLoader([template_dir]))
-    loaders.append(PackageLoader('blag', 'templates'))
-    env = Environment(loader=ChoiceLoader(loaders))
+    env = Environment(loader=FileSystemLoader(template_dir))
     if globals_:
         env.globals = globals_
     return env
 
 
 def build(args: argparse.Namespace) -> None:
     """Build the site.
@@ -225,68 +214,80 @@
     etc.
 
     Parameters
     ----------
     args
 
     """
-    os.makedirs(f'{args.output_dir}', exist_ok=True)
+    os.makedirs(f"{args.output_dir}", exist_ok=True)
     convertibles = []
     for root, dirnames, filenames in os.walk(args.input_dir):
         for filename in filenames:
             rel_src = os.path.relpath(
-                f'{root}/{filename}', start=args.input_dir
+                f"{root}/{filename}", start=args.input_dir
             )
             # all non-markdown files are just copied over, the markdown
             # files are converted to html
-            if rel_src.endswith('.md'):
+            if rel_src.endswith(".md"):
                 rel_dst = rel_src
-                rel_dst = rel_dst[:-3] + '.html'
+                rel_dst = rel_dst[:-3] + ".html"
                 convertibles.append((rel_src, rel_dst))
             else:
                 shutil.copy(
-                    f'{args.input_dir}/{rel_src}',
-                    f'{args.output_dir}/{rel_src}',
+                    f"{args.input_dir}/{rel_src}",
+                    f"{args.output_dir}/{rel_src}",
                 )
         for dirname in dirnames:
             # all directories are copied into the output directory
-            path = os.path.relpath(f'{root}/{dirname}', start=args.input_dir)
-            os.makedirs(f'{args.output_dir}/{path}', exist_ok=True)
+            path = os.path.relpath(f"{root}/{dirname}", start=args.input_dir)
+            os.makedirs(f"{args.output_dir}/{path}", exist_ok=True)
 
     # copy static files over
-    logger.info('Copying static files.')
+    logger.info("Copying static files.")
     if os.path.exists(args.static_dir):
         shutil.copytree(args.static_dir, args.output_dir, dirs_exist_ok=True)
 
-    config = get_config('config.ini')
+    config = get_config("config.ini")
 
     env = environment_factory(args.template_dir, dict(site=config))
 
-    page_template = env.get_template('page.html')
-    article_template = env.get_template('article.html')
-    archive_template = env.get_template('archive.html')
-    tags_template = env.get_template('tags.html')
-    tag_template = env.get_template('tag.html')
+    try:
+        page_template = env.get_template("page.html")
+        article_template = env.get_template("article.html")
+        index_template = env.get_template("index.html")
+        archive_template = env.get_template("archive.html")
+        tags_template = env.get_template("tags.html")
+        tag_template = env.get_template("tag.html")
+    except TemplateNotFound as exc:
+        tmpl = os.path.join(blag.__path__[0], "templates")
+        logger.error(
+            f'Template "{exc.name}" not found in {args.template_dir}! '
+            "Consider running `blag quickstart` or copying the "
+            f"missing template from {tmpl}."
+        )
+
+        sys.exit(1)
 
     articles, pages = process_markdown(
         convertibles,
         args.input_dir,
         args.output_dir,
         page_template,
         article_template,
     )
 
     generate_feed(
         articles,
         args.output_dir,
-        base_url=config['base_url'],
-        blog_title=config['title'],
-        blog_description=config['description'],
-        blog_author=config['author'],
+        base_url=config["base_url"],
+        blog_title=config["title"],
+        blog_description=config["description"],
+        blog_author=config["author"],
     )
+    generate_index(articles, index_template, args.output_dir)
     generate_archive(articles, archive_template, args.output_dir)
     generate_tags(articles, tags_template, tag_template, args.output_dir)
 
 
 def process_markdown(
     convertibles: list[tuple[str, str]],
     input_dir: str,
@@ -298,58 +299,60 @@
 
     This method processes the convertibles, converts them to html and
     saves them to the respective destination paths.
 
     If a markdown file has a `date` metadata field it will be recognized
     as article otherwise as page.
 
+    Articles are sorted by date in descending order.
+
     Parameters
     ----------
     convertibles
         relative paths to markdown- (src) html- (dest) files
     input_dir
     output_dir
     page_template, archive_template
-        templats for pages and articles
+        templates for pages and articles
 
     Returns
     -------
     list[tuple[str, dict[str, Any]]], list[tuple[str, dict[str, Any]]]
-        articles and pages
+        articles and pages, articles are sorted by date in descending order.
 
     """
     logger.info("Converting Markdown files...")
     md = markdown_factory()
 
     articles = []
     pages = []
     for src, dst in convertibles:
-        logger.debug(f'Processing {src}')
+        logger.debug(f"Processing {src}")
 
-        with open(f'{input_dir}/{src}', 'r') as fh:
+        with open(f"{input_dir}/{src}", "r") as fh:
             body = fh.read()
 
         content, meta = convert_markdown(md, body)
 
         context = dict(content=content)
         context.update(meta)
 
         # if markdown has date in meta, we treat it as a blog article,
         # everything else are just pages
-        if meta and 'date' in meta:
+        if meta and "date" in meta:
             articles.append((dst, context))
             result = article_template.render(context)
         else:
             pages.append((dst, context))
             result = page_template.render(context)
-        with open(f'{output_dir}/{dst}', 'w') as fh_dest:
+        with open(f"{output_dir}/{dst}", "w") as fh_dest:
             fh_dest.write(result)
 
     # sort articles by date, descending
-    articles = sorted(articles, key=lambda x: x[1]['date'], reverse=True)
+    articles = sorted(articles, key=lambda x: x[1]["date"], reverse=True)
     return articles, pages
 
 
 def generate_feed(
     articles: list[tuple[str, dict[str, Any]]],
     output_dir: str,
     base_url: str,
@@ -371,64 +374,95 @@
         blog title
     blog_description
         blog description
     blog_author
         blog author
 
     """
-    logger.info('Generating Atom feed.')
+    logger.info("Generating Atom feed.")
     feed = feedgenerator.Atom1Feed(
         link=base_url,
         title=blog_title,
         description=blog_description,
-        feed_url=base_url + 'atom.xml',
+        feed_url=base_url + "atom.xml",
     )
 
     for dst, context in articles:
         # if article has a description, use that. otherwise fall back to
         # the title
-        description = context.get('description', context['title'])
+        description = context.get("description", context["title"])
 
         feed.add_item(
-            title=context['title'],
+            title=context["title"],
             author_name=blog_author,
             link=base_url + dst,
             description=description,
-            content=context['content'],
-            pubdate=context['date'],
+            content=context["content"],
+            pubdate=context["date"],
         )
 
-    with open(f'{output_dir}/atom.xml', 'w') as fh:
-        feed.write(fh, encoding='utf8')
+    with open(f"{output_dir}/atom.xml", "w") as fh:
+        feed.write(fh, encoding="utf8")
+
+
+def generate_index(
+    articles: list[tuple[str, dict[str, Any]]],
+    template: Template,
+    output_dir: str,
+) -> None:
+    """Generate the index page.
+
+    This is used for the index (i.e. landing) page.
+
+    Parameters
+    ----------
+    articles
+        List of articles. Each article has the destination path and a
+        dictionary with the content.
+    template
+    output_dir
+
+    """
+    archive = []
+    for dst, context in articles:
+        entry = context.copy()
+        entry["dst"] = dst
+        archive.append(entry)
+
+    result = template.render(dict(archive=archive))
+    with open(f"{output_dir}/index.html", "w") as fh:
+        fh.write(result)
 
 
 def generate_archive(
     articles: list[tuple[str, dict[str, Any]]],
     template: Template,
     output_dir: str,
 ) -> None:
     """Generate the archive page.
 
+    This is used for the full archive.
+
     Parameters
     ----------
     articles
         List of articles. Each article has the destination path and a
         dictionary with the content.
     template
     output_dir
 
     """
     archive = []
     for dst, context in articles:
         entry = context.copy()
-        entry['dst'] = dst
+        entry["dst"] = dst
         archive.append(entry)
 
     result = template.render(dict(archive=archive))
-    with open(f'{output_dir}/index.html', 'w') as fh:
+    with open(f"{output_dir}/archive.html", "w") as fh:
         fh.write(result)
 
 
 def generate_tags(
     articles: list[tuple[str, dict[str, Any]]],
     tags_template: Template,
     tag_template: Template,
@@ -442,42 +476,42 @@
         List of articles. Each article has the destination path and a
         dictionary with the content.
     tags_template, tag_template
     output_dir
 
     """
     logger.info("Generating Tag-pages.")
-    os.makedirs(f'{output_dir}/tags', exist_ok=True)
+    os.makedirs(f"{output_dir}/tags", exist_ok=True)
     # get tags number of occurrences
     all_tags: dict[str, int] = {}
     for _, context in articles:
-        tags: list[str] = context.get('tags', [])
+        tags: list[str] = context.get("tags", [])
         for tag in tags:
             all_tags[tag] = all_tags.get(tag, 0) + 1
     # sort by occurrence
     taglist: list[tuple[str, int]] = sorted(
         all_tags.items(), key=lambda x: x[1], reverse=True
     )
 
     result = tags_template.render(dict(tags=taglist))
-    with open(f'{output_dir}/tags/index.html', 'w') as fh:
+    with open(f"{output_dir}/tags/index.html", "w") as fh:
         fh.write(result)
 
     # get tags and archive per tag
     all_tags2: dict[str, list[dict[str, Any]]] = {}
     for dst, context in articles:
-        tags = context.get('tags', [])
+        tags = context.get("tags", [])
         for tag in tags:
             archive: list[dict[str, Any]] = all_tags2.get(tag, [])
             entry = context.copy()
-            entry['dst'] = dst
+            entry["dst"] = dst
             archive.append(entry)
             all_tags2[tag] = archive
 
     for tag, archive in all_tags2.items():
         result = tag_template.render(dict(archive=archive, tag=tag))
-        with open(f'{output_dir}/tags/{tag}.html', 'w') as fh:
+        with open(f"{output_dir}/tags/{tag}.html", "w") as fh:
             fh.write(result)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `blag-1.5.0/blag/devserver.py` & `blag-2.0.0/blag/devserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 automatically detects changes in certain directories and rebuilds the
 site if necessary.
 
 """
 
 # remove when we don't support py38 anymore
 from __future__ import annotations
-from typing import NoReturn
-import os
+
+import argparse
 import logging
-import time
 import multiprocessing
-from http.server import SimpleHTTPRequestHandler, HTTPServer
+import os
+import time
 from functools import partial
-import argparse
+from http.server import HTTPServer, SimpleHTTPRequestHandler
+from typing import NoReturn
 
 from blag import blag
 
-
 logger = logging.getLogger(__name__)
 
 
 def get_last_modified(dirs: list[str]) -> float:
     """Get the last modified time.
 
     This method recursively goes through `dirs` and returns the most
@@ -65,37 +65,37 @@
     Parameters
     ----------
     args
         contains the input-, template- and static dir
 
     """
     dirs = [args.input_dir, args.template_dir, args.static_dir]
-    logger.info(f'Monitoring {dirs} for changes...')
+    logger.info(f"Monitoring {dirs} for changes...")
     # make sure we trigger the rebuild immediately when we enter the
     # loop to avoid serving stale contents
     last_mtime = 0.0
     while True:
         mtime = get_last_modified(dirs)
         if mtime > last_mtime:
             last_mtime = mtime
-            logger.info('Change detected, rebuilding...')
+            logger.info("Change detected, rebuilding...")
             blag.build(args)
         time.sleep(1)
 
 
 def serve(args: argparse.Namespace) -> None:
     """Start the webserver and the autoreloader.
 
     Parameters
     ----------
     args
         contains the input-, template- and static dir
 
     """
     httpd = HTTPServer(
-        ('', 8000),
+        ("", 8000),
         partial(SimpleHTTPRequestHandler, directory=args.output_dir),
     )
     proc = multiprocessing.Process(target=autoreload, args=(args,))
     proc.start()
     logger.info("\n\n  Devserver Started -- visit http://localhost:8000\n")
     httpd.serve_forever()
```

### Comparing `blag-1.5.0/blag/markdown.py` & `blag-2.0.0/blag/markdown.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 This module contains the methods responsible for blag's markdown
 processing.
 
 """
 
 # remove when we don't support py38 anymore
 from __future__ import annotations
-from datetime import datetime
+
 import logging
+from datetime import datetime
 from urllib.parse import urlsplit, urlunsplit
 from xml.etree.ElementTree import Element
 
 from markdown import Markdown
 from markdown.extensions import Extension
 from markdown.treeprocessors import Treeprocessor
 
-
 logger = logging.getLogger(__name__)
 
 
 def markdown_factory() -> Markdown:
     """Create a Markdown instance.
 
     This method exists only to ensure we use the same Markdown instance
@@ -29,21 +29,21 @@
     Returns
     -------
     markdown.Markdown
 
     """
     md = Markdown(
         extensions=[
-            'meta',
-            'fenced_code',
-            'codehilite',
-            'smarty',
+            "meta",
+            "fenced_code",
+            "codehilite",
+            "smarty",
             MarkdownLinkExtension(),
         ],
-        output_format='html',
+        output_format="html",
     )
     return md
 
 
 def convert_markdown(
     md: Markdown,
     markdown: str,
@@ -71,63 +71,63 @@
     md.reset()
     content = md.convert(markdown)
     meta = md.Meta  # type: ignore
 
     # markdowns metadata consists as list of strings -- one item per
     # line. let's convert into single strings.
     for key, value in meta.items():
-        value = '\n'.join(value)
+        value = "\n".join(value)
         meta[key] = value
 
     # convert known metadata
     # date: datetime
-    if 'date' in meta:
-        meta['date'] = datetime.fromisoformat(meta['date'])
-        meta['date'] = meta['date'].astimezone()
+    if "date" in meta:
+        meta["date"] = datetime.fromisoformat(meta["date"])
+        meta["date"] = meta["date"].astimezone()
     # tags: list[str] and lower case
-    if 'tags' in meta:
-        tags = meta['tags'].split(',')
+    if "tags" in meta:
+        tags = meta["tags"].split(",")
         tags = [t.lower() for t in tags]
         tags = [t.strip() for t in tags]
-        meta['tags'] = tags
+        meta["tags"] = tags
 
     return content, meta
 
 
 class MarkdownLinkTreeprocessor(Treeprocessor):
     """Converts relative links to .md files to .html"""
 
     def run(self, root: Element) -> Element:
         for element in root.iter():
-            if element.tag == 'a':
-                url = element.get('href')
+            if element.tag == "a":
+                url = element.get("href")
                 # element.get could also return None, we haven't seen this so
                 # far, so lets wait if we raise this
                 assert url is not None
                 url = str(url)
                 converted = self.convert(url)
-                element.set('href', converted)
+                element.set("href", converted)
         return root
 
     def convert(self, url: str) -> str:
         scheme, netloc, path, query, fragment = urlsplit(url)
         logger.debug(
-            f'{url}: {scheme=} {netloc=} {path=} {query=} {fragment=}'
+            f"{url}: {scheme=} {netloc=} {path=} {query=} {fragment=}"
         )
         if scheme or netloc or not path:
             return url
-        if path.endswith('.md'):
-            path = path[:-3] + '.html'
+        if path.endswith(".md"):
+            path = path[:-3] + ".html"
 
         url = urlunsplit((scheme, netloc, path, query, fragment))
         return url
 
 
 class MarkdownLinkExtension(Extension):
     """markdown.extension that converts relative .md- to .html-links."""
 
     def extendMarkdown(self, md: Markdown) -> None:
         md.treeprocessors.register(
             MarkdownLinkTreeprocessor(md),
-            'mdlink',
+            "mdlink",
             0,
         )
```

### Comparing `blag-1.5.0/blag/quickstart.py` & `blag-2.0.0/blag/quickstart.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """Helper methods for blag's quickstart command.
 
 """
 
 # remove when we don't support py38 anymore
 from __future__ import annotations
-import configparser
+
 import argparse
+import configparser
+import os
+import shutil
+
+import blag
 
 
 def get_input(question: str, default: str) -> str:
     """Prompt for user input.
 
     This is a wrapper around the input-builtin. It will show the default answer
     in the prompt and -- if no answer was given -- use the default.
@@ -29,19 +34,41 @@
     """
     reply = input(f"{question} [{default}]: ")
     if not reply:
         reply = default
     return reply
 
 
+def copy_default_theme() -> None:
+    """Copy default theme into current directory.
+
+    The default theme contains the 'templates', 'content' and 'static'
+    directories shipped with blag.
+
+    It will not overwrite existing files.
+
+    """
+    print("Copying default theme...")
+    for dir_ in "templates", "content", "static":
+        print(f"  Copying {dir_}...")
+        try:
+            shutil.copytree(
+                os.path.join(blag.__path__[0], dir_),
+                dir_,
+            )
+        except FileExistsError:
+            print(f"  {dir_} already exist. Skipping.")
+
+
 def quickstart(args: argparse.Namespace | None) -> None:
     """Quickstart.
 
-    This method asks the user some questions and generates a
-    configuration file that is needed in order to run blag.
+    This method asks the user some questions and generates a configuration file
+    that is needed in order to run blag. Additionally, it creates the content
+    and static directories with some initial content, to get the user started.
 
     Parameters
     ----------
     args
         not used
 
     """
@@ -59,15 +86,17 @@
     )
     author = get_input(
         "Author of your website",
         "John Doe",
     )
 
     config = configparser.ConfigParser()
-    config['main'] = {
-        'base_url': base_url,
-        'title': title,
-        'description': description,
-        'author': author,
+    config["main"] = {
+        "base_url": base_url,
+        "title": title,
+        "description": description,
+        "author": author,
     }
-    with open('config.ini', 'w') as fh:
+    with open("config.ini", "w") as fh:
         config.write(fh)
+
+    copy_default_theme()
```

### Comparing `blag-1.5.0/blag/templates/article.html` & `blag-2.0.0/blag/templates/article.html`

 * *Files 0% similar despite different names*

```diff
@@ -18,11 +18,10 @@
         {%- if loop.last and not loop.first %} and {% endif %}
         <a href="/tags/{{ tag }}.html">#{{ tag }}</a>
       {%- endfor %}
     {% endif %}
     </p>
   </aside>
 
-
   {{ content }}
 
 {% endblock %}
```

### Comparing `blag-1.5.0/blag.egg-info/PKG-INFO` & `blag-2.0.0/blag.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blag
-Version: 1.5.0
+Version: 2.0.0
 Summary: blog-aware, static site generator
 Author-email: Bastian Venthur <mail@venthur.de>
 License: MIT License
         
         Copyright (c) 2018 Bastian Venthur
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,14 +48,15 @@
 [venthur.de]: https://venthur.de
 [documentation]: https://blag.readthedocs.io/en/latest/
 
 
 ## Features
 
 * Write content in [Markdown][]
+* Good looking default theme
 * Theming support using [Jinja2][] templates
 * Generation of Atom feeds for blog content
 * Fenced code blocks and syntax highlighting using [Pygments][]
 * Integrated devserver
 * Available on [PyPI][]
 
 blag runs on Linux, Mac and Windows and requires Python >= 3.8
```

### Comparing `blag-1.5.0/pyproject.toml` & `blag-2.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -43,19 +43,23 @@
 
 [tool.setuptools.dynamic]
 version = {attr = "blag.__VERSION__" }
 
 [tool.setuptools]
 packages = [
     "blag",
-    "blag.templates",
+    "tests",
 ]
 
 [tool.setuptools.package-data]
-blag = ["templates/*"]
+blag = [
+    "templates/*",
+    "static/*",
+    "content/*",
+]
 
 [tool.pytest.ini_options]
 addopts = """
     --cov=blag
     --cov=tests
     --cov-report=html
     --cov-report=term-missing:skip-covered
```

### Comparing `blag-1.5.0/tests/test_devserver.py` & `blag-2.0.0/tests/test_devserver.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # remove when we don't support py38 anymore
 from __future__ import annotations
-import time
+
 import threading
+import time
 from argparse import Namespace
 
 import pytest
 
 from blag import devserver
 
 
 def test_get_last_modified(cleandir: str) -> None:
     # take initial time
-    t1 = devserver.get_last_modified(['content'])
+    t1 = devserver.get_last_modified(["content"])
 
     # wait a bit, create a file and measure again
     time.sleep(0.1)
-    with open('content/test', 'w') as fh:
-        fh.write('boo')
-    t2 = devserver.get_last_modified(['content'])
+    with open("content/test", "w") as fh:
+        fh.write("boo")
+    t2 = devserver.get_last_modified(["content"])
 
     # wait a bit and take time again
     time.sleep(0.1)
-    t3 = devserver.get_last_modified(['content'])
+    t3 = devserver.get_last_modified(["content"])
 
     assert t2 > t1
     assert t2 == t3
 
 
 def test_autoreload_builds_immediately(args: Namespace) -> None:
     # create a dummy file that can be build
-    with open('content/test.md', 'w') as fh:
-        fh.write('boo')
+    with open("content/test.md", "w") as fh:
+        fh.write("boo")
 
     t = threading.Thread(
         target=devserver.autoreload,
         args=(args,),
         daemon=True,
     )
-    t0 = devserver.get_last_modified(['build'])
+    t0 = devserver.get_last_modified(["build"])
     t.start()
     # try for 5 seconds...
     for i in range(5):
         time.sleep(1)
-        t1 = devserver.get_last_modified(['build'])
+        t1 = devserver.get_last_modified(["build"])
         print(t1)
         if t1 > t0:
             break
     assert t1 > t0
 
 
 @pytest.mark.filterwarnings(
@@ -56,20 +57,20 @@
     t = threading.Thread(
         target=devserver.autoreload,
         args=(args,),
         daemon=True,
     )
     t.start()
 
-    t0 = devserver.get_last_modified(['build'])
+    t0 = devserver.get_last_modified(["build"])
 
     # create a dummy file that can be build
-    with open('content/test.md', 'w') as fh:
-        fh.write('boo')
+    with open("content/test.md", "w") as fh:
+        fh.write("boo")
 
     # try for 5 seconds to see if we rebuild once...
     for i in range(5):
         time.sleep(1)
-        t1 = devserver.get_last_modified(['build'])
+        t1 = devserver.get_last_modified(["build"])
         if t1 > t0:
             break
     assert t1 > t0
```

### Comparing `blag-1.5.0/tests/test_markdown.py` & `blag-2.0.0/tests/test_markdown.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 # remove when we don't support py38 anymore
 from __future__ import annotations
+
 from datetime import datetime
 from typing import Any
 
-import pytest
 import markdown
+import pytest
 
 from blag.markdown import convert_markdown, markdown_factory
 
 
 @pytest.mark.parametrize(
     "input_, expected",
     [
         # inline
-        ('[test](test.md)', 'test.html'),
-        ('[test](test.md "test")', 'test.html'),
-        ('[test](a/test.md)', 'a/test.html'),
-        ('[test](a/test.md "test")', 'a/test.html'),
-        ('[test](/test.md)', '/test.html'),
-        ('[test](/test.md "test")', '/test.html'),
-        ('[test](/a/test.md)', '/a/test.html'),
-        ('[test](/a/test.md "test")', '/a/test.html'),
+        ("[test](test.md)", "test.html"),
+        ('[test](test.md "test")', "test.html"),
+        ("[test](a/test.md)", "a/test.html"),
+        ('[test](a/test.md "test")', "a/test.html"),
+        ("[test](/test.md)", "/test.html"),
+        ('[test](/test.md "test")', "/test.html"),
+        ("[test](/a/test.md)", "/a/test.html"),
+        ('[test](/a/test.md "test")', "/a/test.html"),
         # reference
-        ('[test][]\n[test]: test.md ' '', 'test.html'),
-        ('[test][]\n[test]: test.md "test"', 'test.html'),
-        ('[test][]\n[test]: a/test.md', 'a/test.html'),
-        ('[test][]\n[test]: a/test.md "test"', 'a/test.html'),
-        ('[test][]\n[test]: /test.md', '/test.html'),
-        ('[test][]\n[test]: /test.md "test"', '/test.html'),
-        ('[test][]\n[test]: /a/test.md', '/a/test.html'),
-        ('[test][]\n[test]: /a/test.md "test"', '/a/test.html'),
+        ("[test][]\n[test]: test.md " "", "test.html"),
+        ('[test][]\n[test]: test.md "test"', "test.html"),
+        ("[test][]\n[test]: a/test.md", "a/test.html"),
+        ('[test][]\n[test]: a/test.md "test"', "a/test.html"),
+        ("[test][]\n[test]: /test.md", "/test.html"),
+        ('[test][]\n[test]: /test.md "test"', "/test.html"),
+        ("[test][]\n[test]: /a/test.md", "/a/test.html"),
+        ('[test][]\n[test]: /a/test.md "test"', "/a/test.html"),
     ],
 )
 def test_convert_markdown_links(input_: str, expected: str) -> None:
     md = markdown_factory()
     html, _ = convert_markdown(md, input_)
     assert expected in html
 
 
 @pytest.mark.parametrize(
     "input_, expected",
     [
         # scheme
-        ('[test](https://)', 'https://'),
+        ("[test](https://)", "https://"),
         # netloc
-        ('[test](//test.md)', '//test.md'),
+        ("[test](//test.md)", "//test.md"),
         # no path
-        ('[test]()', ''),
+        ("[test]()", ""),
     ],
 )
 def test_dont_convert_normal_links(input_: str, expected: str) -> None:
     md = markdown_factory()
     html, _ = convert_markdown(md, input_)
     assert expected in html
 
 
 @pytest.mark.parametrize(
     "input_, expected",
     [
-        ('foo: bar', {'foo': 'bar'}),
-        ('foo: those are several words', {'foo': 'those are several words'}),
-        ('tags: this, is, a, test\n', {'tags': ['this', 'is', 'a', 'test']}),
-        ('tags: this, IS, a, test', {'tags': ['this', 'is', 'a', 'test']}),
+        ("foo: bar", {"foo": "bar"}),
+        ("foo: those are several words", {"foo": "those are several words"}),
+        ("tags: this, is, a, test\n", {"tags": ["this", "is", "a", "test"]}),
+        ("tags: this, IS, a, test", {"tags": ["this", "is", "a", "test"]}),
         (
-            'date: 2020-01-01 12:10',
-            {'date': datetime(2020, 1, 1, 12, 10).astimezone()},
+            "date: 2020-01-01 12:10",
+            {"date": datetime(2020, 1, 1, 12, 10).astimezone()},
         ),
     ],
 )
 def test_convert_metadata(input_: str, expected: dict[str, Any]) -> None:
     md = markdown_factory()
     _, meta = convert_markdown(md, input_)
     assert expected == meta
@@ -84,24 +85,24 @@
 
     md1 = """
 
 this --- is -- a test ...
 
     """
     html, meta = convert_markdown(md, md1)
-    assert 'mdash' in html
-    assert 'ndash' in html
-    assert 'hellip' in html
+    assert "mdash" in html
+    assert "ndash" in html
+    assert "hellip" in html
 
 
 def test_smarty_code() -> None:
     md = markdown_factory()
 
     md1 = """
 ```
 this --- is -- a test ...
 ```
     """
     html, meta = convert_markdown(md, md1)
-    assert 'mdash' not in html
-    assert 'ndash' not in html
-    assert 'hellip' not in html
+    assert "mdash" not in html
+    assert "ndash" not in html
+    assert "hellip" not in html
```

### Comparing `blag-1.5.0/tests/test_quickstart.py` & `blag-2.0.0/tests/test_quickstart.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,45 @@
 # remove when we don't support py38 anymore
 from __future__ import annotations
 
+import os
+
 from pytest import MonkeyPatch
 
 from blag.quickstart import get_input, quickstart
 
 
 def test_get_input_default_answer(monkeypatch: MonkeyPatch) -> None:
-    monkeypatch.setattr('builtins.input', lambda x: '')
+    monkeypatch.setattr("builtins.input", lambda x: "")
     answer = get_input("foo", "bar")
-    assert answer == 'bar'
+    assert answer == "bar"
 
 
 def test_get_input(monkeypatch: MonkeyPatch) -> None:
-    monkeypatch.setattr('builtins.input', lambda x: 'baz')
+    monkeypatch.setattr("builtins.input", lambda x: "baz")
     answer = get_input("foo", "bar")
-    assert answer == 'baz'
+    assert answer == "baz"
 
 
 def test_quickstart(cleandir: str, monkeypatch: MonkeyPatch) -> None:
-    monkeypatch.setattr('builtins.input', lambda x: 'foo')
+    monkeypatch.setattr("builtins.input", lambda x: "foo")
     quickstart(None)
-    with open('config.ini', 'r') as fh:
+    with open("config.ini", "r") as fh:
         data = fh.read()
-    assert 'base_url = foo' in data
-    assert 'title = foo' in data
-    assert 'description = foo' in data
-    assert 'author = foo' in data
+    assert "base_url = foo" in data
+    assert "title = foo" in data
+    assert "description = foo" in data
+    assert "author = foo" in data
+
+    for template in (
+        "archive.html",
+        "article.html",
+        "base.html",
+        "index.html",
+        "page.html",
+        "tag.html",
+        "tags.html",
+    ):
+        assert os.path.exists(f"templates/{template}")
+
+    for directory in "build", "content", "static":
+        assert os.path.exists(directory)
```

### Comparing `blag-1.5.0/tests/test_templates.py` & `blag-2.0.0/tests/test_templates.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,98 @@
 # remove when we don't support py38 anymore
 from __future__ import annotations
+
 import datetime
 
 from jinja2 import Template
 
 
 def test_page(page_template: Template) -> None:
     ctx = {
-        'content': 'this is the content',
-        'title': 'this is the title',
+        "content": "this is the content",
+        "title": "this is the title",
     }
     result = page_template.render(ctx)
-    assert 'this is the content' in result
-    assert 'this is the title' in result
+    assert "this is the content" in result
+    assert "this is the title" in result
 
 
 def test_article(article_template: Template) -> None:
     ctx = {
-        'content': 'this is the content',
-        'title': 'this is the title',
-        'date': datetime.datetime(1980, 5, 9),
+        "content": "this is the content",
+        "title": "this is the title",
+        "date": datetime.datetime(1980, 5, 9),
     }
     result = article_template.render(ctx)
-    assert 'this is the content' in result
-    assert 'this is the title' in result
-    assert '1980-05-09' in result
+    assert "this is the content" in result
+    assert "this is the title" in result
+    assert "1980-05-09" in result
+
+
+def test_index(index_template: Template) -> None:
+    entry = {
+        "title": "this is a title",
+        "dst": "https://example.com/link",
+        "date": datetime.datetime(1980, 5, 9),
+    }
+    archive = [entry]
+    ctx = {
+        "archive": archive,
+    }
+    result = index_template.render(ctx)
+    assert "site title" in result
+
+    assert "this is a title" in result
+    assert "1980-05-09" in result
+    assert "https://example.com/link" in result
+
+    assert "/archive.html" in result
 
 
 def test_archive(archive_template: Template) -> None:
     entry = {
-        'title': 'this is a title',
-        'dst': 'https://example.com/link',
-        'date': datetime.datetime(1980, 5, 9),
+        "title": "this is a title",
+        "dst": "https://example.com/link",
+        "date": datetime.datetime(1980, 5, 9),
     }
     archive = [entry]
     ctx = {
-        'archive': archive,
+        "archive": archive,
     }
     result = archive_template.render(ctx)
-    assert 'site title' in result
+    assert "Archive" in result
 
-    assert 'this is a title' in result
-    assert '1980-05-09' in result
-    assert 'https://example.com/link' in result
+    assert "this is a title" in result
+    assert "1980-05-09" in result
+    assert "https://example.com/link" in result
 
 
 def test_tags(tags_template: Template) -> None:
-    tags = [('foo', 42)]
+    tags = [("foo", 42)]
     ctx = {
-        'tags': tags,
+        "tags": tags,
     }
     result = tags_template.render(ctx)
-    assert 'Tags' in result
+    assert "Tags" in result
 
-    assert 'foo.html' in result
-    assert 'foo' in result
-    assert '42' in result
+    assert "foo.html" in result
+    assert "foo" in result
+    assert "42" in result
 
 
 def test_tag(tag_template: Template) -> None:
     entry = {
-        'title': 'this is a title',
-        'dst': 'https://example.com/link',
-        'date': datetime.datetime(1980, 5, 9),
+        "title": "this is a title",
+        "dst": "https://example.com/link",
+        "date": datetime.datetime(1980, 5, 9),
     }
     archive = [entry]
     ctx = {
-        'tag': 'foo',
-        'archive': archive,
+        "tag": "foo",
+        "archive": archive,
     }
     result = tag_template.render(ctx)
-    assert 'Tag foo' in result
+    assert "foo" in result
 
-    assert 'this is a title' in result
-    assert '1980-05-09' in result
-    assert 'https://example.com/link' in result
+    assert "this is a title" in result
+    assert "1980-05-09" in result
+    assert "https://example.com/link" in result
```

