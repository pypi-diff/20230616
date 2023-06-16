# Comparing `tmp/FontCollector-2.1.0.tar.gz` & `tmp/FontCollector-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FontCollector-2.1.0.tar", last modified: Mon Mar 27 01:08:30 2023, max compression
+gzip compressed data, was "FontCollector-2.1.1.tar", last modified: Fri Jun 16 01:13:12 2023, max compression
```

## Comparing `FontCollector-2.1.0.tar` & `FontCollector-2.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 01:08:30.704796 FontCollector-2.1.0/
-drwxrwxrwx   0        0        0        0 2023-03-27 01:08:30.683870 FontCollector-2.1.0/FontCollector.egg-info/
--rw-rw-rw-   0        0        0     4765 2023-03-27 01:08:30.000000 FontCollector-2.1.0/FontCollector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2023-03-27 01:08:30.000000 FontCollector-2.1.0/FontCollector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 01:08:30.000000 FontCollector-2.1.0/FontCollector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-03-27 01:08:30.000000 FontCollector-2.1.0/FontCollector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2023-03-27 01:08:30.000000 FontCollector-2.1.0/FontCollector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-27 01:08:30.000000 FontCollector-2.1.0/FontCollector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-03-18 01:24:14.000000 FontCollector-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     4765 2023-03-27 01:08:30.703788 FontCollector-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3876 2023-03-27 00:41:02.000000 FontCollector-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 01:08:30.698803 FontCollector-2.1.0/font_collector/
--rw-rw-rw-   0        0        0     1149 2023-03-27 00:40:01.000000 FontCollector-2.1.0/font_collector/__init__.py
--rw-rw-rw-   0        0        0     2936 2023-03-27 00:42:58.000000 FontCollector-2.1.0/font_collector/__main__.py
--rw-rw-rw-   0        0        0       23 2023-03-27 00:40:01.000000 FontCollector-2.1.0/font_collector/_version.py
--rw-rw-rw-   0        0        0     8738 2023-02-26 01:44:56.000000 FontCollector-2.1.0/font_collector/ass_document.py
--rw-rw-rw-   0        0        0     1735 2023-01-02 02:08:59.000000 FontCollector-2.1.0/font_collector/ass_style.py
--rw-rw-rw-   0        0        0      205 2023-03-27 00:40:01.000000 FontCollector-2.1.0/font_collector/exceptions.py
--rw-rw-rw-   0        0        0    10064 2023-03-27 00:41:02.000000 FontCollector-2.1.0/font_collector/font.py
--rw-rw-rw-   0        0        0     6227 2023-03-27 00:23:44.000000 FontCollector-2.1.0/font_collector/font_loader.py
--rw-rw-rw-   0        0        0    22962 2023-03-27 01:07:59.000000 FontCollector-2.1.0/font_collector/font_parser.py
--rw-rw-rw-   0        0        0      510 2023-01-03 18:11:21.000000 FontCollector-2.1.0/font_collector/font_result.py
--rw-rw-rw-   0        0        0     7456 2023-03-27 00:40:01.000000 FontCollector-2.1.0/font_collector/helpers.py
--rw-rw-rw-   0        0        0     5387 2023-02-27 01:22:25.000000 FontCollector-2.1.0/font_collector/mkvpropedit.py
--rw-rw-rw-   0        0        0     3842 2023-01-26 18:34:43.000000 FontCollector-2.1.0/font_collector/parse_arguments.py
--rw-rw-rw-   0        0        0      692 2023-01-03 18:11:21.000000 FontCollector-2.1.0/font_collector/usage_data.py
--rw-rw-rw-   0        0        0       42 2023-03-27 01:08:30.704796 FontCollector-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2747 2023-03-27 00:40:01.000000 FontCollector-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-27 01:08:30.702791 FontCollector-2.1.0/tests/
--rw-rw-rw-   0        0        0      918 2023-01-22 16:04:34.000000 FontCollector-2.1.0/tests/test_ass_document.py
--rw-rw-rw-   0        0        0     8629 2023-03-27 00:40:01.000000 FontCollector-2.1.0/tests/test_font.py
--rw-rw-rw-   0        0        0     1037 2023-03-27 01:07:59.000000 FontCollector-2.1.0/tests/test_font_parser.py
--rw-rw-rw-   0        0        0      883 2023-01-22 16:04:34.000000 FontCollector-2.1.0/tests/test_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:13:12.740296 FontCollector-2.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-16 01:13:12.715363 FontCollector-2.1.1/FontCollector.egg-info/
+-rw-rw-rw-   0        0        0     4765 2023-06-16 01:13:12.000000 FontCollector-2.1.1/FontCollector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      745 2023-06-16 01:13:12.000000 FontCollector-2.1.1/FontCollector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 01:13:12.000000 FontCollector-2.1.1/FontCollector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-16 01:13:12.000000 FontCollector-2.1.1/FontCollector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       82 2023-06-16 01:13:12.000000 FontCollector-2.1.1/FontCollector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-16 01:13:12.000000 FontCollector-2.1.1/FontCollector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-03-18 01:24:14.000000 FontCollector-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4765 2023-06-16 01:13:12.740296 FontCollector-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3876 2023-03-27 00:41:02.000000 FontCollector-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 01:13:12.734313 FontCollector-2.1.1/font_collector/
+-rw-rw-rw-   0        0        0     1048 2023-06-16 01:05:57.000000 FontCollector-2.1.1/font_collector/__init__.py
+-rw-rw-rw-   0        0        0     2936 2023-03-27 00:42:58.000000 FontCollector-2.1.1/font_collector/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-06-16 01:01:23.000000 FontCollector-2.1.1/font_collector/_version.py
+-rw-rw-rw-   0        0        0     8738 2023-02-26 01:44:56.000000 FontCollector-2.1.1/font_collector/ass_document.py
+-rw-rw-rw-   0        0        0     1735 2023-01-02 02:08:59.000000 FontCollector-2.1.1/font_collector/ass_style.py
+-rw-rw-rw-   0        0        0      205 2023-03-27 00:40:01.000000 FontCollector-2.1.1/font_collector/exceptions.py
+-rw-rw-rw-   0        0        0    10064 2023-06-01 00:26:56.000000 FontCollector-2.1.1/font_collector/font.py
+-rw-rw-rw-   0        0        0     5933 2023-06-16 01:01:23.000000 FontCollector-2.1.1/font_collector/font_loader.py
+-rw-rw-rw-   0        0        0    22962 2023-06-12 21:16:42.000000 FontCollector-2.1.1/font_collector/font_parser.py
+-rw-rw-rw-   0        0        0      510 2023-01-03 18:11:21.000000 FontCollector-2.1.1/font_collector/font_result.py
+-rw-rw-rw-   0        0        0     7456 2023-06-16 00:45:55.000000 FontCollector-2.1.1/font_collector/helpers.py
+-rw-rw-rw-   0        0        0     5387 2023-02-27 01:22:25.000000 FontCollector-2.1.1/font_collector/mkvpropedit.py
+-rw-rw-rw-   0        0        0     3842 2023-01-26 18:34:43.000000 FontCollector-2.1.1/font_collector/parse_arguments.py
+-rw-rw-rw-   0        0        0      692 2023-01-03 18:11:21.000000 FontCollector-2.1.1/font_collector/usage_data.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 01:13:12.740296 FontCollector-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2762 2023-06-16 01:01:23.000000 FontCollector-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 01:13:12.739299 FontCollector-2.1.1/tests/
+-rw-rw-rw-   0        0        0      918 2023-01-22 16:04:34.000000 FontCollector-2.1.1/tests/test_ass_document.py
+-rw-rw-rw-   0        0        0     8629 2023-06-01 00:26:56.000000 FontCollector-2.1.1/tests/test_font.py
+-rw-rw-rw-   0        0        0     1037 2023-03-27 01:07:59.000000 FontCollector-2.1.1/tests/test_font_parser.py
+-rw-rw-rw-   0        0        0      902 2023-06-16 01:01:23.000000 FontCollector-2.1.1/tests/test_helpers.py
```

### Comparing `FontCollector-2.1.0/FontCollector.egg-info/PKG-INFO` & `FontCollector-2.1.1/FontCollector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FontCollector
-Version: 2.1.0
+Version: 2.1.1
 Summary: FontCollector for Advanced SubStation Alpha file.
 Home-page: https://github.com/moi15moi/FontCollector/
 Author: moi15moi
 Author-email: moi15moismokerlolilol@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FontCollector/
 Project-URL: Tracker, https://github.com/moi15moi/FontCollector/issues/
```

### Comparing `FontCollector-2.1.0/FontCollector.egg-info/SOURCES.txt` & `FontCollector-2.1.1/FontCollector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/LICENSE` & `FontCollector-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/PKG-INFO` & `FontCollector-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FontCollector
-Version: 2.1.0
+Version: 2.1.1
 Summary: FontCollector for Advanced SubStation Alpha file.
 Home-page: https://github.com/moi15moi/FontCollector/
 Author: moi15moi
 Author-email: moi15moismokerlolilol@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FontCollector/
 Project-URL: Tracker, https://github.com/moi15moi/FontCollector/issues/
```

### Comparing `FontCollector-2.1.0/README.md` & `FontCollector-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/font_collector/__init__.py` & `FontCollector-2.1.1/font_collector/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,19 +6,14 @@
 from .font_result import FontResult
 from .font import Font
 from .helpers import Helpers
 from .mkvpropedit import Mkvpropedit
 from .usage_data import UsageData
 from ._version import __version__
 
-# Set dependency log level to ERROR
-from matplotlib import set_loglevel
-
-set_loglevel("ERROR")
-
 from fontTools.misc.loggingTools import configLogger
 
 configLogger(level="ERROR")
 
 # Set our default logger
 _logger = logging.getLogger(__name__)
 _logger.setLevel(logging.INFO)
```

### Comparing `FontCollector-2.1.0/font_collector/__main__.py` & `FontCollector-2.1.1/font_collector/__main__.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/font_collector/ass_document.py` & `FontCollector-2.1.1/font_collector/ass_document.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/font_collector/ass_style.py` & `FontCollector-2.1.1/font_collector/ass_style.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/font_collector/font.py` & `FontCollector-2.1.1/font_collector/font.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/font_collector/font_loader.py` & `FontCollector-2.1.1/font_collector/font_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import pickle
 from .font import Font
-from matplotlib import font_manager
+from find_system_fonts_filename import get_system_fonts_filename
 from pathlib import Path
 from tempfile import gettempdir
 from typing import List, Set
 
 
 class FontLoader:
     """
@@ -56,15 +56,15 @@
         generated_fonts = FontLoader.load_generated_fonts()
         generated_fonts.add(font)
         FontLoader.save_generated_fonts(generated_fonts)
 
     @staticmethod
     def load_system_fonts() -> Set[Font]:
         system_fonts: Set[Font] = set()
-        fonts_paths: Set[str] = set(font_manager.findSystemFonts())
+        fonts_paths: Set[str] = get_system_fonts_filename()
         system_font_cache_file = FontLoader.get_system_font_cache_file_path()
 
         if os.path.exists(system_font_cache_file):
 
             with open(system_font_cache_file, "rb") as file:
                 cached_fonts: Set[Font] = pickle.load(file)
 
@@ -75,33 +75,25 @@
             system_fonts = set(
                 filter(lambda font: font.filename not in removed, cached_fonts)
             )
 
             # Add font that have been installed since last execution
             added = fonts_paths.difference(cached_paths)
             for font_path in added:
-                try:
-                    system_fonts.update(Font.from_font_path(font_path))
-                except FileExistsError:
-                    # matplotlib can sometimes returns file that aren't font: "C:\WINDOWS\Fonts\desktop.ini"
-                    continue
+                system_fonts.update(Font.from_font_path(font_path))
 
             # If there is a change, update the cache file
             if len(added) > 0 or len(removed) > 0:
                 with open(system_font_cache_file, "wb") as file:
                     pickle.dump(system_fonts, file)
 
         else:
             # Since there is no cache file, load the font
             for font_path in fonts_paths:
-                try:
-                    system_fonts.update(Font.from_font_path(font_path))
-                except FileExistsError:
-                    # matplotlib can sometimes returns file that aren't font: "C:\WINDOWS\Fonts\desktop.ini"
-                    continue
+                system_fonts.update(Font.from_font_path(font_path))
 
             # Save the font into the cache file
             with open(system_font_cache_file, "wb") as file:
                 pickle.dump(system_fonts, file)
 
         return system_fonts
 
@@ -124,16 +116,17 @@
     def load_additional_fonts(additional_fonts_path: List[Path]) -> Set[Font]:
         additional_fonts: Set[Font] = set()
 
         for font_path in additional_fonts_path:
             if os.path.isfile(font_path):
                 additional_fonts.update(Font.from_font_path(font_path))
             elif os.path.isdir(font_path):
-                for path in font_manager.findSystemFonts(fontpaths=str(font_path)):
-                    additional_fonts.update(Font.from_font_path(path))
+                for file in os.listdir(font_path):
+                    if Path(file).suffix.lstrip(".").strip().lower() in ["ttf", "otf", "ttc", "otc"]:
+                        additional_fonts.update(Font.from_font_path(os.path.join(font_path, file)))
             else:
                 raise FileNotFoundError(f"The file {font_path} is not reachable")
         return additional_fonts
 
     @staticmethod
     def save_generated_fonts(generated_fonts: Set[Font]):
         generated_font_cache_file = FontLoader.get_generated_font_cache_file_path()
```

### Comparing `FontCollector-2.1.0/font_collector/font_parser.py` & `FontCollector-2.1.1/font_collector/font_parser.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/font_collector/helpers.py` & `FontCollector-2.1.1/font_collector/helpers.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/font_collector/mkvpropedit.py` & `FontCollector-2.1.1/font_collector/mkvpropedit.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/font_collector/parse_arguments.py` & `FontCollector-2.1.1/font_collector/parse_arguments.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/font_collector/usage_data.py` & `FontCollector-2.1.1/font_collector/usage_data.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/setup.py` & `FontCollector-2.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     packages=["font_collector"],
     python_requires=">=3.8",
     install_requires=[
         "ass",
         "ass-tag-analyzer",
         "fontTools>=4.38.0",
         "freetype-py",
-        "matplotlib>=3.6",
+        "FindSystemFontsFilename>=0.1.1",
     ],
     entry_points={"console_scripts": ["fontcollector=font_collector.__main__:main"]},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Other Audience",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

### Comparing `FontCollector-2.1.0/tests/test_ass_document.py` & `FontCollector-2.1.1/tests/test_ass_document.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/tests/test_font.py` & `FontCollector-2.1.1/tests/test_font.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/tests/test_font_parser.py` & `FontCollector-2.1.1/tests/test_font_parser.py`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.0/tests/test_helpers.py` & `FontCollector-2.1.1/tests/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     styles = subtitle.get_used_style()
     styles = list(styles.keys())
 
     assert len(styles) == 1
 
     style = styles[0]
     font_collection = FontLoader(
-        [os.path.join(dir_path, "fonts", "Raleway")], False
+        [os.path.join(dir_path, "fonts", "Raleway", "generated_fonts")], False
     ).fonts
 
     font_result = Helpers.get_used_font_by_style(font_collection, style)
 
     # VSFilter prefer to match to the weight then the italic.
     # If it would have prefer to match the italic, the weight would be 700 and italic would be true.
     assert font_result.font.weight == 900
```

