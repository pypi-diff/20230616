# Comparing `tmp/screenshotgenerator-0.3.1.tar.gz` & `tmp/screenshotgenerator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenshotgenerator-0.3.1.tar", last modified: Sat Apr  1 21:43:46 2023, max compression
+gzip compressed data, was "screenshotgenerator-0.4.0.tar", last modified: Fri Jun 16 03:08:33 2023, max compression
```

## Comparing `screenshotgenerator-0.3.1.tar` & `screenshotgenerator-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 21:43:46.001675 screenshotgenerator-0.3.1/
--rw-rw-rw-   0        0        0     1076 2023-03-29 21:44:24.000000 screenshotgenerator-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     6033 2023-04-01 21:43:46.255672 screenshotgenerator-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5314 2023-04-01 21:43:23.000000 screenshotgenerator-0.3.1/README.md
--rw-rw-rw-   0        0        0      938 2023-04-01 21:43:36.000000 screenshotgenerator-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-01 21:43:46.259648 screenshotgenerator-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-01 21:43:45.957999 screenshotgenerator-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-01 21:43:46.141801 screenshotgenerator-0.3.1/src/screenshotgenerator/
--rw-rw-rw-   0        0        0      119 2023-03-30 20:05:46.000000 screenshotgenerator-0.3.1/src/screenshotgenerator/__init__.py
--rw-rw-rw-   0        0        0     4065 2023-04-01 20:20:40.000000 screenshotgenerator-0.3.1/src/screenshotgenerator/cli.py
--rw-rw-rw-   0        0        0      370 2023-03-30 17:00:45.000000 screenshotgenerator-0.3.1/src/screenshotgenerator/click_enum_type.py
--rw-rw-rw-   0        0        0      540 2023-04-01 21:31:28.000000 screenshotgenerator-0.3.1/src/screenshotgenerator/defaults.py
--rw-rw-rw-   0        0        0     6269 2023-04-01 21:35:13.000000 screenshotgenerator-0.3.1/src/screenshotgenerator/generate.py
--rw-rw-rw-   0        0        0      136 2023-03-29 22:50:57.000000 screenshotgenerator-0.3.1/src/screenshotgenerator/portrait_preference.py
--rw-rw-rw-   0        0        0      286 2023-03-29 18:38:42.000000 screenshotgenerator-0.3.1/src/screenshotgenerator/screenshot.py
-drwxrwxrwx   0        0        0        0 2023-04-01 21:43:46.241783 screenshotgenerator-0.3.1/src/screenshotgenerator.egg-info/
--rw-rw-rw-   0        0        0     6033 2023-04-01 21:43:45.000000 screenshotgenerator-0.3.1/src/screenshotgenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-04-01 21:43:45.000000 screenshotgenerator-0.3.1/src/screenshotgenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 21:43:45.000000 screenshotgenerator-0.3.1/src/screenshotgenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-04-01 21:43:45.000000 screenshotgenerator-0.3.1/src/screenshotgenerator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-04-01 21:43:45.000000 screenshotgenerator-0.3.1/src/screenshotgenerator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-01 21:43:45.000000 screenshotgenerator-0.3.1/src/screenshotgenerator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 03:08:33.142717 screenshotgenerator-0.4.0/
+-rw-rw-rw-   0        0        0     1076 2023-03-29 21:44:24.000000 screenshotgenerator-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     9488 2023-06-16 03:08:33.144709 screenshotgenerator-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8769 2023-06-16 03:01:55.000000 screenshotgenerator-0.4.0/README.md
+-rw-rw-rw-   0        0        0     1024 2023-06-16 01:31:37.000000 screenshotgenerator-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 03:08:33.155727 screenshotgenerator-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 03:08:32.848890 screenshotgenerator-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 03:08:33.021778 screenshotgenerator-0.4.0/src/screenshotgenerator/
+-rw-rw-rw-   0        0        0      147 2023-06-16 02:52:12.000000 screenshotgenerator-0.4.0/src/screenshotgenerator/__init__.py
+-rw-rw-rw-   0        0        0      370 2023-03-30 17:00:45.000000 screenshotgenerator-0.4.0/src/screenshotgenerator/click_enum_type.py
+-rw-rw-rw-   0        0        0      352 2023-06-16 02:52:01.000000 screenshotgenerator-0.4.0/src/screenshotgenerator/common.py
+-rw-rw-rw-   0        0        0      540 2023-04-01 21:31:28.000000 screenshotgenerator-0.4.0/src/screenshotgenerator/defaults.py
+-rw-rw-rw-   0        0        0     3081 2023-06-16 02:41:43.000000 screenshotgenerator-0.4.0/src/screenshotgenerator/generate.py
+-rw-rw-rw-   0        0        0      136 2023-03-29 22:50:57.000000 screenshotgenerator-0.4.0/src/screenshotgenerator/portrait_preference.py
+-rw-rw-rw-   0        0        0      286 2023-03-29 18:38:42.000000 screenshotgenerator-0.4.0/src/screenshotgenerator/screenshot.py
+-rw-rw-rw-   0        0        0     3860 2023-06-16 02:52:46.000000 screenshotgenerator-0.4.0/src/screenshotgenerator/screenshotgenerator.py
+-rw-rw-rw-   0        0        0     2743 2023-06-16 02:59:39.000000 screenshotgenerator-0.4.0/src/screenshotgenerator/screenshotselector.py
+-rw-rw-rw-   0        0        0     4254 2023-06-16 02:41:43.000000 screenshotgenerator-0.4.0/src/screenshotgenerator/select.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:08:33.129930 screenshotgenerator-0.4.0/src/screenshotgenerator.egg-info/
+-rw-rw-rw-   0        0        0     9488 2023-06-16 03:08:32.000000 screenshotgenerator-0.4.0/src/screenshotgenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-06-16 03:08:32.000000 screenshotgenerator-0.4.0/src/screenshotgenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 03:08:32.000000 screenshotgenerator-0.4.0/src/screenshotgenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2023-06-16 03:08:32.000000 screenshotgenerator-0.4.0/src/screenshotgenerator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-06-16 03:08:32.000000 screenshotgenerator-0.4.0/src/screenshotgenerator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-16 03:08:32.000000 screenshotgenerator-0.4.0/src/screenshotgenerator.egg-info/top_level.txt
```

### Comparing `screenshotgenerator-0.3.1/LICENSE` & `screenshotgenerator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `screenshotgenerator-0.3.1/pyproject.toml` & `screenshotgenerator-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "screenshotgenerator"
-version = "0.3.1"
+version = "0.4.0"
 authors = [
   { name="jonbenta" },
 ]
 description = "A library for automatically generating and selecting video screenshots."
 readme = "README.md"
 requires-python = ">=3.8, <3.11"
 dependencies = ["autogluon", "click", "gdown", "platformdirs", "pymediainfo"]
@@ -18,12 +18,13 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Multimedia :: Video",
     "Topic :: Scientific/Engineering :: Image Recognition",
 ]
 
 [project.scripts]
-"screenshotgenerator" = "screenshotgenerator.cli:main"
+"screenshotgenerator" = "screenshotgenerator.screenshotgenerator:main"
+"screenshotselector" = "screenshotgenerator.screenshotselector:main"
 
 [project.urls]
 "Homepage" = "https://github.com/jonbenta/ScreenshotGenerator"
 "Bug Tracker" = "https://github.com/jonbenta/ScreenshotGenerator/issues"
```

### Comparing `screenshotgenerator-0.3.1/src/screenshotgenerator/cli.py` & `screenshotgenerator-0.4.0/src/screenshotgenerator/screenshotgenerator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from __future__ import annotations
 import click
-import json
 from datetime import datetime
 
 from .click_enum_type import EnumType
+from .common import write_pool_report
 from .defaults import Defaults
 from .generate import generate
 from .portrait_preference import PortraitPreference
 from .screenshot import Screenshot
 
 @click.command()
 @click.option("--end-time",
@@ -81,16 +82,9 @@
         screenshot_directory=screenshot_directory,
         silent=silent,
         start_time=start_time,
         video_path=video_path)
 
     write_pool_report(pool_report_path, sorted_screenshots)
 
-def write_pool_report(report_path: str, sorted_screenshots: list[Screenshot]):
-    if not report_path:
-        return
-    
-    with open(report_path, "w") as pool_list_file:
-        pool_list_file.write(json.dumps(sorted_screenshots, indent=4, default=vars))
-
 if __name__ == "__main__":
     main()
```

### Comparing `screenshotgenerator-0.3.1/src/screenshotgenerator/defaults.py` & `screenshotgenerator-0.4.0/src/screenshotgenerator/defaults.py`

 * *Files identical despite different names*

### Comparing `screenshotgenerator-0.3.1/src/screenshotgenerator.egg-info/SOURCES.txt` & `screenshotgenerator-0.4.0/src/screenshotgenerator.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 LICENSE
 README.md
 pyproject.toml
 src/screenshotgenerator/__init__.py
-src/screenshotgenerator/cli.py
 src/screenshotgenerator/click_enum_type.py
+src/screenshotgenerator/common.py
 src/screenshotgenerator/defaults.py
 src/screenshotgenerator/generate.py
 src/screenshotgenerator/portrait_preference.py
 src/screenshotgenerator/screenshot.py
+src/screenshotgenerator/screenshotgenerator.py
+src/screenshotgenerator/screenshotselector.py
+src/screenshotgenerator/select.py
 src/screenshotgenerator.egg-info/PKG-INFO
 src/screenshotgenerator.egg-info/SOURCES.txt
 src/screenshotgenerator.egg-info/dependency_links.txt
 src/screenshotgenerator.egg-info/entry_points.txt
 src/screenshotgenerator.egg-info/requires.txt
 src/screenshotgenerator.egg-info/top_level.txt
```

