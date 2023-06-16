# Comparing `tmp/hesperos-0.1.9.tar.gz` & `tmp/hesperos-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hesperos-0.1.9.tar", last modified: Tue May 31 17:26:30 2022, max compression
+gzip compressed data, was "hesperos-0.2.tar", last modified: Fri Jun 16 14:05:46 2023, max compression
```

## Comparing `hesperos-0.1.9.tar` & `hesperos-0.2.tar`

### file list

```diff
@@ -1,63 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:30.680699 hesperos-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:30.676699 hesperos-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:30.676699 hesperos-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-05-31 17:26:10.000000 hesperos-0.1.9/.github/workflows/plugin_preview.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2788 2022-05-31 17:26:10.000000 hesperos-0.1.9/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-05-31 17:26:10.000000 hesperos-0.1.9/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:30.676699 hesperos-0.1.9/.napari/
--rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-05-31 17:26:10.000000 hesperos-0.1.9/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-05-31 17:26:10.000000 hesperos-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-05-31 17:26:10.000000 hesperos-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-05-31 17:26:10.000000 hesperos-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3139 2022-05-31 17:26:30.680699 hesperos-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-05-31 17:26:10.000000 hesperos-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-05-31 17:26:10.000000 hesperos-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-05-31 17:26:30.680699 hesperos-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:30.676699 hesperos-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:30.676699 hesperos-0.1.9/src/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/_tests/test_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:30.676699 hesperos-0.1.9/src/hesperos/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    35278 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/_manual_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)    29696 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/_oneshot_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:30.680699 hesperos-0.1.9/src/hesperos/annotation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/annotation/feta.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/annotation/fetus.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/annotation/oneshot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/annotation/shoulder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3572 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/annotation/structuresubpanel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:30.680699 hesperos-0.1.9/src/hesperos/layout/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16771 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/layout/gui_elements.py
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/layout/napari_elements.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:30.680699 hesperos-0.1.9/src/hesperos/one_shot_learning/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/one_shot_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/one_shot_learning/classifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     9075 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/one_shot_learning/features2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/one_shot_learning/features3d.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/one_shot_learning/kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     6044 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/one_shot_learning/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:30.680699 hesperos-0.1.9/src/hesperos/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/resources/_icons.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:30.680699 hesperos-0.1.9/src/hesperos/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/resources/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/resources/icons/backup.svg
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/resources/icons/lock.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/resources/icons/reset.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/resources/icons/save.svg
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/resources/icons/undo.svg
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/resources/icons/unlock.svg
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/hesperos/resources/icons/zoom.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 17:26:30.680699 hesperos-0.1.9/src/hesperos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3139 2022-05-31 17:26:30.000000 hesperos-0.1.9/src/hesperos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-05-31 17:26:30.000000 hesperos-0.1.9/src/hesperos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 17:26:30.000000 hesperos-0.1.9/src/hesperos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-31 17:26:30.000000 hesperos-0.1.9/src/hesperos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-31 17:26:30.000000 hesperos-0.1.9/src/hesperos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-31 17:26:30.000000 hesperos-0.1.9/src/hesperos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-05-31 17:26:10.000000 hesperos-0.1.9/src/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-05-31 17:26:10.000000 hesperos-0.1.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.339913 hesperos-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.323913 hesperos-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.327913 hesperos-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-16 14:05:27.000000 hesperos-0.2/.github/workflows/plugin_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-16 14:05:27.000000 hesperos-0.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-16 14:05:27.000000 hesperos-0.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.327913 hesperos-0.2/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-16 14:05:27.000000 hesperos-0.2/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-16 14:05:27.000000 hesperos-0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-16 14:05:27.000000 hesperos-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 14:05:27.000000 hesperos-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24224 2023-06-16 14:05:46.339913 hesperos-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-06-16 14:05:27.000000 hesperos-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.323913 hesperos-0.2/materials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.331913 hesperos-0.2/materials/interface_tools_screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_delete_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_export_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_load_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_lock_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_save_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_undo_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_unlock_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/contrast_add_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/contrast_choose.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/contrast_export_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/contrast_import_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   454140 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/hesperos_manual_interface.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   510686 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/hesperos_oneshot_interface.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/image_change_axis_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/image_transpose_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/layer_label_erase_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/layer_label_fill_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/layer_label_paint_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/layer_label_zoom_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/open_dicom_serie_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/open_image_file_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/proba_threshold_slider.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/run_segmentation_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/save_probabilities_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/save_segmentation_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   301806 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/screen_tagging_step.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/slice_selection_add_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/slice_selection_drop_down_menu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/slice_selection_goto_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/slice_selection_remove_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/zoom_slider.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-16 14:05:27.000000 hesperos-0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.323913 hesperos-0.2/script_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.331913 hesperos-0.2/script_files/for_Macos/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-16 14:05:27.000000 hesperos-0.2/script_files/for_Macos/install_hesperos_env.command
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 14:05:27.000000 hesperos-0.2/script_files/for_Macos/run_hesperos.command
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.331913 hesperos-0.2/script_files/for_Windows/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-16 14:05:27.000000 hesperos-0.2/script_files/for_Windows/install_hesperos_env.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-16 14:05:27.000000 hesperos-0.2/script_files/for_Windows/run_hesperos.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-16 14:05:46.343913 hesperos-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.331913 hesperos-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.331913 hesperos-0.2/src/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:27.000000 hesperos-0.2/src/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-16 14:05:27.000000 hesperos-0.2/src/_tests/test_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.335913 hesperos-0.2/src/hesperos/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117963 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/_manual_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44800 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/_oneshot_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.335913 hesperos-0.2/src/hesperos/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/feta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/fetus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/larva.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/mouse_embryon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/shoulder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/shoulder_bone_border.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/shoulder_bones.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/shoulder_deltoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/structuresubpanel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.335913 hesperos-0.2/src/hesperos/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22740 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/layout/gui_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/layout/napari_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.339913 hesperos-0.2/src/hesperos/one_shot_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/one_shot_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/one_shot_learning/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/one_shot_learning/features2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/one_shot_learning/features3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/one_shot_learning/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/one_shot_learning/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.339913 hesperos-0.2/src/hesperos/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/group_box_stylesheet.qss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.339913 hesperos-0.2/src/hesperos/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/backup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/chevron_down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/chevron_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/chevron_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/chevron_up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/export.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/import.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/lock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/map.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/minus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/minus2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/next.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/plus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/reset.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/save.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/unlock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/zoom.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.335913 hesperos-0.2/src/hesperos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24224 2023-06-16 14:05:46.000000 hesperos-0.2/src/hesperos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-06-16 14:05:46.000000 hesperos-0.2/src/hesperos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:05:46.000000 hesperos-0.2/src/hesperos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 14:05:46.000000 hesperos-0.2/src/hesperos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-16 14:05:46.000000 hesperos-0.2/src/hesperos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 14:05:46.000000 hesperos-0.2/src/hesperos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-16 14:05:27.000000 hesperos-0.2/src/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-16 14:05:27.000000 hesperos-0.2/tox.ini
```

### Comparing `hesperos-0.1.9/.github/workflows/plugin_preview.yml` & `hesperos-0.2/.github/workflows/plugin_preview.yml`

 * *Files identical despite different names*

### Comparing `hesperos-0.1.9/.github/workflows/test_and_deploy.yml` & `hesperos-0.2/.github/workflows/test_and_deploy.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 jobs:
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
         platform: [windows-latest, macos-latest]
-        python-version: [3.8, 3.9]
+        python-version: [3.8, 3.9, "3.10"]
 
     steps:
       - uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
```

### Comparing `hesperos-0.1.9/.gitignore` & `hesperos-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hesperos-0.1.9/.napari/DESCRIPTION.md` & `hesperos-0.2/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `hesperos-0.1.9/.pre-commit-config.yaml` & `hesperos-0.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.0.1
+    rev: v4.2.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v1.20.0
+    rev: v1.20.1
     hooks:
       - id: setup-cfg-fmt
   - repo: https://github.com/PyCQA/flake8
     rev: 4.0.1
     hooks:
       - id: flake8
         additional_dependencies: [flake8-typing-imports>=1.9.0]
@@ -20,19 +20,19 @@
       - id: autoflake
         args: ["--in-place", "--remove-all-unused-imports"]
   - repo: https://github.com/PyCQA/isort
     rev: 5.10.1
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 21.11b1
+    rev: 22.3.0
     hooks:
       - id: black
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.29.1
+    rev: v2.32.1
     hooks:
       - id: pyupgrade
         args: [--py38-plus, --keep-runtime-typing]
   - repo: https://github.com/tlambert03/napari-plugin-checks
     rev: v0.2.0
     hooks:
       - id: napari-plugin-checks
```

### Comparing `hesperos-0.1.9/LICENSE` & `hesperos-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hesperos-0.1.9/setup.cfg` & `hesperos-0.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hesperos
-version = 0.1.9
+version = 0.2
 author = Charlotte Godard
 author_email = charlotte.godard@pasteur.fr
 url = https://github.com/chgodard/hesperos
 license = BSD-3-Clause
 description = A plugin to manually or semi-automatically segment medical data and correct previous segmentation data.
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -12,16 +12,21 @@
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Developers
 	Framework :: napari
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
-	Operating System :: OS Independent
+	Programming Language :: Python :: 3.10
+	Operating System :: MacOS :: MacOS X
+	Operating System :: Microsoft :: Windows
 	License :: OSI Approved :: BSD License
+project_urls = 
+	Documentation = https://github.com/chgodard/hesperos/blob/main/README.md
+	Source Code = https://github.com/chgodard/hesperos
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 package_dir = 
 	=src
@@ -30,28 +35,30 @@
 	numpy
 	qtpy
 	tifffile
 	scikit-image
 	scikit-learn
 	SimpleITK
 	pandas
-	napari<0.5.0
+	napari<0.4.15
 	napari-plugin-engine
+	imageio_ffmpeg
 
 [options.extras_require]
 testing = 
 	tox
 	pytest  # https://docs.pytest.org/en/latest/contents.html
 	pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
 	pytest-qt  # https://pytest-qt.readthedocs.io/en/latest/
 	napari
 	pyqt5
 
 [options.packages.find]
 where = src
+exclude = _tests
 
 [options.package_data]
 * = *.yaml, *.svg
 
 [options.entry_points]
 napari.manifest = 
 	hesperos = hesperos:napari.yaml
```

### Comparing `hesperos-0.1.9/src/_tests/test_widget.py` & `hesperos-0.2/src/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.1.9/src/hesperos/_manual_widget.py` & `hesperos-0.2/src/hesperos/_oneshot_widget.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,224 +1,281 @@
 # ============ Import python files ============
+# === GUI elements ===
 from hesperos.layout.gui_elements import (
-    add_push_button,
+    add_check_box,
+    add_combo_box,
     add_icon_push_button,
+    add_icon_text_push_button,
+    add_image_widget,
     add_label,
+    add_push_button,
     add_slider,
-    add_combobox,
-    add_image_widget,
     display_warning_box,
     display_save_message_box,
-    display_ok_cancel_question_box
+    display_ok_cancel_question_box,
+    display_yes_no_question_box
 )
-from hesperos.layout.napari_elements import disable_napari_buttons, disable_layer_widgets
+from hesperos.layout.napari_elements import disable_napari_buttons, disable_layer_widgets, reset_dock_widget, disable_dock_widget_buttons
 from hesperos.resources._icons import get_icon_path, get_relative_icon_path
 
-import hesperos.annotation.fetus as fetus_data
-import hesperos.annotation.shoulder as shoulder_data
-import hesperos.annotation.feta as feta_data
+import hesperos.annotation.oneshot as oneshot_data
 from hesperos.annotation.structuresubpanel import StructureSubPanel
 
+# === One Shot learning computation
+from hesperos.one_shot_learning.features3d import Features3D
+from hesperos.one_shot_learning.utilities import run_one_shot_learning
+
+
 # ============ Import python packages ============
 import os
+import json
 import napari
 import numpy as np
 import tifffile as tif
 import SimpleITK as sitk
 from pathlib import Path
-from napari._vispy import VispyCanvas
 
 from qtpy import QtCore
 from qtpy.QtGui import QIcon
 from qtpy.QtWidgets import (
     QGridLayout,
     QGroupBox,
     QWidget,
     QFileDialog,
-    QHBoxLayout,
+    QHBoxLayout
 )
 
+
 # ============ Define variables ============
 COLUMN_WIDTH = 100
-SEGM_METHODS_PANEL_ALIGN = (
-    "center"  # Alignment of text in pushbuttons in methods chooser panel
-)
+if not hasattr(napari, 'DOCK_WIDGETS'):
+    napari.DOCK_WIDGETS = []
 
 
 # ============ Define QWidget Class ============
-class ManualSegmentationWidget(QWidget):
+class OneShotWidget(QWidget):
     """
-    QWidget class for Manual Segmentation in NAPARI
+    QWidget class for One Shot Learning Segmentation in napari
 
     """
     def __init__(self, napari_viewer):
-        """ Initilialisation of the widget in the current napari viewer
+        """ 
+        Initilialisation of the widget in the current napari viewer
 
         Parameters
         ----------
         napari_viewer : napari.Viewer
             active (unique) instance of the napari viewer
 
         """
+
+        # reset_dock_widget(napari_viewer)
+
         super().__init__()
 
         napari.utils.notifications.WarningNotification.blocked = True
         self.viewer = napari_viewer
 
         disable_napari_buttons(self.viewer)
 
+        napari.features_3d = Features3D()
+
         self.generate_main_layout()
-        # self.generate_help_layout()
+
+        napari.DOCK_WIDGETS.append(self)
+        disable_dock_widget_buttons(self.viewer)
 
 
 # ============ Define Layout ============
     def generate_main_layout(self):
         """
-        Generate the main layout of the widget
+        Generate the main layout of widget
+
         """
 
         # === Set layout parameters ===
         self.layout = QGridLayout()
         self.layout.setContentsMargins(10, 10, 10, 10)
         self.layout.setAlignment(QtCore.Qt.AlignTop)
         self.layout.setSpacing(5)
 
         # === Create and add panels to the layout ===
-        self.add_loading_panel(1)
-
+        self.add_import_panel(1)
         self.add_annotation_panel(2)
         self.add_sub_annotation_panel(3)
+        self.add_segmentation_panel(4)
+        self.add_reset_export_panel(5)
 
-        self.add_reset_save_panel(4)
+        # Display status (cannot display progressing bar because napari is freezing)
+        self.status_label = add_label(
+            text='Ready',
+            layout=self.layout,
+            row=6,
+            column=0,
+            visibility=True
+            )
 
-        self.enable_panels(["annotation_panel", "reset_save_panel"], False)
+        self.toggle_panels(["annotation_panel", "segmentation_panel", "reset_export_panel"], False)
 
         self.setLayout(self.layout)
 
     def add_sub_annotation_panel(self, row):
         """
         Create annotation sub panel with the list of all struture to annotate
 
         Parameters
         ----------
         row : int
             row position of the sub panel in the main QGridLayout
 
         """
-        self.fetus = StructureSubPanel(
+        self.oneshot = StructureSubPanel(
             parent=self,
             row=row,
             column=0,
-            list_structures=fetus_data.LIST_STRUCTURES,
-            dict_substructures=fetus_data.DICT_SUB_STRUCTURES,
+            list_structures=oneshot_data.LIST_STRUCTURES,
+            dict_substructures=oneshot_data.DICT_SUB_STRUCTURES,
             dict_sub_substructures=[])
 
-        self.feta = StructureSubPanel(
-            parent=self,
-            row=row,
-            column=0,
-            list_structures=feta_data.LIST_STRUCTURES,
-            dict_substructures=feta_data.DICT_SUB_STRUCTURES,
-            dict_sub_substructures=[])
-
-        self.shoulder = StructureSubPanel(
-            parent=self,
-            row=row,
-            column=0,
-            list_structures=shoulder_data.LIST_STRUCTURES,
-            dict_substructures=shoulder_data.DICT_SUB_STRUCTURES,
-            dict_sub_substructures=shoulder_data.DICT_SUB_SUB_STRUCTURES)
-
-    # def generate_help_layout(self):
-
-    #     self.help_layout = QGridLayout()
-    #     self.help_layout.setContentsMargins(10, 10, 10, 10)
-    #     # self.help_layout.setAlignment(QtCore.Qt.AlignTop)
-    #     self.help_layout.setSpacing(4)
-
-    #     self.add_view_panel(row=0, column=0)
-    #     self.add_atlas_panel(row=0, column=1)
-
-    #     self.help_container = QWidget()
-
-    #     self.help_container.setLayout(self.help_layout)
-
-    #     self.help_dock = self.viewer.window.add_dock_widget(widget=self.help_container, area='bottom')
-
-
-    def add_loading_panel(self, row, column=0):
+    def add_import_panel(self, row, column=0):
         """
-        Create loading panel
+        Create import panel
 
         Parameters
         ----------
         row : int
             row position of the panel in the main QGridLayout
         column : int
             column position of the panel in the main QGridLayout
 
         """
 
         # === Set panel parameters ===
-        self.loading_panel = QGroupBox("1. LOAD IMAGE")
-        self.loading_panel.setStyleSheet("margin-top : 5px;")
+        self.import_panel = QGroupBox("1. IMPORT 3D IMAGE")
+        self.import_panel.setStyleSheet("margin-top : 5px;")
 
         # === Set panel layout parameters ===
-        self.loading_layout = QGridLayout()
-        self.loading_layout.setSpacing(5)
-        self.loading_layout.setContentsMargins(10, 10, 10, 10)
+        self.import_layout = QGridLayout()
+        self.import_layout.setContentsMargins(10, 10, 10, 10)
+        self.import_layout.setSpacing(5)
+        self.import_layout.setAlignment(QtCore.Qt.AlignTop)
 
         # === Add Qwidgets to the panel layout ===
-        self.load_dicom_image_push_button = add_push_button(
-            name="Open DICOM folder",
-            layout=self.loading_layout,
-            callback_function=self.load_dicom_image,
+        self.import_dicom_image_push_button = add_push_button(
+            name="Open DICOM serie",
+            layout=self.import_layout,
+            callback_function=lambda: self.set_image_with_path("folder"),
             row=0,
             column=0,
             minimum_width=COLUMN_WIDTH,
-            alignment=SEGM_METHODS_PANEL_ALIGN,
+            tooltip_text="Import DICOM data from a folder containing one serie",
         )
 
-        self.load_file_image_push_button = add_push_button(
+        self.import_file_image_push_button = add_push_button(
             name="Open image file",
-            layout=self.loading_layout,
-            callback_function=self.load_image,
+            layout=self.import_layout,
+            callback_function=lambda: self.set_image_with_path("file"),
             row=0,
             column=1,
             minimum_width=COLUMN_WIDTH,
-            alignment=SEGM_METHODS_PANEL_ALIGN,
+            tooltip_text="Import image data from one file",
         )
 
         self.file_name_text = add_label(
             text='File/Folder name: ',
-            layout=self.loading_layout,
+            layout=self.import_layout,
             row=1,
             column=0,
-            column_span=1,
+            minimum_width=COLUMN_WIDTH,
             )
 
-        self.file_name = add_label(
+        self.file_name_label = add_label(
             text='',
-            layout=self.loading_layout,
+            layout=self.import_layout,
             row=1,
             column=1,
-            column_span=1,
+            minimum_width=COLUMN_WIDTH,
             )
 
-        self.loading_panel.setLayout(self.loading_layout)
+        self.zoom_slider = add_slider(
+            layout=self.import_layout,
+            bounds=[50, 500],
+            callback_function=self.zoom,
+            row=2,
+            column=0,
+            column_span=2,
+            tooltip_text="Zoom the main camera",
+        )
+        self.zoom_slider.setStyleSheet("""
+            QSlider::handle:horizontal {{
+                image: url({});
+                margin: -30px 0px;
+                width: 25px;
+                background: transparent;
+                }}""".format(get_relative_icon_path('zoom')))
+
+        # Import tools are created in another layout
+        self.tool_import_layout = QHBoxLayout()
+
+        self.set_custom_contrast_push_button = add_icon_push_button(
+            icon=QIcon(get_icon_path('plus')),
+            layout=self.tool_import_layout,
+            callback_function=self.set_custom_contrast,
+            row=0,
+            column=0,
+            tooltip_text="Add custom contrast limit setting. Open it by selecting the Custom Contrast choice.",
+            isHBoxLayout=True,
+        )        
+        self.custom_contrast_limits = None
+        self.hu_limits = []
+
+        self.import_custom_contrast_push_button = add_icon_push_button(
+            icon=QIcon(get_icon_path('import')),
+            layout=self.tool_import_layout,
+            callback_function=self.import_custom_contrast,
+            row=0,
+            column=1,
+            tooltip_text="Import custom contrast limit setting from a .json file.",
+            isHBoxLayout=True,
+        )
+
+        self.export_custom_contrast_push_button = add_icon_push_button(
+            icon=QIcon(get_icon_path('export')),
+            layout=self.tool_import_layout,
+            callback_function=self.export_custom_contrast,
+            row=0,
+            column=2,
+            tooltip_text="Export custom contrast limit setting as .json file.",
+            isHBoxLayout=True,
+        )
+
+        self.default_contrast_combo_box = add_combo_box(
+            list_items=["Set a default contrast", "CT Bone", "CT Soft", "Custom Contrast"],
+            layout=self.tool_import_layout,
+            callback_function=self.set_default_contrast,
+            row=0,
+            column=3,
+            minimum_width=COLUMN_WIDTH,
+            tooltip_text="Use a predefined HU contrast",
+            isHBoxLayout=True,
+        )
+
+        self.import_layout.addLayout(self.tool_import_layout, 3, 0, 1, 2)
+
+        self.import_panel.setLayout(self.import_layout)
 
         # === Add panel to the main layout ===
-        self.layout.addWidget(self.loading_panel, row, column)
+        self.layout.addWidget(self.import_panel, row, column)
 
         # === Make widgets visible (after adding to the main layout to preventing them from briefly appearing in a separate window) ===
-        self.loading_panel.setVisible(True)
-        self.load_dicom_image_push_button.setVisible(True)
-        self.load_file_image_push_button.setVisible(True)
-        self.file_name_text.setVisible(True)
-        self.file_name.setVisible(True)
+        self.import_panel.setVisible(True)
+        self.import_dicom_image_push_button.setVisible(True)
+        self.import_file_image_push_button.setVisible(True)
+        
+        self.toggle_import_panel_widget(False)
 
     def add_annotation_panel(self, row, column=0):
         """
         Create annotation panel
 
         Parameters
         ----------
@@ -236,769 +293,950 @@
         # === Set panel layout parameters ===
         self.annotation_layout = QGridLayout()
         self.annotation_layout.setContentsMargins(10, 10, 10, 10)
         self.annotation_layout.setSpacing(5)
         self.annotation_layout.setAlignment(QtCore.Qt.AlignTop)
 
         # === Add Qwidgets to the panel layout ===
-        self.annotation_text = add_label(
-            text="Choose a type of structure:",
-            layout=self.annotation_layout,
-            row=0,
-            column=0,
-        )
-
-        self.annotation_combo_box = add_combobox(
+        self.import_segmentation_push_button = add_push_button(
+            name="Open segmentation file",
             layout=self.annotation_layout,
-            items=["", "Fetus", "Shoulder", "Feta Challenge"],
-            callback_function=self.toggle_annotation_sub_panel,
+            callback_function=lambda: self.set_segmentation_with_path(None),
             row=0,
             column=1,
-        )
-        # self.annotation_combo_box.setStyleSheet("QComboBox::disabled{background-color: black; color: darkgray;}")
-
-        self.load_label_push_button = add_push_button(
-            name="Open segmentation file",
-            layout=self.annotation_layout,
-            callback_function=self.load_label,
-            row=1,
-            column=0,
             column_span=2,
             minimum_width=COLUMN_WIDTH,
-            alignment=SEGM_METHODS_PANEL_ALIGN,
+            tooltip_text="Open a segmentation file with the same size of the original image",
         )
 
-        # Annotations tools are created in another layout
-        self.tool_annotation_layout = QHBoxLayout()
+        # Annotations tools are created in another layout 
+        # self.tool_annotation_layout = QHBoxLayout()
 
         self.undo_push_button = add_icon_push_button(
-            name="",
             icon=QIcon(get_icon_path('undo')),
-            layout=self.tool_annotation_layout,
-            callback_function=self.undo_label,
+            layout=self.annotation_layout,
+            callback_function=self.undo_segmentation,
             row=0,
             column=0,
             minimum_width=COLUMN_WIDTH,
-            alignment=SEGM_METHODS_PANEL_ALIGN,
-            isBoxLayout=True,
-        )
-        # self.undo_push_button.setStyleSheet("QPushButton::disabled{background-color: black; color: darkgray;}")
-
-        # self.lock_push_button = add_icon_push_button(
-        #     name="",
-        #     icon=QIcon(get_icon_path('unlock')),
-        #     layout=self.tool_annotation_layout,
-        #     callback_function=self.lock_slide,
-        #     row=0,
-        #     column=1,
-        #     minimum_width=COLUMN_WIDTH,
-        #     alignment=SEGM_METHODS_PANEL_ALIGN,
-        #     isBoxLayout=True,
-        # )
-        # self.lock_push_button.setCheckable(True)
-        # self.lock_push_button.setStyleSheet("QPushButton::disabled{background-color: black; color: darkgray;}")
-
-        self.zoom_slider = add_slider(
-            layout=self.tool_annotation_layout,
-            bounds=[50, 500],
-            callback_function=self.zoom,
-            row=0,
-            column=2,
-            isBoxLayout=True
+            tooltip_text="Undo the last painting action",
         )
-        self.zoom_slider.setStyleSheet("""
-            QSlider::handle:horizontal {{
-                image: url({});
-                margin: -30px 0px;
-                width: 25px;
-                background: transparent;
-                }}""".format(get_relative_icon_path('zoom')))
 
-        self.annotation_layout.addLayout(self.tool_annotation_layout, 2, 0, 1, 2)
+        # self.annotation_layout.addLayout(self.tool_annotation_layout, 2, 0, 1, 2)
         self.annotation_panel.setLayout(self.annotation_layout)
 
         # === Add panel to the main layout ===
         self.layout.addWidget(self.annotation_panel, row, column)
 
-    def add_reset_save_panel(self, row, column=0):
+    def add_segmentation_panel(self, row, column=0):
         """
-        Create reset and save panel
+        Create segmentation panel
 
         Parameters
         ----------
         row : int
             row position of the panel in the main QGridLayout
         column : int
             column position of the panel in the main QGridLayout
 
         """
 
         # === Set panel parameters ===
-        self.reset_save_panel = QGroupBox("3. SAVE ANNOTATION")
-        self.reset_save_panel.setStyleSheet("margin-top : 5px;")
+        self.segmentation_panel = QGroupBox("3. SEGMENT")
+        self.segmentation_panel.setStyleSheet("margin-top : 5px;")
 
         # === Set panel layout parameters ===
-        self.reset_save_layout = QGridLayout()
-        self.reset_save_layout.setSpacing(15)
+        self.segmentation_layout = QGridLayout()
+        self.segmentation_layout.setContentsMargins(10, 10, 10, 10)
+        self.segmentation_layout.setSpacing(5)
+        self.segmentation_layout.setAlignment(QtCore.Qt.AlignTop)
 
         # === Add Qwidgets to the panel layout ===
-        self.backup_push_button = add_icon_push_button(
-            name="",
-            icon=QIcon(get_icon_path('backup')),
-            layout=self.reset_save_layout,
-            callback_function=self.activate_backup_label,
+        self.run_segmentation_push_button = add_push_button(
+            name="Run segmentation",
+            layout=self.segmentation_layout,
+            callback_function=self.run_segmentation,
             row=0,
             column=0,
+            column_span=2,
             minimum_width=COLUMN_WIDTH,
-            alignment=SEGM_METHODS_PANEL_ALIGN,
+            tooltip_text="Launch the training and inference of a classifier",
         )
-        self.backup_push_button.setCheckable(True)
 
-        self.save_push_button = add_push_button(
-            name="Save",
-            layout=self.reset_save_layout,
-            callback_function=self.save_label,
-            row=0,
-            column=1,
-            column_span=1,
+        self.threshold_label = add_label(
+            text="Probability threshold:",
+            layout=self.segmentation_layout,
+            row=1,
+            column=0,
             minimum_width=COLUMN_WIDTH,
-            alignment=SEGM_METHODS_PANEL_ALIGN,
         )
 
-        self.reset_push_button = add_push_button(
-            name="Delete all",
-            layout=self.reset_save_layout,
-            callback_function=self.reset_label,
-            row=0,
-            column=2,
-            column_span=1,
+        self.threshold_slider = add_slider(
+            layout=self.segmentation_layout,
+            bounds=[0, 255],
+            callback_function=self.set_probabilities_threshold,
+            row=1,
+            column=1,
             minimum_width=COLUMN_WIDTH,
-            alignment=SEGM_METHODS_PANEL_ALIGN,
+            tooltip_text="Apply threshold on the output probability",
         )
 
-        self.reset_save_panel.setLayout(self.reset_save_layout)
+        self.segmentation_panel.setLayout(self.segmentation_layout)
 
         # === Add panel to the main layout ===
-        self.layout.addWidget(self.reset_save_panel, row, column)
+        self.layout.addWidget(self.segmentation_panel, row, column)       
 
-    def add_view_panel(self, row, column):
+    def add_reset_export_panel(self, row, column=0):
         """
-        Create view panel
+        Create reset and export panel
 
         Parameters
         ----------
         row : int
-            row position of the panel in the help QGridLayout
+            row position of the panel in the main QGridLayout
         column : int
-            column position of the panel in the help QGridLayout
+            column position of the panel in the main QGridLayout
 
         """
 
         # === Set panel parameters ===
-        self.view_panel = QGroupBox("3D VIEW AXIS")
-        self.view_panel.setStyleSheet("margin-top : 5px;")
+        self.reset_export_panel = QGroupBox("4. EXPORT ANNOTATION")
+        self.reset_export_panel.setStyleSheet("margin-top : 5px;")
 
         # === Set panel layout parameters ===
-        self.view_layout = QGridLayout()
-        self.view_layout.setSpacing(5)
-        self.view_layout.setContentsMargins(10, 10, 10, 10)
+        self.reset_export_layout = QGridLayout()
+        self.reset_export_layout.setSpacing(5)
 
         # === Add Qwidgets to the panel layout ===
-        self.view_image_1 = add_image_widget(
-            name="view1",
-            layout=self.view_layout,
-            image_path='',
+        self.export_seg_push_button = add_push_button(
+            name="Export segmentation",
+            layout=self.reset_export_layout,
+            callback_function=self.export_segmentation,
             row=0,
             column=0,
-            visibility=False,
-            minimum_width=0
-            )
+            minimum_width=COLUMN_WIDTH,
+            tooltip_text="Export only the segmented probability data",
+        )
 
-        self.view_image_2 = add_image_widget(
-            name="view2",
-            layout=self.view_layout,
-            image_path='',
+        self.export_proba_push_button = add_push_button(
+            name="Export probabilities",
+            layout=self.reset_export_layout,
+            callback_function=self.export_probabilities,
             row=0,
             column=1,
-            visibility=False,
-            minimum_width=0
-            )
-
-        self.view_panel.setLayout(self.view_layout)
-
-        # === Add panel to the help layout ===
-        self.help_layout.addWidget(self.view_panel, row, column)
-
-    def add_atlas_panel(self, row, column):
-        """
-        Create atlas panel
-
-        Parameters
-        ----------
-        row : int
-            row position of the panel in the help QGridLayout
-        column : int
-            column position of the panel in the help QGridLayout
-
-        """
-
-        # === Set panel parameters ===
-        self.atlas_panel = QGroupBox("ATLAS")
-        self.atlas_panel.setStyleSheet("margin-top : 5px;")
-
-        # === Set panel layout parameters ===
-        self.atlas_layout = QGridLayout()
-        self.atlas_layout.setSpacing(5)
-        self.atlas_layout.setContentsMargins(10, 10, 10, 10)
-
-        # === Add Qwidgets to the panel layout ===
-        self.atlas_label = add_label(
-            text='',
-            layout=self.atlas_layout,
-            row=0,
-            column=0)
+            minimum_width=COLUMN_WIDTH,
+            tooltip_text="Export only the probability data",
+        )
 
-        self.canvas_ax1 = VispyCanvas(
-            keys=None,
-            vsync=True,
-            parent=self.atlas_label,
+        self.reset_push_button = add_push_button(
+            name="Delete all",
+            layout=self.reset_export_layout,
+            callback_function=self.reset_segmentation,
+            row=1,
+            column=0,
+            column_span=2,
+            minimum_width=COLUMN_WIDTH,
+            tooltip_text="Delete all segmentation data",
         )
 
-        self.atlas_panel.setLayout(self.atlas_layout)
+        self.reset_export_panel.setLayout(self.reset_export_layout)
+
+        # === Add panel to the main layout ===
+        self.layout.addWidget(self.reset_export_panel, row, column)
 
-        # === Add panel to the help layout ===
-        self.help_layout.addWidget(self.atlas_panel, row, column)
 
-    def enable_panels(self, list_panel_names, isVisible):
+# ============ Toggle widgets and panel ============
+    def toggle_panels(self, list_panel_names, isVisible):
         """
         Make visible panels
 
         Parameters
         ----------
         list_panel_names : List[str]
             list of the name of the panels to enable
         isVisible : bool
             visible status of the panels
+
         """
         for panel_name in list_panel_names:
             if panel_name == "annotation_panel":
                 self.annotation_panel.setVisible(isVisible)
-                self.annotation_text.setVisible(isVisible)
-                self.annotation_combo_box.setVisible(isVisible)
-                self.load_label_push_button.setVisible(isVisible)
-                self.zoom_slider.setVisible(isVisible)
+                self.import_segmentation_push_button.setVisible(isVisible)
                 self.undo_push_button.setVisible(isVisible)
-                # self.lock_push_button.setVisible(isVisible)
-
-            elif panel_name == "reset_save_panel":
-                self.reset_save_panel.setVisible(isVisible)
-                self.backup_push_button.setVisible(isVisible)
-                self.reset_push_button.setVisible(isVisible)
-                self.save_push_button.setVisible(isVisible)
-
-            elif panel_name == "view_panel":
-                self.view_panel.setVisible(isVisible)
-                self.view_image_1.setVisible(isVisible)
-                self.view_image_2.setVisible(isVisible)
             
-            elif panel_name == "atlas_panel":
-                self.atlas_panel.setVisible(isVisible)
-                self.atlas_label.setVisible(isVisible)
+            elif panel_name == "segmentation_panel":
+                self.segmentation_panel.setVisible(isVisible)
+                self.run_segmentation_push_button.setVisible(isVisible)
+                self.threshold_label.setVisible(isVisible)
+                self.threshold_slider.setVisible(isVisible)
+
+            elif panel_name == "reset_export_panel":
+                self.reset_export_panel.setVisible(isVisible)
+                self.export_seg_push_button.setVisible(isVisible)
+                self.reset_push_button.setVisible(isVisible)
+                self.export_proba_push_button.setVisible(isVisible)
 
-    def toggle_annotation_sub_panel(self):
+    def toggle_annotation_sub_panel(self, isVisible):
         """
             Toggle sub panel of the structure to annotate
+
         """
-        structure_name = self.annotation_combo_box.currentText()
+        self.oneshot.toggle_sub_panel(isVisible)
 
-        isFetus = self.fetus.subpanel.isVisible()
-        isShoulder = self.shoulder.subpanel.isVisible()
-        isFeta = self.feta.subpanel.isVisible()
-
-        if (isFetus and structure_name != "Fetus") or (isShoulder and structure_name != "Shoulder") or (isFeta and structure_name != "Feta Challenge"):
-            canRemoveLabel = self.can_remove_label_data()
-        elif (isFetus and structure_name == "Fetus") or (isShoulder and structure_name == "Shoulder") or (isFeta and structure_name == "Feta Challenge"):
-            return
-        else:
-            canRemoveLabel = True
+        self.reset_annotation_radio_button_checked_id()
+        self.reset_annotation_layer_selected_label()
 
-        if canRemoveLabel:
-            if structure_name == "Fetus":
-                toggle_fetus = True
-                toggle_shoulder = False
-                toggle_feta = False
-
-            elif structure_name == "Shoulder":
-                toggle_fetus = False
-                toggle_shoulder = True
-                toggle_feta = False
-
-            elif structure_name == "Feta Challenge":
-                toggle_fetus = False
-                toggle_shoulder = False
-                toggle_feta = True
+    def toggle_import_panel_widget(self, isVisible, file_type=None):
+        """
+        Toggle widget or the import panel (default contrast option only for DICOM image (use housfield value))
+        
+        Parameters
+        ----------
+        isVisible : bool
+            visible status of the widgets
+        file_type : str
+            type of image loaded : "file" for .tiff, .tif, .nii and .nii.gz and "folder" for DICOM folder
+            
+        """
+        self.zoom_slider.setVisible(isVisible)
+        self.file_name_text.setVisible(isVisible)
+        self.file_name_label.setVisible(isVisible)
+
+        if file_type == "file":
+            self.set_custom_contrast_push_button.setVisible(False)
+            self.import_custom_contrast_push_button.setVisible(False)
+            self.export_custom_contrast_push_button.setVisible(False)
+            self.default_contrast_combo_box.setVisible(False)
+
+        elif file_type == 'folder':
+            self.set_custom_contrast_push_button.setVisible(False)
+            self.import_custom_contrast_push_button.setVisible(True)
+            self.export_custom_contrast_push_button.setVisible(True)
+            self.default_contrast_combo_box.setVisible(True)
+            
+        else:
+            self.set_custom_contrast_push_button.setVisible(False)
+            self.import_custom_contrast_push_button.setVisible(isVisible)
+            self.export_custom_contrast_push_button.setVisible(isVisible)
+            self.default_contrast_combo_box.setVisible(isVisible)
 
-            else:
-                toggle_fetus = False
-                toggle_shoulder = False
-                toggle_feta = False
-
-            self.fetus.toggle_sub_panel(toggle_fetus)
-            self.shoulder.toggle_sub_panel(toggle_shoulder)
-            self.feta.toggle_sub_panel(toggle_feta)
-
-            # Reset label data
-            self.remove_label()
-            self.add_label_layers(label_data=[])
-            self.reset_annotation_radio_buttons()
-
-        else:
-            if isFetus:
-                self.annotation_combo_box.setCurrentText("Fetus")
-            elif isShoulder:
-                self.annotation_combo_box.setCurrentText("Shoulder")
-            elif isFeta:
-                self.annotation_combo_box.setCurrentText("Feta Challenge")
-            else:
-                self.annotation_combo_box.setCurrentText("")
 
-# ============ Define callbacks ============
-    def load_dicom_image(self):
-        """
-        Load a complete DICOM serie and convert it in a .nii file to be directly open in Napari.
-        The created .nii file will be deleted when saving the segmentation (see save_segmentation function).
+# ============ Import data ============
+    def import_dicom_folder(self):
         """
+        Import a complete DICOM serie from a folder
 
+        Returns
+        ----------
+        image_arr : ndarray
+            3D image as a 3D array. None if importation failed.
+
+        """
         dicom_path = QFileDialog.getExistingDirectory(self, 'Choose a DICOM serie directory')
-        self.img_dir = dicom_path
 
         if dicom_path == "":
-            return
-        # if not glob.glob('*.dcm'):
-        #     display_warning_box(self, "Error", "No DICOM files in the directory")
-        #     return
+            return None
 
+        if (Path(dicom_path).name == 'Raw') or (Path(dicom_path).name == 'ST0'):
+            self.image_dir = Path(dicom_path).parents[1]
+            file_name = Path(dicom_path).parents[0].name
+        else:
+            self.image_dir = Path(dicom_path).parents[0]
+            file_name = Path(dicom_path).name
 
         reader = sitk.ImageSeriesReader()
+
+        series_found = reader.GetGDCMSeriesIDs(dicom_path)
+        if len(series_found) > 1:
+            display_warning_box(self, "Error", "More than one DICOM serie in the folder. Select a folder containing a single DICOM serie.")
+            return None
+
         img_names = reader.GetGDCMSeriesFileNames(dicom_path)
         reader.SetFileNames(img_names)
-        self.image_sitk = reader.Execute()
+        try:
+            self.image_sitk = reader.Execute()
+        except:
+            display_warning_box(self, "Error", "NO DICOM data in the folder.")
+            return None
 
-        image = sitk.GetArrayFromImage(self.image_sitk) # z, y, x
+        image_arr = sitk.GetArrayFromImage(self.image_sitk) # z, y, x
         #ITK's Image class does not have a bracket operator. It has a GetPixel which takes an ITK Index object as an argument, which is an array ordered as (x,y,z). This is the convention that SimpleITK's Image class uses for the GetPixel method as well.
         # While in numpy, an array is indexed in the opposite order (z,y,x).
 
-        canRemove = self.can_remove_all()
+        if len(image_arr.shape) != 3:
+            display_warning_box(self, "Error", "Incorrect file size. Need to be a 3D image")
+            return None
 
-        if canRemove:
-            self.remove_image()
-            self.viewer.add_image(image, name='image')
+        self.file_name_label.setText(file_name)
 
-            disable_layer_widgets(self.viewer, 'image')
+        return image_arr
 
-            self.enable_panels(["annotation_panel", "reset_save_panel"], True)
-            self.reset_zoom_slider()
+    def import_image_file(self):
+        """
+        Import a 3D image file of type .tiff, .tif, .nii or .nii.gz
+
+        Returns
+        ----------
+        image_arr : ndarray
+            3D image as a 3D array. None if importation failed.
 
-            self.remove_label()
-            self.add_label_layers(label_data=[])
-            self.reset_annotation_radio_buttons()
-
-            self.fetus.toggle_sub_panel(False)
-            self.shoulder.toggle_sub_panel(False)
-            self.feta.toggle_sub_panel(False)
-            self.annotation_combo_box.setCurrentText("")
+        """
+        files_types = "Image File (*.tif *.tiff *.nii.gz *.nii)"
+        file_path, _ = QFileDialog.getOpenFileName(self, "Choose a 3D image file", "" , files_types )
+
+        if file_path == "":
+            return None
 
-            self.file_name.setText(Path(dicom_path).stem)
+        extensions = Path(file_path).suffixes
+        self.image_dir = Path(file_path).parents[0]
+
+        if (extensions[-1] == ".tif") or (extensions[-1] == ".tiff"):
+            image_arr = tif.imread(file_path)
+            self.image_sitk = sitk.Image(image_arr.shape[2], image_arr.shape[1], image_arr.shape[0], sitk.sitkInt16)
+            self.file_name_label.setText(Path(file_path).stem)
+
+        elif extensions[-1] == ".nii":
+            self.image_sitk = sitk.ReadImage(file_path)
+            image_arr = sitk.GetArrayFromImage(self.image_sitk)
+            self.file_name_label.setText(Path(file_path).stem)
+
+        elif extensions[-1] == ".gz":
+            if len(extensions) >= 2:
+                if extensions[-2] == ".nii":               
+                    self.image_sitk = sitk.ReadImage(file_path)
+                    image_arr = sitk.GetArrayFromImage(self.image_sitk)
+                    self.file_name_label.setText(Path(Path(file_path).stem).stem)
+                else:
+                    return None
 
         else:
-            return
+            return None
 
-    def load_image(self):
+        if len(image_arr.shape) != 3:
+            display_warning_box(self, "Error", "Incorrect file size. Need to be a 3D image")
+            return None
+        
+        return image_arr
+
+    def import_segmentation_file(self, default_file_path=None):
         """
-            Load an image file of type .tiff, .tif, .nii.gz
+        Import segmentation image file of type .tiff, .tif, .nii or .nii.gz
+
+        Parameters
+        ----------
+        default_file_path : Pathlib.Path
+            path of the segmentation image to import. If None, a QFileDialog is open to aks a path.
+
+        Returns
+        ----------
+        segmentation_arr : ndarray
+            segmentation image as a 3D array. None if importation failed.
+
         """
+        if default_file_path is None:
+            files_types = "Image File (*.tif *.tiff *.nii.gz *.nii)"
+            file_path, _ = QFileDialog.getOpenFileName(self, "Choose a segmentation file", "" , files_types)
 
-        files_types = "TIF (*.tif);;TIFF (*.tiff);;NIFTI compressed (*.nii.gz)"
-        file_path, _ = QFileDialog.getOpenFileName(self, "Choose a image file", "" , files_types )
+            if file_path == "":
+                return None
 
-        if file_path == "":
-            return
+        else:
+            file_path = str(default_file_path)
 
         extensions = Path(file_path).suffixes
-        self.img_dir = Path(file_path).parents[0]
 
-        if len(extensions) == 1:
-            if (extensions[0] == ".tif") or (extensions[0] == ".tiff"):           
-                image = tif.imread(file_path)
-                self.image_sitk = sitk.Image(image.shape[2], image.shape[1], image.shape[0], sitk.sitkInt16)
-       
-        elif len(extensions) == 2:
-            if (extensions[0] == ".nii") and (extensions[1] == ".gz"):               
-                self.image_sitk = sitk.ReadImage(file_path)
-                image = sitk.GetArrayFromImage(self.image_sitk)
+        if (extensions[-1] == ".tif") or (extensions[-1] == ".tiff"):
+            segmentation_arr = tif.imread(file_path)
+
+        elif extensions[-1] == ".nii" :
+            segmentation_sitk = sitk.ReadImage(file_path)
+            segmentation_arr = sitk.GetArrayFromImage(segmentation_sitk)
+            segmentation_arr = segmentation_arr.astype(np.uint8)
+
+            if any(n < 0 for n in np.unique(segmentation_arr)):
+                display_warning_box(self, "Error", "Incorrect NIFTI format : negative value")
+                return
+
+        elif extensions[-1] == ".gz":
+            if len(extensions) >= 2:
+                if extensions[-2] == ".nii":                
+                    segmentation_sitk = sitk.ReadImage(file_path)
+                    segmentation_arr = sitk.GetArrayFromImage(segmentation_sitk)
+                    segmentation_arr = segmentation_arr.astype(np.uint8)
+
+                    if any(n < 0 for n in np.unique(segmentation_arr)):
+                        display_warning_box(self, "Error", "Incorrect NIFTI format : negative value")
+                        return
+                else:
+                    return None
+
         else:
+            return None
+
+        if len(segmentation_arr.shape) != 3:
+            display_warning_box(self, "Error", "Incorrect file size. Need to be a 3D image")
+            return None
+        
+        return segmentation_arr
+
+    def import_custom_contrast(self):
+        """
+        Import custom contrast limits from a .json file and apply it
+
+        """
+        files_types = "JSON File (*.json)"
+        file_path, _ = QFileDialog.getOpenFileName(self, "Choose a JSON image", "" , files_types)
+
+        if file_path == "":
+            return None
+
+        self.default_contrast_combo_box.setCurrentText("Set a default contrast")
+
+        with open(file_path) as f:
+            self.import_contrast = json.load(f)
+        
+        if (np.max(self.import_contrast) <= self.viewer.layers['image'].contrast_limits_range[1]) and (np.min(self.import_contrast) >= self.viewer.layers['image'].contrast_limits_range[0]):
+            self.custom_contrast_limits = self.import_contrast
+        else: 
+            display_warning_box(self, "Error", "The imported contrast limit is outside of the image contrast range.")
             return
 
+        self.default_contrast_combo_box.setCurrentText("Custom Contrast")
+
+
+# ============ Update data ============
+    def set_image_with_path(self, file_type):
+        """
+        Update image data by asking file path to the user.
+        Import image data, add it to napari, toggle panels, check if a corresponding segmentation data file exist (if so, import it and add it to napari).
+        
+        Parameters
+        ----------
+        file_type : str
+            type of image loaded : "file" for .tiff, .tif, .nii and .nii.gz and "folder" for DICOM folder
+            
+        """
         canRemove = self.can_remove_all()
 
         if canRemove:
-            self.remove_image()
-            self.viewer.add_image(image, name='image')
+            self.status_label.setText("Loading...")
 
-            disable_layer_widgets(self.viewer, 'image')
+            if file_type == "file":
+                image_arr = self.import_image_file()
+            elif file_type == 'folder':
+                image_arr = self.import_dicom_folder()
+
+            if image_arr is None:
+                self.status_label.setText("Ready")
+                return
+
+            self.set_image_layer(image_arr)
 
-            self.enable_panels(["annotation_panel", "reset_save_panel"], True)
             self.reset_zoom_slider()
+            self.reset_threshold_slider()
+            self.default_contrast_combo_box.setCurrentText("Set a default contrast")
+
+            self.toggle_import_panel_widget(True, file_type)
+            self.toggle_panels(["annotation_panel", "segmentation_panel", "reset_export_panel"], True)
 
-            self.remove_label()
-            self.add_label_layers(label_data=[])
-            self.reset_annotation_radio_buttons()
-
-            self.fetus.toggle_sub_panel(False)
-            self.shoulder.toggle_sub_panel(False)
-            self.feta.toggle_sub_panel(False)
-            self.annotation_combo_box.setCurrentText("")
+            segmentation_arr = np.zeros(image_arr.shape, dtype=np.int8)
+            self.set_segmentation_layer(segmentation_arr)
+
+            self.remove_probabilities_layer()
+            self.remove_segmented_probabilities_layer()
+
+            self.toggle_annotation_sub_panel(True)
+
+            napari.features_3d = Features3D()
+
+            self.status_label.setText("Ready")
+
+        else:
+            return
 
-            self.file_name.setText(Path(file_path).stem)
+    def set_segmentation_with_path(self, segmentation_path=None):
+        """
+        Update segmentation data from a file path : import data and add it to napari.
+        
+        Parameters
+        ----------
+        segmentation_path : str
+            path of the segmentation file
+            
+        """
 
+        # not from a corresponding segmentation file found for the image
+        if segmentation_path is None:
+            canRemove = self.can_remove_segmentation_data()
+        # from a corresponding segmentation file found for the image (not ask for remove because all ready done)
         else:
+            canRemove = True
+
+        if canRemove:
+            self.status_label.setText("Loading...")
+
+            segmentation_arr = self.import_segmentation_file(segmentation_path)
+
+            if segmentation_arr is None:
+                self.status_label.setText("Ready")
+                return
+            
+            if "image" in self.viewer.layers:
+                image_arr = self.viewer.layers['image'].data 
+                if segmentation_arr.shape != image_arr.shape:
+                    display_warning_box(self, "Error", "Size of the segmentation file doesn't correspond to the size of the source image")
+                    self.status_label.setText("Ready")
+                    return
+
+                self.set_segmentation_layer(segmentation_arr)
+                self.status_label.setText("Ready")
+
+
+# ============ Export data ============
+    def export_segmentation(self):
+        """
+            Export the labelled data as a unique 3D image, or multiple 3D images (one by label)
+
+        """
+        files_types = "Image File (*.tif *.tiff *.nii.gz *.nii)"
+
+        default_filepath = Path(self.image_dir).joinpath(self.file_name_label.text() + "_segmented_probabilities.tif")
+        file_path, _ = QFileDialog.getSaveFileName(self, "Export Segmentation", str(default_filepath), files_types)
+
+        # If choose "Cancel"
+        if file_path == "":
             return
 
-    def load_label(self):
+        if hasattr(self.viewer, 'layers'):
+            if "segmented probabilities" in self.viewer.layers:
+                self.status_label.setText("Saving...")
+
+                segmentation_arr = self.viewer.layers['segmented probabilities'].data
+
+                extensions = Path(file_path).suffixes
+                if len(extensions) == 1:
+                    if (extensions[0] == ".tif") or (extensions[0] == ".tiff"): 
+                        tif.imsave(file_path, segmentation_arr)
+                    elif extensions[0] == ".nii":
+                        result_image_sitk = sitk.GetImageFromArray(segmentation_arr.astype(np.uint16))
+                        result_image_sitk.CopyInformation(self.image_sitk)
+                        sitk.WriteImage(result_image_sitk, file_path)
+                elif len(extensions) == 2:
+                    if (extensions[0] == ".nii") and (extensions[1] == ".gz"):
+                        result_image_sitk = sitk.GetImageFromArray(segmentation_arr.astype(np.uint16))
+                        result_image_sitk.CopyInformation(self.image_sitk)
+                        sitk.WriteImage(result_image_sitk, file_path)
+
+                self.status_label.setText("Ready")
+
+            else:
+                display_warning_box(self, "Error", "No segmentation data find")
+                return
+
+    def export_probabilities(self):
         """
-            Load label image file of type .tiff, .tif or .nii.gz
+            Export the labelled data as a unique 3D image, or multiple 3D images (one by label)
+
         """
+        files_types = "Image File (*.tif *.tiff *.nii.gz *.nii)"
 
-        files_types = "TIF (*.tif);;TIFF (*.tiff);;NIFTI compressed (*.nii.gz)"
-        file_path, _ = QFileDialog.getOpenFileName(self, "Choose a segmentation file", "" , files_types )
+        default_filepath = Path(self.image_dir).joinpath(self.file_name_label.text() + "_probabilities.tif")
+        file_path, _ = QFileDialog.getSaveFileName(self, "Export Probabilities", str(default_filepath), files_types)
 
+        # If choose "Cancel"
         if file_path == "":
             return
 
-        canRemoveLabel = self.can_remove_label_data()
+        if hasattr(self.viewer, 'layers'):
+            if "probabilities" in self.viewer.layers:
+
+                self.status_label.setText("Saving...")
 
-        if canRemoveLabel:
-            self.remove_label()
+                proba_arr = self.viewer.layers['probabilities'].data
 
-            extensions = Path(file_path).suffixes
+                extensions = Path(file_path).suffixes
 
-            if len(extensions) == 1:
-                if (extensions[0] == ".tif") or (extensions[0] == ".tiff"): 
-                    label = tif.imread(file_path)
-                    self.add_label_layers(label_data=label)
-
-            elif len(extensions) == 2:
-                if (extensions[0] == ".nii") and (extensions[1] == ".gz"):
-                    label_sitk = sitk.ReadImage(file_path)
-                    label = sitk.GetArrayFromImage(label_sitk)
-                    label = label.astype(np.uint8)
-                    # self.originalType = label.dtype
+                if (extensions[-1] == ".tif") or (extensions[-1] == ".tiff"): 
+                    tif.imsave(file_path, proba_arr)
+
+                elif extensions[-1] == ".nii": 
+                    result_image_sitk = sitk.GetImageFromArray(proba_arr.astype(np.uint8))
+                    result_image_sitk.CopyInformation(self.image_sitk)
+                    sitk.WriteImage(result_image_sitk, file_path)
+
+                elif extensions[-1] == ".gz":
+                    if len(extensions) >= 2:
+                        if extensions[-2] == ".nii": 
+                            result_image_sitk = sitk.GetImageFromArray(proba_arr.astype(np.uint8))
+                            result_image_sitk.CopyInformation(self.image_sitk)
+                            sitk.WriteImage(result_image_sitk, file_path)
+                
+                self.status_label.setText("Ready")
 
-                    if any(n < 0 for n in np.unique(label)):
-                        display_warning_box(self, "Error", "Incorrect NIFTI format : negative value")
-                        return
-                    self.add_label_layers(label_data=label)
             else:
+                display_warning_box(self, "Error", "No segmentation data find")
                 return
 
-            self.reset_annotation_radio_buttons()
+    def export_custom_contrast(self):
+        """
+        Export custom contrast limits as a .json file that can be re-open in the plugin
 
-            # self.fetus.toggle_sub_panel(False)
-            # self.shoulder.toggle_sub_panel(False)
-            # self.feta.toggle_sub_panel(False)
-            # self.annotation_combo_box.setCurrentText("")
+        """
+        if self.custom_contrast_limits is not None:
 
+            files_types = "JSON File (*.json)"
+
+            default_filepath = Path(self.image_dir).joinpath(self.file_name_label.text() + "_custom_contrast.json")
+            file_path, _ = QFileDialog.getSaveFileName(self, "Export contrast limit parameters", str(default_filepath), files_types)
+
+            # If choose "Cancel"
+            if file_path == "":
+                return
+
+            with open(file_path, 'w') as f:
+                json.dump(self.custom_contrast_limits, f)
+            
         else:
+            display_warning_box(self, "Error", "No custom contrast limits saved. Click on + button to add one (it will take the value of the current contrast limits used).")
+
+
+# ============ Run One Shot Learning ============
+    def run_segmentation(self):
+        """
+            Run One shot learning : training and inference steps
+
+        """
+        self.status_label.setText("Computing...")
+
+        if hasattr(self.viewer, 'layers'):
+            if 'image' in self.viewer.layers:
+                image_arr = self.viewer.layers['image'].data
+            else:
+                display_warning_box(self, "Error", "No image data.")
+                self.status_label.setText("Ready")
+                return
+
+            if 'annotations' in self.viewer.layers:
+                segmentation_arr = self.viewer.layers['annotations'].data
+            else:
+                display_warning_box(self, "Error", "No annotation data.")
+                self.status_label.setText("Ready")
+                return
+
+        #check if 2 classes have been annotated 
+        label_items = np.unique(segmentation_arr)
+        label_items = np.delete(label_items, 0)
+        if len(label_items) != 2:
+            display_warning_box(self, "Error", "Incorrect number of classes. You have to annotate 2 differents classes (background not included).")
+            self.status_label.setText("Ready")
             return
 
-    def add_label_layers(self, label_data=[]):
+        files_types = "PICKLE (*.pckl)"
+
+        default_filepath = Path(self.image_dir).joinpath(self.file_name_label.text() + "_model_rfc.pckl")
+        output_classifier_path, _ = QFileDialog.getSaveFileName(self, "Export Model File", str(default_filepath), files_types)
+
+        output_proba = run_one_shot_learning(image_arr, segmentation_arr, str(output_classifier_path))
+
+        self.set_probabilities_layer(output_proba)
+
+        self.reset_threshold_slider()
+        output_threshold = np.where(output_proba > self.threshold_slider.value(), 255, 0)
+        self.set_segmented_probabilities_layer(output_threshold)
+
+        self.status_label.setText("Ready")
+
+
+# ============ Update napari layers ============
+    def set_image_layer(self, array):
+        """
+        Remove the image layer from Napari and add a new image layer (faster than changing the data of an existing layer)
+
+        Parameters
+        ----------
+        array : ndarray
+            3D image data to add
+
         """
-        Add a new layer to the NAPARI viewer for annotation.
+        self.remove_image_layer()
+        self.viewer.add_image(array, name='image')
+        self.viewer.layers['image'].contrast_limits = (np.min(array), np.max(array))
+        disable_layer_widgets(self.viewer, layer_name='image', layer_type='image')
+        self.viewer.layers['image'].events.contrast_limits.connect(self.reset_default_contrast_combo_box)
+
+    def set_segmentation_layer(self, array):
+        """
+        Remove the segmentation layer from Napari and add a new segmentation layer (faster than changing the data of an existing layer)
         New layer can be empty for initialisation.
 
         Parameters
         ----------
-        label_data : 3Darray
-            labelled data with the same size than the raw image (display in the 'image' layer)
+        array : ndarray
+            3D segmentation data with the same size than the raw image (display in the 'image' layer)
 
         """
-        if hasattr(self.viewer, 'layers'):
-            if 'image' in self.viewer.layers:
-                source_img = self.viewer.layers['image'].data
+        self.remove_segmentation_layer()
+        self.viewer.add_labels(array, name='annotations')
+        self.reset_annotation_layer_selected_label()
+        disable_layer_widgets(self.viewer, layer_name='annotations', layer_type='label')
+    
+    def set_probabilities_layer(self, array):
+        """
+        Remove the probabilities layer from Napari and add a new probabilities layer (faster than changing the data of an existing layer)
+        New layer can be empty for initialisation.
 
-                if label_data == []:
-                    label_img = np.zeros(source_img.shape, dtype=np.int8)
-                else:
-                    label_img = label_data
-                    if label_img.shape != source_img.shape:
-                        display_warning_box(self, "Error", "Size of the segmentation file doesn't correspond to the size of the source image")
-                        return
+        Parameters
+        ----------
+        array : ndarray
+            3D probabilities data
 
+        """
+        self.remove_probabilities_layer()
+        self.viewer.add_image(array, name='probabilities')
+        disable_layer_widgets(self.viewer, layer_name='probabilities', layer_type='image')
+        self.viewer.layers['probabilities'].visible = False
+ 
+    def set_segmented_probabilities_layer(self, array):
+        """
+        Remove the segmented probabilities layer from Napari and add a new segmented probabilities layer (faster than changing the data of an existing layer)
 
-                labels_layer = self.viewer.add_labels(label_img, name='annotations')
+        Parameters
+        ----------
+        array : ndarray
+            probabilities data (0-1)
 
-                if self.annotation_combo_box.currentText() == "Fetus":
-                    self.viewer.layers['annotations'].selected_label = self.fetus.nbr_buttons
-                elif self.annotation_combo_box.currentText() == "Shoulder":
-                    self.viewer.layers['annotations'].selected_label = self.shoulder.nbr_buttons
-                elif self.annotation_combo_box.currentText() == "Feta Challenge":
-                    self.viewer.layers['annotations'].selected_label = self.feta.nbr_buttons
-                else:
-                    self.viewer.layers['annotations'].selected_label = 0
+        """
+        if "segmented probabilities" in self.viewer.layers:
+            self.viewer.layers["segmented probabilities"].data = array
+        else:
+            self.viewer.add_image(array, name='segmented probabilities', colormap="red", opacity=0.5)
+            disable_layer_widgets(self.viewer, layer_name='segmented probabilities', layer_type='image')
 
-                self.viewer.layers['annotations'].mode = "PAINT"
 
-                disable_layer_widgets(self.viewer, 'annotations')
+# ============ Apply widget value ============
+    def set_custom_contrast(self):
+        """
+        Save the current contrast limits as a "Custom Contrast" to be re-used.
 
-                # qctrl = self.viewer.window._qt_viewer.controls.widgets[self.viewer.layers['annotations']]
-                # qctrl.opacitySlider.setMaximum(0.8)
-            else:
-                display_warning_box(self, "Error", "Load first a image")
+        """
+        if "image" in self.viewer.layers:
+            self.custom_contrast_limits = self.viewer.layers['image'].contrast_limits
+            self.default_contrast_combo_box.setCurrentText("Custom Contrast")
 
-        else:
-            display_warning_box(self, "Error", "Load first a image")
+    def set_default_contrast(self):
+        """
+        Change the image contrast limits according to a predefined contrast window ("CT Bone" or "CT Soft").
+        Can only be apply to a DICOM image, because windows are defined using the Hounsfiled units.
 
-    def zoom(self):
         """
-            Zoom the camera view of the main canvas of NAPARI
+        if "image" in self.viewer.layers:
+            rescale_intercept = - self.viewer.layers['image'].contrast_limits_range[0]
+            if self.default_contrast_combo_box.currentText() == "CT Bone":
+                self.hu_limits = (-450, 1050)
+                # hu = pixel_value * slope + intercept
+                self.viewer.layers['image'].contrast_limits = self.hu_limits
+                # self.viewer.layers['image'].contrast_limits_range = (self.viewer.layers['image'].data.min(), self.viewer.layers['image'].data.max())
+           
+            elif self.default_contrast_combo_box.currentText() == "CT Soft":
+                self.hu_limits = (-160, 240)
+                self.viewer.layers['image'].contrast_limits = self.hu_limits
+
+            elif self.default_contrast_combo_box.currentText() == "Custom Contrast":
+                if self.custom_contrast_limits is not None:
+                    self.viewer.layers['image'].contrast_limits = self.custom_contrast_limits
+                else:
+                    display_warning_box(self, "Error", "No custom contrast limits saved. Click on + button to add one (it will take the value of the current contrast limits used).")
+
+            else:
+                return
+        else:
+            self.default_contrast_combo_box.setCurrentText("Set a default contrast")
+    
+    def set_probabilities_threshold(self):
+        """
+        Update threshold value use to create the segmented probabilities.
+        
         """
-        # TODO check value slider
-        self.viewer.camera.zoom = self.zoom_slider.value() / 100
+        value = self.threshold_slider.value()
 
-    def undo_label(self):
+        if hasattr(self.viewer, 'layers'):
+            if 'probabilities' in self.viewer.layers:
+                output_proba = self.viewer.layers["probabilities"].data
+                threshold_arr = np.where(output_proba > value, 255, 0)
+                self.set_segmented_probabilities_layer(threshold_arr)
+    
+    def undo_segmentation(self):
         """
             Undo last operation of annotation
+
         """
         if hasattr(self.viewer, 'layers'):
             if 'annotations' in self.viewer.layers:
-                label_layer = self.viewer.layers['annotations']
-                label_layer.undo()
+                segmentation_layer = self.viewer.layers['annotations']
+                segmentation_layer.undo()
+
+    def zoom(self):
+        """
+            Zoom the camera view of the main canvas of napari
 
-    # def lock_slide(self):
-    #     """
-    #     """
+        """
+        self.viewer.camera.zoom = self.zoom_slider.value() / 100
 
-    #     if self.lock_push_button.isChecked() == True:
-    #         self.lock_push_button.setIcon(QIcon(get_icon_path('lock')))
-    #     else:
-    #         self.lock_push_button.setIcon(QIcon(get_icon_path('unlock')))
 
-    def save_label(self):
+# ============ Reset widget options ============
+    def reset_annotation_layer_selected_label(self):
         """
-            Save the labelled data as a unique 3D image, or multiple 3D images (one by label)
+        Reset the selected structure to annotate.
+
         """
-        files_types = "TIFF (*.tiff);;TIF (*.tif);;NIFTI compressed (*.nii.gz)"
+        if "annotations" in self.viewer.layers:
+            self.viewer.layers['annotations'].selected_label = 1
+            self.viewer.layers['annotations'].mode = "PAINT"
+            self.viewer.layers['annotations'].opacity = 0.6
 
-        default_filepath = Path(self.img_dir).joinpath("segmentation.tif")
-        file_path, _ = QFileDialog.getSaveFileName(self, "Save Segmentation", str(default_filepath), files_types)
+    def reset_annotation_radio_button_checked_id(self):
+        """
+        Reset selected radio button (i.e. the element to annotate) to the first item of the list.
 
-        # If choose "Cancel"
-        if file_path == "":
-            return
+        """
+        radio_button_to_check = self.oneshot.group_radio_button.button(1)
+        radio_button_to_check.setChecked(True)
+    
+    def reset_default_contrast_combo_box(self):
+        """
+        Reset the selected structure to annotate.
 
-        if hasattr(self.viewer, 'layers'):
-            if "annotations" in self.viewer.layers:
+        """
+        if "image" in self.viewer.layers:
+            if (self.default_contrast_combo_box.currentText() == "CT Bone") or (self.default_contrast_combo_box.currentText() == "CT Soft"):
+                if self.viewer.layers['image'].contrast_limits != list(self.hu_limits):
+                    self.default_contrast_combo_box.setCurrentText("Set a default contrast")
 
-                saving_mode = display_save_message_box(
-                    "Saving Mode",
-                    "Do you want to save all label in once file, or independently ?",
-                )
+    def reset_threshold_slider(self):
+        """
+        Reset the threshold slider to 125
 
-                label_img = self.viewer.layers['annotations'].data
+        """
+        self.threshold_slider.setValue(125)
 
-                extensions = Path(file_path).suffixes
+    def reset_zoom_slider(self):
+        """
+        Reset the zoom slider to 100 (i.e. no zoom)
 
-                if saving_mode: # if All
-                    if len(extensions) == 1:
-                        if (extensions[0] == ".tif") or (extensions[0] == ".tiff"): 
-                            tif.imsave(file_path, label_img)
-                    elif len(extensions) == 2:
-                        if (extensions[0] == ".nii") and (extensions[1] == ".gz"):
-                            result_image_sitk = sitk.GetImageFromArray(label_img.astype(np.uint16))
-                            # result_image_sitk = sitk.GetImageFromArray(label_img)
-                            result_image_sitk.CopyInformation(self.image_sitk)
-                            sitk.WriteImage(result_image_sitk, file_path)
+        """
+        self.zoom_slider.setValue(int(self.viewer.camera.zoom * 100))
 
-                else: # If independently
-                    structure_name = self.annotation_combo_box.currentText()
-                    if structure_name == "Fetus":
-                        structure_list = self.fetus.list_structure_name
-                    elif structure_name == "Shoulder":
-                        structure_list = self.shoulder.list_structure_name
-                    elif structure_name == "Feta Challenge":
-                        structure_list = self.feta.list_structure_name
-                    else:
-                        structure_list=[]
-
-                    for idx, struc in enumerate(structure_list):
-                        label_struc = np.zeros(label_img.shape, dtype=np.uint16)
-                        label_struc[label_img == (idx + 1)] = 255
-
-                        if len(extensions) == 1:
-                            if (extensions[0] == ".tif") or (extensions[0] == ".tiff"):
-                                file_name = Path(file_path).stem 
-                                new_file_name = file_name + '_' + struc + extensions[0]
-                                new_file_path = Path(Path(file_path).parent).joinpath(new_file_name)
-                                tif.imsave(str(new_file_path), label_struc)
-                        elif len(extensions) == 2:
-                            if (extensions[0] == ".nii") and (extensions[1] == ".gz"):
-                                file_name = Path(Path(file_path).stem).stem
-                                new_file_name = file_name + '_' + struc + extensions[0] + extensions[1]
-                                new_file_path = Path(Path(file_path).parent).joinpath(new_file_name)
-                                result_image_sitk = sitk.GetImageFromArray(label_struc)
-                                result_image_sitk.CopyInformation(self.image_sitk)
-                                sitk.WriteImage(result_image_sitk, str(new_file_path))
 
-                self.remove_backup_label_file()
+# ============ Remove data ============
+    def remove_image_layer(self):
+        """
+            Remove image layer from napari viewer
 
-            else:
-                display_warning_box(self, "Error", "No segmentation data find")
-                return
+        """
+        if "image" in self.viewer.layers:
+            self.viewer.layers.remove('image')
 
-    def backup_save_label(self):
+    def remove_probabilities_layer(self):
         """
-            Save a backup of the 3D segmentation data as a .tif file
+            Remove probabilities layer from napari viewer
+
         """
+        if "probabilities" in self.viewer.layers:
+            self.viewer.layers.remove('probabilities')
 
-        if hasattr(self.viewer, 'layers'):
-            if "annotations" in self.viewer.layers:
-                label_img = self.viewer.layers['annotations'].data
+    def remove_segmentation_layer(self):
+        """
+            Remove segmentation layer from napari viewer
 
-                #TIF OPTION
-                temp_label_data_file_path = Path(self.img_dir).joinpath("TEMP_segmentation.tif")
-                
-                tif.imsave(str(temp_label_data_file_path), label_img)       
+        """
+        if "annotations" in self.viewer.layers:
+            self.viewer.layers.remove('annotations')
 
-                # NII GZ OPTION
+    def remove_segmented_probabilities_layer(self):
+        """
+            Remove segmented probabilities' layer from napari viewer
 
-                # temp_label_data_file_path = Path(self.img_dir).joinpath("TEMP_segmentation.nii.gz")
-                # result_image_sitk = sitk.GetImageFromArray(label_img.astype(np.uint16))
-                # # result_image_sitk = sitk.GetImageFromArray(label_img)
-                # result_image_sitk.CopyInformation(self.image_sitk)
-                # sitk.WriteImage(result_image_sitk, str(temp_label_data_file_path))
+        """
+        if "segmented probabilities" in self.viewer.layers:
+            self.viewer.layers.remove('segmented probabilities')
 
-    def activate_backup_label(self):
+    def reset_segmentation(self):
         """
-        TODO
+            Reset segmentation data
+
         """
-        if self.backup_push_button.isChecked() == True:
-            self.viewer.dims.events.emitters['current_step'].connect(self.backup_save_label)
+        canRemoveSegmentation = self.can_remove_segmentation_data()
+
+        if canRemoveSegmentation:
+            if "image" in self.viewer.layers:
+                image_arr = self.viewer.layers['image'].data 
+                segmentation_arr = np.zeros(image_arr.shape, dtype=np.int8)
+                self.set_segmentation_layer(segmentation_arr)
         else:
-            self.viewer.dims.events.emitters['current_step'].disconnect(self.backup_save_label)
-            
+            return
 
 
 # ============ Display warning/question message box ============
     def can_remove_image_data(self):
         """
-            Display a question box to remove image data
+        Display a question box to remove image data
+
+        Returns
+        ----------
+        choice : bool
+            answer to the question : True if Ok, False if Cancel (default=True)
+
         """
         if "image" in self.viewer.layers:
             choice = display_ok_cancel_question_box(
                 "Warning",
-                "This will reset image data. Do you want to continue ?",
+                "This will delete image data. Do you want to continue ?",
             )
         else:
             choice = True
 
         return choice
 
-    def can_remove_label_data(self):
+    def can_remove_segmentation_data(self):
         """
-            Display a question box to remove segmentation data
+        Display a question box to remove segmentation data
+
+        Returns
+        ----------
+        choice : bool
+            answer to the question : True if Ok, False if Cancel (default=True)
+
         """
         if "annotations" in self.viewer.layers:
             choice = display_ok_cancel_question_box(
                 "Warning",
-                "This will reset segmentation data. Do you want to continue ?",
+                "This will delete segmentation data. Do you want to continue ?",
             )
         else:
             choice = True
 
         return choice
 
     def can_remove_all(self):
         """
-            Display a question box to remove all data
+        Display a question box to remove all data
+
+        Returns
+        ----------
+        choice : bool
+            answer to the question : True if Ok, False if Cancel (default=True)
+
         """
-        if "image" in self.viewer.layers or "annotations" in self.viewer.layers:
+        if ("image" in self.viewer.layers) or ("annotations" in self.viewer.layers) or ("probabilities" in self.viewer.layers) or ("segmented probabilities" in self.viewer.layers):
             choice = display_ok_cancel_question_box(
                 "Warning",
-                "This will reset all data. Do you want to continue ?",
+                "This will delete all data. Do you want to continue ?",
             )
         else:
             choice = True
 
         return choice
 
-# ============ Remove or reset data ============
-    def remove_image(self):
-        """
-            Remove image data
-        """
-        if "image" in self.viewer.layers:
-            self.viewer.layers.remove('image')
-
-    def remove_label(self):
-        """
-            Remove segmentation data
-        """
-        if "annotations" in self.viewer.layers:
-            self.viewer.layers.remove('annotations')
-
-    def remove_backup_label_file(self):
-        """
-            Delete the backup segmentation file
-        """
-
-        temp_label_data_file_path = Path(self.img_dir).joinpath("TEMP_segmentation.tif")
-        if temp_label_data_file_path.exists():
-            temp_label_data_file_path.unlink()
-
-    def reset_label(self):
-        """
-            Reset segmentation data
-        """
-        canRemoveLabel = self.can_remove_label_data()
-
-        if canRemoveLabel:
-            self.remove_label()
-            self.add_label_layers(label_data=[])
-            self.reset_annotation_radio_buttons()
-            self.remove_backup_label_file()
-        else:
-            return
-
-    def reset_annotation_radio_buttons(self):
-        structure_name = self.annotation_combo_box.currentText()
-        if structure_name == "Fetus":
-            radio_button_to_check = self.fetus.group_radio_button.button(self.fetus.nbr_buttons)
-            radio_button_to_check.setChecked(True)
-
-        elif structure_name == "Shoulder":
-            radio_button_to_check = self.shoulder.group_radio_button.button(self.shoulder.nbr_buttons)
-            radio_button_to_check.setChecked(True)
-
-        elif structure_name == "Feta Challenge":
-            radio_button_to_check = self.feta.group_radio_button.button(self.feta.nbr_buttons)
-            radio_button_to_check.setChecked(True)
-
-    def reset_zoom_slider(self):
-        median = round( (self.zoom_slider.maximum() - self.zoom_slider.minimum()) / 2)
-        self.zoom_slider.setValue(median)
-
-    # def slicer_change(self):
-    #     index = self.viewer.dims.current_step
-    #     print(index)
-
-    #     # image_to_display = self.image[index, :, :]
-
-    #     if 'image' in self.viewer.layers:
-    #             source_img = self.viewer.layers['image'].data
-
-
-    #     pixmap = QPixmap(image_path)
-    #     view_image_1.setPixmap(pixmap)
 
 # ============ For testing ============
     def _on_click(self):
         print("napari has", len(self.viewer.layers), "layers")
```

### Comparing `hesperos-0.1.9/src/hesperos/annotation/shoulder.py` & `hesperos-0.2/src/hesperos/annotation/shoulder.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,54 +4,65 @@
     "BONES",
     "MUSCLES",
 ]
 
 DICT_SUB_STRUCTURES = {
     "BONES":[
         'Clavicle',
-        'Acromion',
+        'Elbow',
+        'Glenoid',
         'Humerus',
-        'Humeral Head',
         'Scapula',
-        'Glenoid',
-        'Coracoid process',
-        'Elbow'],
-    "MUSCLES": [
-        'Supraspinatus ',
-        'Infra spinatus',
-        'Teres minor',
-        'Deltoid anterior',
-        'Deltoid lateral part',
-        'Deltoid posterior part',
-        'Sub scapularis ',
-        'Triceps brachii',
-        'Coraco-Brachialis',
-        'Pec major',
-        'Pec minor',
+        'Sternum',
+        'Vertebrae'],
+
+    "MUSCLES":[     
+        'Biceps',
+        'Coracobrachialis',
+        'Deltoid',
         'Latissimus dorsi',
+        'Pectoralis',
         'Rhomboid',
+        'Teres major',
         'Trapezius',
-        'Long Biceps']
+        'Triceps brachii',
+        'Cuff Muscles',
+        'Tendons']
 }
 
 DICT_SUB_SUB_STRUCTURES = {
     "Scapula":[
-        'Body',
-        'Epine',
         'Acromion',
-        'Coracoid'],
-    "Humeral Head" : [
+        'Body',
+        'Coracoid process',
+        'Spine'],
+
+    "Humerus":[
+        'Diaphyse',
+        'Head',
         'Trochiter',
-        'Trochin',
-        'Tete',
-        'Diaphise'],
-    "Muscle de la coiffe": [
-        'Supra',
-        'Infra',
-        'Supscapu'],
-    "Elbow": [
-        'ole crade',
-        'Radius',
-        'Palet humérale'],
-}
+        'Trochin'],
+
+    "Cuff Muscles":[
+        'Infra-spinatus',
+        'Sub-scapularis',
+        'Supra-spinatus',
+        'Terres minor'],
+
+    "Elbow":[
+        'Humeral pallet',
+        'Olecranon',
+        'Radius'],
+
+    "Deltoid":[
+        'Anterior',
+        'Lateral',
+        'Posterior'],
+
+    "Biceps":[
+        'Long',
+        'Short'],
 
-# COLUMN_WIDTH = 30
+    "Pectoralis":[
+        'Major',
+        'Minor'],    
+}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hesperos-0.1.9/src/hesperos/layout/gui_elements.py` & `hesperos-0.2/src/hesperos/layout/gui_elements.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,189 +1,231 @@
 # ============ Import python packages ============
+import functools
+from qtpy import QtCore
+from qtpy.QtTest import QTest
 from qtpy.QtWidgets import (
     QPushButton,
     QCheckBox,
     QLabel,
     QComboBox,
     QRadioButton,
     QButtonGroup,
     QMessageBox,
     QSlider,
     QGroupBox,
     QGridLayout,
+    QTextEdit,
+    QSpinBox
 )
-
 from qtpy.QtGui import QPixmap, QFont
-from qtpy import QtCore
+from pathlib import Path, PurePath
+
+
+from hesperos.layout.napari_elements import label_colors
 
 
 # ============ Functions to add custom QWidgets ============
-def add_push_button(name, layout, callback_function, row, column, column_span=1, visibility=False, minimum_width=0, alignment="center"):
+def add_combo_box(list_items, layout, callback_function, row, column, column_span=1, visibility=False, minimum_width=0, tooltip_text="", isHBoxLayout=False):
     """
-    Create a QPushButton and add it to the corresponding layout
+    Create a QComboBox and add it to the corresponding layout
 
     Parameters
     ----------
-    name : str
-        name of the push button to be displayed
-    layout : QGridLayout
+    list_items : List[str]
+        list of item to display
+    layout : QGridLayout or QHBoxLayout
         layout containing the widget
     callback_function : func
-        function to call when clicking on the push button
+        function to call when changing selected item in the combobox
     row : int
-        row of the widget in the grid
+        row of the widget (used if the layout is a QGridLayout)
     column : int
-        column  of the widget in the grid
+        column of the widget in the layout
     column_span : int
-        column span of the widget
+        column span of the widget (used if the layout is a QGridLayout)
     visibility : bool
         visibility status of the widget
     minimum_width : int
         minimum width of the widget
-    alignment : Qt.Alignment
-        alignement inside the widget
+    isHBoxLayout : bool
+        status of the layout : true if the layout is a QHBoxLayout, false if not
 
     Returns
     ----------
-    out : QPushButton
+    out : QComboBox
 
+    """ 
+    combo_box = QComboBox()
+    combo_box.setToolTip(tooltip_text)
+
+    combo_box.setVisible(visibility)
+    combo_box.addItems(list_items)
+    combo_box.setCurrentIndex(0)
+
+    combo_box.setMinimumWidth(minimum_width)
+
+    if isHBoxLayout:
+        layout.addWidget(combo_box)
+    else:
+        layout.addWidget(combo_box, row, column, 1, column_span)
+    combo_box.currentIndexChanged.connect(callback_function)
+    # combo_box.activated[str].connect(callback_function)
+
+    return combo_box
+
+def add_check_box(text, layout, callback_function, row, column, column_span=1, visibility=False, minimum_width=0, tooltip_text=""):
     """
+    Create a QCheckBox and add it to the corresponding layout
 
-    button = QPushButton(name)
-    button.setVisible(visibility)
+    Parameters
+    ----------
+    text : str
+        text to be displayed
+    layout : QGridLayout
+        layout containing the widget
+    callback_function : func
+        function to call when changing the state of the box
+    row : int
+        row of the widget in the grid
+    column : int
+        column of the widget in the grid
+    column_span : int
+        column span of the widget in the grid
+    visibility : bool
+        visibility status of the widget
+    minimum_width : int
+        minimum width of the widget
 
-    if alignment == "center":
-        pass
-    elif alignment == "left":
-        button.setStyleSheet("QPushButton { text-align: left; }")
-    elif alignment == "right":
-        button.setStyleSheet("QPushButton { text-align: right; }")
+    Returns
+    ----------
+    out : QCheckBox
 
+    """
+    check_box = QCheckBox(text)
+    check_box.setVisible(visibility)
+    check_box.setToolTip(tooltip_text)
 
-    button.setMinimumWidth(minimum_width)
-    layout.addWidget(button, row, column, 1, column_span)
-    button.clicked.connect(callback_function)
+    check_box.setMinimumWidth(minimum_width)
+    layout.addWidget(check_box, row, column, 1, column_span)
+    check_box.stateChanged.connect(callback_function)
 
-    return button
+    return check_box
 
-def add_icon_push_button(name, icon, layout, callback_function, row, column, column_span=1, visibility=False, minimum_width=0, alignment="center", isBoxLayout=False):
+def add_icon_push_button(icon, layout, callback_function, row, column, column_span=1, visibility=False, minimum_width=0, tooltip_text="", isHBoxLayout=False):
     """
     Create a QPushButton with only a icon image (no text) and add it to the corresponding layout
 
     Parameters
     ----------
-    name : str
-        name of the push button to be displayed
     icon : QIcon
         icon of the widget
-    layout : QGridLayout or QVBox TODO : check if use of vertical layout
+    layout : QGridLayout or QHBoxLayout
         layout containing the widget
     callback_function : func
         function to call when clicking on the push button
     row : int
-        row of the widget in the grid (used if the layout is a QGridLayout)
+        row of the widget (used if the layout is a QGridLayout)
     column : int
-        column  of the widget in the grid
+        column of the widget in the layout
     column_span : int
         column span of the widget (used if the layout is a QGridLayout)
     visibility : bool
         visibility status of the widget
     minimum_width : int
         minimum width of the widget
-    alignment : Qt.Alignment
-        alignement inside the widget
-    isBoxLayout : bool
-        status of the layout : true if the layout is a QGridLayout, false if not
+    isHBoxLayout : bool
+        status of the layout : true if the layout is a QHBoxLayout, false if not
 
     Returns
     ----------
     out : QPushButton
 
     """
-
-    button = QPushButton(icon, name)
+    button = QPushButton(icon, "")
     button.setVisible(visibility)
+    button.setToolTip(tooltip_text)
 
     button.setFixedSize(25, 25)
     button.setIconSize(QtCore.QSize(20,20))
-    button.setStyleSheet("text-align: center;")
+    button.setStyleSheet("QPushButton {text-align: center;}")
 
-    if isBoxLayout:
-        layout.addWidget(button, column)
+    if isHBoxLayout:
+        layout.addWidget(button)
     else:
         layout.addWidget(button, row, column, 1, column_span)
     button.clicked.connect(callback_function)
 
     return button
 
-def add_radio_button(name, layout, callback_function, row, column, visibility=False, minimum_width=0, alignment="center"):
+def add_icon_text_push_button(icon, text, layout, callback_function, row, column, column_span=1, visibility=False, minimum_width=0, tooltip_text="", isHBoxLayout=False):
     """
-    Create a QRadioButton and add it to the corresponding layout
+    Create a QPushButton with only a icon image (no text) and add it to the corresponding layout
 
     Parameters
     ----------
-    name : str
-        name of the push button to be displayed
-    layout : QGridLayout
+    icon : QIcon
+        icon of the widget
+    text : str
+        text to be displayed
+    layout : QGridLayout or QHBoxLayout
         layout containing the widget
     callback_function : func
         function to call when clicking on the push button
     row : int
-        row of the widget in the grid
+        row of the widget (used if the layout is a QGridLayout)
     column : int
-        column  of the widget in the grid
+        column of the widget in the layout
+    column_span : int
+        column span of the widget (used if the layout is a QGridLayout)
     visibility : bool
         visibility status of the widget
     minimum_width : int
         minimum width of the widget
-    alignment : Qt.Alignment
-        alignement inside the widget
+    isHBoxLayout : bool
+        status of the layout : true if the layout is a QHBoxLayout, false if not
 
     Returns
     ----------
-    out : QRadioButton
+    out : QPushButton
 
     """
 
-    button = QRadioButton(name)
+    button = QPushButton(icon, text)
     button.setVisible(visibility)
+    button.setToolTip(tooltip_text)
 
-    if alignment == "center":
-        pass
-    elif alignment == "left":
-        button.setStyleSheet(
-            "QRadioButton { text-align: left; padding: 0; spacing: 30px;}"
-        )
-    elif alignment == "right":
-        button.setStyleSheet(
-            "QRadioButton { text-align: right; padding: 0; spacing: 30px;}"
-        )
+    button.setIconSize(QtCore.QSize(20,20))
+    button.setStyleSheet("QPushButton {text-align: center;}")
 
-    button.setMinimumWidth(minimum_width)
-    layout.addWidget(button, row, column)
+    if isHBoxLayout:
+        layout.addWidget(button)
+    else:
+        layout.addWidget(button, row, column, 1, column_span)
     button.clicked.connect(callback_function)
 
     return button
 
-def add_image_widget(name, layout, image_path, row, column, visibility=False, minimum_width=0):
+def add_image_widget(name, layout, image_path, row, column, column_span=1, visibility=False, minimum_width=0):
     """
     Create a QLabel with an image and add it to the corresponding layout
 
     Parameters
     ----------
     name : str
         name of the push button to be displayed
     layout : QGridLayout
         layout containing the widget
     image_path : str
         file path of the 2D image to display
     row : int
         row of the widget in the grid
     column : int
-        column  of the widget in the grid
+        column of the widget in the grid
+    column_span : int
+        column span of the widget in the grid
     visibility : bool
         visibility status of the widget
     minimum_width : int
         minimum width of the widget
 
     Returns
     ----------
@@ -192,113 +234,316 @@
     """
     label = QLabel(name)
     pixmap = QPixmap(image_path)
     label.setPixmap(pixmap)
 
     label.setVisible(visibility)
     label.setMinimumWidth(minimum_width)
-    layout.addWidget(label, row, column)
+    layout.addWidget(label, row, column, 1, column_span)
 
     return label
 
-def add_group_radio_button(name, items, layout, callback_function, column=0, visibility=False, minimum_width=0, alignment="center"):
+def add_label(text, layout, row, column, column_span=1, visibility=False, minimum_width=0, isHBoxLayout=False, isResizingWithTextSize=False):
     """
-    Create a QButtonGroup of QRadioButton and add it to the corresponding layout
+    Create a QLabel and add it to the corresponding layout
+
+    Parameters
+    ----------
+    text : str
+        text to display in the widget
+    layout : QGridLayout or QHBoxLayout
+        layout containing the widget
+    row : int
+        row of the widget in the grid
+    column : int
+        column of the widget in the grid
+    column_span : int
+        column span of the widget in the grid
+    visibility : bool
+        visibility status of the widget
+    minimum_width : int
+        minimum width of the widget
+    isHBoxLayout : bool
+        status of the layout : true if the layout is a QGridLayout, false if not
+    isResizingWithTextSize : bool
+        resizing according to the text size if true
+
+    Returns
+    ----------
+    out : QLabel
+
+    """
+    label = QLabel(text)
+    label.setVisible(visibility)
+    label.setMinimumWidth(minimum_width)
+    
+    if isResizingWithTextSize:
+        label.setFixedWidth(label.sizeHint().width() + 5)
+        
+    if isHBoxLayout:
+        layout.addWidget(label)
+    else:
+        layout.addWidget(label, row, column, 1, column_span)
+
+    return label
+
+def add_push_button(name, layout, callback_function, row, column, column_span=1, visibility=False, minimum_width=0, tooltip_text=""):
+    """
+    Create a QPushButton and add it to the corresponding layout
 
     Parameters
     ----------
     name : str
         name of the push button to be displayed
-    items :TODO
+    layout : QGridLayout
+        layout containing the widget
+    callback_function : func
+        function to call when clicking on the push button
+    row : int
+        row of the widget in the grid
+    column : int
+        column of the widget in the grid
+    column_span : int
+        column span of the widget in the grid
+    visibility : bool
+        visibility status of the widget
+    minimum_width : int
+        minimum width of the widget
+
+    Returns
+    ----------
+    out : QPushButton
+
+    """
+
+    button = QPushButton(name)
+    button.setVisible(visibility)
+    button.setToolTip(tooltip_text)
+
+    button.setMinimumWidth(minimum_width)
+    layout.addWidget(button, row, column, 1, column_span)
+    button.clicked.connect(callback_function)
+
+    return button
+
+def add_text_edit(text, layout, row, column, column_span=1, visibility=False, minimum_width=0):
+    """
+    Create a QTextEdit and add it to the corresponding layout
+
+    Parameters
+    ----------
+    text : str
+        text to display in the widget
+    layout : QGridLayout
+        layout containing the widget
+    row : int
+        row of the widget in the grid
+    column : int
+        column of the widget in the grid
+    column_span : int
+        column span of the widget in the grid
+    visibility : bool
+        visibility status of the widget
+    minimum_width : int
+        minimum width of the widget
+
+    Returns
+    ----------
+    out : QTextEdit
+
+    """
+    text_edit = QTextEdit(text)
+    text_edit.setVisible(visibility)
+    text_edit.setMinimumWidth(minimum_width)
+    layout.addWidget(text_edit, row, column, 1, column_span)
 
-    layout : QVBoxLayout TODO TOCHECK
+    return text_edit
+
+def add_slider(layout, bounds , callback_function, row, column, column_span=1, visibility=False, minimum_width=0, tooltip_text="", isHBoxLayout=False):
+    """
+    Create a QSlider and add it to the corresponding layout
+
+    Parameters
+    ----------
+    layout : QGridLayout or QHBoxLayout
         layout containing the widget
+    bounds : Tuple[int, int]
+        lower and upped bounds of the slider
     callback_function : func
         function to call when clicking on the push button
+    row : int
+        row of the widget (used if the layout is a QGridLayout)
     column : int
-        column  of the widget in the grid
+        column of the widget in the layout
+    column_span : int
+        column span of the widget (used if the layout is a QGridLayout)
     visibility : bool
         visibility status of the widget
     minimum_width : int
         minimum width of the widget
-    alignment : Qt.Alignment
-        alignement inside the widget
+    isHBoxLayout : bool
+        status of the layout : true if the layout is a QGridLayout, false if not
 
     Returns
     ----------
-    button : QButtonGroup
+    out : QSlider
+
+    """
+    slider = QSlider(orientation=QtCore.Qt.Horizontal)
+    slider.setVisible(visibility)
+    slider.setToolTip(tooltip_text)
+
+    slider.setMinimum(bounds[0])
+    slider.setMaximum(bounds[1])
+    slider.setSingleStep(1)
+
+    # slider.setMinimumWidth(minimum_width)
+
+    if isHBoxLayout:
+        layout.addWidget(slider)
+    else:
+        layout.addWidget(slider, row, column, 1, column_span)
+
+    slider.valueChanged[int].connect(callback_function)
 
-    nbr_buttons: int
-        number of QRadioButtons in the QButtonGroup
+    return slider
 
+def add_spin_box(layout, row, column, column_span=1, visibility=False, minimum_width=0, tooltip_text="", isHBoxLayout=False):
     """
+    Create a QSpinBox and add it to the corresponding layout
+
+    Parameters
+    ----------
+    layout : QGridLayout or QHBoxLayout
+        layout containing the widget
+    row : int
+        row of the widget (used if the layout is a QGridLayout)
+    column : int
+        column of the widget in the layout
+    column_span : int
+        column span of the widget (used if the layout is a QGridLayout)
+    visibility : bool
+        visibility status of the widget
+    minimum_width : int
+        minimum width of the widget
+    isHBoxLayout : bool
+        status of the layout : true if the layout is a QHBoxLayout, false if not
+
+    Returns
+    ----------
+    out : QSpinBox
+
+    """ 
+    spin_box = QSpinBox()
+    spin_box.setVisible(visibility)
+    spin_box.setToolTip(tooltip_text)
     
+    spin_box.setMinimum(1)
+    spin_box.setValue(1)
+    spin_box.setDisplayIntegerBase(10)
+
+    spin_box.setMinimumWidth(minimum_width)
+    spin_box.setAlignment(QtCore.Qt.AlignCenter)
+
+    if isHBoxLayout:
+        layout.addWidget(spin_box)
+    else:
+        layout.addWidget(spin_box, row, column, 1, column_span)
+
+    return spin_box
+
+
+# ============ Functions to add custom radio buttons subgroups ============
+def add_group_radio_button(list_items, layout, callback_function, row=0, column=0, visibility=False, minimum_width=0, tooltip_text=""):
+    """
+    Create a QButtonGroup of QRadioButton and add it to the corresponding layout
+
+    Parameters
+    ----------
+    list_items : list[str]
+        list of name of radio buttons to create
+    layout : QGridLayout
+        layout containing the widget
+    callback_function : func
+        function to call when selecting a radio button
+    row : int
+        row of the widget in the grid
+    column : int
+        column of the widget in the grid
+    visibility : bool
+        visibility status of the widget
+    minimum_width : int
+        minimum width of the widget
+
+    Returns
+    ----------
+    button : QButtonGroup
+
+    """
     group_button = QButtonGroup()
 
-    for label, item in enumerate(items):
+    for label, item in enumerate(list_items):
         button = QRadioButton(item)
         button.setVisible(visibility)
+        button.setToolTip(tooltip_text)
 
         button.setMinimumWidth(minimum_width)
 
         group_button.addButton(button, label + 1)
         layout.addWidget(button, label, column)
 
     radio_button_to_check = group_button.button(label + 1)
     radio_button_to_check.setChecked(True)
 
     nbr_buttons = label + 1
 
     group_button.buttonClicked.connect(callback_function)
 
-    return group_button, nbr_buttons
+    return group_button
 
-def add_sub_subgroup_radio_button(name, list_items, layout, callback_function, column=0, visibility=False, minimum_width=0, dict_subgroups={}, dict_sub_subgroups={}):
+def add_sub_subgroup_radio_button(list_items, layout, callback_function, row=0, column=0, visibility=False, minimum_width=0, tooltip_text="", dict_subgroups={}, dict_sub_subgroups={}):
     """
-    Create a QButtonGroup of QRadioButton and add it to the corresponding layout
+    Create a QButtonGroup with sub groups of QRadioButton and add it to the corresponding layout
 
     Parameters
     ----------
-    name : str
-        name of the push button to be displayed
     list_items: list[str]
-    TODO
-
-    layout : QVBoxLayout TODO TOCHECK
+        list of the main groups of radio buttons
+    layout : QGridLayout
         layout containing the widget
     callback_function : func
-        function to call when clicking on the push button
+        function to call when selecting a radio button
+    row : int
+        row of the widget in the grid
     column : int
-        column  of the widget in the grid
+        column of the widget in the grid
     visibility : bool
         visibility status of the widget
     minimum_width : int
         minimum width of the widget
     dict_subgroups : dict[str, str]
-    TODO
-
+        dictionnary of subgroups of main groups (name of radio buttons)
     dict_sub_subgroups : dict[str, str]
-    TODO
-
+        dictionnary of sub-subgroups of subgroups (name of radio buttons)
 
     Returns
     ----------
     button : QButtonGroup
+        widget created
+    list_button_name : List[str]
+        list of name of all QRadioButtons in the QButtonGroup
+    list_button_in_subgroups : list[QRadioButtons]
+        list of QRadioButtons in subgroup
 
-    nbr_buttons : int
-        number of QRadioButtons in the QButtonGroup
-
-    list_structure_name : List[str]
-        list of all structure to annotate
-
-    """
-    
+    """    
     group_button = QButtonGroup()
 
-    list_structure_name = []
+    list_button_name = []
+    list_button_in_subgroups = []
+    list_sub_panel = []
     label = 0
     for column_grp, item in enumerate(list_items):
         if item in dict_subgroups:
             main_panel = QGroupBox(item)
 
             main_panel.setObjectName('MainPanel')
             main_panel.setStyleSheet("""
@@ -310,209 +555,111 @@
                 QGroupBox::title#MainPanel{
                     subcontrol-origin: margin;
                     subcontrol-position: top center;
                     padding: 0 3px;
                     background-color: transparent;
                 }""")
 
-
             layout_main_panel = QGridLayout()
-
+            layout_main_panel.setAlignment(QtCore.Qt.AlignTop)
+           
             for subindex, subitem in enumerate(dict_subgroups[item]):
                 if subitem in dict_sub_subgroups:
                     sub_panel = QGroupBox(subitem)
+                    sub_panel.setCheckable(True)
                     layout_sub_panel = QGridLayout()
+                    layout_sub_panel.setAlignment(QtCore.Qt.AlignTop)
 
                     sub_panel.setObjectName("SubPanel")
 
                     font = QFont()
                     font.setItalic(True)
                     sub_panel.setFont(font)
 
-                    sub_panel.setStyleSheet("""
-                    QGroupBox#SubPanel {
-                        border: 1px solid rgb(90, 98, 108);
-                        margin-top: 0.5em;
-                        color: rgb(90, 98, 108);
-                        font-weight: normal;
-                    },
-                    QGroupBox::title#SubPanel {
-                        top: -6px;
-                        left: 10px;
-                    }""")
-
+                    style_sheet_path = Path(__file__).parent.parent.joinpath('resources', 'group_box_stylesheet.qss')
+                    sub_panel.setStyleSheet(open(str(style_sheet_path)).read())
 
                     for sub_subindex, sub_subitem in enumerate(dict_sub_subgroups[subitem]):
                         button = QRadioButton(sub_subitem)
                         button.setVisible(visibility)
                         button.setMinimumWidth(minimum_width)
+                        button.setToolTip(tooltip_text)
 
                         font = QFont()
                         font.setItalic(False)
                         button.setFont(font)
 
-                        button.setStyleSheet("color: rgb(240, 241, 242);")
+                        # button.setStyleSheet("color: rgb(240, 241, 242);")
 
                         # button.setStyleSheet(
-                        #     """QRadioButton::indicator{
-                        #         background-color: yellow;
-                        #     }""")
+                            # """QRadioButton::indicator{{
+                            #     background-color: {};
+                            # }}""".format(label_colors))
 
                         group_button.addButton(button, label + 1)
                         layout_sub_panel.addWidget(button, sub_subindex, 0)
 
-                        list_structure_name.append(sub_subitem)
+                        list_button_name.append(sub_subitem)
+                        list_button_in_subgroups.append(button)
 
                         label = label + 1
 
                     sub_panel.setLayout(layout_sub_panel)
 
                     layout_main_panel.addWidget(sub_panel, subindex, 0)
 
+                    list_sub_panel.append(sub_panel)
+                   
                 else:
                     button = QRadioButton(subitem)
                     button.setVisible(visibility)
+                    button.setToolTip(tooltip_text)
                     button.setMinimumWidth(minimum_width)
                     button.setStyleSheet("font-weight: normal;")
 
                     group_button.addButton(button, label + 1)
                     layout_main_panel.addWidget(button, subindex, 0)
 
-                    list_structure_name.append(subitem)
+                    list_button_name.append(subitem)
 
                     label = label + 1
 
             main_panel.setLayout(layout_main_panel)
-            layout.addWidget(main_panel, 0, column + column_grp)
+            layout.addWidget(main_panel, row, column + column_grp)
 
     nbr_buttons = label
     radio_button_to_check = group_button.button(nbr_buttons)
     radio_button_to_check.setChecked(True)
 
     group_button.buttonClicked.connect(callback_function)
 
-    return group_button, nbr_buttons, list_structure_name
-
-def add_label(text, layout, row, column, column_span=1, visibility=False, minimum_width=0):
-    """
-    Create a QLabel and add it to the corresponding layout
-
-    Parameters
-    ----------
-    text : str
-        text to display in the widget
-    layout : QVBoxLayout TODO TOCHECK
-        layout containing the widget
-    row : int
-        row of the widget in the grid
-    column : int
-        column of the widget in the grid
-    column_span : int
-        column span of the widget in the grid
-    visibility : bool
-        visibility status of the widget
-    minimum_width : int
-        minimum width of the widget
-
-    Returns
-    ----------
-    out : QLabel
-
-    """
-    label = QLabel(text)
-    label.setVisible(visibility)
-    label.setMinimumWidth(minimum_width)
-    layout.addWidget(label, row, column, 1, column_span)
-
-    return label
-
-def add_combobox(layout, items, callback_function, row, column, column_span=1, visibility=False):
-    """
-    Create a QComboBox and add it to the corresponding layout
-
-    Parameters
-    ----------
-    layout : QVBoxLayout TODO TOCHECK
-        layout containing the widget
-    items : List[str]
-        TODO
-    callback_function : func
-        function to call when clicking on the push button
-    row : int
-        row of the widget in the grid
-    column : int
-        column of the widget in the grid
-    column_span : int
-        column span of the widget in the grid
-    visibility : bool
-        visibility status of the widget
-
-    Returns
-    ----------
-    out : QComboBox
-
-    """
-    
-    combobox = QComboBox()
-    # combobox.setVisible(visibility)
-    combobox.addItems(items)
-    combobox.setCurrentIndex(0)
-    combobox.currentIndexChanged.connect(callback_function)
-    # combobox.activated[str].connect(callback_function)
+    for index, group_box in enumerate(list_sub_panel):
+        group_box.toggled.connect(functools.partial(toggle_group_box, list_sub_panel, index))  
+        group_box.setChecked(False) 
 
-    layout.addWidget(combobox, row, column, 1, column_span)
-    return combobox
+    return group_button, list_button_name, list_button_in_subgroups
 
-def add_slider(layout, bounds , callback_function, row, column, column_span=1, visibility=False, minimum_width=0, isBoxLayout=False):
+def toggle_group_box(list_sub_panel, index):
     """
-    Create a QSlider and add it to the corresponding layout
+    Toggle widgets in a QGroupBox if the GroupBox is clicked 
 
     Parameters
     ----------
-    layout : QVBoxLayout TODO TOCHECK
-        layout containing the widget
-    bounds : Tuple[int, int]
-        lower and upped bounds of the slider
-    callback_function : func
-        function to call when clicking on the push button
-    row : int
-        row of the widget in the grid
-    column : int
-        column of the widget in the grid
-    column_span : int
-        column span of the widget in the grid
-    visibility : bool
-        visibility status of the widget
-    minimum_width : int
-        minimum width of the widget
-    isBoxLayout : bool
-        status of the layout : true if the layout is a QGridLayout, false if not
-
-    Returns
-    ----------
-    out : QSlider
+    list_sub_panel : list[QGroupBox]
+        list of QGroupBox in the sub panel
+    index : int
+        index of the clicked QGroupBox
 
     """
-    slider = QSlider(orientation=QtCore.Qt.Horizontal)
-    slider.setVisible(visibility)
-    slider.setMinimum(bounds[0])
-    slider.setMaximum(bounds[1])
-    slider.setSingleStep(1)
-    slider.setValue(round((bounds[1] - bounds[0])/2))
-
-    # slider.setMinimumWidth(minimum_width)
+    group_box = list_sub_panel[index]
 
-    if isBoxLayout:
-        layout.addWidget(slider, column)
-    else:
-        layout.addWidget(slider, row, column, 1, column_span)
-
-    slider.valueChanged[int].connect(callback_function)
-
-    return slider
+    state = group_box.isChecked()
+    for widget in group_box.children():
+        if widget.isWidgetType():
+            widget.setVisible(state) 
 
 
 # ============ Display warning box ============
 def display_warning_box(widget, title, message):
     """
     Display a warning message in a pop up window
 
@@ -520,51 +667,53 @@
     ----------
     widget : QWidget
         parent widget
     title : str
         title of the pop up window
     message : str
         text to display
+
     """
     QMessageBox.warning(
         widget,
         title,
         message,
     )
 
 def display_save_message_box(title, message):
     """
-    Display a message in a pop up window and ask the user about the different saving mode (all or independently)
+    Display a message in a pop up window and ask the user about the different saving mode (Unique or Several)
 
     Parameters
     ----------
     title : str
         title of the pop up window
     message : str
         text to display
 
     Returns
     ----------
     choice : bool
-        answer to the question. True if "all", False if "Independently"
-    """
+        answer to the question. True if "Unique", False if "Several"
 
+    """
     msg_box = QMessageBox()
     msg_box.setWindowTitle(title)
     msg_box.setText(message)
     msg_box.setIcon(QMessageBox.Question)
 
-    all_button = msg_box.addButton('All', QMessageBox.YesRole)
-    independent_button = msg_box.addButton('Independently', QMessageBox.NoRole)
+    unique_button = msg_box.addButton('Unique', QMessageBox.YesRole)
+    several_button = msg_box.addButton('Several', QMessageBox.NoRole)
+    msg_box.setDefaultButton(unique_button)
 
     msg_box.exec_()
 
-    if msg_box.clickedButton() == all_button:
+    if msg_box.clickedButton() == unique_button:
         return True
-    elif msg_box.clickedButton() == independent_button:
+    elif msg_box.clickedButton() == several_button:
         return False
 
 def display_ok_cancel_question_box(title, message):
     """
     Display a message in a pop up window to confirm or cancel an action
 
     Parameters
@@ -574,22 +723,53 @@
     message : str
         text to display
 
     Returns
     ----------
     choice : bool
         answer to the question
-    """
 
+    """
     msg_box = QMessageBox()
     msg_box.setWindowTitle(title)
     msg_box.setText(message)
 
     msg_box.addButton(QMessageBox.Ok)
     msg_box.addButton(QMessageBox.Cancel)
 
     message_reply = msg_box.exec_()
 
     if message_reply == QMessageBox.Ok:
         return True
     else:
+        return False
+
+def display_yes_no_question_box(title, message):
+    """
+    Display a message in a pop up window to confirm or not an action
+
+    Parameters
+    ----------
+    title : str
+        title of the pop up window
+    message : str
+        text to display
+
+    Returns
+    ----------
+    choice : bool
+        answer to the question
+
+    """
+    msg_box = QMessageBox()
+    msg_box.setWindowTitle(title)
+    msg_box.setText(message)
+
+    msg_box.addButton(QMessageBox.Yes)
+    msg_box.addButton(QMessageBox.No)
+
+    message_reply = msg_box.exec_()
+
+    if message_reply == QMessageBox.Yes:
+        return True
+    else:
         return False
```

### Comparing `hesperos-0.1.9/src/hesperos/napari.yaml` & `hesperos-0.2/src/hesperos/napari.yaml`

 * *Files identical despite different names*

### Comparing `hesperos-0.1.9/src/hesperos/one_shot_learning/kernel.py` & `hesperos-0.2/src/hesperos/one_shot_learning/kernel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# ============ 2D Kernel definition used to compute features of the raw image ============
-
+# ============ Import python packages ============
 import numpy as np
 
+
+# ============ 2D Kernel definition used to compute features of the raw image ============
 gaussian_kernel_3x3 = np.array((
         [ [1,2,1], [2,4,2], [1,2,1]]), dtype="int")
 gaussian_kernel_5x5 = np.array((
         [ [1,2,4,2,1], [2,4,8,4,2], [4,8,16,8,4], [2,4,8,4,2], [1,2,4,2,1]]), dtype="int")
 
 prewitt_kernel_3x3 = np.array((
         [ [1,0,-1], [1,0,-1], [1,0,-1]]), dtype="int")
```

### Comparing `hesperos-0.1.9/src/hesperos/one_shot_learning/utilities.py` & `hesperos-0.2/src/hesperos/one_shot_learning/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,30 +21,31 @@
         features (normed 0-255) of all labeled pixels (0-1) of the 3D image
         as { 'LABEL'    : [0, ...., 0, 1, ....., 1],
             'Feature1' : [5, ...., 80, 255, ...., 5],
             'Feature2' : [ ... ],
                 ...
             }
     output_classifier_path : str
-        path file where the classifier will be saved as a .pckl file
+        path file where the classifier will be exported as a .pckl file
     """
 
     # === Create Random Forest Classifier
     rfc = RandomForestClassifier(classifier_path='NONE', features_df=features_df)
 
     # === Load and equalize features data
     rfc._prepare_data_for_training()
 
     # === Fit the classifier using the features
     rfc.model.fit(rfc.features, rfc.labels)
     # score = rfc.model.score(rfc.features, rfc.labels)
 
-    # === Save the classifier
+    # === Export the classifier
     pickle.dump(rfc.model, open(output_classifier_path, 'wb'))
 
+
 # ============ Infer a probability for all the pixels of a 3D image ============
 def rfc_inference(features_df, output_classifier_path, proba_list, size_y, size_x):
     """
     Run a inference of a trained Random Forest Classifier on the features data given (without label data)
 
     Parameters
     ----------
@@ -80,14 +81,15 @@
 
     # === Convert it to probabilities ===
     output_proba = np.exp(log_proba)
     output_proba = output_proba * 255
 
     proba_list.append(output_proba.reshape(size_y, size_x).astype(np.uint8))
 
+
 # ============ Run Process ============
 def run_one_shot_learning(source_img, label, output_classifier_path):
     """
     Run one shot learning proccess (learning and inference)
 
     Parameters
     ----------
@@ -102,49 +104,36 @@
     ----------
     output_proba : ndarray
         output probabilities normed between 0 to 1 (same size than source_img) where 1 is the highest probabilities for a pixel to be in the region of interest
 
     """
 
     # === Load data ===
-    # tiff
     size_z , size_y, size_x = source_img.shape
-    # DICOM
-    # size_x, size_y, size_z  = source_img.shape
 
     # === Extract tagged pixels ===
     # suppose only 2 labels
-    _, label_roi, label_background = np.unique(label)
+    _, label_roi, label_other = np.unique(label)
 
     mask_roi = (label == label_roi)
-    mask_background = (label == label_background)
+    mask_other = (label == label_other)
 
     # incr = round(source_img.shape[size_z]/50)
 
     # === Compute all features ===
-    # Pool
     if not napari.features_3d.is_feature_computed:
         napari.features_3d._set_source_img(source_img)
         napari.features_3d._compute_features_3d()
 
     # === Create features data needed for training a RFC ===
-
-    # tiff
     train_features = TrainingFeatures()
     for z in range(size_z):
         # Extract only features of tagged pixels
         train_features.features_2d_array = napari.features_3d.features_3d_list[z]
-        train_features._extract_tagged_features(mask_roi[z, :, :], mask_background[z, :, :])
-
-    # DICOM
-    # train_features = TrainingFeatures()
-    # for z in range(size_z):
-    #     # Extract only features of tagged pixels
-    #     train_features.features_2d_array = napari.features_3d.features_3d_list[z]
-    #     train_features._extract_tagged_features(mask_roi[:, :, z], mask_background[:, :, z])
+        train_features._extract_tagged_features(mask_roi[z, :, :], mask_other[z, :, :])
 
     train_features._create_features_df()
 
     # === Train the classifier ===
     rfc_training(train_features.features_df, output_classifier_path)
     del train_features
 
@@ -164,14 +153,10 @@
         # Create feature dataframe
         infer_features._create_features_df()
 
     # === Infer the classifier for the corresponding 2D slice ===
         rfc_inference(infer_features.features_df, output_classifier_path, proba_list, size_y, size_x)
 
     # === Display the output results ===
-
-    # tiff
     output_proba = np.stack(proba_list, axis=0)
-    #DICOM
-    # output_proba = np.stack(proba_list, axis=2)
 
-    return output_proba
+    return output_proba
```

### Comparing `hesperos-0.1.9/src/hesperos/resources/_icons.py` & `hesperos-0.2/src/hesperos/resources/_icons.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+# ============ Import python packages ============
 from pathlib import Path, PurePath
+from qtpy import QtCore
 
+
+# ============ Same as napari CODE ============
 ICON_PATH = (Path(__file__).parent / 'icons').resolve()
 ICONS = {x.stem: str(x) for x in ICON_PATH.iterdir() if x.suffix == '.svg'}
 
-## FROM NAPARI CODE
+QtCore.QDir.addSearchPath('icons', str(ICON_PATH))
 
 def get_icon_path(name):
     """Return path to an SVG in the theme icons."""
     if name not in ICONS:
         raise ValueError(
             trans._(
                 "unrecognized icon name: {name!r}. Known names: {icons}",
```

### Comparing `hesperos-0.1.9/src/hesperos/resources/icons/backup.svg` & `hesperos-0.2/src/hesperos/resources/icons/backup.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.1.9/src/hesperos/resources/icons/lock.svg` & `hesperos-0.2/src/hesperos/resources/icons/lock.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.1.9/src/hesperos/resources/icons/reset.svg` & `hesperos-0.2/src/hesperos/resources/icons/reset.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.1.9/src/hesperos/resources/icons/save.svg` & `hesperos-0.2/src/hesperos/resources/icons/save.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.1.9/src/hesperos/resources/icons/undo.svg` & `hesperos-0.2/src/hesperos/resources/icons/undo.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.1.9/src/hesperos/resources/icons/unlock.svg` & `hesperos-0.2/src/hesperos/resources/icons/unlock.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.1.9/src/hesperos/resources/icons/zoom.svg` & `hesperos-0.2/src/hesperos/resources/icons/zoom.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.1.9/tox.ini` & `hesperos-0.2/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # For more information about tox, see https://tox.readthedocs.io/en/latest/
 [tox]
-envlist = py{38,39}-{macos,windows}
+envlist = py{38,39,310}-{macos,windows}
 isolated_build=true
 
 [gh-actions]
 python =
     3.8: py38
     3.9: py39
+    3.10: py310
 
 [gh-actions:env]
 PLATFORM =
-    macos-latest: macos
+    macos-test: macos
     windows-latest: windows
 
 [testenv]
 platform =
     macos: darwin
     windows: win32
 passenv =
     CI
     GITHUB_ACTIONS
-    DISPLAY XAUTHORITY
+    DISPLAY_XAUTHORITY
     NUMPY_EXPERIMENTAL_ARRAY_FUNCTION
     PYVISTA_OFF_SCREEN
 extras =
     testing
 commands = pytest -v --color=yes --cov=hesperos --cov-report=xml
```

