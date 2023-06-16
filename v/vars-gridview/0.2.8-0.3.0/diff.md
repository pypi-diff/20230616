# Comparing `tmp/vars_gridview-0.2.8.tar.gz` & `tmp/vars_gridview-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vars_gridview-0.2.8.tar", max compression
+gzip compressed data, was "vars_gridview-0.3.0.tar", max compression
```

## Comparing `vars_gridview-0.2.8.tar` & `vars_gridview-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1104 2023-02-03 23:02:37.185892 vars_gridview-0.2.8/LICENSE
--rw-r--r--   0        0        0     1194 2023-02-03 23:04:10.385326 vars_gridview-0.2.8/README.md
--rw-r--r--   0        0        0      862 2023-06-13 17:16:13.762346 vars_gridview-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.2.8/vars_gridview/__init__.py
--rw-r--r--   0        0        0      865 2023-03-22 18:43:10.077134 vars_gridview-0.2.8/vars_gridview/assets/base_query.sql
--rw-r--r--   0        0        0    24010 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/assets/gridview.ui
--rw-r--r--   0        0        0    31829 2023-02-03 23:02:37.185892 vars_gridview-0.2.8/vars_gridview/assets/style/dark.qss
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.2.8/vars_gridview/lib/__init__.py
--rw-r--r--   0        0        0     4963 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/annotation.py
--rw-r--r--   0        0        0     6242 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/boxes.py
--rw-r--r--   0        0        0      633 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/constants.py
--rw-r--r--   0        0        0    28311 2023-06-13 17:16:13.762346 vars_gridview-0.2.8/vars_gridview/lib/image_mosaic.py
--rw-r--r--   0        0        0     1733 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/log.py
--rw-r--r--   0        0        0     1680 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/m3/__init__.py
--rw-r--r--   0        0        0     5174 2023-06-13 16:10:14.348688 vars_gridview-0.2.8/vars_gridview/lib/m3/clients.py
--rw-r--r--   0        0        0     7188 2023-06-13 16:10:14.348688 vars_gridview-0.2.8/vars_gridview/lib/m3/operations.py
--rw-r--r--   0        0        0      729 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/raziel.py
--rw-r--r--   0        0        0     2645 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/settings.py
--rw-r--r--   0        0        0     3815 2023-06-12 16:29:02.472896 vars_gridview-0.2.8/vars_gridview/lib/sort_methods.py
--rw-r--r--   0        0        0     3008 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/sql.py
--rw-r--r--   0        0        0     1887 2023-06-12 16:29:22.672801 vars_gridview-0.2.8/vars_gridview/lib/util.py
--rw-r--r--   0        0        0    10361 2023-06-13 17:16:13.762346 vars_gridview-0.2.8/vars_gridview/lib/widgets.py
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.2.8/vars_gridview/scripts/__init__.py
--rw-r--r--   0        0        0    22075 2023-06-13 17:16:13.762346 vars_gridview-0.2.8/vars_gridview/scripts/run.py
--rw-r--r--   0        0        0     2932 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/ui/LoginDialog.py
--rw-r--r--   0        0        0    16306 2023-03-22 18:43:10.077134 vars_gridview-0.2.8/vars_gridview/ui/QueryDialog.py
--rw-r--r--   0        0        0        0 2023-02-17 22:27:04.735716 vars_gridview-0.2.8/vars_gridview/ui/__init__.py
--rw-r--r--   0        0        0     2790 2023-02-17 22:27:04.735716 vars_gridview-0.2.8/vars_gridview/ui/settings/SettingsDialog.py
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.2.8/vars_gridview/ui/settings/__init__.py
--rw-r--r--   0        0        0      822 2023-02-17 22:27:04.735716 vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
--rw-r--r--   0        0        0      710 2023-02-17 22:27:04.735716 vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/M3Tab.py
--rw-r--r--   0        0        0     2004 2023-02-17 22:27:04.735716 vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/SQLTab.py
--rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/__init__.py
--rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 vars_gridview-0.2.8/setup.py
--rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 vars_gridview-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1104 2023-02-03 23:02:37.185892 vars_gridview-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1194 2023-02-03 23:04:10.385326 vars_gridview-0.3.0/README.md
+-rw-r--r--   0        0        0      891 2023-06-16 00:39:48.645233 vars_gridview-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.3.0/vars_gridview/__init__.py
+-rw-r--r--   0        0        0      865 2023-03-22 18:43:10.077134 vars_gridview-0.3.0/vars_gridview/assets/base_query.sql
+-rw-r--r--   0        0        0    24010 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/assets/gridview.ui
+-rw-r--r--   0        0        0    31829 2023-02-03 23:02:37.185892 vars_gridview-0.3.0/vars_gridview/assets/style/dark.qss
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.3.0/vars_gridview/lib/__init__.py
+-rw-r--r--   0        0        0     4963 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/annotation.py
+-rw-r--r--   0        0        0     6242 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/boxes.py
+-rw-r--r--   0        0        0      633 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/constants.py
+-rw-r--r--   0        0        0    28311 2023-06-13 17:16:13.762346 vars_gridview-0.3.0/vars_gridview/lib/image_mosaic.py
+-rw-r--r--   0        0        0     1733 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/log.py
+-rw-r--r--   0        0        0     1680 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/m3/__init__.py
+-rw-r--r--   0        0        0     5174 2023-06-13 16:10:14.348688 vars_gridview-0.3.0/vars_gridview/lib/m3/clients.py
+-rw-r--r--   0        0        0     7188 2023-06-13 16:10:14.348688 vars_gridview-0.3.0/vars_gridview/lib/m3/operations.py
+-rw-r--r--   0        0        0      729 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/raziel.py
+-rw-r--r--   0        0        0     2645 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/settings.py
+-rw-r--r--   0        0        0     3815 2023-06-12 16:29:02.472896 vars_gridview-0.3.0/vars_gridview/lib/sort_methods.py
+-rw-r--r--   0        0        0     3008 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/lib/sql.py
+-rw-r--r--   0        0        0     1887 2023-06-12 16:29:22.672801 vars_gridview-0.3.0/vars_gridview/lib/util.py
+-rw-r--r--   0        0        0    10361 2023-06-13 17:16:13.762346 vars_gridview-0.3.0/vars_gridview/lib/widgets.py
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.0/vars_gridview/scripts/__init__.py
+-rw-r--r--   0        0        0    24463 2023-06-16 00:39:48.645233 vars_gridview-0.3.0/vars_gridview/scripts/run.py
+-rw-r--r--   0        0        0     2932 2023-02-17 22:27:04.731716 vars_gridview-0.3.0/vars_gridview/ui/LoginDialog.py
+-rw-r--r--   0        0        0    16306 2023-03-22 18:43:10.077134 vars_gridview-0.3.0/vars_gridview/ui/QueryDialog.py
+-rw-r--r--   0        0        0        0 2023-02-17 22:27:04.735716 vars_gridview-0.3.0/vars_gridview/ui/__init__.py
+-rw-r--r--   0        0        0     2790 2023-02-17 22:27:04.735716 vars_gridview-0.3.0/vars_gridview/ui/settings/SettingsDialog.py
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.0/vars_gridview/ui/settings/__init__.py
+-rw-r--r--   0        0        0      822 2023-02-17 22:27:04.735716 vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
+-rw-r--r--   0        0        0      710 2023-02-17 22:27:04.735716 vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/M3Tab.py
+-rw-r--r--   0        0        0     2004 2023-02-17 22:27:04.735716 vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/SQLTab.py
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/__init__.py
+-rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 vars_gridview-0.3.0/setup.py
+-rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 vars_gridview-0.3.0/PKG-INFO
```

### Comparing `vars_gridview-0.2.8/LICENSE` & `vars_gridview-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/README.md` & `vars_gridview-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/pyproject.toml` & `vars_gridview-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vars-gridview"
-version = "0.2.8"
+version = "0.3.0"
 description = "VARS GridView is a tool for reviewing and correcting VARS localizations in bulk."
 authors = [
     "Kevin Barnard <kbarnard@mbari.org>",
     "Paul Roberts <proberts@mbari.org>"
 ]
 readme = "README.md"
 repository = "https://github.com/mbari-org/vars-gridview"
@@ -17,14 +17,15 @@
 pyqt6 = "^6.4.0"
 pymssql = "^2.2.4"
 requests = "^2.27.1"
 pyqtgraph = "^0.13.0"
 opencv-python-headless = "^4.5.5.62"
 qdarkstyle = "^3.0.3"
 beholder-client = "^0.1.0"
+sharktopoda-client = "0.4.0"
 
 [tool.poetry.scripts]
 vars-gridview = "vars_gridview.scripts.run:main"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
```

### Comparing `vars_gridview-0.2.8/vars_gridview/assets/base_query.sql` & `vars_gridview-0.3.0/vars_gridview/assets/base_query.sql`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/assets/gridview.ui` & `vars_gridview-0.3.0/vars_gridview/assets/gridview.ui`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/assets/style/dark.qss` & `vars_gridview-0.3.0/vars_gridview/assets/style/dark.qss`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/annotation.py` & `vars_gridview-0.3.0/vars_gridview/lib/annotation.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/boxes.py` & `vars_gridview-0.3.0/vars_gridview/lib/boxes.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/constants.py` & `vars_gridview-0.3.0/vars_gridview/lib/constants.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/image_mosaic.py` & `vars_gridview-0.3.0/vars_gridview/lib/image_mosaic.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/log.py` & `vars_gridview-0.3.0/vars_gridview/lib/log.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/m3/__init__.py` & `vars_gridview-0.3.0/vars_gridview/lib/m3/__init__.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/m3/clients.py` & `vars_gridview-0.3.0/vars_gridview/lib/m3/clients.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/m3/operations.py` & `vars_gridview-0.3.0/vars_gridview/lib/m3/operations.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/raziel.py` & `vars_gridview-0.3.0/vars_gridview/lib/raziel.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/settings.py` & `vars_gridview-0.3.0/vars_gridview/lib/settings.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/sort_methods.py` & `vars_gridview-0.3.0/vars_gridview/lib/sort_methods.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/sql.py` & `vars_gridview-0.3.0/vars_gridview/lib/sql.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/util.py` & `vars_gridview-0.3.0/vars_gridview/lib/util.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/lib/widgets.py` & `vars_gridview-0.3.0/vars_gridview/lib/widgets.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/scripts/run.py` & `vars_gridview-0.3.0/vars_gridview/scripts/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,32 +16,35 @@
 http://synapses.awardspace.info/pages-scripts/python/pages/python-pyqt_qgraphicsview-thumbnails-grid.py.html
 """
 
 import datetime
 import json
 import os
 import sys
+from time import sleep
+from uuid import UUID, uuid4
 import webbrowser
 from pathlib import Path
 from typing import Optional, Tuple
 
 import cv2
 import pyqtgraph as pg
 import qdarkstyle
+from sharktopoda_client.client import SharktopodaClient
+from sharktopoda_client.dto import Localization
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 from vars_gridview.lib import constants, m3, raziel, sql
 from vars_gridview.lib.boxes import BoxHandler
 from vars_gridview.lib.image_mosaic import ImageMosaic
 from vars_gridview.lib.log import LOGGER
 from vars_gridview.lib.m3.operations import (
     get_kb_concepts,
     get_kb_parts,
     get_vars_imaged_moment,
-    get_videos_at_datetime,
 )
 from vars_gridview.lib.settings import SettingsManager
 from vars_gridview.lib.sort_methods import (
     AreaSort,
     AssociationUUIDSort,
     DepthSort,
     HeightSort,
@@ -115,14 +118,17 @@
             None  # Image mosaic (holds the thumbnails as a grid of RectWidgets)
         )
         self.box_handler = None  # Box handler (handles the ROIs and annotations)
 
         self.cached_moment_concepts = (
             {}
         )  # Cache for imaged moment -> set of observed concepts
+        
+        self.sharktopoda_client = None  # Sharktopoda client
+        self.sharktopoda_connected = False  # Whether the Sharktopoda client is connected
 
         # Connect signals to slots
         self.ui.discardButton.clicked.connect(self.delete)
         self.ui.clearSelections.clicked.connect(self.clear_selected)
         self.ui.labelSelectedButton.clicked.connect(self.update_labels)
         self.ui.zoomSpinBox.valueChanged.connect(self.update_zoom)
         self.ui.sortMethod.currentTextChanged.connect(self.update_layout)
@@ -155,14 +161,17 @@
         self._setup_label_boxes()
 
         # Set up the sort method combo box
         self._setup_sort_methods()
 
         # Set up the menu bar
         self._setup_menu_bar()
+        
+        # Set up Sharktopoda client
+        self._setup_sharktopoda_client()
 
         LOGGER.info("Launch successful")
 
     def _get_login(self) -> Optional[Tuple[str, str, str]]:
         """
         Prompt a login dialog and return the username, password, and Raziel URL. If failed, returns None.
         """
@@ -255,14 +264,27 @@
 
         query_menu = menu_bar.addMenu("&Query")
 
         query_action = QtGui.QAction("&Query", self)
         query_action.setShortcut("Ctrl+Q")
         query_action.triggered.connect(self._do_query)
         query_menu.addAction(query_action)
+    
+    def _setup_sharktopoda_client(self):
+        """
+        Create the Sharktopoda video player client.
+        """
+        self.sharktopoda_client = SharktopodaClient("::1", 8800, 8801)
+        ok = self.sharktopoda_client.connect()
+        self.sharktopoda_connected = ok
+        
+        if not ok:
+            LOGGER.error("Failed to connect to Sharktopoda")
+            QtWidgets.QMessageBox.critical(self, "Sharktopoda connection failed", "Failed to connect to Sharktopoda. Falling back on web browser player.")
+            return
 
     def _open_settings(self):
         """
         Open the settings dialog.
         """
         self.settings_dialog.show()
 
@@ -532,17 +554,19 @@
     def open_video(self):
         """
         Open the video of the last selected ROI, if available
         """
         if not self.last_selected_rect:
             QtWidgets.QMessageBox.warning(self, "No ROI Selected", "No ROI selected.")
             return
+        
+        rect = self.last_selected_rect
 
         # Get the annotation imaged moment UUID
-        imaged_moment_uuid = self.last_selected_rect.imaged_moment_uuid
+        imaged_moment_uuid = rect.imaged_moment_uuid
         
         # Get the annotation MP4 video data
         mp4_video_data = self.image_mosaic.moment_mp4_data.get(imaged_moment_uuid, None)
         if mp4_video_data is None:
             QtWidgets.QMessageBox.warning(
                 self, "Missing Video", "ROI lacks MP4 video."
             )
@@ -556,20 +580,55 @@
 
         # Get the annotation timestamp
         annotation_datetime = self.image_mosaic.moment_timestamps[imaged_moment_uuid]
 
         # Compute the timedelta between the annotation and video start
         annotation_timedelta = annotation_datetime - mp4_start_timestamp
 
-        # Open the MP4 video at the computed timedelta (in seconds)
-        annotation_seconds = max(annotation_timedelta.total_seconds(), 0)
-        url = mp4_video_url + "#t={},{}".format(
-            annotation_seconds, annotation_seconds + 1e-3
-        )  # "pause" at the annotation
-        webbrowser.open(url)
+        if not self.sharktopoda_connected:
+            # Open the MP4 video at the computed timedelta (in seconds)
+            annotation_seconds = max(annotation_timedelta.total_seconds(), 0)
+            url = mp4_video_url + "#t={},{}".format(
+                annotation_seconds, annotation_seconds + 1e-3
+            )  # "pause" at the annotation
+            webbrowser.open(url)
+            return
+        
+        # Open the video in Sharktopoda 2
+        annotation_milliseconds = max(annotation_timedelta.total_seconds() * 1000, 0)
+        video_reference_uuid = UUID(mp4_video_reference["uuid"])
+        
+        def color_for_concept(concept: str):
+            hash = sum(map(ord, concept)) << 5
+            color = QtGui.QColor()
+            color.setHsl(round((hash % 360) / 360 * 255), 255, 217, 255)
+            return color
+        
+        localization = Localization(
+            uuid=uuid4(),
+            concept=rect.localization.concept,
+            elapsed_time_millis=annotation_milliseconds,
+            x=rect.localization.x,
+            y=rect.localization.y,
+            width=rect.localization.width,
+            height=rect.localization.height,
+            duration_millis=1000,
+            color=color_for_concept(rect.localization.concept).name()
+        )
+        
+        def show_localization():
+            self.sharktopoda_client.seek_elapsed_time(video_reference_uuid, annotation_milliseconds)
+            self.sharktopoda_client.clear_localizations(video_reference_uuid)
+            self.sharktopoda_client.add_localizations(video_reference_uuid, [localization])
+        
+        self.sharktopoda_client.open(
+            video_reference_uuid, 
+            mp4_video_url, 
+            callback=show_localization
+        )
 
     @QtCore.pyqtSlot()
     def _style_gui(self):
         """
         Set the GUI stylesheet.
         """
         # setup stylesheet
```

### Comparing `vars_gridview-0.2.8/vars_gridview/ui/LoginDialog.py` & `vars_gridview-0.3.0/vars_gridview/ui/LoginDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/ui/QueryDialog.py` & `vars_gridview-0.3.0/vars_gridview/ui/QueryDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/ui/settings/SettingsDialog.py` & `vars_gridview-0.3.0/vars_gridview/ui/settings/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py` & `vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/M3Tab.py` & `vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/M3Tab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/SQLTab.py` & `vars_gridview-0.3.0/vars_gridview/ui/settings/tabs/SQLTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.8/setup.py` & `vars_gridview-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 install_requires = \
 ['beholder-client>=0.1.0,<0.2.0',
  'opencv-python-headless>=4.5.5.62,<5.0.0.0',
  'pymssql>=2.2.4,<3.0.0',
  'pyqt6>=6.4.0,<7.0.0',
  'pyqtgraph>=0.13.0,<0.14.0',
  'qdarkstyle>=3.0.3,<4.0.0',
- 'requests>=2.27.1,<3.0.0']
+ 'requests>=2.27.1,<3.0.0',
+ 'sharktopoda-client==0.4.0']
 
 entry_points = \
 {'console_scripts': ['vars-gridview = vars_gridview.scripts.run:main']}
 
 setup_kwargs = {
     'name': 'vars-gridview',
-    'version': '0.2.8',
+    'version': '0.3.0',
     'description': 'VARS GridView is a tool for reviewing and correcting VARS localizations in bulk.',
     'long_description': '# vars-gridview\n\n**VARS GridView** is a tool for reviewing and correcting VARS localizations in bulk.\n\n[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)\n[![Python](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/downloads/)\n\nAuthors: Kevin Barnard ([kbarnard@mbari.org](mailto:kbarnard@mbari.org)), Paul Roberts ([proberts@mbari.org](mailto:proberts@mbari.org))\n\n---\n\n## Install\n\n### From PyPI\n\nVARS GridView is available on PyPI as `vars-gridview`. To install, run:\n\n```bash\npip install vars-gridview\n```\n\n### From source\n\nThis project is built with [Poetry](https://python-poetry.org/). To install from source, run (in the project root):\n\n```bash\npoetry install\n```\n\n## Run\n\nOnce VARS GridView is installed, you can run it from the command line:\n\n```bash\nvars-gridview\n```\n\nYou will first be prompted to log in. Enter your VARS username and password. \n\n*Note: If you are not using MBARI production VARS, change the "Config server" field to point to your instance of Raziel. This setting is persisted.*\n\n---\n\nCopyright &copy; 2020&ndash;2023 [Monterey Bay Aquarium Research Institute](https://www.mbari.org)',
     'author': 'Kevin Barnard',
     'author_email': 'kbarnard@mbari.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mbari-org/vars-gridview',
```

### Comparing `vars_gridview-0.2.8/PKG-INFO` & `vars_gridview-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vars-gridview
-Version: 0.2.8
+Version: 0.3.0
 Summary: VARS GridView is a tool for reviewing and correcting VARS localizations in bulk.
 Home-page: https://github.com/mbari-org/vars-gridview
 License: MIT
 Keywords: VARS,localization,annotation
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Requires-Python: >=3.8,<4.0
@@ -17,14 +17,15 @@
 Requires-Dist: beholder-client (>=0.1.0,<0.2.0)
 Requires-Dist: opencv-python-headless (>=4.5.5.62,<5.0.0.0)
 Requires-Dist: pymssql (>=2.2.4,<3.0.0)
 Requires-Dist: pyqt6 (>=6.4.0,<7.0.0)
 Requires-Dist: pyqtgraph (>=0.13.0,<0.14.0)
 Requires-Dist: qdarkstyle (>=3.0.3,<4.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: sharktopoda-client (==0.4.0)
 Project-URL: Repository, https://github.com/mbari-org/vars-gridview
 Description-Content-Type: text/markdown
 
 # vars-gridview
 
 **VARS GridView** is a tool for reviewing and correcting VARS localizations in bulk.
```

