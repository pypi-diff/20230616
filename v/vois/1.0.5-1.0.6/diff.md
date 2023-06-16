# Comparing `tmp/vois-1.0.5.tar.gz` & `tmp/vois-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vois-1.0.5.tar", last modified: Tue Jun 13 09:32:16 2023, max compression
+gzip compressed data, was "vois-1.0.6.tar", last modified: Fri Jun 16 10:50:19 2023, max compression
```

## Comparing `vois-1.0.5.tar` & `vois-1.0.6.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 09:32:16.053506 vois-1.0.5/
--rw-rw-rw-   0        0        0    14155 2023-06-09 08:06:09.000000 vois-1.0.5/LICENCE
--rw-rw-rw-   0        0        0      631 2023-06-09 16:48:21.000000 vois-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    73887 2023-06-09 08:06:09.000000 vois-1.0.5/Notice.txt
--rw-rw-rw-   0        0        0    19318 2023-06-13 09:32:16.052506 vois-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1511 2023-06-13 09:22:47.000000 vois-1.0.5/README.md
--rw-rw-rw-   0        0        0     6089 2023-06-13 09:25:30.000000 vois-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 09:32:16.053506 vois-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 09:32:14.878835 vois-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 09:32:15.267584 vois-1.0.5/src/vois/
--rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/__init__.py
--rw-rw-rw-   0        0        0    11918 2023-06-09 16:34:04.000000 vois-1.0.5/src/vois/colors.py
--rw-rw-rw-   0        0        0     4168 2023-06-09 16:34:04.000000 vois-1.0.5/src/vois/download.py
--rw-rw-rw-   0        0        0    17916 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/eucountries.py
--rw-rw-rw-   0        0        0    10493 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/geojsonUtils.py
--rw-rw-rw-   0        0        0    66667 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/interMap.py
--rw-rw-rw-   0        0        0     9302 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/ipytrees.py
--rw-rw-rw-   0        0        0    35732 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/leafletMap.py
--rw-rw-rw-   0        0        0    29755 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgBubblesChart.py
--rw-rw-rw-   0        0        0    11325 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgGraph.py
--rw-rw-rw-   0        0        0    18669 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgHeatmap.py
--rw-rw-rw-   0        0        0  1033396 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgMap.py
--rw-rw-rw-   0        0        0    21956 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgPackedCirclesChart.py
--rw-rw-rw-   0        0        0    18049 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgRankChart.py
--rw-rw-rw-   0        0        0    48423 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/svgUtils.py
--rw-rw-rw-   0        0        0     7363 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/treemapPlotly.py
--rw-rw-rw-   0        0        0     2290 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/urlOpen.py
--rw-rw-rw-   0        0        0     2017 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/urlUpdate.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:32:16.005533 vois-1.0.5/src/vois/vuetify/
--rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/__init__.py
--rw-rw-rw-   0        0        0    52950 2023-06-13 09:22:47.000000 vois-1.0.5/src/vois/vuetify/app.py
--rw-rw-rw-   0        0        0    43073 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/basemaps.py
--rw-rw-rw-   0        0        0    13241 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/button.py
--rw-rw-rw-   0        0        0    12444 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/card.py
--rw-rw-rw-   0        0        0    10734 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/cardsGrid.py
--rw-rw-rw-   0        0        0     8770 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/colorPicker.py
--rw-rw-rw-   0        0        0    10437 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/datatable.py
--rw-rw-rw-   0        0        0     7269 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/datePicker.py
--rw-rw-rw-   0        0        0     9643 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/dialogGeneric.py
--rw-rw-rw-   0        0        0     4250 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/dialogMessage.py
--rw-rw-rw-   0        0        0     5785 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/dialogWait.py
--rw-rw-rw-   0        0        0     5369 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/dialogYesNo.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:32:16.047508 vois-1.0.5/src/vois/vuetify/extra/
--rw-rw-rw-   0        0        0       47 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/extra/__init__.py
--rw-rw-rw-   0        0        0     6838 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/extra/file_input.py
--rw-rw-rw-   0        0        0     2251 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/extra/file_input.vue
--rw-rw-rw-   0        0        0    12885 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/fab.py
--rw-rw-rw-   0        0        0      996 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/fontsettings.py
--rw-rw-rw-   0        0        0    13881 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/footer.py
--rw-rw-rw-   0        0        0     8029 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/label.py
--rw-rw-rw-   0        0        0    48546 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/layers.py
--rw-rw-rw-   0        0        0    22786 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/mainPage.py
--rw-rw-rw-   0        0        0     6454 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/menu.py
--rw-rw-rw-   0        0        0     7649 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/multiSwitch.py
--rw-rw-rw-   0        0        0    56576 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/page.py
--rw-rw-rw-   0        0        0    24701 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/paletteEditor.py
--rw-rw-rw-   0        0        0    15331 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/palettePicker.py
--rw-rw-rw-   0        0        0     8048 2023-06-09 16:34:03.000000 vois-1.0.5/src/vois/vuetify/palettePickerEx.py
--rw-rw-rw-   0        0        0     6284 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/popup.py
--rw-rw-rw-   0        0        0     6181 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/progress.py
--rw-rw-rw-   0        0        0     1821 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/queryStrings.py
--rw-rw-rw-   0        0        0     4708 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/radio.py
--rw-rw-rw-   0        0        0     4390 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/rangeSlider.py
--rw-rw-rw-   0        0        0    17054 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/rangeSliderFloat.py
--rw-rw-rw-   0        0        0     9365 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/selectImage.py
--rw-rw-rw-   0        0        0     6052 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/selectMultiple.py
--rw-rw-rw-   0        0        0     8721 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/selectSingle.py
--rw-rw-rw-   0        0        0     4816 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/settings.py
--rw-rw-rw-   0        0        0     6679 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/sidePanel.py
--rw-rw-rw-   0        0        0     5546 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/slider.py
--rw-rw-rw-   0        0        0    12119 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/sliderFloat.py
--rw-rw-rw-   0        0        0     4590 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/snackbar.py
--rw-rw-rw-   0        0        0    24635 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/sortableList.py
--rw-rw-rw-   0        0        0     6575 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/svgsGrid.py
--rw-rw-rw-   0        0        0     4695 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/switch.py
--rw-rw-rw-   0        0        0     6967 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/tabs.py
--rw-rw-rw-   0        0        0     6369 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/textlist.py
--rw-rw-rw-   0        0        0     7009 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/title.py
--rw-rw-rw-   0        0        0     7465 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/toggle.py
--rw-rw-rw-   0        0        0     3179 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/tooltip.py
--rw-rw-rw-   0        0        0    68877 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/treeview.py
--rw-rw-rw-   0        0        0     5036 2023-06-09 16:34:02.000000 vois-1.0.5/src/vois/vuetify/upload.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:32:15.301129 vois-1.0.5/src/vois.egg-info/
--rw-rw-rw-   0        0        0    19318 2023-06-13 09:32:14.000000 vois-1.0.5/src/vois.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2188 2023-06-13 09:32:14.000000 vois-1.0.5/src/vois.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 09:32:14.000000 vois-1.0.5/src/vois.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-06-13 09:32:14.000000 vois-1.0.5/src/vois.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-13 09:32:14.000000 vois-1.0.5/src/vois.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 10:50:19.090562 vois-1.0.6/
+-rw-rw-rw-   0        0        0    14155 2023-06-09 08:06:09.000000 vois-1.0.6/LICENCE
+-rw-rw-rw-   0        0        0      631 2023-06-09 16:48:21.000000 vois-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    73887 2023-06-09 08:06:09.000000 vois-1.0.6/Notice.txt
+-rw-rw-rw-   0        0        0    21395 2023-06-16 10:50:19.088565 vois-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2023-06-16 10:48:12.000000 vois-1.0.6/README.md
+-rw-rw-rw-   0        0        0     6091 2023-06-16 10:48:12.000000 vois-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 10:50:19.090562 vois-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 10:50:17.689317 vois-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 10:50:18.122982 vois-1.0.6/src/vois/
+-rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/__init__.py
+-rw-rw-rw-   0        0        0    11918 2023-06-09 16:34:04.000000 vois-1.0.6/src/vois/colors.py
+-rw-rw-rw-   0        0        0     4168 2023-06-09 16:34:04.000000 vois-1.0.6/src/vois/download.py
+-rw-rw-rw-   0        0        0    17916 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/eucountries.py
+-rw-rw-rw-   0        0        0    10493 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/geojsonUtils.py
+-rw-rw-rw-   0        0        0    66667 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/interMap.py
+-rw-rw-rw-   0        0        0     9302 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/ipytrees.py
+-rw-rw-rw-   0        0        0    35732 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/leafletMap.py
+-rw-rw-rw-   0        0        0    29755 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/svgBubblesChart.py
+-rw-rw-rw-   0        0        0    11325 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/svgGraph.py
+-rw-rw-rw-   0        0        0    18669 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/svgHeatmap.py
+-rw-rw-rw-   0        0        0  1033396 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/svgMap.py
+-rw-rw-rw-   0        0        0    21956 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/svgPackedCirclesChart.py
+-rw-rw-rw-   0        0        0    18049 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/svgRankChart.py
+-rw-rw-rw-   0        0        0    48423 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/svgUtils.py
+-rw-rw-rw-   0        0        0     7363 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/treemapPlotly.py
+-rw-rw-rw-   0        0        0     2290 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/urlOpen.py
+-rw-rw-rw-   0        0        0     2017 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/urlUpdate.py
+drwxrwxrwx   0        0        0        0 2023-06-16 10:50:19.042590 vois-1.0.6/src/vois/vuetify/
+-rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/__init__.py
+-rw-rw-rw-   0        0        0    52950 2023-06-13 09:22:47.000000 vois-1.0.6/src/vois/vuetify/app.py
+-rw-rw-rw-   0        0        0    43073 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/basemaps.py
+-rw-rw-rw-   0        0        0    13241 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/button.py
+-rw-rw-rw-   0        0        0    12779 2023-06-16 10:48:12.000000 vois-1.0.6/src/vois/vuetify/card.py
+-rw-rw-rw-   0        0        0    10734 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/cardsGrid.py
+-rw-rw-rw-   0        0        0     8770 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/colorPicker.py
+-rw-rw-rw-   0        0        0    10437 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/datatable.py
+-rw-rw-rw-   0        0        0     7269 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/datePicker.py
+-rw-rw-rw-   0        0        0     9643 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/dialogGeneric.py
+-rw-rw-rw-   0        0        0     4250 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/dialogMessage.py
+-rw-rw-rw-   0        0        0     5785 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/dialogWait.py
+-rw-rw-rw-   0        0        0     5369 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/dialogYesNo.py
+drwxrwxrwx   0        0        0        0 2023-06-16 10:50:19.085566 vois-1.0.6/src/vois/vuetify/extra/
+-rw-rw-rw-   0        0        0       47 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/extra/__init__.py
+-rw-rw-rw-   0        0        0     6838 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/extra/file_input.py
+-rw-rw-rw-   0        0        0     2251 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/extra/file_input.vue
+-rw-rw-rw-   0        0        0    12885 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/fab.py
+-rw-rw-rw-   0        0        0      996 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/fontsettings.py
+-rw-rw-rw-   0        0        0    13881 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/footer.py
+-rw-rw-rw-   0        0        0     8029 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/label.py
+-rw-rw-rw-   0        0        0    48546 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/layers.py
+-rw-rw-rw-   0        0        0    23017 2023-06-16 10:48:12.000000 vois-1.0.6/src/vois/vuetify/mainPage.py
+-rw-rw-rw-   0        0        0     6454 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/menu.py
+-rw-rw-rw-   0        0        0     7649 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/multiSwitch.py
+-rw-rw-rw-   0        0        0    56576 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/page.py
+-rw-rw-rw-   0        0        0    24701 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/paletteEditor.py
+-rw-rw-rw-   0        0        0    15331 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/palettePicker.py
+-rw-rw-rw-   0        0        0     8048 2023-06-09 16:34:03.000000 vois-1.0.6/src/vois/vuetify/palettePickerEx.py
+-rw-rw-rw-   0        0        0     6284 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/popup.py
+-rw-rw-rw-   0        0        0     6181 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/progress.py
+-rw-rw-rw-   0        0        0     1821 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/queryStrings.py
+-rw-rw-rw-   0        0        0     4708 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/radio.py
+-rw-rw-rw-   0        0        0     4390 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/rangeSlider.py
+-rw-rw-rw-   0        0        0    17054 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/rangeSliderFloat.py
+-rw-rw-rw-   0        0        0     9365 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/selectImage.py
+-rw-rw-rw-   0        0        0     6052 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/selectMultiple.py
+-rw-rw-rw-   0        0        0     8721 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/selectSingle.py
+-rw-rw-rw-   0        0        0     4816 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/settings.py
+-rw-rw-rw-   0        0        0     6679 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/sidePanel.py
+-rw-rw-rw-   0        0        0     5546 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/slider.py
+-rw-rw-rw-   0        0        0    12119 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/sliderFloat.py
+-rw-rw-rw-   0        0        0     4590 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/snackbar.py
+-rw-rw-rw-   0        0        0    24635 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/sortableList.py
+-rw-rw-rw-   0        0        0     6575 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/svgsGrid.py
+-rw-rw-rw-   0        0        0     4695 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/switch.py
+-rw-rw-rw-   0        0        0     6967 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/tabs.py
+-rw-rw-rw-   0        0        0     6369 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/textlist.py
+-rw-rw-rw-   0        0        0     7009 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/title.py
+-rw-rw-rw-   0        0        0     7465 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/toggle.py
+-rw-rw-rw-   0        0        0     3179 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/tooltip.py
+-rw-rw-rw-   0        0        0    68877 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/treeview.py
+-rw-rw-rw-   0        0        0     5036 2023-06-09 16:34:02.000000 vois-1.0.6/src/vois/vuetify/upload.py
+drwxrwxrwx   0        0        0        0 2023-06-16 10:50:18.156912 vois-1.0.6/src/vois.egg-info/
+-rw-rw-rw-   0        0        0    21395 2023-06-16 10:50:17.000000 vois-1.0.6/src/vois.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2188 2023-06-16 10:50:17.000000 vois-1.0.6/src/vois.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 10:50:17.000000 vois-1.0.6/src/vois.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-06-16 10:50:17.000000 vois-1.0.6/src/vois.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-16 10:50:17.000000 vois-1.0.6/src/vois.egg-info/top_level.txt
```

### Comparing `vois-1.0.5/LICENCE` & `vois-1.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/MANIFEST.in` & `vois-1.0.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/Notice.txt` & `vois-1.0.6/Notice.txt`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/PKG-INFO` & `vois-1.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vois
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python Voilà simplification library
 Author-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 Maintainer-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 License: Copyright © European Union 2022-2023
         
         
                               EUROPEAN UNION PUBLIC LICENCE v. 1.2
@@ -325,29 +325,58 @@
 The PDF documentation for the vois library is available [here](https://vois.readthedocs.io/_/downloads/en/latest/pdf/)
 
 The source repository is available [here](https://code.europa.eu/jrc-bdap/vois)
 
 
 The vois library contains:
 
-folder **vois**: helper functions for tasks not directly related to ipyvuetify (manage geojson files, create an interactive map to display custom geojson, simplify visualization of hierarchical data in Plotly, create custom SVG visualizations, etc.)
+package **vois**: helper functions for tasks not directly related to ipyvuetify (manage geojson files, create an interactive map to display custom geojson, simplify visualization of hierarchical data in Plotly, create custom SVG visualizations, etc.)
 
-folder **vois/vuetify**: classes to simplify the development of GUIs using ipyvuetify (each source file contains a wrapper to simplify the usage of a ipyvuetify widget)
+package **vois/vuetify**: classes to simplify the development of GUIs using ipyvuetify (each source file contains a wrapper to simplify the usage of a ipyvuetify widget)
 
 
 ## License
 
 VOIS library is released under a
 [EUPL Version 1.2](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12) license.
 
+
 ## Setup
 
 The vois library can be installed using this command:
 
 `pip install vois`
 
 
 ## Tutorial
 
 The tutorial section of the documentation available [here](https://vois.readthedocs.io/en/latest/2_tutorial.html) provides a step by step example for the construction of a dashboard to display EUROSTAT data on Energy Consumption in Europe.
 
 ![screenshot](https://jeodpp.jrc.ec.europa.eu/services/shared/pngs/vois_example.png)
+
+These are the links to all the steps of the example dashboard deployed and published by Hugginface Spaces:
+
+[Step.1: Creation of the dashboard structure using the app class](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.1.ipynb)
+
+[Step.2: Use Pandas to read the input CSVs and display the DataFrame as a table](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.2.ipynb)
+
+[Step.3: Add the filtering controls to the dashboard to select countries and sector](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.3.ipynb)
+
+[Step.4: Add the Plotly Bar Chart View](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.4.ipynb)
+
+[Step.5: Add the SVG Static Map View](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.5.ipynb)
+
+[Step.6: Add the Dynamic Map View](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.6.ipynb)
+
+[Step.7: Add the functions for downloading chart, table and map](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.7.ipynb)
+
+[Step.8: Manage the parameters passsed in the URL and open external URLs](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.8.ipynb)
+
+[Step.9: Add an interactive AnimatedPieChart in SVG to select the consumption sector](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.9.ipynb)
+
+[Step.Final: Add minipanel to footer bar and the function to generate and download a report in docx format](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.Final.ipynb)
+
+[Step.Final.Dark: Dark version of the final dashboard](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.Final.ThemeDark.ipynb)
+
+An example multi-page dashboard can be viewed at this link: [Example multi-page dashboard](https://davidedemarchi-voila.hf.space/voila/render/tutorial/MultipageDemo.ipynb)
+
+![screenshot](./docs/figures/multipage.png)
```

### Comparing `vois-1.0.5/pyproject.toml` & `vois-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 name = "vois"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.5"  # Required
+version = "1.0.6"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A Python Voilà simplification library"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -143,8 +143,8 @@
 repository = "https://github.com/DavideDeMarchi/vois/"
 
 
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
 include = ["*"]  # package names should match these glob patterns (["*"] by default)
 exclude = []  # exclude packages matching these glob patterns (empty by default)
-namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
+namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
```

### Comparing `vois-1.0.5/src/vois/colors.py` & `vois-1.0.6/src/vois/colors.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/download.py` & `vois-1.0.6/src/vois/download.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/eucountries.py` & `vois-1.0.6/src/vois/eucountries.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/geojsonUtils.py` & `vois-1.0.6/src/vois/geojsonUtils.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/interMap.py` & `vois-1.0.6/src/vois/interMap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/ipytrees.py` & `vois-1.0.6/src/vois/ipytrees.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/leafletMap.py` & `vois-1.0.6/src/vois/leafletMap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/svgBubblesChart.py` & `vois-1.0.6/src/vois/svgBubblesChart.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/svgGraph.py` & `vois-1.0.6/src/vois/svgGraph.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/svgHeatmap.py` & `vois-1.0.6/src/vois/svgHeatmap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/svgMap.py` & `vois-1.0.6/src/vois/svgMap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/svgPackedCirclesChart.py` & `vois-1.0.6/src/vois/svgPackedCirclesChart.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/svgRankChart.py` & `vois-1.0.6/src/vois/svgRankChart.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/svgUtils.py` & `vois-1.0.6/src/vois/svgUtils.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/treemapPlotly.py` & `vois-1.0.6/src/vois/treemapPlotly.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/urlOpen.py` & `vois-1.0.6/src/vois/urlOpen.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/urlUpdate.py` & `vois-1.0.6/src/vois/urlUpdate.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/app.py` & `vois-1.0.6/src/vois/vuetify/app.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/basemaps.py` & `vois-1.0.6/src/vois/vuetify/basemaps.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/button.py` & `vois-1.0.6/src/vois/vuetify/button.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/card.py` & `vois-1.0.6/src/vois/vuetify/card.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         Size of the area where the icon is displayed (default is '32px')
     image : str, optional
         URL of the image to display in the right side of the card (default is '')
     imagesize : str, optional
         Size of the area where the image is displayed (default is '190px')
     on_click : function, optional
         Python function to call when the user clicks on the card. The function will receive no parameters. (default is None)
+    argument : any, optional
+        Argument to pass to the on_click python function (default is None)
     responsive : bool, optional
         If True, the font size is automatically changed according to the page size (default is False)
     fontsizemultiplier : float, optional
         Multiply factor for changing the standard size of the font used for title and subtitle (default is 1.0)
     backgroundimageurl : str, optional
         URL of the optional image to display as background of the card (default is '')
     tooltip : str, optional
@@ -110,14 +112,15 @@
     title      = traitlets.Unicode('Title').tag(sync=True)
     subtitle   = traitlets.Unicode('Subtitle').tag(sync=True)
     icon       = traitlets.Unicode('').tag(sync=True)
     iconsize   = traitlets.Unicode('32px').tag(sync=True)
     image      = traitlets.Unicode('').tag(sync=True)
     imagesize  = traitlets.Unicode('190px').tag(sync=True)
     on_click   = traitlets.Any(None).tag(sync=False)
+    argument   = traitlets.Any(None).tag(sync=False)
     responsive = traitlets.Bool(False).tag(sync=True)
     fontsizemultiplier = traitlets.Float(1.0).tag(sync=True)
     backgroundimageurl = traitlets.Unicode('').tag(sync=True)
     
     subtitlemargins = traitlets.Unicode('ma-0 ml-4 mb-4 mt-0 mr-4').tag(sync=True)
     focusedopacity  = traitlets.Float(0.1).tag(sync=True)
     textcolor       = traitlets.Unicode('black').tag(sync=True)
@@ -253,14 +256,15 @@
                  title='Title',
                  subtitle='Subtitle',
                  icon='',
                  iconsize='32px',
                  image='',
                  imagesize='190px',
                  on_click=None,
+                 argument=None,
                  responsive=False,
                  fontsizemultiplier=1.0,
                  backgroundimageurl='',
                  tooltip='',
                  titletooltip='',
                  focusedopacity=0.1,     # Opacity for the background when the card is clicked (has focus)
                  textcolor='black',
@@ -292,18 +296,22 @@
         else:              self.iconsize = iconsize
         
         self.image = image
         if len(image) == 0: self.imagesize = '0px'
         else:               self.imagesize = imagesize
         
         self.on_click = on_click
+        self.argument = argument
         
         self.responsive         = responsive
         self.fontsizemultiplier = fontsizemultiplier
         self.backgroundimageurl = backgroundimageurl
         
         super().__init__(*args, **kwargs)
     
     # Manage event "click"
     def vue_clicked(self, data):
         if not self.on_click is None:
-            self.on_click()
+            if self.argument is None:
+                self.on_click()
+            else:
+                self.on_click(self.argument)
```

### Comparing `vois-1.0.5/src/vois/vuetify/cardsGrid.py` & `vois-1.0.6/src/vois/vuetify/cardsGrid.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/colorPicker.py` & `vois-1.0.6/src/vois/vuetify/colorPicker.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/datatable.py` & `vois-1.0.6/src/vois/vuetify/datatable.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/datePicker.py` & `vois-1.0.6/src/vois/vuetify/datePicker.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/dialogGeneric.py` & `vois-1.0.6/src/vois/vuetify/dialogGeneric.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/dialogMessage.py` & `vois-1.0.6/src/vois/vuetify/dialogMessage.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/dialogWait.py` & `vois-1.0.6/src/vois/vuetify/dialogWait.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/dialogYesNo.py` & `vois-1.0.6/src/vois/vuetify/dialogYesNo.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/extra/file_input.py` & `vois-1.0.6/src/vois/vuetify/extra/file_input.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/extra/file_input.vue` & `vois-1.0.6/src/vois/vuetify/extra/file_input.vue`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/fab.py` & `vois-1.0.6/src/vois/vuetify/fab.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/fontsettings.py` & `vois-1.0.6/src/vois/vuetify/fontsettings.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/footer.py` & `vois-1.0.6/src/vois/vuetify/footer.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/label.py` & `vois-1.0.6/src/vois/vuetify/label.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/layers.py` & `vois-1.0.6/src/vois/vuetify/layers.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/mainPage.py` & `vois-1.0.6/src/vois/vuetify/mainPage.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,18 +100,15 @@
     Examples
     --------
     Creation of a main page with 6 buttons displaying random images from https://picsum.photos/::
         
         from vois.vuetify import mainPage
         from random import randrange
         
-        def on_click():
-            pass
-            
-        def onclick():
+        def onclick1():
             print("Clicked Function 1")
 
         m = mainPage.mainPage(title='mainPage demo',
                               subtitle='Showcase how easy is to create a front page for an app',
                               credits="vois library development team",
                               titlebox_widthpercent=50, titlebox_opacity=0.2, titlebox_border=0,
                               vois_show=True, vois_opacity=0.1,
@@ -121,15 +118,15 @@
                               creditbox_opacity=0,
                               text_color='#222222')
 
         m.addButton('Function 1',
                     subtitle='Launch calculation of ...',
                     tooltip='Tooltip text to display on hover',
                     image='https://picsum.photos/seed/%d/200/200'%randrange(1000),
-                    onclick=onclick)
+                    onclick=onclick1)
 
         for i in range(2,7): m.addButton('Function %d'%i, image='https://picsum.photos/seed/%d/200/200'%randrange(1000))
 
         m.open()
 
 
     .. figure:: figures/mainPage.png
@@ -359,37 +356,40 @@
         self.hunit = v.Html(tag='div', children=[cardunit], class_="pa-0 ma-0",
                             style_='width: %fvw; height: %fvh; border: 0px solid #000000; border-radius: 12px; position: absolute; top: %fvh; left: %fvw; background-color: %s; overflow: hidden;'%(self.creditbox_widthpercent, self.creditbox_heightpercent,
                             self.creditbox_toppercent, (100.0-self.creditbox_widthpercent)/2.0, bcol))
 
 
 
     # Add a button
-    def addButton(self, title, subtitle='', tooltip='', image='', onclick=None):
+    def addButton(self, title, subtitle='', tooltip='', image='', onclick=None, argument=None):
         """
         Add a button to the page
         
         Parameters
         ----------
         title : str
             Title of the button
         subtitle : str, optional
             Subtitle of the button (default is '')
         tooltip : str, optional
             Tooltip to show when hovering the button title (default is '')
         image : str, optional
             Image to show on the right side of the button (default is '')
         onclick : function, optional
-            Python function to call when the user clicks on the button. The function will receive no parameters (default is None)
+            Python function to call when the user clicks on the button. The function will receive the argument value as parameter if it is not None, otherwise it will be calle with no parameters. Default is None
+        argument : any, optional
+            Argument to pass to the onclick python function (default is None)
             
         """
         self.buttons.append({'title':    title,
                              'subtitle': subtitle,
                              'tooltip':  tooltip,
                              'image':    image,
-                             'onclick':  onclick})
+                             'onclick':  onclick,
+                             'argument': argument})
         
         
     # Display the page as a fullscreen dialog-box
     def open(self):
         """Open the page"""
         nbuttons_per_row = self.buttonbox_widthpercent // self.button_widthpercent
         
@@ -397,15 +397,15 @@
         
         children = []
         i = 0
         for b in self.buttons:
             c = card.card(elevation=self.button_elevation, width='%fvw'%self.button_widthpercent, imagesize="%fvh"%self.button_heightpercent, responsive=True,
                           title=b['title'], subtitle=b['subtitle'], titletooltip=b['tooltip'],
                           color='#ffffff%0.2X'%int(self.button_opacity*255), fontsizemultiplier=1.1, subtitleweight=400,
-                          image=b['image'], on_click=b['onclick'], textcolor=self.text_color)
+                          image=b['image'], on_click=b['onclick'], argument=b['argument'], textcolor=self.text_color)
             if len(children) > 0:
                 children.append(self.spacer)
             children.append(c)
             
             i += 1
             if i >= nbuttons_per_row:
                 r = v.Row(justify="center", children=children, class_="pa-0 ma-0 mt-2")
```

### Comparing `vois-1.0.5/src/vois/vuetify/menu.py` & `vois-1.0.6/src/vois/vuetify/menu.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/multiSwitch.py` & `vois-1.0.6/src/vois/vuetify/multiSwitch.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/page.py` & `vois-1.0.6/src/vois/vuetify/page.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/paletteEditor.py` & `vois-1.0.6/src/vois/vuetify/paletteEditor.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/palettePicker.py` & `vois-1.0.6/src/vois/vuetify/palettePicker.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/palettePickerEx.py` & `vois-1.0.6/src/vois/vuetify/palettePickerEx.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/popup.py` & `vois-1.0.6/src/vois/vuetify/popup.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/progress.py` & `vois-1.0.6/src/vois/vuetify/progress.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/queryStrings.py` & `vois-1.0.6/src/vois/vuetify/queryStrings.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/radio.py` & `vois-1.0.6/src/vois/vuetify/radio.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/rangeSlider.py` & `vois-1.0.6/src/vois/vuetify/rangeSlider.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/rangeSliderFloat.py` & `vois-1.0.6/src/vois/vuetify/rangeSliderFloat.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/selectImage.py` & `vois-1.0.6/src/vois/vuetify/selectImage.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/selectMultiple.py` & `vois-1.0.6/src/vois/vuetify/selectMultiple.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/selectSingle.py` & `vois-1.0.6/src/vois/vuetify/selectSingle.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/settings.py` & `vois-1.0.6/src/vois/vuetify/settings.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/sidePanel.py` & `vois-1.0.6/src/vois/vuetify/sidePanel.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/slider.py` & `vois-1.0.6/src/vois/vuetify/slider.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/sliderFloat.py` & `vois-1.0.6/src/vois/vuetify/sliderFloat.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/snackbar.py` & `vois-1.0.6/src/vois/vuetify/snackbar.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/sortableList.py` & `vois-1.0.6/src/vois/vuetify/sortableList.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/svgsGrid.py` & `vois-1.0.6/src/vois/vuetify/svgsGrid.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/switch.py` & `vois-1.0.6/src/vois/vuetify/switch.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/tabs.py` & `vois-1.0.6/src/vois/vuetify/tabs.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/textlist.py` & `vois-1.0.6/src/vois/vuetify/textlist.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/title.py` & `vois-1.0.6/src/vois/vuetify/title.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/toggle.py` & `vois-1.0.6/src/vois/vuetify/toggle.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/tooltip.py` & `vois-1.0.6/src/vois/vuetify/tooltip.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/treeview.py` & `vois-1.0.6/src/vois/vuetify/treeview.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois/vuetify/upload.py` & `vois-1.0.6/src/vois/vuetify/upload.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.5/src/vois.egg-info/PKG-INFO` & `vois-1.0.6/src/vois.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vois
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python Voilà simplification library
 Author-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 Maintainer-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 License: Copyright © European Union 2022-2023
         
         
                               EUROPEAN UNION PUBLIC LICENCE v. 1.2
@@ -325,29 +325,58 @@
 The PDF documentation for the vois library is available [here](https://vois.readthedocs.io/_/downloads/en/latest/pdf/)
 
 The source repository is available [here](https://code.europa.eu/jrc-bdap/vois)
 
 
 The vois library contains:
 
-folder **vois**: helper functions for tasks not directly related to ipyvuetify (manage geojson files, create an interactive map to display custom geojson, simplify visualization of hierarchical data in Plotly, create custom SVG visualizations, etc.)
+package **vois**: helper functions for tasks not directly related to ipyvuetify (manage geojson files, create an interactive map to display custom geojson, simplify visualization of hierarchical data in Plotly, create custom SVG visualizations, etc.)
 
-folder **vois/vuetify**: classes to simplify the development of GUIs using ipyvuetify (each source file contains a wrapper to simplify the usage of a ipyvuetify widget)
+package **vois/vuetify**: classes to simplify the development of GUIs using ipyvuetify (each source file contains a wrapper to simplify the usage of a ipyvuetify widget)
 
 
 ## License
 
 VOIS library is released under a
 [EUPL Version 1.2](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12) license.
 
+
 ## Setup
 
 The vois library can be installed using this command:
 
 `pip install vois`
 
 
 ## Tutorial
 
 The tutorial section of the documentation available [here](https://vois.readthedocs.io/en/latest/2_tutorial.html) provides a step by step example for the construction of a dashboard to display EUROSTAT data on Energy Consumption in Europe.
 
 ![screenshot](https://jeodpp.jrc.ec.europa.eu/services/shared/pngs/vois_example.png)
+
+These are the links to all the steps of the example dashboard deployed and published by Hugginface Spaces:
+
+[Step.1: Creation of the dashboard structure using the app class](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.1.ipynb)
+
+[Step.2: Use Pandas to read the input CSVs and display the DataFrame as a table](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.2.ipynb)
+
+[Step.3: Add the filtering controls to the dashboard to select countries and sector](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.3.ipynb)
+
+[Step.4: Add the Plotly Bar Chart View](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.4.ipynb)
+
+[Step.5: Add the SVG Static Map View](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.5.ipynb)
+
+[Step.6: Add the Dynamic Map View](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.6.ipynb)
+
+[Step.7: Add the functions for downloading chart, table and map](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.7.ipynb)
+
+[Step.8: Manage the parameters passsed in the URL and open external URLs](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.8.ipynb)
+
+[Step.9: Add an interactive AnimatedPieChart in SVG to select the consumption sector](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.9.ipynb)
+
+[Step.Final: Add minipanel to footer bar and the function to generate and download a report in docx format](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.Final.ipynb)
+
+[Step.Final.Dark: Dark version of the final dashboard](https://davidedemarchi-voila.hf.space/voila/render/tutorial/EnergyConsumption.Final.ThemeDark.ipynb)
+
+An example multi-page dashboard can be viewed at this link: [Example multi-page dashboard](https://davidedemarchi-voila.hf.space/voila/render/tutorial/MultipageDemo.ipynb)
+
+![screenshot](./docs/figures/multipage.png)
```

### Comparing `vois-1.0.5/src/vois.egg-info/SOURCES.txt` & `vois-1.0.6/src/vois.egg-info/SOURCES.txt`

 * *Files identical despite different names*

