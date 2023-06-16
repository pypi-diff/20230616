# Comparing `tmp/fake-bpy-module-latest-20230615.tar.gz` & `tmp/fake-bpy-module-latest-20230616.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fake-bpy-module-latest-20230615.tar", last modified: Thu Jun 15 06:27:07 2023, max compression
+gzip compressed data, was "dist/fake-bpy-module-latest-20230616.tar", last modified: Fri Jun 16 06:22:11 2023, max compression
```

## Comparing `fake-bpy-module-latest-20230615.tar` & `fake-bpy-module-latest-20230616.tar`

### file list

```diff
@@ -1,356 +1,356 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-15 06:26:56.000000 fake-bpy-module-latest-20230615/addon_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-15 06:26:55.000000 fake-bpy-module-latest-20230615/animsys_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30417 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/aud.py
--rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-06-15 06:24:17.000000 fake-bpy-module-latest-20230615/bgl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/bl_app_override/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_app_override/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_app_override/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bl_app_override/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_app_template_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/bl_console_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_console_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/bl_console_utils/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_console_utils/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_console_utils/autocomplete/complete_calltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_console_utils/autocomplete/complete_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_console_utils/autocomplete/complete_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_console_utils/autocomplete/intellisense.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bl_console_utils/autocomplete/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bl_console_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/bl_i18n_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_i18n_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_i18n_utils/bl_extract_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_i18n_utils/merge_po.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bl_i18n_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_i18n_utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_i18n_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_i18n_utils/utils_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_i18n_utils/utils_languages_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_i18n_utils/utils_rtl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/bl_keymap_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_keymap_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_keymap_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_keymap_utils/keymap_from_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_keymap_utils/keymap_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_keymap_utils/platform_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bl_keymap_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_keymap_utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-15 06:24:24.000000 fake-bpy-module-latest-20230615/bl_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/bl_operators/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/bl_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-15 06:26:58.000000 fake-bpy-module-latest-20230615/bl_operators/add_mesh_torus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-06-15 06:27:03.000000 fake-bpy-module-latest-20230615/bl_operators/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_operators/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/bl_operators/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_operators/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_operators/bmesh/find_adjacent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bl_operators/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-06-15 06:27:04.000000 fake-bpy-module-latest-20230615/bl_operators/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_operators/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-15 06:27:03.000000 fake-bpy-module-latest-20230615/bl_operators/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-15 06:26:59.000000 fake-bpy-module-latest-20230615/bl_operators/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-15 06:27:03.000000 fake-bpy-module-latest-20230615/bl_operators/freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-06-15 06:26:59.000000 fake-bpy-module-latest-20230615/bl_operators/geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-15 06:26:59.000000 fake-bpy-module-latest-20230615/bl_operators/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-15 06:27:04.000000 fake-bpy-module-latest-20230615/bl_operators/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-06-15 06:27:03.000000 fake-bpy-module-latest-20230615/bl_operators/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    38122 2023-06-15 06:27:04.000000 fake-bpy-module-latest-20230615/bl_operators/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-15 06:26:59.000000 fake-bpy-module-latest-20230615/bl_operators/object_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-15 06:27:03.000000 fake-bpy-module-latest-20230615/bl_operators/object_quick_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-15 06:26:58.000000 fake-bpy-module-latest-20230615/bl_operators/object_randomize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-06-15 06:26:58.000000 fake-bpy-module-latest-20230615/bl_operators/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bl_operators/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-15 06:26:59.000000 fake-bpy-module-latest-20230615/bl_operators/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-15 06:27:03.000000 fake-bpy-module-latest-20230615/bl_operators/screen_play_rendered_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-06-15 06:26:58.000000 fake-bpy-module-latest-20230615/bl_operators/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-15 06:26:59.000000 fake-bpy-module-latest-20230615/bl_operators/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-15 06:26:58.000000 fake-bpy-module-latest-20230615/bl_operators/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-06-15 06:27:00.000000 fake-bpy-module-latest-20230615/bl_operators/userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-15 06:26:58.000000 fake-bpy-module-latest-20230615/bl_operators/uvcalc_follow_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/bl_operators/uvcalc_lightmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-15 06:26:58.000000 fake-bpy-module-latest-20230615/bl_operators/uvcalc_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-15 06:27:03.000000 fake-bpy-module-latest-20230615/bl_operators/vertexpaint_dirt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-06-15 06:26:59.000000 fake-bpy-module-latest-20230615/bl_operators/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-06-15 06:27:03.000000 fake-bpy-module-latest-20230615/bl_operators/wm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/bl_previews_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 06:26:54.000000 fake-bpy-module-latest-20230615/bl_previews_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-15 06:26:54.000000 fake-bpy-module-latest-20230615/bl_previews_utils/bl_previews_render.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bl_previews_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/bl_rna_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-15 06:26:56.000000 fake-bpy-module-latest-20230615/bl_rna_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-15 06:26:56.000000 fake-bpy-module-latest-20230615/bl_rna_utils/data_path.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bl_rna_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/bl_ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-06-15 06:24:24.000000 fake-bpy-module-latest-20230615/bl_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-15 06:26:09.000000 fake-bpy-module-latest-20230615/bl_ui/generic_ui_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-15 06:26:04.000000 fake-bpy-module-latest-20230615/bl_ui/node_add_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)   110864 2023-06-15 06:26:41.000000 fake-bpy-module-latest-20230615/bl_ui/node_add_menu_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-15 06:25:00.000000 fake-bpy-module-latest-20230615/bl_ui/properties_animviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-06-15 06:24:31.000000 fake-bpy-module-latest-20230615/bl_ui/properties_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-06-15 06:24:55.000000 fake-bpy-module-latest-20230615/bl_ui/properties_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-06-15 06:26:49.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-06-15 06:26:38.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_bone.py
--rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-06-15 06:26:54.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-06-15 06:24:39.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-06-15 06:26:03.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-15 06:26:10.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-06-15 06:26:07.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-06-15 06:24:38.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-06-15 06:24:32.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-06-15 06:24:38.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_lightprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)    52746 2023-06-15 06:24:30.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-15 06:24:58.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_metaball.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-15 06:26:04.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-06-15 06:24:24.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-15 06:24:38.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_shaderfx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-15 06:24:39.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-06-15 06:26:03.000000 fake-bpy-module-latest-20230615/bl_ui/properties_data_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-06-15 06:26:37.000000 fake-bpy-module-latest-20230615/bl_ui/properties_freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-06-15 06:25:00.000000 fake-bpy-module-latest-20230615/bl_ui/properties_grease_pencil_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-06-15 06:26:52.000000 fake-bpy-module-latest-20230615/bl_ui/properties_mask_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-06-15 06:26:24.000000 fake-bpy-module-latest-20230615/bl_ui/properties_material.py
--rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-06-15 06:26:09.000000 fake-bpy-module-latest-20230615/bl_ui/properties_material_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-06-15 06:26:04.000000 fake-bpy-module-latest-20230615/bl_ui/properties_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-06-15 06:26:39.000000 fake-bpy-module-latest-20230615/bl_ui/properties_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-15 06:26:09.000000 fake-bpy-module-latest-20230615/bl_ui/properties_paint_common.py
--rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-06-15 06:26:46.000000 fake-bpy-module-latest-20230615/bl_ui/properties_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-15 06:26:24.000000 fake-bpy-module-latest-20230615/bl_ui/properties_physics_cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-15 06:24:56.000000 fake-bpy-module-latest-20230615/bl_ui/properties_physics_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-06-15 06:26:47.000000 fake-bpy-module-latest-20230615/bl_ui/properties_physics_dynamicpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-06-15 06:26:48.000000 fake-bpy-module-latest-20230615/bl_ui/properties_physics_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-06-15 06:24:58.000000 fake-bpy-module-latest-20230615/bl_ui/properties_physics_fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-15 06:26:54.000000 fake-bpy-module-latest-20230615/bl_ui/properties_physics_geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-15 06:26:07.000000 fake-bpy-module-latest-20230615/bl_ui/properties_physics_rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-06-15 06:26:49.000000 fake-bpy-module-latest-20230615/bl_ui/properties_physics_rigidbody_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-06-15 06:24:39.000000 fake-bpy-module-latest-20230615/bl_ui/properties_physics_softbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-06-15 06:26:18.000000 fake-bpy-module-latest-20230615/bl_ui/properties_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-06-15 06:26:54.000000 fake-bpy-module-latest-20230615/bl_ui/properties_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-06-15 06:26:36.000000 fake-bpy-module-latest-20230615/bl_ui/properties_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-06-15 06:26:53.000000 fake-bpy-module-latest-20230615/bl_ui/properties_view_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-15 06:26:47.000000 fake-bpy-module-latest-20230615/bl_ui/properties_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-06-15 06:24:30.000000 fake-bpy-module-latest-20230615/bl_ui/properties_world.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bl_ui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   176850 2023-06-15 06:26:23.000000 fake-bpy-module-latest-20230615/bl_ui/space_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-06-15 06:26:35.000000 fake-bpy-module-latest-20230615/bl_ui/space_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    64929 2023-06-15 06:24:56.000000 fake-bpy-module-latest-20230615/bl_ui/space_dopesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-06-15 06:26:51.000000 fake-bpy-module-latest-20230615/bl_ui/space_filebrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    50899 2023-06-15 06:26:49.000000 fake-bpy-module-latest-20230615/bl_ui/space_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-06-15 06:24:29.000000 fake-bpy-module-latest-20230615/bl_ui/space_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-06-15 06:26:51.000000 fake-bpy-module-latest-20230615/bl_ui/space_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-06-15 06:26:08.000000 fake-bpy-module-latest-20230615/bl_ui/space_nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    75065 2023-06-15 06:26:06.000000 fake-bpy-module-latest-20230615/bl_ui/space_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-06-15 06:26:11.000000 fake-bpy-module-latest-20230615/bl_ui/space_outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-15 06:24:58.000000 fake-bpy-module-latest-20230615/bl_ui/space_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-06-15 06:26:16.000000 fake-bpy-module-latest-20230615/bl_ui/space_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-15 06:26:06.000000 fake-bpy-module-latest-20230615/bl_ui/space_spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-15 06:26:10.000000 fake-bpy-module-latest-20230615/bl_ui/space_statusbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-06-15 06:26:10.000000 fake-bpy-module-latest-20230615/bl_ui/space_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-06-15 06:26:35.000000 fake-bpy-module-latest-20230615/bl_ui/space_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-15 06:24:58.000000 fake-bpy-module-latest-20230615/bl_ui/space_toolsystem_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-06-15 06:26:39.000000 fake-bpy-module-latest-20230615/bl_ui/space_toolsystem_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-06-15 06:26:53.000000 fake-bpy-module-latest-20230615/bl_ui/space_topbar.py
--rw-r--r--   0 runner    (1001) docker     (123)   215185 2023-06-15 06:24:38.000000 fake-bpy-module-latest-20230615/bl_ui/space_userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)   616417 2023-06-15 06:26:03.000000 fake-bpy-module-latest-20230615/bl_ui/space_view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   239548 2023-06-15 06:26:34.000000 fake-bpy-module-latest-20230615/bl_ui/space_view3d_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-15 06:26:48.000000 fake-bpy-module-latest-20230615/bl_ui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/bl_ui_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-15 06:26:55.000000 fake-bpy-module-latest-20230615/bl_ui_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-15 06:26:55.000000 fake-bpy-module-latest-20230615/bl_ui_utils/bug_report_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-15 06:26:55.000000 fake-bpy-module-latest-20230615/bl_ui_utils/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bl_ui_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/blend_render_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-15 06:24:17.000000 fake-bpy-module-latest-20230615/blf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bmesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    77492 2023-06-15 06:24:24.000000 fake-bpy-module-latest-20230615/bmesh/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36665 2023-06-15 06:24:21.000000 fake-bpy-module-latest-20230615/bmesh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-15 06:24:21.000000 fake-bpy-module-latest-20230615/bmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/bpy/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/bpy/app/
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-15 06:24:13.000000 fake-bpy-module-latest-20230615/bpy/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-15 06:24:13.000000 fake-bpy-module-latest-20230615/bpy/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-15 06:24:13.000000 fake-bpy-module-latest-20230615/bpy/app/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bpy/app/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-15 06:24:13.000000 fake-bpy-module-latest-20230615/bpy/app/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-15 06:24:13.000000 fake-bpy-module-latest-20230615/bpy/app/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-15 06:24:14.000000 fake-bpy-module-latest-20230615/bpy/msgbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/bpy/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-15 06:23:21.000000 fake-bpy-module-latest-20230615/bpy/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-06-15 06:23:26.000000 fake-bpy-module-latest-20230615/bpy/ops/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-06-15 06:23:48.000000 fake-bpy-module-latest-20230615/bpy/ops/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    25486 2023-06-15 06:24:04.000000 fake-bpy-module-latest-20230615/bpy/ops/armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-15 06:23:22.000000 fake-bpy-module-latest-20230615/bpy/ops/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-15 06:23:51.000000 fake-bpy-module-latest-20230615/bpy/ops/boid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-15 06:23:36.000000 fake-bpy-module-latest-20230615/bpy/ops/brush.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-06-15 06:23:41.000000 fake-bpy-module-latest-20230615/bpy/ops/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-06-15 06:23:56.000000 fake-bpy-module-latest-20230615/bpy/ops/cachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-15 06:23:45.000000 fake-bpy-module-latest-20230615/bpy/ops/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    70588 2023-06-15 06:23:48.000000 fake-bpy-module-latest-20230615/bpy/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-15 06:23:42.000000 fake-bpy-module-latest-20230615/bpy/ops/cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-15 06:24:05.000000 fake-bpy-module-latest-20230615/bpy/ops/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-06-15 06:23:32.000000 fake-bpy-module-latest-20230615/bpy/ops/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-06-15 06:24:13.000000 fake-bpy-module-latest-20230615/bpy/ops/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    40670 2023-06-15 06:24:00.000000 fake-bpy-module-latest-20230615/bpy/ops/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-06-15 06:23:27.000000 fake-bpy-module-latest-20230615/bpy/ops/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-15 06:23:44.000000 fake-bpy-module-latest-20230615/bpy/ops/cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-15 06:23:28.000000 fake-bpy-module-latest-20230615/bpy/ops/dpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-06-15 06:23:43.000000 fake-bpy-module-latest-20230615/bpy/ops/ed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-15 06:23:52.000000 fake-bpy-module-latest-20230615/bpy/ops/export_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-15 06:23:44.000000 fake-bpy-module-latest-20230615/bpy/ops/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    35992 2023-06-15 06:23:58.000000 fake-bpy-module-latest-20230615/bpy/ops/export_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-06-15 06:23:23.000000 fake-bpy-module-latest-20230615/bpy/ops/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-15 06:23:43.000000 fake-bpy-module-latest-20230615/bpy/ops/fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-06-15 06:23:30.000000 fake-bpy-module-latest-20230615/bpy/ops/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-15 06:24:05.000000 fake-bpy-module-latest-20230615/bpy/ops/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-15 06:23:28.000000 fake-bpy-module-latest-20230615/bpy/ops/gizmogroup.py
--rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-06-15 06:23:38.000000 fake-bpy-module-latest-20230615/bpy/ops/gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    50489 2023-06-15 06:23:44.000000 fake-bpy-module-latest-20230615/bpy/ops/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-06-15 06:23:43.000000 fake-bpy-module-latest-20230615/bpy/ops/grease_pencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-06-15 06:23:54.000000 fake-bpy-module-latest-20230615/bpy/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-15 06:23:31.000000 fake-bpy-module-latest-20230615/bpy/ops/import_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-15 06:23:43.000000 fake-bpy-module-latest-20230615/bpy/ops/import_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-15 06:23:32.000000 fake-bpy-module-latest-20230615/bpy/ops/import_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-06-15 06:23:29.000000 fake-bpy-module-latest-20230615/bpy/ops/import_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-15 06:23:32.000000 fake-bpy-module-latest-20230615/bpy/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-15 06:23:30.000000 fake-bpy-module-latest-20230615/bpy/ops/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-06-15 06:23:44.000000 fake-bpy-module-latest-20230615/bpy/ops/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-06-15 06:24:05.000000 fake-bpy-module-latest-20230615/bpy/ops/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-15 06:23:38.000000 fake-bpy-module-latest-20230615/bpy/ops/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-15 06:23:51.000000 fake-bpy-module-latest-20230615/bpy/ops/mball.py
--rw-r--r--   0 runner    (1001) docker     (123)   179170 2023-06-15 06:24:03.000000 fake-bpy-module-latest-20230615/bpy/ops/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-06-15 06:23:47.000000 fake-bpy-module-latest-20230615/bpy/ops/nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    72286 2023-06-15 06:23:40.000000 fake-bpy-module-latest-20230615/bpy/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (123)   225774 2023-06-15 06:23:36.000000 fake-bpy-module-latest-20230615/bpy/ops/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-06-15 06:23:49.000000 fake-bpy-module-latest-20230615/bpy/ops/outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)    44093 2023-06-15 06:23:41.000000 fake-bpy-module-latest-20230615/bpy/ops/paint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-15 06:23:45.000000 fake-bpy-module-latest-20230615/bpy/ops/paintcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-15 06:23:43.000000 fake-bpy-module-latest-20230615/bpy/ops/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-06-15 06:23:42.000000 fake-bpy-module-latest-20230615/bpy/ops/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39854 2023-06-15 06:23:27.000000 fake-bpy-module-latest-20230615/bpy/ops/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-15 06:23:52.000000 fake-bpy-module-latest-20230615/bpy/ops/poselib.py
--rw-r--r--   0 runner    (1001) docker     (123)    32889 2023-06-15 06:23:28.000000 fake-bpy-module-latest-20230615/bpy/ops/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-15 06:23:43.000000 fake-bpy-module-latest-20230615/bpy/ops/ptcache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bpy/ops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-06-15 06:23:39.000000 fake-bpy-module-latest-20230615/bpy/ops/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-06-15 06:23:22.000000 fake-bpy-module-latest-20230615/bpy/ops/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-06-15 06:23:52.000000 fake-bpy-module-latest-20230615/bpy/ops/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-06-15 06:24:05.000000 fake-bpy-module-latest-20230615/bpy/ops/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-15 06:23:28.000000 fake-bpy-module-latest-20230615/bpy/ops/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-06-15 06:23:31.000000 fake-bpy-module-latest-20230615/bpy/ops/sculpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-15 06:23:43.000000 fake-bpy-module-latest-20230615/bpy/ops/sculpt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    94657 2023-06-15 06:23:51.000000 fake-bpy-module-latest-20230615/bpy/ops/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-06-15 06:23:29.000000 fake-bpy-module-latest-20230615/bpy/ops/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-15 06:23:46.000000 fake-bpy-module-latest-20230615/bpy/ops/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-06-15 06:23:28.000000 fake-bpy-module-latest-20230615/bpy/ops/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-15 06:23:22.000000 fake-bpy-module-latest-20230615/bpy/ops/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-15 06:23:29.000000 fake-bpy-module-latest-20230615/bpy/ops/text_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-15 06:23:38.000000 fake-bpy-module-latest-20230615/bpy/ops/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    72215 2023-06-15 06:23:56.000000 fake-bpy-module-latest-20230615/bpy/ops/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-06-15 06:23:59.000000 fake-bpy-module-latest-20230615/bpy/ops/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-15 06:23:28.000000 fake-bpy-module-latest-20230615/bpy/ops/uilist.py
--rw-r--r--   0 runner    (1001) docker     (123)    57216 2023-06-15 06:23:46.000000 fake-bpy-module-latest-20230615/bpy/ops/uv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-06-15 06:23:43.000000 fake-bpy-module-latest-20230615/bpy/ops/view2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    55643 2023-06-15 06:23:26.000000 fake-bpy-module-latest-20230615/bpy/ops/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   246250 2023-06-15 06:24:13.000000 fake-bpy-module-latest-20230615/bpy/ops/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-15 06:23:27.000000 fake-bpy-module-latest-20230615/bpy/ops/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-15 06:23:51.000000 fake-bpy-module-latest-20230615/bpy/ops/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-15 06:24:14.000000 fake-bpy-module-latest-20230615/bpy/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-06-15 06:24:14.000000 fake-bpy-module-latest-20230615/bpy/props.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)  3490007 2023-06-15 06:23:21.000000 fake-bpy-module-latest-20230615/bpy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/bpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-06-15 06:24:14.000000 fake-bpy-module-latest-20230615/bpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-15 06:24:14.000000 fake-bpy-module-latest-20230615/bpy/utils/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bpy/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-15 06:24:14.000000 fake-bpy-module-latest-20230615/bpy/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/bpy_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/anim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/asset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/bmesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/id_map_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/keyconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/node_shader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bpy_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/view3d_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/bpy_extras/wm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/wm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/bpy_extras/wm_utils/progress_report.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/bpy_extras/wm_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-15 06:26:55.000000 fake-bpy-module-latest-20230615/bpy_restrict_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-06-15 06:26:56.000000 fake-bpy-module-latest-20230615/bpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-15 06:26:54.000000 fake-bpy-module-latest-20230615/console_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/console_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/fake_bpy_module_latest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/fake_bpy_module_latest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/fake_bpy_module_latest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/fake_bpy_module_latest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/fake_bpy_module_latest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/fake_bpy_module_latest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/freestyle/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/freestyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/freestyle/chainingiterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/freestyle/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/freestyle/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/freestyle/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-06-15 06:24:19.000000 fake-bpy-module-latest-20230615/freestyle/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/freestyle/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/freestyle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/freestyle/utils/ContextFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-15 06:24:20.000000 fake-bpy-module-latest-20230615/freestyle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/freestyle/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/gpu/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/gpu/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/gpu/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/gpu/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/gpu/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/gpu/shader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/gpu/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/gpu/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/gpu/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/gpu_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/gpu_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/gpu_extras/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/gpu_extras/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/gpu_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/graphviz_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/idprop/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-15 06:24:24.000000 fake-bpy-module-latest-20230615/idprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/idprop/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-15 06:24:24.000000 fake-bpy-module-latest-20230615/idprop/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/imbuf/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-15 06:24:24.000000 fake-bpy-module-latest-20230615/imbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/imbuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-15 06:24:24.000000 fake-bpy-module-latest-20230615/imbuf/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/keyingsets_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-15 06:26:57.000000 fake-bpy-module-latest-20230615/keyingsets_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/mathutils/
--rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/mathutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/mathutils/bvhtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/mathutils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/mathutils/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/mathutils/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-06-15 06:24:18.000000 fake-bpy-module-latest-20230615/mathutils/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:14:16.000000 fake-bpy-module-latest-20230615/mathutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/nodeitems_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/nodeitems_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/rna_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/rna_keymap_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-15 06:27:05.000000 fake-bpy-module-latest-20230615/rna_prop_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-15 06:26:55.000000 fake-bpy-module-latest-20230615/rna_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:27:07.000000 fake-bpy-module-latest-20230615/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-15 06:27:06.000000 fake-bpy-module-latest-20230615/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-15 06:24:24.000000 fake-bpy-module-latest-20230615/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-06-16 06:22:10.000000 fake-bpy-module-latest-20230616/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/addon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-16 06:22:09.000000 fake-bpy-module-latest-20230616/animsys_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30417 2023-06-16 06:20:15.000000 fake-bpy-module-latest-20230616/aud.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-06-16 06:20:12.000000 fake-bpy-module-latest-20230616/bgl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bl_app_override/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_app_override/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_app_override/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bl_app_override/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_app_template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bl_console_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_console_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bl_console_utils/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_console_utils/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_console_utils/autocomplete/complete_calltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_console_utils/autocomplete/complete_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_console_utils/autocomplete/complete_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_console_utils/autocomplete/intellisense.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bl_console_utils/autocomplete/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bl_console_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bl_i18n_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-16 06:22:10.000000 fake-bpy-module-latest-20230616/bl_i18n_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-16 06:22:10.000000 fake-bpy-module-latest-20230616/bl_i18n_utils/bl_extract_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-16 06:22:10.000000 fake-bpy-module-latest-20230616/bl_i18n_utils/merge_po.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bl_i18n_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-16 06:22:10.000000 fake-bpy-module-latest-20230616/bl_i18n_utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-16 06:22:10.000000 fake-bpy-module-latest-20230616/bl_i18n_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 06:22:10.000000 fake-bpy-module-latest-20230616/bl_i18n_utils/utils_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-16 06:22:10.000000 fake-bpy-module-latest-20230616/bl_i18n_utils/utils_languages_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-16 06:22:10.000000 fake-bpy-module-latest-20230616/bl_i18n_utils/utils_rtl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bl_keymap_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_keymap_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_keymap_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_keymap_utils/keymap_from_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_keymap_utils/keymap_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_keymap_utils/platform_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bl_keymap_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_keymap_utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-16 06:20:18.000000 fake-bpy-module-latest-20230616/bl_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bl_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-16 06:22:03.000000 fake-bpy-module-latest-20230616/bl_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-16 06:22:07.000000 fake-bpy-module-latest-20230616/bl_operators/add_mesh_torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-06-16 06:22:06.000000 fake-bpy-module-latest-20230616/bl_operators/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-16 06:22:07.000000 fake-bpy-module-latest-20230616/bl_operators/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bl_operators/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-16 06:22:07.000000 fake-bpy-module-latest-20230616/bl_operators/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-16 06:22:07.000000 fake-bpy-module-latest-20230616/bl_operators/bmesh/find_adjacent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bl_operators/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-06-16 06:22:08.000000 fake-bpy-module-latest-20230616/bl_operators/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-16 06:22:07.000000 fake-bpy-module-latest-20230616/bl_operators/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-16 06:22:08.000000 fake-bpy-module-latest-20230616/bl_operators/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-16 06:22:05.000000 fake-bpy-module-latest-20230616/bl_operators/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-16 06:22:06.000000 fake-bpy-module-latest-20230616/bl_operators/freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-06-16 06:22:04.000000 fake-bpy-module-latest-20230616/bl_operators/geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-16 06:22:04.000000 fake-bpy-module-latest-20230616/bl_operators/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-16 06:22:05.000000 fake-bpy-module-latest-20230616/bl_operators/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-06-16 06:22:07.000000 fake-bpy-module-latest-20230616/bl_operators/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38122 2023-06-16 06:22:06.000000 fake-bpy-module-latest-20230616/bl_operators/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-16 06:22:07.000000 fake-bpy-module-latest-20230616/bl_operators/object_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-16 06:22:06.000000 fake-bpy-module-latest-20230616/bl_operators/object_quick_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-16 06:22:07.000000 fake-bpy-module-latest-20230616/bl_operators/object_randomize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-06-16 06:22:07.000000 fake-bpy-module-latest-20230616/bl_operators/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bl_operators/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-16 06:22:07.000000 fake-bpy-module-latest-20230616/bl_operators/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-16 06:22:07.000000 fake-bpy-module-latest-20230616/bl_operators/screen_play_rendered_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-06-16 06:22:03.000000 fake-bpy-module-latest-20230616/bl_operators/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-16 06:22:03.000000 fake-bpy-module-latest-20230616/bl_operators/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-16 06:22:04.000000 fake-bpy-module-latest-20230616/bl_operators/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-06-16 06:22:09.000000 fake-bpy-module-latest-20230616/bl_operators/userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-16 06:22:07.000000 fake-bpy-module-latest-20230616/bl_operators/uvcalc_follow_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-16 06:22:08.000000 fake-bpy-module-latest-20230616/bl_operators/uvcalc_lightmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-16 06:22:05.000000 fake-bpy-module-latest-20230616/bl_operators/uvcalc_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-16 06:22:06.000000 fake-bpy-module-latest-20230616/bl_operators/vertexpaint_dirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-06-16 06:22:05.000000 fake-bpy-module-latest-20230616/bl_operators/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-06-16 06:22:05.000000 fake-bpy-module-latest-20230616/bl_operators/wm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bl_previews_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 06:22:09.000000 fake-bpy-module-latest-20230616/bl_previews_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-16 06:22:09.000000 fake-bpy-module-latest-20230616/bl_previews_utils/bl_previews_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bl_previews_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bl_rna_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 06:22:03.000000 fake-bpy-module-latest-20230616/bl_rna_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-16 06:22:03.000000 fake-bpy-module-latest-20230616/bl_rna_utils/data_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bl_rna_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bl_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-06-16 06:20:18.000000 fake-bpy-module-latest-20230616/bl_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-16 06:21:31.000000 fake-bpy-module-latest-20230616/bl_ui/generic_ui_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-16 06:20:36.000000 fake-bpy-module-latest-20230616/bl_ui/node_add_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110864 2023-06-16 06:21:52.000000 fake-bpy-module-latest-20230616/bl_ui/node_add_menu_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-16 06:20:24.000000 fake-bpy-module-latest-20230616/bl_ui/properties_animviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-06-16 06:21:55.000000 fake-bpy-module-latest-20230616/bl_ui/properties_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-06-16 06:21:46.000000 fake-bpy-module-latest-20230616/bl_ui/properties_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-06-16 06:21:32.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-06-16 06:21:28.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_bone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-06-16 06:21:28.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-06-16 06:20:36.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-16 06:22:00.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-06-16 06:22:00.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-06-16 06:21:29.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-06-16 06:21:29.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-06-16 06:21:55.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_lightprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52746 2023-06-16 06:21:31.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-16 06:21:46.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_metaball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-16 06:21:31.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-06-16 06:21:47.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-16 06:21:53.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_shaderfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-16 06:20:36.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-06-16 06:20:18.000000 fake-bpy-module-latest-20230616/bl_ui/properties_data_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_ui/properties_freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-06-16 06:21:53.000000 fake-bpy-module-latest-20230616/bl_ui/properties_grease_pencil_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-06-16 06:21:54.000000 fake-bpy-module-latest-20230616/bl_ui/properties_mask_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-06-16 06:20:25.000000 fake-bpy-module-latest-20230616/bl_ui/properties_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-06-16 06:20:27.000000 fake-bpy-module-latest-20230616/bl_ui/properties_material_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-06-16 06:22:01.000000 fake-bpy-module-latest-20230616/bl_ui/properties_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-06-16 06:21:54.000000 fake-bpy-module-latest-20230616/bl_ui/properties_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-16 06:21:28.000000 fake-bpy-module-latest-20230616/bl_ui/properties_paint_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-06-16 06:21:59.000000 fake-bpy-module-latest-20230616/bl_ui/properties_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-16 06:20:27.000000 fake-bpy-module-latest-20230616/bl_ui/properties_physics_cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-16 06:20:25.000000 fake-bpy-module-latest-20230616/bl_ui/properties_physics_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-06-16 06:20:23.000000 fake-bpy-module-latest-20230616/bl_ui/properties_physics_dynamicpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-06-16 06:20:19.000000 fake-bpy-module-latest-20230616/bl_ui/properties_physics_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-06-16 06:21:47.000000 fake-bpy-module-latest-20230616/bl_ui/properties_physics_fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-16 06:21:28.000000 fake-bpy-module-latest-20230616/bl_ui/properties_physics_geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-16 06:20:25.000000 fake-bpy-module-latest-20230616/bl_ui/properties_physics_rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-06-16 06:20:25.000000 fake-bpy-module-latest-20230616/bl_ui/properties_physics_rigidbody_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-06-16 06:20:27.000000 fake-bpy-module-latest-20230616/bl_ui/properties_physics_softbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-06-16 06:21:30.000000 fake-bpy-module-latest-20230616/bl_ui/properties_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-06-16 06:21:55.000000 fake-bpy-module-latest-20230616/bl_ui/properties_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-06-16 06:20:36.000000 fake-bpy-module-latest-20230616/bl_ui/properties_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-06-16 06:20:18.000000 fake-bpy-module-latest-20230616/bl_ui/properties_view_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-16 06:21:53.000000 fake-bpy-module-latest-20230616/bl_ui/properties_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-06-16 06:21:53.000000 fake-bpy-module-latest-20230616/bl_ui/properties_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bl_ui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   176850 2023-06-16 06:20:31.000000 fake-bpy-module-latest-20230616/bl_ui/space_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/bl_ui/space_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64929 2023-06-16 06:21:49.000000 fake-bpy-module-latest-20230616/bl_ui/space_dopesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-06-16 06:20:24.000000 fake-bpy-module-latest-20230616/bl_ui/space_filebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50899 2023-06-16 06:21:52.000000 fake-bpy-module-latest-20230616/bl_ui/space_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-06-16 06:20:22.000000 fake-bpy-module-latest-20230616/bl_ui/space_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-06-16 06:22:01.000000 fake-bpy-module-latest-20230616/bl_ui/space_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-06-16 06:21:53.000000 fake-bpy-module-latest-20230616/bl_ui/space_nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75065 2023-06-16 06:21:57.000000 fake-bpy-module-latest-20230616/bl_ui/space_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-06-16 06:21:56.000000 fake-bpy-module-latest-20230616/bl_ui/space_outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-16 06:20:31.000000 fake-bpy-module-latest-20230616/bl_ui/space_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-06-16 06:21:36.000000 fake-bpy-module-latest-20230616/bl_ui/space_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-16 06:20:31.000000 fake-bpy-module-latest-20230616/bl_ui/space_spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-16 06:21:53.000000 fake-bpy-module-latest-20230616/bl_ui/space_statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-06-16 06:20:26.000000 fake-bpy-module-latest-20230616/bl_ui/space_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-06-16 06:21:28.000000 fake-bpy-module-latest-20230616/bl_ui/space_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-16 06:21:30.000000 fake-bpy-module-latest-20230616/bl_ui/space_toolsystem_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-06-16 06:21:29.000000 fake-bpy-module-latest-20230616/bl_ui/space_toolsystem_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-06-16 06:21:50.000000 fake-bpy-module-latest-20230616/bl_ui/space_topbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   215185 2023-06-16 06:20:35.000000 fake-bpy-module-latest-20230616/bl_ui/space_userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)   616417 2023-06-16 06:21:20.000000 fake-bpy-module-latest-20230616/bl_ui/space_view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239548 2023-06-16 06:21:27.000000 fake-bpy-module-latest-20230616/bl_ui/space_view3d_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-16 06:21:30.000000 fake-bpy-module-latest-20230616/bl_ui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bl_ui_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-16 06:22:09.000000 fake-bpy-module-latest-20230616/bl_ui_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-16 06:22:09.000000 fake-bpy-module-latest-20230616/bl_ui_utils/bug_report_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-16 06:22:09.000000 fake-bpy-module-latest-20230616/bl_ui_utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bl_ui_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-16 06:22:09.000000 fake-bpy-module-latest-20230616/blend_render_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-16 06:20:12.000000 fake-bpy-module-latest-20230616/blf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-16 06:20:15.000000 fake-bpy-module-latest-20230616/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-16 06:20:15.000000 fake-bpy-module-latest-20230616/bmesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77492 2023-06-16 06:20:17.000000 fake-bpy-module-latest-20230616/bmesh/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36665 2023-06-16 06:20:17.000000 fake-bpy-module-latest-20230616/bmesh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-16 06:20:17.000000 fake-bpy-module-latest-20230616/bmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bpy/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-16 06:20:10.000000 fake-bpy-module-latest-20230616/bpy/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-16 06:20:10.000000 fake-bpy-module-latest-20230616/bpy/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-16 06:20:10.000000 fake-bpy-module-latest-20230616/bpy/app/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bpy/app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-16 06:20:10.000000 fake-bpy-module-latest-20230616/bpy/app/timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-16 06:20:10.000000 fake-bpy-module-latest-20230616/bpy/app/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-16 06:20:10.000000 fake-bpy-module-latest-20230616/bpy/msgbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bpy/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 06:19:32.000000 fake-bpy-module-latest-20230616/bpy/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-06-16 06:19:55.000000 fake-bpy-module-latest-20230616/bpy/ops/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-06-16 06:19:46.000000 fake-bpy-module-latest-20230616/bpy/ops/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25486 2023-06-16 06:19:48.000000 fake-bpy-module-latest-20230616/bpy/ops/armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-16 06:19:55.000000 fake-bpy-module-latest-20230616/bpy/ops/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-16 06:19:55.000000 fake-bpy-module-latest-20230616/bpy/ops/boid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-16 06:19:54.000000 fake-bpy-module-latest-20230616/bpy/ops/brush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-06-16 06:19:42.000000 fake-bpy-module-latest-20230616/bpy/ops/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-06-16 06:19:35.000000 fake-bpy-module-latest-20230616/bpy/ops/cachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-16 06:19:55.000000 fake-bpy-module-latest-20230616/bpy/ops/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70588 2023-06-16 06:19:54.000000 fake-bpy-module-latest-20230616/bpy/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-16 06:20:02.000000 fake-bpy-module-latest-20230616/bpy/ops/cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-16 06:19:32.000000 fake-bpy-module-latest-20230616/bpy/ops/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-06-16 06:19:44.000000 fake-bpy-module-latest-20230616/bpy/ops/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-06-16 06:19:42.000000 fake-bpy-module-latest-20230616/bpy/ops/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40670 2023-06-16 06:19:46.000000 fake-bpy-module-latest-20230616/bpy/ops/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-06-16 06:19:57.000000 fake-bpy-module-latest-20230616/bpy/ops/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-16 06:19:55.000000 fake-bpy-module-latest-20230616/bpy/ops/cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-16 06:20:00.000000 fake-bpy-module-latest-20230616/bpy/ops/dpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-06-16 06:20:02.000000 fake-bpy-module-latest-20230616/bpy/ops/ed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-16 06:19:55.000000 fake-bpy-module-latest-20230616/bpy/ops/export_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-16 06:19:54.000000 fake-bpy-module-latest-20230616/bpy/ops/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35992 2023-06-16 06:20:07.000000 fake-bpy-module-latest-20230616/bpy/ops/export_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-06-16 06:19:32.000000 fake-bpy-module-latest-20230616/bpy/ops/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-16 06:19:56.000000 fake-bpy-module-latest-20230616/bpy/ops/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-06-16 06:19:50.000000 fake-bpy-module-latest-20230616/bpy/ops/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-16 06:19:56.000000 fake-bpy-module-latest-20230616/bpy/ops/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-16 06:19:55.000000 fake-bpy-module-latest-20230616/bpy/ops/gizmogroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-06-16 06:20:02.000000 fake-bpy-module-latest-20230616/bpy/ops/gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50489 2023-06-16 06:19:57.000000 fake-bpy-module-latest-20230616/bpy/ops/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-06-16 06:20:10.000000 fake-bpy-module-latest-20230616/bpy/ops/grease_pencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-06-16 06:19:48.000000 fake-bpy-module-latest-20230616/bpy/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-16 06:19:44.000000 fake-bpy-module-latest-20230616/bpy/ops/import_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-16 06:19:33.000000 fake-bpy-module-latest-20230616/bpy/ops/import_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-16 06:19:44.000000 fake-bpy-module-latest-20230616/bpy/ops/import_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-06-16 06:19:52.000000 fake-bpy-module-latest-20230616/bpy/ops/import_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-16 06:19:46.000000 fake-bpy-module-latest-20230616/bpy/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-16 06:19:52.000000 fake-bpy-module-latest-20230616/bpy/ops/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-06-16 06:19:50.000000 fake-bpy-module-latest-20230616/bpy/ops/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-06-16 06:20:05.000000 fake-bpy-module-latest-20230616/bpy/ops/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-16 06:19:57.000000 fake-bpy-module-latest-20230616/bpy/ops/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-16 06:19:52.000000 fake-bpy-module-latest-20230616/bpy/ops/mball.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179170 2023-06-16 06:20:05.000000 fake-bpy-module-latest-20230616/bpy/ops/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-06-16 06:19:47.000000 fake-bpy-module-latest-20230616/bpy/ops/nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72286 2023-06-16 06:19:51.000000 fake-bpy-module-latest-20230616/bpy/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)   225774 2023-06-16 06:20:00.000000 fake-bpy-module-latest-20230616/bpy/ops/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-06-16 06:19:45.000000 fake-bpy-module-latest-20230616/bpy/ops/outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44093 2023-06-16 06:20:10.000000 fake-bpy-module-latest-20230616/bpy/ops/paint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-16 06:19:51.000000 fake-bpy-module-latest-20230616/bpy/ops/paintcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-16 06:19:53.000000 fake-bpy-module-latest-20230616/bpy/ops/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-06-16 06:20:05.000000 fake-bpy-module-latest-20230616/bpy/ops/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39854 2023-06-16 06:20:09.000000 fake-bpy-module-latest-20230616/bpy/ops/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-16 06:19:32.000000 fake-bpy-module-latest-20230616/bpy/ops/poselib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32889 2023-06-16 06:19:55.000000 fake-bpy-module-latest-20230616/bpy/ops/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-16 06:19:32.000000 fake-bpy-module-latest-20230616/bpy/ops/ptcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bpy/ops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-06-16 06:19:41.000000 fake-bpy-module-latest-20230616/bpy/ops/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-06-16 06:20:10.000000 fake-bpy-module-latest-20230616/bpy/ops/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-06-16 06:19:36.000000 fake-bpy-module-latest-20230616/bpy/ops/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-06-16 06:19:52.000000 fake-bpy-module-latest-20230616/bpy/ops/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-16 06:19:52.000000 fake-bpy-module-latest-20230616/bpy/ops/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-06-16 06:19:53.000000 fake-bpy-module-latest-20230616/bpy/ops/sculpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-16 06:19:42.000000 fake-bpy-module-latest-20230616/bpy/ops/sculpt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94657 2023-06-16 06:19:44.000000 fake-bpy-module-latest-20230616/bpy/ops/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-06-16 06:19:45.000000 fake-bpy-module-latest-20230616/bpy/ops/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-16 06:19:49.000000 fake-bpy-module-latest-20230616/bpy/ops/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-06-16 06:19:42.000000 fake-bpy-module-latest-20230616/bpy/ops/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-16 06:19:42.000000 fake-bpy-module-latest-20230616/bpy/ops/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-16 06:19:49.000000 fake-bpy-module-latest-20230616/bpy/ops/text_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-16 06:20:06.000000 fake-bpy-module-latest-20230616/bpy/ops/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72215 2023-06-16 06:20:08.000000 fake-bpy-module-latest-20230616/bpy/ops/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-06-16 06:20:02.000000 fake-bpy-module-latest-20230616/bpy/ops/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-16 06:19:32.000000 fake-bpy-module-latest-20230616/bpy/ops/uilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57216 2023-06-16 06:19:35.000000 fake-bpy-module-latest-20230616/bpy/ops/uv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-06-16 06:19:32.000000 fake-bpy-module-latest-20230616/bpy/ops/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55643 2023-06-16 06:19:49.000000 fake-bpy-module-latest-20230616/bpy/ops/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   246250 2023-06-16 06:19:41.000000 fake-bpy-module-latest-20230616/bpy/ops/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-16 06:19:46.000000 fake-bpy-module-latest-20230616/bpy/ops/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-16 06:19:45.000000 fake-bpy-module-latest-20230616/bpy/ops/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-16 06:20:10.000000 fake-bpy-module-latest-20230616/bpy/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-06-16 06:19:32.000000 fake-bpy-module-latest-20230616/bpy/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)  3490007 2023-06-16 06:19:31.000000 fake-bpy-module-latest-20230616/bpy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-06-16 06:20:10.000000 fake-bpy-module-latest-20230616/bpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-16 06:20:10.000000 fake-bpy-module-latest-20230616/bpy/utils/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bpy/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-16 06:20:10.000000 fake-bpy-module-latest-20230616/bpy/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bpy_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/bpy_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/bpy_extras/anim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/bpy_extras/asset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-16 06:20:15.000000 fake-bpy-module-latest-20230616/bpy_extras/bmesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/bpy_extras/id_map_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/bpy_extras/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/bpy_extras/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/bpy_extras/keyconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/bpy_extras/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-16 06:20:15.000000 fake-bpy-module-latest-20230616/bpy_extras/node_shader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/bpy_extras/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/bpy_extras/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bpy_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/bpy_extras/view3d_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/bpy_extras/wm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/bpy_extras/wm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-16 06:20:15.000000 fake-bpy-module-latest-20230616/bpy_extras/wm_utils/progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/bpy_extras/wm_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-16 06:22:09.000000 fake-bpy-module-latest-20230616/bpy_restrict_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-06-16 06:22:10.000000 fake-bpy-module-latest-20230616/bpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-16 06:22:09.000000 fake-bpy-module-latest-20230616/console_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/console_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/fake_bpy_module_latest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/fake_bpy_module_latest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/fake_bpy_module_latest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/fake_bpy_module_latest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/fake_bpy_module_latest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/fake_bpy_module_latest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/freestyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/freestyle/chainingiterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/freestyle/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/freestyle/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/freestyle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/freestyle/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/freestyle/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/freestyle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/freestyle/utils/ContextFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/freestyle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/freestyle/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-16 06:20:13.000000 fake-bpy-module-latest-20230616/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/gpu/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/gpu/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/gpu/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/gpu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/gpu/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/gpu/shader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/gpu/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/gpu/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-06-16 06:20:13.000000 fake-bpy-module-latest-20230616/gpu/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/gpu_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/gpu_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/gpu_extras/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-16 06:20:14.000000 fake-bpy-module-latest-20230616/gpu_extras/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/gpu_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-16 06:22:03.000000 fake-bpy-module-latest-20230616/graphviz_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/idprop/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 06:20:17.000000 fake-bpy-module-latest-20230616/idprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/idprop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-16 06:20:17.000000 fake-bpy-module-latest-20230616/idprop/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/imbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-16 06:20:17.000000 fake-bpy-module-latest-20230616/imbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/imbuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-16 06:20:17.000000 fake-bpy-module-latest-20230616/imbuf/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-06-16 06:22:03.000000 fake-bpy-module-latest-20230616/keyingsets_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 06:22:09.000000 fake-bpy-module-latest-20230616/keyingsets_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/mathutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-06-16 06:20:13.000000 fake-bpy-module-latest-20230616/mathutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-16 06:20:13.000000 fake-bpy-module-latest-20230616/mathutils/bvhtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-06-16 06:20:13.000000 fake-bpy-module-latest-20230616/mathutils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 06:20:13.000000 fake-bpy-module-latest-20230616/mathutils/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-16 06:20:13.000000 fake-bpy-module-latest-20230616/mathutils/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-06-16 06:20:13.000000 fake-bpy-module-latest-20230616/mathutils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:13:12.000000 fake-bpy-module-latest-20230616/mathutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-16 06:22:03.000000 fake-bpy-module-latest-20230616/nodeitems_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/nodeitems_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-16 06:22:03.000000 fake-bpy-module-latest-20230616/rna_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/rna_keymap_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-16 06:22:09.000000 fake-bpy-module-latest-20230616/rna_prop_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-16 06:22:09.000000 fake-bpy-module-latest-20230616/rna_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:22:11.000000 fake-bpy-module-latest-20230616/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-16 06:22:10.000000 fake-bpy-module-latest-20230616/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 06:22:02.000000 fake-bpy-module-latest-20230616/sys_info.py
```

### Comparing `fake-bpy-module-latest-20230615/PKG-INFO` & `fake-bpy-module-latest-20230616/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230615
+Version: 20230616
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230615/README.rst` & `fake-bpy-module-latest-20230616/README.rst`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/addon_utils.py` & `fake-bpy-module-latest-20230616/addon_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/animsys_refactor.py` & `fake-bpy-module-latest-20230616/animsys_refactor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/aud.py` & `fake-bpy-module-latest-20230616/aud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bgl.py` & `fake-bpy-module-latest-20230616/bgl.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_app_override/helpers.py` & `fake-bpy-module-latest-20230616/bl_app_override/helpers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_i18n_utils/bl_extract_messages.py` & `fake-bpy-module-latest-20230616/bl_i18n_utils/bl_extract_messages.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_i18n_utils/settings.py` & `fake-bpy-module-latest-20230616/bl_i18n_utils/settings.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_i18n_utils/utils.py` & `fake-bpy-module-latest-20230616/bl_i18n_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_keymap_utils/io.py` & `fake-bpy-module-latest-20230616/bl_keymap_utils/io.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_math.py` & `fake-bpy-module-latest-20230616/bl_math.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/__init__.py` & `fake-bpy-module-latest-20230616/bl_operators/__init__.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import sys
 import typing
-from . import presets
-from . import text
-from . import uvcalc_follow_active
-from . import add_mesh_torus
-from . import uvcalc_transform
 from . import sequencer
-from . import object_randomize_transform
-from . import geometry_nodes
-from . import file
-from . import rigidbody
 from . import spreadsheet
-from . import object_align
+from . import geometry_nodes
+from . import text
 from . import image
-from . import view3d
-from . import userpref
 from . import wm
-from . import vertexpaint_dirt
-from . import screen_play_rendered_anim
-from . import node
-from . import constraint
-from . import freestyle
+from . import mesh
+from . import view3d
+from . import file
+from . import uvcalc_transform
+from . import object
 from . import anim
+from . import freestyle
+from . import vertexpaint_dirt
 from . import object_quick_effects
-from . import object
-from . import mesh
-from . import clip
 from . import console
+from . import rigidbody
+from . import add_mesh_torus
+from . import screen_play_rendered_anim
+from . import object_align
 from . import assets
+from . import object_randomize_transform
+from . import node
+from . import uvcalc_follow_active
 from . import bmesh
+from . import presets
 from . import uvcalc_lightmap
+from . import clip
+from . import constraint
+from . import userpref
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def register():
     '''
```

### Comparing `fake-bpy-module-latest-20230615/bl_operators/add_mesh_torus.py` & `fake-bpy-module-latest-20230616/bl_operators/add_mesh_torus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/anim.py` & `fake-bpy-module-latest-20230616/bl_operators/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/assets.py` & `fake-bpy-module-latest-20230616/bl_operators/assets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/bmesh/find_adjacent.py` & `fake-bpy-module-latest-20230616/bl_operators/bmesh/find_adjacent.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/clip.py` & `fake-bpy-module-latest-20230616/bl_operators/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/console.py` & `fake-bpy-module-latest-20230616/bl_operators/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/constraint.py` & `fake-bpy-module-latest-20230616/bl_operators/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/file.py` & `fake-bpy-module-latest-20230616/bl_operators/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/freestyle.py` & `fake-bpy-module-latest-20230616/bl_operators/freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/geometry_nodes.py` & `fake-bpy-module-latest-20230616/bl_operators/geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/image.py` & `fake-bpy-module-latest-20230616/bl_operators/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/mesh.py` & `fake-bpy-module-latest-20230616/bl_operators/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/node.py` & `fake-bpy-module-latest-20230616/bl_operators/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/object.py` & `fake-bpy-module-latest-20230616/bl_operators/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/object_align.py` & `fake-bpy-module-latest-20230616/bl_operators/object_align.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/object_quick_effects.py` & `fake-bpy-module-latest-20230616/bl_operators/object_quick_effects.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/object_randomize_transform.py` & `fake-bpy-module-latest-20230616/bl_operators/object_randomize_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/presets.py` & `fake-bpy-module-latest-20230616/bl_operators/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/rigidbody.py` & `fake-bpy-module-latest-20230616/bl_operators/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/screen_play_rendered_anim.py` & `fake-bpy-module-latest-20230616/bl_operators/screen_play_rendered_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/sequencer.py` & `fake-bpy-module-latest-20230616/bl_operators/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/spreadsheet.py` & `fake-bpy-module-latest-20230616/bl_operators/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/text.py` & `fake-bpy-module-latest-20230616/bl_operators/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/userpref.py` & `fake-bpy-module-latest-20230616/bl_operators/userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/uvcalc_follow_active.py` & `fake-bpy-module-latest-20230616/bl_operators/uvcalc_follow_active.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/uvcalc_lightmap.py` & `fake-bpy-module-latest-20230616/bl_operators/uvcalc_lightmap.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/uvcalc_transform.py` & `fake-bpy-module-latest-20230616/bl_operators/uvcalc_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/vertexpaint_dirt.py` & `fake-bpy-module-latest-20230616/bl_operators/vertexpaint_dirt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/view3d.py` & `fake-bpy-module-latest-20230616/bl_operators/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_operators/wm.py` & `fake-bpy-module-latest-20230616/bl_operators/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_previews_utils/bl_previews_render.py` & `fake-bpy-module-latest-20230616/bl_previews_utils/bl_previews_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/__init__.py` & `fake-bpy-module-latest-20230616/bl_ui/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 import sys
 import typing
 import bpy_types
 
-from . import properties_data_pointcloud
+from . import properties_data_volume
+from . import properties_view_layer
+from . import properties_physics_field
 from . import space_image
-from . import properties_data_mesh
-from . import properties_world
-from . import properties_collection
-from . import properties_data_light
-from . import space_userpref
-from . import properties_data_lightprobe
-from . import properties_data_shaderfx
-from . import properties_data_lattice
-from . import properties_data_curve
-from . import properties_physics_softbody
-from . import properties_data_speaker
-from . import properties_constraint
-from . import space_dopesheet
-from . import properties_physics_common
-from . import properties_physics_fluid
-from . import space_toolsystem_common
-from . import space_properties
-from . import properties_data_metaball
-from . import properties_grease_pencil_common
+from . import properties_physics_dynamicpaint
+from . import space_filebrowser
 from . import properties_animviz
-from . import space_view3d
-from . import properties_data_curves
-from . import properties_data_volume
-from . import properties_object
-from . import node_add_menu
-from . import properties_data_modifier
-from . import space_node
-from . import space_spreadsheet
 from . import properties_physics_rigidbody
-from . import properties_data_gpencil
-from . import space_nla
-from . import properties_material_gpencil
-from . import generic_ui_list
-from . import properties_paint_common
+from . import properties_physics_common
+from . import properties_physics_rigidbody_constraint
+from . import properties_material
 from . import space_text
-from . import properties_data_empty
-from . import space_statusbar
-from . import space_outliner
-from . import space_sequencer
-from . import properties_render
-from . import space_clip
 from . import properties_physics_cloth
-from . import properties_material
-from . import space_view3d_toolbar
-from . import space_time
-from . import space_console
+from . import properties_material_gpencil
+from . import properties_physics_softbody
+from . import space_clip
+from . import space_properties
+from . import space_spreadsheet
+from . import space_userpref
 from . import properties_texture
-from . import properties_freestyle
+from . import node_add_menu
+from . import properties_data_curves
+from . import properties_data_speaker
+from . import space_view3d
+from . import space_view3d_toolbar
+from . import properties_data_camera
+from . import properties_physics_geometry_nodes
 from . import properties_data_bone
-from . import properties_output
+from . import properties_paint_common
+from . import space_time
+from . import properties_data_light
+from . import properties_data_lattice
 from . import space_toolsystem_toolbar
-from . import node_add_menu_geometry
-from . import properties_particle
-from . import properties_physics_dynamicpaint
-from . import properties_workspace
-from . import properties_physics_field
+from . import properties_render
+from . import space_toolsystem_common
 from . import utils
-from . import space_graph
+from . import properties_data_mesh
+from . import generic_ui_list
+from . import properties_data_modifier
 from . import properties_data_armature
-from . import properties_physics_rigidbody_constraint
-from . import space_filebrowser
-from . import space_info
-from . import properties_mask_common
+from . import space_sequencer
+from . import properties_constraint
+from . import properties_data_metaball
+from . import properties_physics_fluid
+from . import properties_data_pointcloud
+from . import space_dopesheet
 from . import space_topbar
-from . import properties_view_layer
-from . import properties_data_camera
+from . import node_add_menu_geometry
+from . import space_graph
+from . import properties_grease_pencil_common
+from . import properties_world
+from . import properties_workspace
+from . import space_nla
+from . import space_statusbar
+from . import properties_data_shaderfx
+from . import properties_output
+from . import properties_mask_common
+from . import properties_data_lightprobe
+from . import properties_collection
 from . import properties_scene
-from . import properties_physics_geometry_nodes
+from . import space_outliner
+from . import space_node
+from . import properties_particle
+from . import properties_data_gpencil
+from . import properties_data_empty
+from . import properties_object
+from . import space_info
+from . import properties_freestyle
+from . import properties_data_curve
+from . import space_console
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class UI_MT_button_context_menu(bpy_types.Menu, bpy_types._GenericUI):
     bl_idname = None
     ''' '''
```

### Comparing `fake-bpy-module-latest-20230615/bl_ui/generic_ui_list.py` & `fake-bpy-module-latest-20230616/bl_ui/generic_ui_list.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/node_add_menu_geometry.py` & `fake-bpy-module-latest-20230616/bl_ui/node_add_menu_geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_animviz.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_animviz.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_collection.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_constraint.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_armature.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_bone.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_bone.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_camera.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_curve.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_curves.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_empty.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_empty.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_gpencil.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_lattice.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_light.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_light.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_lightprobe.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_lightprobe.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_mesh.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_metaball.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_metaball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_modifier.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_modifier.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_pointcloud.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_pointcloud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_shaderfx.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_shaderfx.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_speaker.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_speaker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_data_volume.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_data_volume.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_freestyle.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_grease_pencil_common.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_grease_pencil_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_mask_common.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_mask_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_material.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_material_gpencil.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_material_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_object.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_output.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_output.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_paint_common.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_paint_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_particle.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_physics_cloth.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_physics_cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_physics_common.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_physics_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_physics_dynamicpaint.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_physics_dynamicpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_physics_field.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_physics_field.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_physics_fluid.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_physics_fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_physics_geometry_nodes.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_physics_geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_physics_rigidbody.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_physics_rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_physics_rigidbody_constraint.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_physics_rigidbody_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_physics_softbody.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_physics_softbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_render.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_scene.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_texture.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_view_layer.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_view_layer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_workspace.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/properties_world.py` & `fake-bpy-module-latest-20230616/bl_ui/properties_world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_clip.py` & `fake-bpy-module-latest-20230616/bl_ui/space_clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_console.py` & `fake-bpy-module-latest-20230616/bl_ui/space_console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_dopesheet.py` & `fake-bpy-module-latest-20230616/bl_ui/space_dopesheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_filebrowser.py` & `fake-bpy-module-latest-20230616/bl_ui/space_filebrowser.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_graph.py` & `fake-bpy-module-latest-20230616/bl_ui/space_graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_image.py` & `fake-bpy-module-latest-20230616/bl_ui/space_image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_info.py` & `fake-bpy-module-latest-20230616/bl_ui/space_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_nla.py` & `fake-bpy-module-latest-20230616/bl_ui/space_nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_node.py` & `fake-bpy-module-latest-20230616/bl_ui/space_node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_outliner.py` & `fake-bpy-module-latest-20230616/bl_ui/space_outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_properties.py` & `fake-bpy-module-latest-20230616/bl_ui/space_properties.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_sequencer.py` & `fake-bpy-module-latest-20230616/bl_ui/space_sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_spreadsheet.py` & `fake-bpy-module-latest-20230616/bl_ui/space_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_statusbar.py` & `fake-bpy-module-latest-20230616/bl_ui/space_statusbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_text.py` & `fake-bpy-module-latest-20230616/bl_ui/space_text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_time.py` & `fake-bpy-module-latest-20230616/bl_ui/space_time.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_toolsystem_common.py` & `fake-bpy-module-latest-20230616/bl_ui/space_toolsystem_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_toolsystem_toolbar.py` & `fake-bpy-module-latest-20230616/bl_ui/space_toolsystem_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_topbar.py` & `fake-bpy-module-latest-20230616/bl_ui/space_topbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_userpref.py` & `fake-bpy-module-latest-20230616/bl_ui/space_userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_view3d.py` & `fake-bpy-module-latest-20230616/bl_ui/space_view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/space_view3d_toolbar.py` & `fake-bpy-module-latest-20230616/bl_ui/space_view3d_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bl_ui/utils.py` & `fake-bpy-module-latest-20230616/bl_ui/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/blf.py` & `fake-bpy-module-latest-20230616/blf.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bmesh/__init__.py` & `fake-bpy-module-latest-20230616/bmesh/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
 import typing
 import bpy.types
 import bmesh.types
 
 from . import geometry
+from . import ops
 from . import types
 from . import utils
-from . import ops
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def from_edit_mesh(mesh: 'bpy.types.Mesh') -> 'bmesh.types.BMesh':
     ''' Return a BMesh from this mesh, currently the mesh must already be in editmode.
```

### Comparing `fake-bpy-module-latest-20230615/bmesh/geometry.py` & `fake-bpy-module-latest-20230616/bmesh/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bmesh/ops.py` & `fake-bpy-module-latest-20230616/bmesh/ops.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bmesh/types.py` & `fake-bpy-module-latest-20230616/bmesh/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bmesh/utils.py` & `fake-bpy-module-latest-20230616/bmesh/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/app/__init__.py` & `fake-bpy-module-latest-20230616/bpy/app/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import typing
-from . import handlers
 from . import translations
 from . import timers
+from . import handlers
 from . import icons
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def help_text(all: typing.Optional[bool] = False):
     ''' Return the help text as a string.
```

### Comparing `fake-bpy-module-latest-20230615/bpy/app/handlers.py` & `fake-bpy-module-latest-20230616/bpy/app/handlers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/app/icons.py` & `fake-bpy-module-latest-20230616/bpy/app/icons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/app/timers.py` & `fake-bpy-module-latest-20230616/bpy/app/timers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/app/translations.py` & `fake-bpy-module-latest-20230616/bpy/app/translations.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/msgbus.py` & `fake-bpy-module-latest-20230616/bpy/msgbus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/__init__.py` & `fake-bpy-module-latest-20230616/bpy/ops/__init__.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 import sys
 import typing
-from . import text
-from . import asset
-from . import rigidbody
-from . import file
-from . import view3d
-from . import action
-from . import workspace
-from . import pose
-from . import curves
-from . import preferences
+from . import view2d
 from . import uilist
+from . import collection
+from . import file
+from . import ptcache
+from . import poselib
+from . import import_curve
+from . import uv
+from . import cachefile
+from . import scene
+from . import wm
+from . import render
+from . import text
+from . import sculpt_curves
 from . import surface
-from . import dpaint
-from . import gizmogroup
-from . import script
-from . import import_scene
+from . import constraint
+from . import buttons
+from . import sequencer
+from . import import_mesh
+from . import import_anim
+from . import console
+from . import outliner
 from . import sound
+from . import world
+from . import curve
+from . import info
+from . import workspace
+from . import anim
+from . import nla
+from . import image
+from . import armature
+from . import view3d
 from . import text_editor
+from . import spreadsheet
+from . import marker
 from . import font
+from . import node
+from . import paintcurve
+from . import import_scene
 from . import lattice
+from . import script
+from . import mball
+from . import screen
 from . import sculpt
-from . import import_anim
-from . import import_mesh
-from . import info
-from . import console
-from . import object
-from . import brush
-from . import gpencil
-from . import texture
-from . import material
-from . import render
-from . import node
-from . import buttons
-from . import paint
-from . import particle
-from . import cloth
-from . import ed
 from . import palette
-from . import sculpt_curves
-from . import ptcache
-from . import fluid
-from . import view2d
-from . import import_curve
-from . import grease_pencil
-from . import graph
-from . import cycles
+from . import clip
 from . import export_mesh
-from . import marker
-from . import paintcurve
+from . import brush
+from . import export_anim
 from . import camera
-from . import uv
-from . import spreadsheet
-from . import nla
-from . import clip
-from . import anim
-from . import outliner
-from . import sequencer
+from . import asset
+from . import gizmogroup
 from . import boid
-from . import mball
-from . import world
-from . import scene
-from . import poselib
-from . import export_anim
-from . import image
-from . import transform
-from . import cachefile
-from . import export_scene
+from . import action
+from . import cycles
+from . import preferences
+from . import geometry
+from . import fluid
+from . import graph
+from . import curves
+from . import material
+from . import object
+from . import dpaint
+from . import gpencil
 from . import ui
-from . import curve
+from . import ed
+from . import cloth
 from . import mesh
-from . import armature
-from . import screen
-from . import collection
-from . import geometry
 from . import mask
-from . import wm
-from . import constraint
+from . import particle
+from . import texture
+from . import export_scene
+from . import transform
+from . import pose
+from . import paint
+from . import grease_pencil
+from . import rigidbody
 
 GenericType = typing.TypeVar("GenericType")
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/action.py` & `fake-bpy-module-latest-20230616/bpy/ops/action.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/anim.py` & `fake-bpy-module-latest-20230616/bpy/ops/anim.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,15 @@
 
 def clear_useless_actions(override_context: typing.
                           Union[typing.Dict, 'bpy.types.Context'] = None,
                           execution_context: typing.Union[str, int] = None,
                           undo: typing.Optional[bool] = None,
                           *,
                           only_unused: typing.Union[bool, typing.Any] = True):
-    ''' Mark actions with no F-Curves for deletion after save and reload of file preserving "action libraries" :File: `startup/bl_operators/anim.py\:322 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/anim.py#L322>`__
+    ''' Mark actions with no F-Curves for deletion after save and reload of file preserving "action libraries" :File: `startup/bl_operators/anim.py\:325 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/anim.py#L325>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param only_unused: Only Unused, Only unused (Fake User only) actions get considered
     :type only_unused: typing.Union[bool, typing.Any]
     '''
@@ -720,15 +720,15 @@
                       execution_context: typing.Union[str, int] = None,
                       undo: typing.Optional[bool] = None,
                       *,
                       filepath: typing.Union[str, typing.Any] = "",
                       filter_folder: typing.Union[bool, typing.Any] = True,
                       filter_text: typing.Union[bool, typing.Any] = True,
                       filter_python: typing.Union[bool, typing.Any] = True):
-    ''' Export Keying Set to a Python script :File: `startup/bl_operators/anim.py\:46 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/anim.py#L46>`__
+    ''' Export Keying Set to a Python script :File: `startup/bl_operators/anim.py\:49 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/anim.py#L49>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     :param filter_folder: Filter folders
@@ -891,15 +891,15 @@
 def update_animated_transform_constraints(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         use_convert_to_radians: typing.Union[bool, typing.Any] = True):
-    ''' Update f-curves/drivers affecting Transform constraints (use it with files from 2.70 and earlier) :File: `startup/bl_operators/anim.py\:358 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/anim.py#L358>`__
+    ''' Update f-curves/drivers affecting Transform constraints (use it with files from 2.70 and earlier) :File: `startup/bl_operators/anim.py\:361 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/anim.py#L361>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param use_convert_to_radians: Use this only once
     :type use_convert_to_radians: typing.Union[bool, typing.Any]
     '''
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/armature.py` & `fake-bpy-module-latest-20230616/bpy/ops/armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/asset.py` & `fake-bpy-module-latest-20230616/bpy/ops/asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 GenericType = typing.TypeVar("GenericType")
 
 
 def assign_action(override_context: typing.
                   Union[typing.Dict, 'bpy.types.Context'] = None,
                   execution_context: typing.Union[str, int] = None,
                   undo: typing.Optional[bool] = None):
-    ''' Set this pose Action as active Action on the active Object :File: `addons/pose_library/operators.py\:196 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L196>`__
+    ''' Set this pose Action as active Action on the active Object :File: `addons/pose_library/operators.py\:198 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L198>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -245,43 +245,43 @@
 
 
 def open_containing_blend_file(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Open the blend file that contains the active asset :File: `startup/bl_operators/assets.py\:94 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/assets.py#L94>`__
+    ''' Open the blend file that contains the active asset :File: `startup/bl_operators/assets.py\:97 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/assets.py#L97>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def tag_add(override_context: typing.Union[typing.
                                            Dict, 'bpy.types.Context'] = None,
             execution_context: typing.Union[str, int] = None,
             undo: typing.Optional[bool] = None):
-    ''' Add a new keyword tag to the active asset :File: `startup/bl_operators/assets.py\:39 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/assets.py#L39>`__
+    ''' Add a new keyword tag to the active asset :File: `startup/bl_operators/assets.py\:42 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/assets.py#L42>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def tag_remove(override_context: typing.
                Union[typing.Dict, 'bpy.types.Context'] = None,
                execution_context: typing.Union[str, int] = None,
                undo: typing.Optional[bool] = None):
-    ''' Remove an existing keyword tag from the active asset :File: `startup/bl_operators/assets.py\:62 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/assets.py#L62>`__
+    ''' Remove an existing keyword tag from the active asset :File: `startup/bl_operators/assets.py\:65 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/assets.py#L65>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/boid.py` & `fake-bpy-module-latest-20230616/bpy/ops/boid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/brush.py` & `fake-bpy-module-latest-20230616/bpy/ops/brush.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/buttons.py` & `fake-bpy-module-latest-20230616/bpy/ops/buttons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/cachefile.py` & `fake-bpy-module-latest-20230616/bpy/ops/cachefile.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/camera.py` & `fake-bpy-module-latest-20230616/bpy/ops/camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
                execution_context: typing.Union[str, int] = None,
                undo: typing.Optional[bool] = None,
                *,
                name: typing.Union[str, typing.Any] = "",
                remove_name: typing.Union[bool, typing.Any] = False,
                remove_active: typing.Union[bool, typing.Any] = False,
                use_focal_length: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove a Camera Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove a Camera Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
@@ -37,15 +37,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         name: typing.Union[str, typing.Any] = "",
         remove_name: typing.Union[bool, typing.Any] = False,
         remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove a Safe Areas Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove a Safe Areas Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/clip.py` & `fake-bpy-module-latest-20230616/bpy/ops/clip.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     pass
 
 
 def bundles_to_mesh(override_context: typing.
                     Union[typing.Dict, 'bpy.types.Context'] = None,
                     execution_context: typing.Union[str, int] = None,
                     undo: typing.Optional[bool] = None):
-    ''' Create vertex cloud using coordinates of reconstructed tracks :File: `startup/bl_operators/clip.py\:281 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L281>`__
+    ''' Create vertex cloud using coordinates of reconstructed tracks :File: `startup/bl_operators/clip.py\:284 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L284>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -137,15 +137,15 @@
                       execution_context: typing.Union[str, int] = None,
                       undo: typing.Optional[bool] = None,
                       *,
                       name: typing.Union[str, typing.Any] = "",
                       remove_name: typing.Union[bool, typing.Any] = False,
                       remove_active: typing.Union[bool, typing.Any] = False,
                       use_focal_length: typing.Union[bool, typing.Any] = True):
-    ''' Add or remove a Tracking Camera Intrinsics Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove a Tracking Camera Intrinsics Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
@@ -236,15 +236,15 @@
     pass
 
 
 def constraint_to_fcurve(override_context: typing.
                          Union[typing.Dict, 'bpy.types.Context'] = None,
                          execution_context: typing.Union[str, int] = None,
                          undo: typing.Optional[bool] = None):
-    ''' Create F-Curves for object which will copy object's movement caused by this constraint :File: `startup/bl_operators/clip.py\:521 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L521>`__
+    ''' Create F-Curves for object which will copy object's movement caused by this constraint :File: `startup/bl_operators/clip.py\:524 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L524>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -314,15 +314,15 @@
     pass
 
 
 def delete_proxy(override_context: typing.
                  Union[typing.Dict, 'bpy.types.Context'] = None,
                  execution_context: typing.Union[str, int] = None,
                  undo: typing.Optional[bool] = None):
-    ''' Delete movie clip proxy files from the hard drive :File: `startup/bl_operators/clip.py\:348 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L348>`__
+    ''' Delete movie clip proxy files from the hard drive :File: `startup/bl_operators/clip.py\:351 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L351>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -429,15 +429,15 @@
 
 def filter_tracks(override_context: typing.
                   Union[typing.Dict, 'bpy.types.Context'] = None,
                   execution_context: typing.Union[str, int] = None,
                   undo: typing.Optional[bool] = None,
                   *,
                   track_threshold: typing.Optional[typing.Any] = 5.0):
-    ''' Filter tracks which has weirdly looking spikes in motion curves :File: `startup/bl_operators/clip.py\:195 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L195>`__
+    ''' Filter tracks which has weirdly looking spikes in motion curves :File: `startup/bl_operators/clip.py\:198 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L198>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param track_threshold: Track Threshold, Filter Threshold to select problematic tracks
     :type track_threshold: typing.Optional[typing.Any]
     '''
@@ -1072,15 +1072,15 @@
     pass
 
 
 def set_active_clip(override_context: typing.
                     Union[typing.Dict, 'bpy.types.Context'] = None,
                     execution_context: typing.Union[str, int] = None,
                     undo: typing.Optional[bool] = None):
-    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/clip.py\:210 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L210>`__
+    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/clip.py\:213 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L213>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1208,29 +1208,29 @@
     pass
 
 
 def set_viewport_background(override_context: typing.
                             Union[typing.Dict, 'bpy.types.Context'] = None,
                             execution_context: typing.Union[str, int] = None,
                             undo: typing.Optional[bool] = None):
-    ''' Set current movie clip as a camera background in 3D Viewport (works only when a 3D Viewport is visible) :File: `startup/bl_operators/clip.py\:409 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L409>`__
+    ''' Set current movie clip as a camera background in 3D Viewport (works only when a 3D Viewport is visible) :File: `startup/bl_operators/clip.py\:412 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L412>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def setup_tracking_scene(override_context: typing.
                          Union[typing.Dict, 'bpy.types.Context'] = None,
                          execution_context: typing.Union[str, int] = None,
                          undo: typing.Optional[bool] = None):
-    ''' Prepare scene for compositing 3D objects into this footage :File: `startup/bl_operators/clip.py\:971 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L971>`__
+    ''' Prepare scene for compositing 3D objects into this footage :File: `startup/bl_operators/clip.py\:974 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L974>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1373,15 +1373,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         name: typing.Union[str, typing.Any] = "",
         remove_name: typing.Union[bool, typing.Any] = False,
         remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove a Clip Track Color Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove a Clip Track Color Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
@@ -1428,43 +1428,43 @@
     pass
 
 
 def track_settings_as_default(override_context: typing.
                               Union[typing.Dict, 'bpy.types.Context'] = None,
                               execution_context: typing.Union[str, int] = None,
                               undo: typing.Optional[bool] = None):
-    ''' Copy tracking settings from active track to default settings :File: `startup/bl_operators/clip.py\:1000 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L1000>`__
+    ''' Copy tracking settings from active track to default settings :File: `startup/bl_operators/clip.py\:1003 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L1003>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def track_settings_to_track(override_context: typing.
                             Union[typing.Dict, 'bpy.types.Context'] = None,
                             execution_context: typing.Union[str, int] = None,
                             undo: typing.Optional[bool] = None):
-    ''' Copy tracking settings from active track to selected tracks :File: `startup/bl_operators/clip.py\:1049 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L1049>`__
+    ''' Copy tracking settings from active track to selected tracks :File: `startup/bl_operators/clip.py\:1052 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L1052>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def track_to_empty(override_context: typing.
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None):
-    ''' Create an Empty object which will be copying movement of active track :File: `startup/bl_operators/clip.py\:257 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L257>`__
+    ''' Create an Empty object which will be copying movement of active track :File: `startup/bl_operators/clip.py\:260 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/clip.py#L260>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1503,15 +1503,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         name: typing.Union[str, typing.Any] = "",
         remove_name: typing.Union[bool, typing.Any] = False,
         remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove a motion tracking settings preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove a motion tracking settings preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/cloth.py` & `fake-bpy-module-latest-20230616/bpy/ops/text_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                Union[typing.Dict, 'bpy.types.Context'] = None,
                execution_context: typing.Union[str, int] = None,
                undo: typing.Optional[bool] = None,
                *,
                name: typing.Union[str, typing.Any] = "",
                remove_name: typing.Union[bool, typing.Any] = False,
                remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove a Cloth Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove a Text Editor Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/collection.py` & `fake-bpy-module-latest-20230616/bpy/ops/collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/console.py` & `fake-bpy-module-latest-20230616/bpy/ops/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 GenericType = typing.TypeVar("GenericType")
 
 
 def autocomplete(override_context: typing.
                  Union[typing.Dict, 'bpy.types.Context'] = None,
                  execution_context: typing.Union[str, int] = None,
                  undo: typing.Optional[bool] = None):
-    ''' Evaluate the namespace up until the cursor and give a list of options or complete the name if there is only one :File: `startup/bl_operators/console.py\:56 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/console.py#L56>`__
+    ''' Evaluate the namespace up until the cursor and give a list of options or complete the name if there is only one :File: `startup/bl_operators/console.py\:59 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/console.py#L59>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def banner(override_context: typing.Union[typing.
                                           Dict, 'bpy.types.Context'] = None,
            execution_context: typing.Union[str, int] = None,
            undo: typing.Optional[bool] = None):
-    ''' Print a message when the terminal initializes :File: `startup/bl_operators/console.py\:101 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/console.py#L101>`__
+    ''' Print a message when the terminal initializes :File: `startup/bl_operators/console.py\:104 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/console.py#L104>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -82,15 +82,15 @@
     pass
 
 
 def copy_as_script(override_context: typing.
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None):
-    ''' Copy the console contents for use in a script :File: `startup/bl_operators/console.py\:78 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/console.py#L78>`__
+    ''' Copy the console contents for use in a script :File: `startup/bl_operators/console.py\:81 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/console.py#L81>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -116,15 +116,15 @@
 
 def execute(override_context: typing.Union[typing.
                                            Dict, 'bpy.types.Context'] = None,
             execution_context: typing.Union[str, int] = None,
             undo: typing.Optional[bool] = None,
             *,
             interactive: typing.Union[bool, typing.Any] = False):
-    ''' Execute the current console line as a Python expression :File: `startup/bl_operators/console.py\:32 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/console.py#L32>`__
+    ''' Execute the current console line as a Python expression :File: `startup/bl_operators/console.py\:35 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/console.py#L35>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param interactive: interactive
     :type interactive: typing.Union[bool, typing.Any]
     '''
@@ -222,15 +222,15 @@
 
 def language(override_context: typing.Union[typing.
                                             Dict, 'bpy.types.Context'] = None,
              execution_context: typing.Union[str, int] = None,
              undo: typing.Optional[bool] = None,
              *,
              language: typing.Union[str, typing.Any] = ""):
-    ''' Set the current language for this console :File: `startup/bl_operators/console.py\:133 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/console.py#L133>`__
+    ''' Set the current language for this console :File: `startup/bl_operators/console.py\:136 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/console.py#L136>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param language: Language
     :type language: typing.Union[str, typing.Any]
     '''
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/constraint.py` & `fake-bpy-module-latest-20230616/bpy/ops/constraint.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 GenericType = typing.TypeVar("GenericType")
 
 
 def add_target(override_context: typing.
                Union[typing.Dict, 'bpy.types.Context'] = None,
                execution_context: typing.Union[str, int] = None,
                undo: typing.Optional[bool] = None):
-    ''' Add a target to the constraint :File: `startup/bl_operators/constraint.py\:23 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/constraint.py#L23>`__
+    ''' Add a target to the constraint :File: `startup/bl_operators/constraint.py\:26 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/constraint.py#L26>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -154,15 +154,15 @@
     pass
 
 
 def disable_keep_transform(override_context: typing.
                            Union[typing.Dict, 'bpy.types.Context'] = None,
                            execution_context: typing.Union[str, int] = None,
                            undo: typing.Optional[bool] = None):
-    ''' Set the influence of this constraint to zero while trying to maintain the object's transformation. Other active constraints can still influence the final transformation :File: `startup/bl_operators/constraint.py\:83 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/constraint.py#L83>`__
+    ''' Set the influence of this constraint to zero while trying to maintain the object's transformation. Other active constraints can still influence the final transformation :File: `startup/bl_operators/constraint.py\:86 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/constraint.py#L86>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -282,15 +282,15 @@
     pass
 
 
 def normalize_target_weights(override_context: typing.
                              Union[typing.Dict, 'bpy.types.Context'] = None,
                              execution_context: typing.Union[str, int] = None,
                              undo: typing.Optional[bool] = None):
-    ''' Normalize weights of all target bones :File: `startup/bl_operators/constraint.py\:58 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/constraint.py#L58>`__
+    ''' Normalize weights of all target bones :File: `startup/bl_operators/constraint.py\:61 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/constraint.py#L61>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -341,15 +341,15 @@
 
 def remove_target(override_context: typing.
                   Union[typing.Dict, 'bpy.types.Context'] = None,
                   execution_context: typing.Union[str, int] = None,
                   undo: typing.Optional[bool] = None,
                   *,
                   index: typing.Optional[typing.Any] = 0):
-    ''' Remove the target from the constraint :File: `startup/bl_operators/constraint.py\:41 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/constraint.py#L41>`__
+    ''' Remove the target from the constraint :File: `startup/bl_operators/constraint.py\:44 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/constraint.py#L44>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param index: index
     :type index: typing.Optional[typing.Any]
     '''
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/curve.py` & `fake-bpy-module-latest-20230616/bpy/ops/curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/curves.py` & `fake-bpy-module-latest-20230616/bpy/ops/curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/cycles.py` & `fake-bpy-module-latest-20230616/bpy/ops/cycles.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/dpaint.py` & `fake-bpy-module-latest-20230616/bpy/ops/dpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/ed.py` & `fake-bpy-module-latest-20230616/bpy/ops/ed.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/export_anim.py` & `fake-bpy-module-latest-20230616/bpy/ops/export_anim.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         check_existing: typing.Union[bool, typing.Any] = True,
         filter_glob: typing.Union[str, typing.Any] = "*.bvh",
         global_scale: typing.Optional[typing.Any] = 1.0,
         frame_start: typing.Optional[typing.Any] = 0,
         frame_end: typing.Optional[typing.Any] = 0,
         rotate_mode: typing.Optional[typing.Any] = 'NATIVE',
         root_transform_only: typing.Union[bool, typing.Any] = False):
-    ''' Save a BVH motion capture file from an armature :File: `addons/io_anim_bvh/__init__.py\:278 <https://projects.blender.org/blender/blender-addons/addons/io_anim_bvh/__init__.py#L278>`__
+    ''' Save a BVH motion capture file from an armature :File: `addons/io_anim_bvh/__init__.py\:280 <https://projects.blender.org/blender/blender-addons/addons/io_anim_bvh/__init__.py#L280>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: File Path, Filepath used for exporting the file
     :type filepath: typing.Union[str, typing.Any]
     :param check_existing: Check Existing, Check and warn on overwriting existing files
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/export_mesh.py` & `fake-bpy-module-latest-20230616/bpy/ops/export_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         global_space: typing.Optional[typing.Any] = ((0.0, 0.0, 0.0, 0.0),
                                                      (0.0, 0.0, 0.0,
                                                       0.0), (0.0, 0.0, 0.0,
                                                              0.0), (0.0, 0.0,
                                                                     0.0, 0.0)),
         axis_forward: typing.Optional[typing.Any] = 'Y',
         axis_up: typing.Optional[typing.Any] = 'Z'):
-    ''' Save STL triangle mesh data :File: `addons/io_mesh_stl/__init__.py\:240 <https://projects.blender.org/blender/blender-addons/addons/io_mesh_stl/__init__.py#L240>`__
+    ''' Save STL triangle mesh data :File: `addons/io_mesh_stl/__init__.py\:242 <https://projects.blender.org/blender/blender-addons/addons/io_mesh_stl/__init__.py#L242>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: File Path, Filepath used for exporting the file
     :type filepath: typing.Union[str, typing.Any]
     :param check_existing: Check Existing, Check and warn on overwriting existing files
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/export_scene.py` & `fake-bpy-module-latest-20230616/bpy/ops/export_scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         path_mode: typing.Optional[typing.Any] = 'AUTO',
         embed_textures: typing.Union[bool, typing.Any] = False,
         batch_mode: typing.Optional[typing.Any] = 'OFF',
         use_batch_own_dir: typing.Union[bool, typing.Any] = True,
         use_metadata: typing.Union[bool, typing.Any] = True,
         axis_forward: typing.Optional[typing.Any] = '-Z',
         axis_up: typing.Optional[typing.Any] = 'Y'):
-    ''' Write a FBX file :File: `addons/io_scene_fbx/__init__.py\:643 <https://projects.blender.org/blender/blender-addons/addons/io_scene_fbx/__init__.py#L643>`__
+    ''' Write a FBX file :File: `addons/io_scene_fbx/__init__.py\:645 <https://projects.blender.org/blender/blender-addons/addons/io_scene_fbx/__init__.py#L645>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: File Path, Filepath used for exporting the file
     :type filepath: typing.Union[str, typing.Any]
     :param check_existing: Check Existing, Check and warn on overwriting existing files
@@ -220,15 +220,15 @@
         export_morph_tangent: typing.Union[bool, typing.Any] = False,
         export_morph_animation: typing.Union[bool, typing.Any] = True,
         export_morph_reset_sk_data: typing.Union[bool, typing.Any] = True,
         export_lights: typing.Union[bool, typing.Any] = False,
         export_nla_strips: typing.Union[bool, typing.Any] = True,
         will_save_settings: typing.Union[bool, typing.Any] = False,
         filter_glob: typing.Union[str, typing.Any] = "*.glb"):
-    ''' Export scene as glTF 2.0 file :File: `addons/io_scene_gltf2/__init__.py\:694 <https://projects.blender.org/blender/blender-addons/addons/io_scene_gltf2/__init__.py#L694>`__
+    ''' Export scene as glTF 2.0 file :File: `addons/io_scene_gltf2/__init__.py\:695 <https://projects.blender.org/blender/blender-addons/addons/io_scene_gltf2/__init__.py#L695>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: File Path, Filepath used for exporting the file
     :type filepath: typing.Union[str, typing.Any]
     :param check_existing: Check Existing, Check and warn on overwriting existing files
@@ -384,15 +384,15 @@
         use_hierarchy: typing.Union[bool, typing.Any] = True,
         name_decorations: typing.Union[bool, typing.Any] = True,
         use_h3d: typing.Union[bool, typing.Any] = False,
         global_scale: typing.Optional[typing.Any] = 1.0,
         path_mode: typing.Optional[typing.Any] = 'AUTO',
         axis_forward: typing.Optional[typing.Any] = 'Z',
         axis_up: typing.Optional[typing.Any] = 'Y'):
-    ''' Export selection to Extensible 3D file (.x3d) :File: `addons/io_scene_x3d/__init__.py\:206 <https://projects.blender.org/blender/blender-addons/addons/io_scene_x3d/__init__.py#L206>`__
+    ''' Export selection to Extensible 3D file (.x3d) :File: `addons/io_scene_x3d/__init__.py\:208 <https://projects.blender.org/blender/blender-addons/addons/io_scene_x3d/__init__.py#L208>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: File Path, Filepath used for exporting the file
     :type filepath: typing.Union[str, typing.Any]
     :param check_existing: Check Existing, Check and warn on overwriting existing files
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/file.py` & `fake-bpy-module-latest-20230616/bpy/ops/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/fluid.py` & `fake-bpy-module-latest-20230616/bpy/ops/fluid.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                Union[typing.Dict, 'bpy.types.Context'] = None,
                execution_context: typing.Union[str, int] = None,
                undo: typing.Optional[bool] = None,
                *,
                name: typing.Union[str, typing.Any] = "",
                remove_name: typing.Union[bool, typing.Any] = False,
                remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove a Fluid Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove a Fluid Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/font.py` & `fake-bpy-module-latest-20230616/bpy/ops/font.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/geometry.py` & `fake-bpy-module-latest-20230616/bpy/ops/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/gizmogroup.py` & `fake-bpy-module-latest-20230616/bpy/ops/gizmogroup.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/gpencil.py` & `fake-bpy-module-latest-20230616/bpy/ops/gpencil.py`

 * *Files 0% similar despite different names*

```diff
@@ -2628,15 +2628,15 @@
     pass
 
 
 def tint_flip(override_context: typing.Union[typing.
                                              Dict, 'bpy.types.Context'] = None,
               execution_context: typing.Union[str, int] = None,
               undo: typing.Optional[bool] = None):
-    ''' Switch tint colors :File: `startup/bl_ui/properties_grease_pencil_common.py\:876 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_ui/properties_grease_pencil_common.py#L876>`__
+    ''' Switch tint colors :File: `startup/bl_ui/properties_grease_pencil_common.py\:878 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_ui/properties_grease_pencil_common.py#L878>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/graph.py` & `fake-bpy-module-latest-20230616/bpy/ops/graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/grease_pencil.py` & `fake-bpy-module-latest-20230616/bpy/ops/grease_pencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/image.py` & `fake-bpy-module-latest-20230616/bpy/ops/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
 def external_edit(override_context: typing.
                   Union[typing.Dict, 'bpy.types.Context'] = None,
                   execution_context: typing.Union[str, int] = None,
                   undo: typing.Optional[bool] = None,
                   *,
                   filepath: typing.Union[str, typing.Any] = ""):
-    ''' Edit image in an external application :File: `startup/bl_operators/image.py\:44 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/image.py#L44>`__
+    ''' Edit image in an external application :File: `startup/bl_operators/image.py\:46 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/image.py#L46>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     '''
@@ -470,29 +470,29 @@
     pass
 
 
 def project_apply(override_context: typing.
                   Union[typing.Dict, 'bpy.types.Context'] = None,
                   execution_context: typing.Union[str, int] = None,
                   undo: typing.Optional[bool] = None):
-    ''' Project edited image back onto the object :File: `startup/bl_operators/image.py\:179 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/image.py#L179>`__
+    ''' Project edited image back onto the object :File: `startup/bl_operators/image.py\:181 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/image.py#L181>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def project_edit(override_context: typing.
                  Union[typing.Dict, 'bpy.types.Context'] = None,
                  execution_context: typing.Union[str, int] = None,
                  undo: typing.Optional[bool] = None):
-    ''' Edit a snapshot of the 3D Viewport in an external image editor :File: `startup/bl_operators/image.py\:109 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/image.py#L109>`__
+    ''' Edit a snapshot of the 3D Viewport in an external image editor :File: `startup/bl_operators/image.py\:111 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/image.py#L111>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/import_anim.py` & `fake-bpy-module-latest-20230616/bpy/ops/import_anim.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         use_fps_scale: typing.Union[bool, typing.Any] = False,
         update_scene_fps: typing.Union[bool, typing.Any] = False,
         update_scene_duration: typing.Union[bool, typing.Any] = False,
         use_cyclic: typing.Union[bool, typing.Any] = False,
         rotate_mode: typing.Optional[typing.Any] = 'NATIVE',
         axis_forward: typing.Optional[typing.Any] = '-Z',
         axis_up: typing.Optional[typing.Any] = 'Y'):
-    ''' Load a BVH motion capture file :File: `addons/io_anim_bvh/__init__.py\:114 <https://projects.blender.org/blender/blender-addons/addons/io_anim_bvh/__init__.py#L114>`__
+    ''' Load a BVH motion capture file :File: `addons/io_anim_bvh/__init__.py\:116 <https://projects.blender.org/blender/blender-addons/addons/io_anim_bvh/__init__.py#L116>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: File Path, Filepath used for importing the file
     :type filepath: typing.Union[str, typing.Any]
     :param filter_glob: filter_glob
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/import_curve.py` & `fake-bpy-module-latest-20230616/bpy/ops/import_curve.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def svg(override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         filepath: typing.Union[str, typing.Any] = "",
         filter_glob: typing.Union[str, typing.Any] = "*.svg"):
-    ''' Load a SVG file :File: `addons/io_curve_svg/__init__.py\:38 <https://projects.blender.org/blender/blender-addons/addons/io_curve_svg/__init__.py#L38>`__
+    ''' Load a SVG file :File: `addons/io_curve_svg/__init__.py\:40 <https://projects.blender.org/blender/blender-addons/addons/io_curve_svg/__init__.py#L40>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: File Path, Filepath used for importing the file
     :type filepath: typing.Union[str, typing.Any]
     :param filter_glob: filter_glob
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/import_mesh.py` & `fake-bpy-module-latest-20230616/bpy/ops/import_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             'bpy.types.OperatorFileListElement']] = None,
         directory: typing.Union[str, typing.Any] = "",
         global_scale: typing.Optional[typing.Any] = 1.0,
         use_scene_unit: typing.Union[bool, typing.Any] = False,
         use_facet_normal: typing.Union[bool, typing.Any] = False,
         axis_forward: typing.Optional[typing.Any] = 'Y',
         axis_up: typing.Optional[typing.Any] = 'Z'):
-    ''' Load STL triangle mesh data :File: `addons/io_mesh_stl/__init__.py\:95 <https://projects.blender.org/blender/blender-addons/addons/io_mesh_stl/__init__.py#L95>`__
+    ''' Load STL triangle mesh data :File: `addons/io_mesh_stl/__init__.py\:97 <https://projects.blender.org/blender/blender-addons/addons/io_mesh_stl/__init__.py#L97>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: File Path, Filepath used for importing the file
     :type filepath: typing.Union[str, typing.Any]
     :param filter_glob: filter_glob
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/import_scene.py` & `fake-bpy-module-latest-20230616/bpy/ops/import_scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         force_connect_children: typing.Union[bool, typing.Any] = False,
         automatic_bone_orientation: typing.Union[bool, typing.Any] = False,
         primary_bone_axis: typing.Optional[typing.Any] = 'Y',
         secondary_bone_axis: typing.Optional[typing.Any] = 'X',
         use_prepost_rot: typing.Union[bool, typing.Any] = True,
         axis_forward: typing.Optional[typing.Any] = '-Z',
         axis_up: typing.Optional[typing.Any] = 'Y'):
-    ''' Load a FBX file :File: `addons/io_scene_fbx/__init__.py\:196 <https://projects.blender.org/blender/blender-addons/addons/io_scene_fbx/__init__.py#L196>`__
+    ''' Load a FBX file :File: `addons/io_scene_fbx/__init__.py\:198 <https://projects.blender.org/blender/blender-addons/addons/io_scene_fbx/__init__.py#L198>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: File Path, Filepath used for importing the file
     :type filepath: typing.Union[str, typing.Any]
     :param directory: directory
@@ -112,15 +112,15 @@
              'bpy.types.OperatorFileListElement']] = None,
          loglevel: typing.Optional[typing.Any] = 0,
          import_pack_images: typing.Union[bool, typing.Any] = True,
          merge_vertices: typing.Union[bool, typing.Any] = False,
          import_shading: typing.Optional[typing.Any] = 'NORMALS',
          bone_heuristic: typing.Optional[typing.Any] = 'TEMPERANCE',
          guess_original_bind_pose: typing.Union[bool, typing.Any] = True):
-    ''' Load a glTF 2.0 file :File: `addons/io_scene_gltf2/__init__.py\:1596 <https://projects.blender.org/blender/blender-addons/addons/io_scene_gltf2/__init__.py#L1596>`__
+    ''' Load a glTF 2.0 file :File: `addons/io_scene_gltf2/__init__.py\:1597 <https://projects.blender.org/blender/blender-addons/addons/io_scene_gltf2/__init__.py#L1597>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: File Path, Filepath used for importing the file
     :type filepath: typing.Union[str, typing.Any]
     :param export_import_convert_lighting_mode: Lighting Mode, Optional backwards compatibility for non-standard render engines. Applies to lights * ``SPEC`` Standard -- Physically-based glTF lighting units (cd, lx, nt). * ``COMPAT`` Unitless -- Non-physical, unitless lighting. Useful when exposure controls are not available. * ``RAW`` Raw (Deprecated) -- Blender lighting strengths with no conversion.
@@ -151,15 +151,15 @@
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         filepath: typing.Union[str, typing.Any] = "",
         filter_glob: typing.Union[str, typing.Any] = "*.x3d;*.wrl",
         axis_forward: typing.Optional[typing.Any] = 'Z',
         axis_up: typing.Optional[typing.Any] = 'Y'):
-    ''' Import an X3D or VRML2 file :File: `addons/io_scene_x3d/__init__.py\:48 <https://projects.blender.org/blender/blender-addons/addons/io_scene_x3d/__init__.py#L48>`__
+    ''' Import an X3D or VRML2 file :File: `addons/io_scene_x3d/__init__.py\:50 <https://projects.blender.org/blender/blender-addons/addons/io_scene_x3d/__init__.py#L50>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: File Path, Filepath used for importing the file
     :type filepath: typing.Union[str, typing.Any]
     :param filter_glob: filter_glob
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/info.py` & `fake-bpy-module-latest-20230616/bpy/ops/info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/lattice.py` & `fake-bpy-module-latest-20230616/bpy/ops/lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/marker.py` & `fake-bpy-module-latest-20230616/bpy/ops/marker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/mask.py` & `fake-bpy-module-latest-20230616/bpy/ops/mask.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/material.py` & `fake-bpy-module-latest-20230616/bpy/ops/material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/mball.py` & `fake-bpy-module-latest-20230616/bpy/ops/mball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/mesh.py` & `fake-bpy-module-latest-20230616/bpy/ops/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1175,15 +1175,15 @@
 def faces_mirror_uv(override_context: typing.
                     Union[typing.Dict, 'bpy.types.Context'] = None,
                     execution_context: typing.Union[str, int] = None,
                     undo: typing.Optional[bool] = None,
                     *,
                     direction: typing.Optional[typing.Any] = 'POSITIVE',
                     precision: typing.Optional[typing.Any] = 3):
-    ''' Copy mirror UV coordinates on the X axis based on a mirrored mesh :File: `startup/bl_operators/mesh.py\:130 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/mesh.py#L130>`__
+    ''' Copy mirror UV coordinates on the X axis based on a mirrored mesh :File: `startup/bl_operators/mesh.py\:132 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/mesh.py#L132>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param direction: Axis Direction
     :type direction: typing.Optional[typing.Any]
     :param precision: Precision, Tolerance for finding vertex duplicates
@@ -2615,15 +2615,15 @@
         minor_segments: typing.Optional[typing.Any] = 12,
         mode: typing.Optional[typing.Any] = 'MAJOR_MINOR',
         major_radius: typing.Optional[typing.Any] = 1.0,
         minor_radius: typing.Optional[typing.Any] = 0.25,
         abso_major_rad: typing.Optional[typing.Any] = 1.25,
         abso_minor_rad: typing.Optional[typing.Any] = 0.75,
         generate_uvs: typing.Union[bool, typing.Any] = True):
-    ''' Construct a torus mesh :File: `startup/bl_operators/add_mesh_torus.py\:220 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/add_mesh_torus.py#L220>`__
+    ''' Construct a torus mesh :File: `startup/bl_operators/add_mesh_torus.py\:223 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/add_mesh_torus.py#L223>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param align: Align * ``WORLD`` World -- Align the new object to the world. * ``VIEW`` View -- Align the new object to the view. * ``CURSOR`` 3D Cursor -- Use the 3D cursor orientation for the new object.
     :type align: typing.Optional[typing.Any]
     :param location: Location
@@ -3153,15 +3153,15 @@
     pass
 
 
 def select_next_item(override_context: typing.
                      Union[typing.Dict, 'bpy.types.Context'] = None,
                      execution_context: typing.Union[str, int] = None,
                      undo: typing.Optional[bool] = None):
-    ''' Select the next element (using selection order) :File: `startup/bl_operators/mesh.py\:195 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/mesh.py#L195>`__
+    ''' Select the next element (using selection order) :File: `startup/bl_operators/mesh.py\:197 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/mesh.py#L197>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -3225,15 +3225,15 @@
     pass
 
 
 def select_prev_item(override_context: typing.
                      Union[typing.Dict, 'bpy.types.Context'] = None,
                      execution_context: typing.Union[str, int] = None,
                      undo: typing.Optional[bool] = None):
-    ''' Select the previous element (using selection order) :File: `startup/bl_operators/mesh.py\:220 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/mesh.py#L220>`__
+    ''' Select the previous element (using selection order) :File: `startup/bl_operators/mesh.py\:222 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/mesh.py#L222>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/nla.py` & `fake-bpy-module-latest-20230616/bpy/ops/nla.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
          only_selected: typing.Union[bool, typing.Any] = True,
          visual_keying: typing.Union[bool, typing.Any] = False,
          clear_constraints: typing.Union[bool, typing.Any] = False,
          clear_parents: typing.Union[bool, typing.Any] = False,
          use_current_action: typing.Union[bool, typing.Any] = False,
          clean_curves: typing.Union[bool, typing.Any] = False,
          bake_types: typing.Optional[typing.Any] = {'POSE'}):
-    ''' Bake all selected objects location/scale/rotation animation to an action :File: `startup/bl_operators/anim.py\:253 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/anim.py#L253>`__
+    ''' Bake all selected objects location/scale/rotation animation to an action :File: `startup/bl_operators/anim.py\:256 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/anim.py#L256>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param frame_start: Start Frame, Start frame for baking
     :type frame_start: typing.Optional[typing.Any]
     :param frame_end: End Frame, End frame for baking
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/node.py` & `fake-bpy-module-latest-20230616/bpy/ops/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
              execution_context: typing.Union[str, int] = None,
              undo: typing.Optional[bool] = None,
              *,
              use_transform: typing.Union[bool, typing.Any] = False,
              settings: typing.Optional[bpy.types.bpy_prop_collection[
                  'bl_operators.node.NodeSetting']] = None,
              type: typing.Union[str, typing.Any] = ""):
-    ''' Add a node to the active tree :File: `startup/bl_operators/node.py\:136 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L136>`__
+    ''' Add a node to the active tree :File: `startup/bl_operators/node.py\:139 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L139>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param use_transform: Use Transform, Start transform operator after inserting the node
     :type use_transform: typing.Union[bool, typing.Any]
     :param settings: Settings, Settings to be applied on the newly created node
@@ -275,15 +275,15 @@
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         use_transform: typing.Union[bool, typing.Any] = False,
         settings: typing.Optional[bpy.types.bpy_prop_collection[
             'bl_operators.node.NodeSetting']] = None,
         offset: typing.Optional[typing.Any] = (150.0, 0.0)):
-    ''' Add simulation zone input and output nodes to the active tree :File: `startup/bl_operators/node.py\:169 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L169>`__
+    ''' Add simulation zone input and output nodes to the active tree :File: `startup/bl_operators/node.py\:172 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L172>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param use_transform: Use Transform, Start transform operator after inserting the node
     :type use_transform: typing.Union[bool, typing.Any]
     :param settings: Settings, Settings to be applied on the newly created node
@@ -416,15 +416,15 @@
 
 
 def collapse_hide_unused_toggle(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Toggle collapsed nodes and hide unused sockets :File: `startup/bl_operators/node.py\:209 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L209>`__
+    ''' Toggle collapsed nodes and hide unused sockets :File: `startup/bl_operators/node.py\:212 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L212>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -641,15 +641,15 @@
 
 
 def gltf_settings_node_operator(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Add a node to the active tree for glTF export :File: `addons/io_scene_gltf2/blender/com/gltf2_blender_ui.py\:32 <https://projects.blender.org/blender/blender-addons/addons/io_scene_gltf2/blender/com/gltf2_blender_ui.py#L32>`__
+    ''' Add a node to the active tree for glTF export :File: `addons/io_scene_gltf2/blender/com/gltf2_blender_ui.py\:33 <https://projects.blender.org/blender/blender-addons/addons/io_scene_gltf2/blender/com/gltf2_blender_ui.py#L33>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -978,30 +978,30 @@
 
 
 def new_geometry_node_group_assign(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Create a new geometry node group and assign it to the active modifier :File: `startup/bl_operators/geometry_nodes.py\:237 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L237>`__
+    ''' Create a new geometry node group and assign it to the active modifier :File: `startup/bl_operators/geometry_nodes.py\:239 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L239>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def new_geometry_nodes_modifier(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Create a new modifier with a new geometry node group :File: `startup/bl_operators/geometry_nodes.py\:214 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L214>`__
+    ''' Create a new modifier with a new geometry node group :File: `startup/bl_operators/geometry_nodes.py\:216 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L216>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1033,15 +1033,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         name: typing.Union[str, typing.Any] = "",
         remove_name: typing.Union[bool, typing.Any] = False,
         remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove a Node Color Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove a Node Color Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
@@ -1133,15 +1133,15 @@
     pass
 
 
 def panel_add(override_context: typing.Union[typing.
                                              Dict, 'bpy.types.Context'] = None,
               execution_context: typing.Union[str, int] = None,
               undo: typing.Optional[bool] = None):
-    ''' Add a new panel to the tree :File: `startup/bl_operators/node.py\:267 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L267>`__
+    ''' Add a new panel to the tree :File: `startup/bl_operators/node.py\:270 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L270>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1149,15 +1149,15 @@
 
 def panel_move(override_context: typing.
                Union[typing.Dict, 'bpy.types.Context'] = None,
                execution_context: typing.Union[str, int] = None,
                undo: typing.Optional[bool] = None,
                *,
                direction: typing.Optional[typing.Any] = 'UP'):
-    ''' Move a panel to another position :File: `startup/bl_operators/node.py\:311 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L311>`__
+    ''' Move a panel to another position :File: `startup/bl_operators/node.py\:314 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L314>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param direction: Direction
     :type direction: typing.Optional[typing.Any]
     '''
@@ -1165,15 +1165,15 @@
     pass
 
 
 def panel_remove(override_context: typing.
                  Union[typing.Dict, 'bpy.types.Context'] = None,
                  execution_context: typing.Union[str, int] = None,
                  undo: typing.Optional[bool] = None):
-    ''' Remove a panel from the tree :File: `startup/bl_operators/node.py\:287 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L287>`__
+    ''' Remove a panel from the tree :File: `startup/bl_operators/node.py\:290 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L290>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1500,15 +1500,15 @@
     pass
 
 
 def simulation_zone_item_add(override_context: typing.
                              Union[typing.Dict, 'bpy.types.Context'] = None,
                              execution_context: typing.Union[str, int] = None,
                              undo: typing.Optional[bool] = None):
-    ''' Add a state item to the simulation zone :File: `startup/bl_operators/geometry_nodes.py\:282 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L282>`__
+    ''' Add a state item to the simulation zone :File: `startup/bl_operators/geometry_nodes.py\:284 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L284>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1516,15 +1516,15 @@
 
 def simulation_zone_item_move(override_context: typing.
                               Union[typing.Dict, 'bpy.types.Context'] = None,
                               execution_context: typing.Union[str, int] = None,
                               undo: typing.Optional[bool] = None,
                               *,
                               direction: typing.Optional[typing.Any] = 'UP'):
-    ''' Move a simulation state item up or down in the list :File: `startup/bl_operators/geometry_nodes.py\:325 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L325>`__
+    ''' Move a simulation state item up or down in the list :File: `startup/bl_operators/geometry_nodes.py\:327 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L327>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param direction: Direction
     :type direction: typing.Optional[typing.Any]
     '''
@@ -1533,15 +1533,15 @@
 
 
 def simulation_zone_item_remove(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Remove a state item from the simulation zone :File: `startup/bl_operators/geometry_nodes.py\:302 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L302>`__
+    ''' Remove a state item from the simulation zone :File: `startup/bl_operators/geometry_nodes.py\:304 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L304>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1606,15 +1606,15 @@
     pass
 
 
 def tree_path_parent(override_context: typing.
                      Union[typing.Dict, 'bpy.types.Context'] = None,
                      execution_context: typing.Union[str, int] = None,
                      undo: typing.Optional[bool] = None):
-    ''' Go to parent node tree :File: `startup/bl_operators/node.py\:239 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L239>`__
+    ''' Go to parent node tree :File: `startup/bl_operators/node.py\:242 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/node.py#L242>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/object.py` & `fake-bpy-module-latest-20230616/bpy/ops/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
           execution_context: typing.Union[str, int] = None,
           undo: typing.Optional[bool] = None,
           *,
           bb_quality: typing.Union[bool, typing.Any] = True,
           align_mode: typing.Optional[typing.Any] = 'OPT_2',
           relative_to: typing.Optional[typing.Any] = 'OPT_4',
           align_axis: typing.Optional[typing.Any] = {}):
-    ''' Align objects :File: `startup/bl_operators/object_align.py\:391 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object_align.py#L391>`__
+    ''' Align objects :File: `startup/bl_operators/object_align.py\:393 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object_align.py#L393>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param bb_quality: High Quality, Enables high quality but slow calculation of the bounding box for perfect results on complex shape meshes with rotation/scale
     :type bb_quality: typing.Union[bool, typing.Any]
     :param align_mode: Align Mode, Side of object to use for alignment
@@ -106,15 +106,15 @@
     pass
 
 
 def anim_transforms_to_deltas(override_context: typing.
                               Union[typing.Dict, 'bpy.types.Context'] = None,
                               execution_context: typing.Union[str, int] = None,
                               undo: typing.Optional[bool] = None):
-    ''' Convert object animation for normal transforms to delta transforms :File: `startup/bl_operators/object.py\:776 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L776>`__
+    ''' Convert object animation for normal transforms to delta transforms :File: `startup/bl_operators/object.py\:778 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L778>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -157,15 +157,15 @@
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         process_data: typing.Union[bool, typing.Any] = True,
         process_bones: typing.Union[bool, typing.Any] = True):
-    ''' Assign the current values of custom properties as their defaults, for use as part of the rest pose state in NLA track mixing :File: `startup/bl_operators/object.py\:1000 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L1000>`__
+    ''' Assign the current values of custom properties as their defaults, for use as part of the rest pose state in NLA track mixing :File: `startup/bl_operators/object.py\:1002 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L1002>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param process_data: Process data properties
     :type process_data: typing.Union[bool, typing.Any]
     :param process_bones: Process bone properties
@@ -1132,15 +1132,15 @@
 
 
 def geometry_nodes_move_to_nodes(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Move inputs and outputs from in the modifier to a new node group :File: `startup/bl_operators/geometry_nodes.py\:117 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L117>`__
+    ''' Move inputs and outputs from in the modifier to a new node group :File: `startup/bl_operators/geometry_nodes.py\:119 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L119>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1407,15 +1407,15 @@
     pass
 
 
 def hide_render_clear_all(override_context: typing.
                           Union[typing.Dict, 'bpy.types.Context'] = None,
                           execution_context: typing.Union[str, int] = None,
                           undo: typing.Optional[bool] = None):
-    ''' Reveal all render objects by setting the hide render flag :File: `startup/bl_operators/object.py\:683 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L683>`__
+    ''' Reveal all render objects by setting the hide render flag :File: `startup/bl_operators/object.py\:685 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L685>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1580,58 +1580,58 @@
 
 
 def instance_offset_from_cursor(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Set offset used for collection instances based on cursor position :File: `startup/bl_operators/object.py\:861 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L861>`__
+    ''' Set offset used for collection instances based on cursor position :File: `startup/bl_operators/object.py\:863 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L863>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def instance_offset_from_object(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Set offset used for collection instances based on the active object position :File: `startup/bl_operators/object.py\:893 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L893>`__
+    ''' Set offset used for collection instances based on the active object position :File: `startup/bl_operators/object.py\:895 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L895>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def instance_offset_to_cursor(override_context: typing.
                               Union[typing.Dict, 'bpy.types.Context'] = None,
                               execution_context: typing.Union[str, int] = None,
                               undo: typing.Optional[bool] = None):
-    ''' Set cursor position to the offset used for collection instances :File: `startup/bl_operators/object.py\:876 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L876>`__
+    ''' Set cursor position to the offset used for collection instances :File: `startup/bl_operators/object.py\:878 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L878>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def isolate_type_render(override_context: typing.
                         Union[typing.Dict, 'bpy.types.Context'] = None,
                         execution_context: typing.Union[str, int] = None,
                         undo: typing.Optional[bool] = None):
-    ''' Hide unselected render objects of same type as active by setting the hide render flag :File: `startup/bl_operators/object.py\:663 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L663>`__
+    ''' Hide unselected render objects of same type as active by setting the hide render flag :File: `startup/bl_operators/object.py\:665 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L665>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1665,15 +1665,15 @@
     pass
 
 
 def join_uvs(override_context: typing.Union[typing.
                                             Dict, 'bpy.types.Context'] = None,
              execution_context: typing.Union[str, int] = None,
              undo: typing.Optional[bool] = None):
-    ''' Transfer UV Maps from active to selected objects (needs matching geometry) :File: `startup/bl_operators/object.py\:566 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L566>`__
+    ''' Transfer UV Maps from active to selected objects (needs matching geometry) :File: `startup/bl_operators/object.py\:568 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L568>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -2000,15 +2000,15 @@
                           execution_context: typing.Union[str, int] = None,
                           undo: typing.Optional[bool] = None,
                           *,
                           filepath: typing.Union[str, typing.Any] = "",
                           filter_image: typing.Union[bool, typing.Any] = True,
                           filter_folder: typing.Union[bool, typing.Any] = True,
                           view_align: typing.Union[bool, typing.Any] = True):
-    ''' Add a reference image into the background behind objects :File: `startup/bl_operators/object.py\:924 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L924>`__
+    ''' Add a reference image into the background behind objects :File: `startup/bl_operators/object.py\:926 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L926>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     :param filter_image: filter_image
@@ -2027,15 +2027,15 @@
                          execution_context: typing.Union[str, int] = None,
                          undo: typing.Optional[bool] = None,
                          *,
                          filepath: typing.Union[str, typing.Any] = "",
                          filter_image: typing.Union[bool, typing.Any] = True,
                          filter_folder: typing.Union[bool, typing.Any] = True,
                          view_align: typing.Union[bool, typing.Any] = True):
-    ''' Add a reference image into the scene between objects :File: `startup/bl_operators/object.py\:924 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L924>`__
+    ''' Add a reference image into the scene between objects :File: `startup/bl_operators/object.py\:926 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L926>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     :param filter_image: filter_image
@@ -2067,15 +2067,15 @@
     pass
 
 
 def make_dupli_face(override_context: typing.
                     Union[typing.Dict, 'bpy.types.Context'] = None,
                     execution_context: typing.Union[str, int] = None,
                     undo: typing.Optional[bool] = None):
-    ''' Convert objects into instanced faces :File: `startup/bl_operators/object.py\:646 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L646>`__
+    ''' Convert objects into instanced faces :File: `startup/bl_operators/object.py\:648 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L648>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -3191,15 +3191,15 @@
                   style: typing.Optional[typing.Any] = 'EXPLODE',
                   amount: typing.Optional[typing.Any] = 100,
                   frame_duration: typing.Optional[typing.Any] = 50,
                   frame_start: typing.Optional[typing.Any] = 1,
                   frame_end: typing.Optional[typing.Any] = 10,
                   velocity: typing.Optional[typing.Any] = 1.0,
                   fade: typing.Union[bool, typing.Any] = True):
-    ''' Make selected objects explode :File: `startup/bl_operators/object_quick_effects.py\:258 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object_quick_effects.py#L258>`__
+    ''' Make selected objects explode :File: `startup/bl_operators/object_quick_effects.py\:260 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object_quick_effects.py#L260>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param style: Explode Style
     :type style: typing.Optional[typing.Any]
     :param amount: Number of Pieces
@@ -3227,15 +3227,15 @@
               density: typing.Optional[typing.Any] = 'MEDIUM',
               length: typing.Optional[typing.Any] = 0.1,
               radius: typing.Optional[typing.Any] = 0.001,
               view_percentage: typing.Optional[typing.Any] = 1.0,
               apply_hair_guides: typing.Union[bool, typing.Any] = True,
               use_noise: typing.Union[bool, typing.Any] = True,
               use_frizz: typing.Union[bool, typing.Any] = True):
-    ''' Add a fur setup to the selected objects :File: `startup/bl_operators/object_quick_effects.py\:89 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object_quick_effects.py#L89>`__
+    ''' Add a fur setup to the selected objects :File: `startup/bl_operators/object_quick_effects.py\:91 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object_quick_effects.py#L91>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param density: Density
     :type density: typing.Optional[typing.Any]
     :param length: Length
@@ -3257,15 +3257,15 @@
 
 def quick_liquid(override_context: typing.
                  Union[typing.Dict, 'bpy.types.Context'] = None,
                  execution_context: typing.Union[str, int] = None,
                  undo: typing.Optional[bool] = None,
                  *,
                  show_flows: typing.Union[bool, typing.Any] = False):
-    ''' Make selected objects liquid :File: `startup/bl_operators/object_quick_effects.py\:542 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object_quick_effects.py#L542>`__
+    ''' Make selected objects liquid :File: `startup/bl_operators/object_quick_effects.py\:544 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object_quick_effects.py#L544>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param show_flows: Render Liquid Objects, Keep the liquid objects visible during rendering
     :type show_flows: typing.Union[bool, typing.Any]
     '''
@@ -3276,15 +3276,15 @@
 def quick_smoke(override_context: typing.
                 Union[typing.Dict, 'bpy.types.Context'] = None,
                 execution_context: typing.Union[str, int] = None,
                 undo: typing.Optional[bool] = None,
                 *,
                 style: typing.Optional[typing.Any] = 'SMOKE',
                 show_flows: typing.Union[bool, typing.Any] = False):
-    ''' Use selected objects as smoke emitters :File: `startup/bl_operators/object_quick_effects.py\:436 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object_quick_effects.py#L436>`__
+    ''' Use selected objects as smoke emitters :File: `startup/bl_operators/object_quick_effects.py\:438 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object_quick_effects.py#L438>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param style: Smoke Style
     :type style: typing.Optional[typing.Any]
     :param show_flows: Render Smoke Objects, Keep the smoke objects visible during rendering
@@ -3304,15 +3304,15 @@
                         use_loc: typing.Union[bool, typing.Any] = True,
                         loc: typing.Optional[typing.Any] = (0.0, 0.0, 0.0),
                         use_rot: typing.Union[bool, typing.Any] = True,
                         rot: typing.Optional[typing.Any] = (0.0, 0.0, 0.0),
                         use_scale: typing.Union[bool, typing.Any] = True,
                         scale_even: typing.Union[bool, typing.Any] = False,
                         scale: typing.Optional[typing.Any] = (1.0, 1.0, 1.0)):
-    ''' Randomize objects location, rotation, and scale :File: `startup/bl_operators/object_randomize_transform.py\:162 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object_randomize_transform.py#L162>`__
+    ''' Randomize objects location, rotation, and scale :File: `startup/bl_operators/object_randomize_transform.py\:164 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object_randomize_transform.py#L164>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param random_seed: Random Seed, Seed value for the random generator
     :type random_seed: typing.Optional[typing.Any]
     :param use_delta: Transform Delta, Randomize delta transform values instead of regular transform
@@ -3427,15 +3427,15 @@
 
 def select_camera(override_context: typing.
                   Union[typing.Dict, 'bpy.types.Context'] = None,
                   execution_context: typing.Union[str, int] = None,
                   undo: typing.Optional[bool] = None,
                   *,
                   extend: typing.Union[bool, typing.Any] = False):
-    ''' Select the active camera :File: `startup/bl_operators/object.py\:115 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L115>`__
+    ''' Select the active camera :File: `startup/bl_operators/object.py\:117 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L117>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param extend: Extend, Extend the selection
     :type extend: typing.Union[bool, typing.Any]
     '''
@@ -3467,15 +3467,15 @@
 def select_hierarchy(override_context: typing.
                      Union[typing.Dict, 'bpy.types.Context'] = None,
                      execution_context: typing.Union[str, int] = None,
                      undo: typing.Optional[bool] = None,
                      *,
                      direction: typing.Optional[typing.Any] = 'PARENT',
                      extend: typing.Union[bool, typing.Any] = False):
-    ''' Select object relative to the active object's position in the hierarchy :File: `startup/bl_operators/object.py\:165 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L165>`__
+    ''' Select object relative to the active object's position in the hierarchy :File: `startup/bl_operators/object.py\:167 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L167>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param direction: Direction, Direction to select in the hierarchy
     :type direction: typing.Optional[typing.Any]
     :param extend: Extend, Extend the existing selection
@@ -3556,15 +3556,15 @@
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None,
                    *,
                    pattern: typing.Union[str, typing.Any] = "*",
                    case_sensitive: typing.Union[bool, typing.Any] = False,
                    extend: typing.Union[bool, typing.Any] = True):
-    ''' Select objects matching a naming pattern :File: `startup/bl_operators/object.py\:38 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L38>`__
+    ''' Select objects matching a naming pattern :File: `startup/bl_operators/object.py\:40 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L40>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param pattern: Pattern, Name filter using '*', '?' and '[abc]' unix style wildcards
     :type pattern: typing.Union[str, typing.Any]
     :param case_sensitive: Case Sensitive, Do a case sensitive compare
@@ -3873,15 +3873,15 @@
 def shape_key_transfer(override_context: typing.
                        Union[typing.Dict, 'bpy.types.Context'] = None,
                        execution_context: typing.Union[str, int] = None,
                        undo: typing.Optional[bool] = None,
                        *,
                        mode: typing.Optional[typing.Any] = 'OFFSET',
                        use_clamp: typing.Union[bool, typing.Any] = False):
-    ''' Copy the active shape key of another selected object to this one :File: `startup/bl_operators/object.py\:463 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L463>`__
+    ''' Copy the active shape key of another selected object to this one :File: `startup/bl_operators/object.py\:465 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L465>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param mode: Transformation Mode, Relative shape positions to the new shape method * ``OFFSET`` Offset -- Apply the relative positional offset. * ``RELATIVE_FACE`` Relative Face -- Calculate relative position (using faces). * ``RELATIVE_EDGE`` Relative Edge -- Calculate relative position (using edges).
     :type mode: typing.Optional[typing.Any]
     :param use_clamp: Clamp Offset, Clamp the transformation to the distance each vertex moves in the original shape
@@ -4045,15 +4045,15 @@
 def subdivision_set(override_context: typing.
                     Union[typing.Dict, 'bpy.types.Context'] = None,
                     execution_context: typing.Union[str, int] = None,
                     undo: typing.Optional[bool] = None,
                     *,
                     level: typing.Optional[typing.Any] = 1,
                     relative: typing.Union[bool, typing.Any] = False):
-    ''' Sets a Subdivision Surface level (1 to 5) :File: `startup/bl_operators/object.py\:233 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L233>`__
+    ''' Sets a Subdivision Surface level (1 to 5) :File: `startup/bl_operators/object.py\:235 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L235>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param level: Level
     :type level: typing.Optional[typing.Any]
     :param relative: Relative, Apply the subdivision surface level as an offset relative to the current level
@@ -4250,15 +4250,15 @@
 def transforms_to_deltas(override_context: typing.
                          Union[typing.Dict, 'bpy.types.Context'] = None,
                          execution_context: typing.Union[str, int] = None,
                          undo: typing.Optional[bool] = None,
                          *,
                          mode: typing.Optional[typing.Any] = 'ALL',
                          reset_values: typing.Union[bool, typing.Any] = True):
-    ''' Convert normal object transforms to delta transforms, any existing delta transforms will be included as well :File: `startup/bl_operators/object.py\:718 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L718>`__
+    ''' Convert normal object transforms to delta transforms, any existing delta transforms will be included as well :File: `startup/bl_operators/object.py\:720 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L720>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param mode: Mode, Which transforms to transfer * ``ALL`` All Transforms -- Transfer location, rotation, and scale transforms. * ``LOC`` Location -- Transfer location transforms only. * ``ROT`` Rotation -- Transfer rotation transforms only. * ``SCALE`` Scale -- Transfer scale transforms only.
     :type mode: typing.Optional[typing.Any]
     :param reset_values: Reset Values, Clear transform values after transferring to deltas
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/outliner.py` & `fake-bpy-module-latest-20230616/bpy/ops/outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/paint.py` & `fake-bpy-module-latest-20230616/bpy/ops/paint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/paintcurve.py` & `fake-bpy-module-latest-20230616/bpy/ops/paintcurve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/palette.py` & `fake-bpy-module-latest-20230616/bpy/ops/palette.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/particle.py` & `fake-bpy-module-latest-20230616/bpy/ops/particle.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         name: typing.Union[str, typing.Any] = "",
         remove_name: typing.Union[bool, typing.Any] = False,
         remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove a Hair Dynamics Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove a Hair Dynamics Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/pose.py` & `fake-bpy-module-latest-20230616/bpy/ops/pose.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/poselib.py` & `fake-bpy-module-latest-20230616/bpy/ops/poselib.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,43 +51,43 @@
 
 
 def convert_old_object_poselib(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Create a pose asset for each pose marker in this legacy pose library data-block :File: `addons/pose_library/operators.py\:432 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L432>`__
+    ''' Create a pose asset for each pose marker in this legacy pose library data-block :File: `addons/pose_library/operators.py\:434 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L434>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def convert_old_poselib(override_context: typing.
                         Union[typing.Dict, 'bpy.types.Context'] = None,
                         execution_context: typing.Union[str, int] = None,
                         undo: typing.Optional[bool] = None):
-    ''' Create a pose asset for each pose marker in the current action :File: `addons/pose_library/operators.py\:398 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L398>`__
+    ''' Create a pose asset for each pose marker in the current action :File: `addons/pose_library/operators.py\:400 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L400>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def copy_as_asset(override_context: typing.
                   Union[typing.Dict, 'bpy.types.Context'] = None,
                   execution_context: typing.Union[str, int] = None,
                   undo: typing.Optional[bool] = None):
-    ''' Create a new pose asset on the clipboard, to be pasted into an Asset Browser :File: `addons/pose_library/operators.py\:209 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L209>`__
+    ''' Create a new pose asset on the clipboard, to be pasted into an Asset Browser :File: `addons/pose_library/operators.py\:211 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L211>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -97,15 +97,15 @@
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         pose_name: typing.Union[str, typing.Any] = "",
         activate_new_action: typing.Union[bool, typing.Any] = True):
-    ''' Create a new Action that contains the pose of the selected bones, and mark it as Asset. The asset will be stored in the current blend file :File: `addons/pose_library/operators.py\:82 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L82>`__
+    ''' Create a new Action that contains the pose of the selected bones, and mark it as Asset. The asset will be stored in the current blend file :File: `addons/pose_library/operators.py\:84 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L84>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param pose_name: Pose Name
     :type pose_name: typing.Union[str, typing.Any]
     :param activate_new_action: Activate New Action
@@ -115,15 +115,15 @@
     pass
 
 
 def paste_asset(override_context: typing.
                 Union[typing.Dict, 'bpy.types.Context'] = None,
                 execution_context: typing.Union[str, int] = None,
                 undo: typing.Optional[bool] = None):
-    ''' Paste the Asset that was previously copied using Copy As Asset :File: `addons/pose_library/operators.py\:281 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L281>`__
+    ''' Paste the Asset that was previously copied using Copy As Asset :File: `addons/pose_library/operators.py\:283 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L283>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -132,15 +132,15 @@
 def pose_asset_select_bones(override_context: typing.
                             Union[typing.Dict, 'bpy.types.Context'] = None,
                             execution_context: typing.Union[str, int] = None,
                             undo: typing.Optional[bool] = None,
                             *,
                             select: typing.Union[bool, typing.Any] = True,
                             flipped: typing.Union[bool, typing.Any] = False):
-    ''' Select those bones that are used in this pose :File: `addons/pose_library/operators.py\:319 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L319>`__
+    ''' Select those bones that are used in this pose :File: `addons/pose_library/operators.py\:321 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L321>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param select: Select
     :type select: typing.Union[bool, typing.Any]
     :param flipped: Flipped
@@ -150,15 +150,15 @@
     pass
 
 
 def restore_previous_action(override_context: typing.
                             Union[typing.Dict, 'bpy.types.Context'] = None,
                             execution_context: typing.Union[str, int] = None,
                             undo: typing.Optional[bool] = None):
-    ''' Switch back to the previous Action, after creating a pose asset :File: `addons/pose_library/operators.py\:158 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L158>`__
+    ''' Switch back to the previous Action, after creating a pose asset :File: `addons/pose_library/operators.py\:160 <https://projects.blender.org/blender/blender-addons/addons/pose_library/operators.py#L160>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/preferences.py` & `fake-bpy-module-latest-20230616/bpy/ops/preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def addon_disable(override_context: typing.
                   Union[typing.Dict, 'bpy.types.Context'] = None,
                   execution_context: typing.Union[str, int] = None,
                   undo: typing.Optional[bool] = None,
                   *,
                   module: typing.Union[str, typing.Any] = ""):
-    ''' Disable an add-on :File: `startup/bl_operators/userpref.py\:481 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L481>`__
+    ''' Disable an add-on :File: `startup/bl_operators/userpref.py\:483 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L483>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param module: Module, Module name of the add-on to disable
     :type module: typing.Union[str, typing.Any]
     '''
@@ -25,15 +25,15 @@
 
 def addon_enable(override_context: typing.
                  Union[typing.Dict, 'bpy.types.Context'] = None,
                  execution_context: typing.Union[str, int] = None,
                  undo: typing.Optional[bool] = None,
                  *,
                  module: typing.Union[str, typing.Any] = ""):
-    ''' Enable an add-on :File: `startup/bl_operators/userpref.py\:435 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L435>`__
+    ''' Enable an add-on :File: `startup/bl_operators/userpref.py\:437 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L437>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param module: Module, Module name of the add-on to enable
     :type module: typing.Union[str, typing.Any]
     '''
@@ -43,15 +43,15 @@
 
 def addon_expand(override_context: typing.
                  Union[typing.Dict, 'bpy.types.Context'] = None,
                  execution_context: typing.Union[str, int] = None,
                  undo: typing.Optional[bool] = None,
                  *,
                  module: typing.Union[str, typing.Any] = ""):
-    ''' Display information and preferences for this add-on :File: `startup/bl_operators/userpref.py\:817 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L817>`__
+    ''' Display information and preferences for this add-on :File: `startup/bl_operators/userpref.py\:819 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L819>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param module: Module, Module name of the add-on to expand
     :type module: typing.Union[str, typing.Any]
     '''
@@ -66,15 +66,15 @@
                   *,
                   overwrite: typing.Union[bool, typing.Any] = True,
                   target: typing.Union[str, int, typing.Any] = '',
                   filepath: typing.Union[str, typing.Any] = "",
                   filter_folder: typing.Union[bool, typing.Any] = True,
                   filter_python: typing.Union[bool, typing.Any] = True,
                   filter_glob: typing.Union[str, typing.Any] = "*.py;*.zip"):
-    ''' Install an add-on :File: `startup/bl_operators/userpref.py\:623 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L623>`__
+    ''' Install an add-on :File: `startup/bl_operators/userpref.py\:625 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L625>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param overwrite: Overwrite, Remove existing add-ons with the same ID
     :type overwrite: typing.Union[bool, typing.Any]
     :param target: Target Path
@@ -92,15 +92,15 @@
     pass
 
 
 def addon_refresh(override_context: typing.
                   Union[typing.Dict, 'bpy.types.Context'] = None,
                   execution_context: typing.Union[str, int] = None,
                   undo: typing.Optional[bool] = None):
-    ''' Scan add-on directories for new modules :File: `startup/bl_operators/userpref.py\:571 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L571>`__
+    ''' Scan add-on directories for new modules :File: `startup/bl_operators/userpref.py\:573 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L573>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -108,15 +108,15 @@
 
 def addon_remove(override_context: typing.
                  Union[typing.Dict, 'bpy.types.Context'] = None,
                  execution_context: typing.Union[str, int] = None,
                  undo: typing.Optional[bool] = None,
                  *,
                  module: typing.Union[str, typing.Any] = ""):
-    ''' Delete the add-on from the file system :File: `startup/bl_operators/userpref.py\:772 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L772>`__
+    ''' Delete the add-on from the file system :File: `startup/bl_operators/userpref.py\:774 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L774>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param module: Module, Module name of the add-on to remove
     :type module: typing.Union[str, typing.Any]
     '''
@@ -126,15 +126,15 @@
 
 def addon_show(override_context: typing.
                Union[typing.Dict, 'bpy.types.Context'] = None,
                execution_context: typing.Union[str, int] = None,
                undo: typing.Optional[bool] = None,
                *,
                module: typing.Union[str, typing.Any] = ""):
-    ''' Show add-on preferences :File: `startup/bl_operators/userpref.py\:841 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L841>`__
+    ''' Show add-on preferences :File: `startup/bl_operators/userpref.py\:843 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L843>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param module: Module, Module name of the add-on to expand
     :type module: typing.Union[str, typing.Any]
     '''
@@ -147,15 +147,15 @@
                          execution_context: typing.Union[str, int] = None,
                          undo: typing.Optional[bool] = None,
                          *,
                          overwrite: typing.Union[bool, typing.Any] = True,
                          filepath: typing.Union[str, typing.Any] = "",
                          filter_folder: typing.Union[bool, typing.Any] = True,
                          filter_glob: typing.Union[str, typing.Any] = "*.zip"):
-    ''' Install an application template :File: `startup/bl_operators/userpref.py\:887 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L887>`__
+    ''' Install an application template :File: `startup/bl_operators/userpref.py\:889 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L889>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param overwrite: Overwrite, Remove existing template with the same ID
     :type overwrite: typing.Union[bool, typing.Any]
     :param filepath: filepath
@@ -317,15 +317,15 @@
     pass
 
 
 def copy_prev(override_context: typing.Union[typing.
                                              Dict, 'bpy.types.Context'] = None,
               execution_context: typing.Union[str, int] = None,
               undo: typing.Optional[bool] = None):
-    ''' Copy settings from previous version :File: `startup/bl_operators/userpref.py\:142 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L142>`__
+    ''' Copy settings from previous version :File: `startup/bl_operators/userpref.py\:144 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L144>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -333,15 +333,15 @@
 
 def keyconfig_activate(override_context: typing.
                        Union[typing.Dict, 'bpy.types.Context'] = None,
                        execution_context: typing.Union[str, int] = None,
                        undo: typing.Optional[bool] = None,
                        *,
                        filepath: typing.Union[str, typing.Any] = ""):
-    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/userpref.py\:63 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L63>`__
+    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/userpref.py\:65 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L65>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     '''
@@ -355,15 +355,15 @@
                      undo: typing.Optional[bool] = None,
                      *,
                      all: typing.Union[bool, typing.Any] = False,
                      filepath: typing.Union[str, typing.Any] = "",
                      filter_folder: typing.Union[bool, typing.Any] = True,
                      filter_text: typing.Union[bool, typing.Any] = True,
                      filter_python: typing.Union[bool, typing.Any] = True):
-    ''' Export key configuration to a Python script :File: `startup/bl_operators/userpref.py\:277 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L277>`__
+    ''' Export key configuration to a Python script :File: `startup/bl_operators/userpref.py\:279 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L279>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param all: All Keymaps, Write all keymaps (not just user modified)
     :type all: typing.Union[bool, typing.Any]
     :param filepath: filepath
@@ -385,15 +385,15 @@
                      undo: typing.Optional[bool] = None,
                      *,
                      filepath: typing.Union[str, typing.Any] = "keymap.py",
                      filter_folder: typing.Union[bool, typing.Any] = True,
                      filter_text: typing.Union[bool, typing.Any] = True,
                      filter_python: typing.Union[bool, typing.Any] = True,
                      keep_original: typing.Union[bool, typing.Any] = True):
-    ''' Import key configuration from a Python script :File: `startup/bl_operators/userpref.py\:206 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L206>`__
+    ''' Import key configuration from a Python script :File: `startup/bl_operators/userpref.py\:208 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L208>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     :param filter_folder: Filter folders
@@ -409,43 +409,43 @@
     pass
 
 
 def keyconfig_remove(override_context: typing.
                      Union[typing.Dict, 'bpy.types.Context'] = None,
                      execution_context: typing.Union[str, int] = None,
                      undo: typing.Optional[bool] = None):
-    ''' Remove key config :File: `startup/bl_operators/userpref.py\:415 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L415>`__
+    ''' Remove key config :File: `startup/bl_operators/userpref.py\:417 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L417>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def keyconfig_test(override_context: typing.
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None):
-    ''' Test key configuration for conflicts :File: `startup/bl_operators/userpref.py\:164 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L164>`__
+    ''' Test key configuration for conflicts :File: `startup/bl_operators/userpref.py\:166 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L166>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def keyitem_add(override_context: typing.
                 Union[typing.Dict, 'bpy.types.Context'] = None,
                 execution_context: typing.Union[str, int] = None,
                 undo: typing.Optional[bool] = None):
-    ''' Add key map item :File: `startup/bl_operators/userpref.py\:363 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L363>`__
+    ''' Add key map item :File: `startup/bl_operators/userpref.py\:365 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L365>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -453,15 +453,15 @@
 
 def keyitem_remove(override_context: typing.
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None,
                    *,
                    item_id: typing.Optional[typing.Any] = 0):
-    ''' Remove key map item :File: `startup/bl_operators/userpref.py\:395 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L395>`__
+    ''' Remove key map item :File: `startup/bl_operators/userpref.py\:397 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L397>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param item_id: Item Identifier, Identifier of the item to remove
     :type item_id: typing.Optional[typing.Any]
     '''
@@ -471,15 +471,15 @@
 
 def keyitem_restore(override_context: typing.
                     Union[typing.Dict, 'bpy.types.Context'] = None,
                     execution_context: typing.Union[str, int] = None,
                     undo: typing.Optional[bool] = None,
                     *,
                     item_id: typing.Optional[typing.Any] = 0):
-    ''' Restore key map item :File: `startup/bl_operators/userpref.py\:348 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L348>`__
+    ''' Restore key map item :File: `startup/bl_operators/userpref.py\:350 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L350>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param item_id: Item Identifier, Identifier of the item to restore
     :type item_id: typing.Optional[typing.Any]
     '''
@@ -489,15 +489,15 @@
 
 def keymap_restore(override_context: typing.
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None,
                    *,
                    all: typing.Union[bool, typing.Any] = False):
-    ''' Restore key map(s) :File: `startup/bl_operators/userpref.py\:319 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L319>`__
+    ''' Restore key map(s) :File: `startup/bl_operators/userpref.py\:321 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L321>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param all: All Keymaps, Restore all keymaps to default
     :type all: typing.Union[bool, typing.Any]
     '''
@@ -522,15 +522,15 @@
 def script_directory_add(override_context: typing.
                          Union[typing.Dict, 'bpy.types.Context'] = None,
                          execution_context: typing.Union[str, int] = None,
                          undo: typing.Optional[bool] = None,
                          *,
                          directory: typing.Union[str, typing.Any] = "",
                          filter_folder: typing.Union[bool, typing.Any] = True):
-    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/userpref.py\:1164 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L1164>`__
+    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/userpref.py\:1166 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L1166>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param directory: directory
     :type directory: typing.Union[str, typing.Any]
     :param filter_folder: Filter Folders
@@ -542,15 +542,15 @@
 
 def script_directory_remove(override_context: typing.
                             Union[typing.Dict, 'bpy.types.Context'] = None,
                             execution_context: typing.Union[str, int] = None,
                             undo: typing.Optional[bool] = None,
                             *,
                             index: typing.Optional[typing.Any] = 0):
-    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/userpref.py\:1194 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L1194>`__
+    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/userpref.py\:1196 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L1196>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param index: Index, Index of the script directory to remove
     :type index: typing.Optional[typing.Any]
     '''
@@ -560,15 +560,15 @@
 
 def studiolight_copy_settings(override_context: typing.
                               Union[typing.Dict, 'bpy.types.Context'] = None,
                               execution_context: typing.Union[str, int] = None,
                               undo: typing.Optional[bool] = None,
                               *,
                               index: typing.Optional[typing.Any] = 0):
-    ''' Copy Studio Light settings to the Studio Light editor :File: `startup/bl_operators/userpref.py\:1119 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L1119>`__
+    ''' Copy Studio Light settings to the Studio Light editor :File: `startup/bl_operators/userpref.py\:1121 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L1121>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param index: index
     :type index: typing.Optional[typing.Any]
     '''
@@ -584,15 +584,15 @@
         *,
         files: typing.Optional[bpy.types.bpy_prop_collection[
             'bpy.types.OperatorFileListElement']] = None,
         directory: typing.Union[str, typing.Any] = "",
         filter_folder: typing.Union[bool, typing.Any] = True,
         filter_glob: typing.Union[str, typing.Any] = "*.png;*.jpg;*.hdr;*.exr",
         type: typing.Optional[typing.Any] = 'MATCAP'):
-    ''' Install a user defined light :File: `startup/bl_operators/userpref.py\:996 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L996>`__
+    ''' Install a user defined light :File: `startup/bl_operators/userpref.py\:998 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L998>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param files: File Path
     :type files: typing.Optional[bpy.types.bpy_prop_collection['bpy.types.OperatorFileListElement']]
     :param directory: directory
@@ -610,15 +610,15 @@
 
 def studiolight_new(override_context: typing.
                     Union[typing.Dict, 'bpy.types.Context'] = None,
                     execution_context: typing.Union[str, int] = None,
                     undo: typing.Optional[bool] = None,
                     *,
                     filename: typing.Union[str, typing.Any] = "StudioLight"):
-    ''' Save custom studio light from the studio light editor settings :File: `startup/bl_operators/userpref.py\:1042 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L1042>`__
+    ''' Save custom studio light from the studio light editor settings :File: `startup/bl_operators/userpref.py\:1044 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L1044>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filename: Name
     :type filename: typing.Union[str, typing.Any]
     '''
@@ -626,15 +626,15 @@
     pass
 
 
 def studiolight_show(override_context: typing.
                      Union[typing.Dict, 'bpy.types.Context'] = None,
                      execution_context: typing.Union[str, int] = None,
                      undo: typing.Optional[bool] = None):
-    ''' Show light preferences :File: `startup/bl_operators/userpref.py\:1145 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L1145>`__
+    ''' Show light preferences :File: `startup/bl_operators/userpref.py\:1147 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L1147>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -642,15 +642,15 @@
 
 def studiolight_uninstall(override_context: typing.
                           Union[typing.Dict, 'bpy.types.Context'] = None,
                           execution_context: typing.Union[str, int] = None,
                           undo: typing.Optional[bool] = None,
                           *,
                           index: typing.Optional[typing.Any] = 0):
-    ''' Delete Studio Light :File: `startup/bl_operators/userpref.py\:1096 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L1096>`__
+    ''' Delete Studio Light :File: `startup/bl_operators/userpref.py\:1098 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L1098>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param index: index
     :type index: typing.Optional[typing.Any]
     '''
@@ -663,15 +663,15 @@
                   execution_context: typing.Union[str, int] = None,
                   undo: typing.Optional[bool] = None,
                   *,
                   overwrite: typing.Union[bool, typing.Any] = True,
                   filepath: typing.Union[str, typing.Any] = "",
                   filter_folder: typing.Union[bool, typing.Any] = True,
                   filter_glob: typing.Union[str, typing.Any] = "*.xml"):
-    ''' Load and apply a Blender XML theme file :File: `startup/bl_operators/userpref.py\:523 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L523>`__
+    ''' Load and apply a Blender XML theme file :File: `startup/bl_operators/userpref.py\:525 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/userpref.py#L525>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param overwrite: Overwrite, Remove existing theme file if exists
     :type overwrite: typing.Union[bool, typing.Any]
     :param filepath: filepath
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/ptcache.py` & `fake-bpy-module-latest-20230616/bpy/ops/ptcache.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/render.py` & `fake-bpy-module-latest-20230616/bpy/ops/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         name: typing.Union[str, typing.Any] = "",
         remove_name: typing.Union[bool, typing.Any] = False,
         remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add an Integrator Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add an Integrator Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
@@ -35,15 +35,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         name: typing.Union[str, typing.Any] = "",
         remove_name: typing.Union[bool, typing.Any] = False,
         remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add an Performance Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add an Performance Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
@@ -60,15 +60,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         name: typing.Union[str, typing.Any] = "",
         remove_name: typing.Union[bool, typing.Any] = False,
         remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add a Sampling Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add a Sampling Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
@@ -85,15 +85,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         name: typing.Union[str, typing.Any] = "",
         remove_name: typing.Union[bool, typing.Any] = False,
         remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add a Viewport Sampling Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add a Viewport Sampling Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
@@ -135,15 +135,15 @@
     pass
 
 
 def play_rendered_anim(override_context: typing.
                        Union[typing.Dict, 'bpy.types.Context'] = None,
                        execution_context: typing.Union[str, int] = None,
                        undo: typing.Optional[bool] = None):
-    ''' Play back rendered frames/movies using an external player :File: `startup/bl_operators/screen_play_rendered_anim.py\:65 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/screen_play_rendered_anim.py#L65>`__
+    ''' Play back rendered frames/movies using an external player :File: `startup/bl_operators/screen_play_rendered_anim.py\:67 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/screen_play_rendered_anim.py#L67>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -153,15 +153,15 @@
                Union[typing.Dict, 'bpy.types.Context'] = None,
                execution_context: typing.Union[str, int] = None,
                undo: typing.Optional[bool] = None,
                *,
                name: typing.Union[str, typing.Any] = "",
                remove_name: typing.Union[bool, typing.Any] = False,
                remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove a Render Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove a Render Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/rigidbody.py` & `fake-bpy-module-latest-20230616/bpy/ops/rigidbody.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                       Union[typing.Dict, 'bpy.types.Context'] = None,
                       execution_context: typing.Union[str, int] = None,
                       undo: typing.Optional[bool] = None,
                       *,
                       frame_start: typing.Optional[typing.Any] = 1,
                       frame_end: typing.Optional[typing.Any] = 250,
                       step: typing.Optional[typing.Any] = 1):
-    ''' Bake rigid body transformations of selected objects to keyframes :File: `startup/bl_operators/rigidbody.py\:106 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/rigidbody.py#L106>`__
+    ''' Bake rigid body transformations of selected objects to keyframes :File: `startup/bl_operators/rigidbody.py\:108 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/rigidbody.py#L108>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param frame_start: Start Frame, Start frame for baking
     :type frame_start: typing.Optional[typing.Any]
     :param frame_end: End Frame, End frame for baking
@@ -34,15 +34,15 @@
             execution_context: typing.Union[str, int] = None,
             undo: typing.Optional[bool] = None,
             *,
             con_type: typing.Optional[typing.Any] = 'FIXED',
             pivot_type: typing.Optional[typing.Any] = 'CENTER',
             connection_pattern: typing.Optional[typing.
                                                 Any] = 'SELECTED_TO_ACTIVE'):
-    ''' Create rigid body constraints between selected rigid bodies :File: `startup/bl_operators/rigidbody.py\:268 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/rigidbody.py#L268>`__
+    ''' Create rigid body constraints between selected rigid bodies :File: `startup/bl_operators/rigidbody.py\:270 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/rigidbody.py#L270>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param con_type: Type, Type of generated constraint * ``FIXED`` Fixed -- Glue rigid bodies together. * ``POINT`` Point -- Constrain rigid bodies to move around common pivot point. * ``HINGE`` Hinge -- Restrict rigid body rotation to one axis. * ``SLIDER`` Slider -- Restrict rigid body translation to one axis. * ``PISTON`` Piston -- Restrict rigid body translation and rotation to one axis. * ``GENERIC`` Generic -- Restrict translation and rotation to specified axes. * ``GENERIC_SPRING`` Generic Spring -- Restrict translation and rotation to specified axes with springs. * ``MOTOR`` Motor -- Drive rigid body around or along an axis.
     :type con_type: typing.Optional[typing.Any]
     :param pivot_type: Location, Constraint pivot location * ``CENTER`` Center -- Pivot location is between the constrained rigid bodies. * ``ACTIVE`` Active -- Pivot location is at the active object position. * ``SELECTED`` Selected -- Pivot location is at the selected object position.
@@ -139,15 +139,15 @@
     pass
 
 
 def object_settings_copy(override_context: typing.
                          Union[typing.Dict, 'bpy.types.Context'] = None,
                          execution_context: typing.Union[str, int] = None,
                          undo: typing.Optional[bool] = None):
-    ''' Copy Rigid Body settings from active object to selected :File: `startup/bl_operators/rigidbody.py\:43 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/rigidbody.py#L43>`__
+    ''' Copy Rigid Body settings from active object to selected :File: `startup/bl_operators/rigidbody.py\:45 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/rigidbody.py#L45>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/scene.py` & `fake-bpy-module-latest-20230616/bpy/ops/scene.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 
 def freestyle_add_edge_marks_to_keying_set(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Add the data paths to the Freestyle Edge Mark property of selected edges to the active keying set :File: `startup/bl_operators/freestyle.py\:134 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/freestyle.py#L134>`__
+    ''' Add the data paths to the Freestyle Edge Mark property of selected edges to the active keying set :File: `startup/bl_operators/freestyle.py\:136 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/freestyle.py#L136>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def freestyle_add_face_marks_to_keying_set(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Add the data paths to the Freestyle Face Mark property of selected polygons to the active keying set :File: `startup/bl_operators/freestyle.py\:165 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/freestyle.py#L165>`__
+    ''' Add the data paths to the Freestyle Face Mark property of selected polygons to the active keying set :File: `startup/bl_operators/freestyle.py\:167 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/freestyle.py#L167>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -91,15 +91,15 @@
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         type: typing.Optional[typing.Any] = 'COLOR',
         name: typing.Union[str, typing.Any] = ""):
-    ''' Fill the Range Min/Max entries by the min/max distance between selected mesh objects and the source object (either a user-specified object or the active camera) :File: `startup/bl_operators/freestyle.py\:40 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/freestyle.py#L40>`__
+    ''' Fill the Range Min/Max entries by the min/max distance between selected mesh objects and the source object (either a user-specified object or the active camera) :File: `startup/bl_operators/freestyle.py\:42 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/freestyle.py#L42>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param type: Type, Type of the modifier to work on * ``COLOR`` Color -- Color modifier type. * ``ALPHA`` Alpha -- Alpha modifier type. * ``THICKNESS`` Thickness -- Thickness modifier type.
     :type type: typing.Optional[typing.Any]
     :param name: Name, Name of the modifier to work on
@@ -298,15 +298,15 @@
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         filepath: typing.Union[str, typing.Any] = "",
         make_internal: typing.Union[bool, typing.Any] = True):
-    ''' Open a style module file :File: `startup/bl_operators/freestyle.py\:209 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/freestyle.py#L209>`__
+    ''' Open a style module file :File: `startup/bl_operators/freestyle.py\:211 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/freestyle.py#L211>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     :param make_internal: Make internal, Make module file internal after loading
@@ -369,15 +369,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         name: typing.Union[str, typing.Any] = "",
         remove_name: typing.Union[bool, typing.Any] = False,
         remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove grease pencil brush preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove grease pencil brush preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
@@ -394,15 +394,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         name: typing.Union[str, typing.Any] = "",
         remove_name: typing.Union[bool, typing.Any] = False,
         remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove grease pencil material preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove grease pencil material preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/screen.py` & `fake-bpy-module-latest-20230616/bpy/ops/screen.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/script.py` & `fake-bpy-module-latest-20230616/bpy/ops/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def execute_preset(override_context: typing.
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None,
                    *,
                    filepath: typing.Union[str, typing.Any] = "",
                    menu_idname: typing.Union[str, typing.Any] = ""):
-    ''' Load a preset :File: `startup/bl_operators/presets.py\:231 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L231>`__
+    ''' Load a preset :File: `startup/bl_operators/presets.py\:233 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L233>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     :param menu_idname: Menu ID Name, ID name of the menu this was called from
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/sculpt.py` & `fake-bpy-module-latest-20230616/bpy/ops/sculpt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/sculpt_curves.py` & `fake-bpy-module-latest-20230616/bpy/ops/sculpt_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/sequencer.py` & `fake-bpy-module-latest-20230616/bpy/ops/sequencer.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     pass
 
 
 def crossfade_sounds(override_context: typing.
                      Union[typing.Dict, 'bpy.types.Context'] = None,
                      execution_context: typing.Union[str, int] = None,
                      undo: typing.Optional[bool] = None):
-    ''' Do cross-fading volume animation of two selected sound strips :File: `startup/bl_operators/sequencer.py\:26 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/sequencer.py#L26>`__
+    ''' Do cross-fading volume animation of two selected sound strips :File: `startup/bl_operators/sequencer.py\:28 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/sequencer.py#L28>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -204,15 +204,15 @@
 
 
 def deinterlace_selected_movies(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Deinterlace all selected movie sources :File: `startup/bl_operators/sequencer.py\:114 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/sequencer.py#L114>`__
+    ''' Deinterlace all selected movie sources :File: `startup/bl_operators/sequencer.py\:116 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/sequencer.py#L116>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -429,15 +429,15 @@
 def fades_add(override_context: typing.Union[typing.
                                              Dict, 'bpy.types.Context'] = None,
               execution_context: typing.Union[str, int] = None,
               undo: typing.Optional[bool] = None,
               *,
               duration_seconds: typing.Optional[typing.Any] = 1.0,
               type: typing.Optional[typing.Any] = 'IN_OUT'):
-    ''' Adds or updates a fade animation for either visual or audio strips :File: `startup/bl_operators/sequencer.py\:192 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/sequencer.py#L192>`__
+    ''' Adds or updates a fade animation for either visual or audio strips :File: `startup/bl_operators/sequencer.py\:194 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/sequencer.py#L194>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param duration_seconds: Fade Duration, Duration of the fade in seconds
     :type duration_seconds: typing.Optional[typing.Any]
     :param type: Fade Type, Fade in, out, both in and out, to, or from the current frame. Default is both in and out * ``IN_OUT`` Fade In and Out -- Fade selected strips in and out. * ``IN`` Fade In -- Fade in selected strips. * ``OUT`` Fade Out -- Fade out selected strips. * ``CURSOR_FROM`` From Current Frame -- Fade from the time cursor to the end of overlapping sequences. * ``CURSOR_TO`` To Current Frame -- Fade from the start of sequences under the time cursor to the current frame.
@@ -447,15 +447,15 @@
     pass
 
 
 def fades_clear(override_context: typing.
                 Union[typing.Dict, 'bpy.types.Context'] = None,
                 execution_context: typing.Union[str, int] = None,
                 undo: typing.Optional[bool] = None):
-    ''' Removes fade animation from selected sequences :File: `startup/bl_operators/sequencer.py\:133 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/sequencer.py#L133>`__
+    ''' Removes fade animation from selected sequences :File: `startup/bl_operators/sequencer.py\:135 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/sequencer.py#L135>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1668,15 +1668,15 @@
 
 def split_multicam(override_context: typing.
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None,
                    *,
                    camera: typing.Optional[typing.Any] = 1):
-    ''' Split multicam strip and select camera :File: `startup/bl_operators/sequencer.py\:81 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/sequencer.py#L81>`__
+    ''' Split multicam strip and select camera :File: `startup/bl_operators/sequencer.py\:83 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/sequencer.py#L83>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param camera: Camera
     :type camera: typing.Optional[typing.Any]
     '''
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/sound.py` & `fake-bpy-module-latest-20230616/bpy/ops/sound.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/spreadsheet.py` & `fake-bpy-module-latest-20230616/bpy/ops/spreadsheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     pass
 
 
 def toggle_pin(override_context: typing.
                Union[typing.Dict, 'bpy.types.Context'] = None,
                execution_context: typing.Union[str, int] = None,
                undo: typing.Optional[bool] = None):
-    ''' Turn on or off pinning :File: `startup/bl_operators/spreadsheet.py\:19 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/spreadsheet.py#L19>`__
+    ''' Turn on or off pinning :File: `startup/bl_operators/spreadsheet.py\:21 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/spreadsheet.py#L21>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/surface.py` & `fake-bpy-module-latest-20230616/bpy/ops/surface.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/text.py` & `fake-bpy-module-latest-20230616/bpy/ops/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
                           Union[typing.Dict, 'bpy.types.Context'] = None,
                           execution_context: typing.Union[str, int] = None,
                           undo: typing.Optional[bool] = None,
                           *,
                           filepath: typing.Union[str, typing.Any] = "",
                           line: typing.Optional[typing.Any] = 0,
                           column: typing.Optional[typing.Any] = 0):
-    ''' Edit text file in external text editor :File: `startup/bl_operators/text.py\:20 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/text.py#L20>`__
+    ''' Edit text file in external text editor :File: `startup/bl_operators/text.py\:22 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/text.py#L22>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     :param line: line
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/text_editor.py` & `fake-bpy-module-latest-20230616/bpy/ops/cloth.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                Union[typing.Dict, 'bpy.types.Context'] = None,
                execution_context: typing.Union[str, int] = None,
                undo: typing.Optional[bool] = None,
                *,
                name: typing.Union[str, typing.Any] = "",
                remove_name: typing.Union[bool, typing.Any] = False,
                remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove a Text Editor Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove a Cloth Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/texture.py` & `fake-bpy-module-latest-20230616/bpy/ops/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/transform.py` & `fake-bpy-module-latest-20230616/bpy/ops/transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/ui.py` & `fake-bpy-module-latest-20230616/bpy/ops/ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/uilist.py` & `fake-bpy-module-latest-20230616/bpy/ops/uilist.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def entry_add(override_context: typing.Union[typing.
                                              Dict, 'bpy.types.Context'] = None,
               execution_context: typing.Union[str, int] = None,
               undo: typing.Optional[bool] = None,
               *,
               list_path: typing.Union[str, typing.Any] = "",
               active_index_path: typing.Union[str, typing.Any] = ""):
-    ''' Add an entry to the list after the current active item :File: `startup/bl_ui/generic_ui_list.py\:208 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_ui/generic_ui_list.py#L208>`__
+    ''' Add an entry to the list after the current active item :File: `startup/bl_ui/generic_ui_list.py\:210 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_ui/generic_ui_list.py#L210>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param list_path: list_path
     :type list_path: typing.Union[str, typing.Any]
     :param active_index_path: active_index_path
@@ -30,15 +30,15 @@
                Union[typing.Dict, 'bpy.types.Context'] = None,
                execution_context: typing.Union[str, int] = None,
                undo: typing.Optional[bool] = None,
                *,
                list_path: typing.Union[str, typing.Any] = "",
                active_index_path: typing.Union[str, typing.Any] = "",
                direction: typing.Optional[typing.Any] = 'UP'):
-    ''' Move an entry in the list up or down :File: `startup/bl_ui/generic_ui_list.py\:236 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_ui/generic_ui_list.py#L236>`__
+    ''' Move an entry in the list up or down :File: `startup/bl_ui/generic_ui_list.py\:238 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_ui/generic_ui_list.py#L238>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param list_path: list_path
     :type list_path: typing.Union[str, typing.Any]
     :param active_index_path: active_index_path
@@ -53,15 +53,15 @@
 def entry_remove(override_context: typing.
                  Union[typing.Dict, 'bpy.types.Context'] = None,
                  execution_context: typing.Union[str, int] = None,
                  undo: typing.Optional[bool] = None,
                  *,
                  list_path: typing.Union[str, typing.Any] = "",
                  active_index_path: typing.Union[str, typing.Any] = ""):
-    ''' Remove the selected entry from the list :File: `startup/bl_ui/generic_ui_list.py\:191 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_ui/generic_ui_list.py#L191>`__
+    ''' Remove the selected entry from the list :File: `startup/bl_ui/generic_ui_list.py\:193 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_ui/generic_ui_list.py#L193>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param list_path: list_path
     :type list_path: typing.Union[str, typing.Any]
     :param active_index_path: active_index_path
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/uv.py` & `fake-bpy-module-latest-20230616/bpy/ops/uv.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 def align_rotation(override_context: typing.
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None,
                    *,
                    method: typing.Optional[typing.Any] = 'AUTO',
                    axis: typing.Optional[typing.Any] = 'X'):
-    ''' Align the UV island's rotation :File: `startup/bl_operators/uvcalc_transform.py\:275 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/uvcalc_transform.py#L275>`__
+    ''' Align the UV island's rotation :File: `startup/bl_operators/uvcalc_transform.py\:277 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/uvcalc_transform.py#L277>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param method: Method, Method to calculate rotation angle * ``AUTO`` Auto -- Align from all edges. * ``EDGE`` Edge -- Only selected edges. * ``GEOMETRY`` Geometry -- Align to Geometry axis.
     :type method: typing.Optional[typing.Any]
     :param axis: Axis, Axis to align to * ``X`` X -- X axis. * ``Y`` Y -- Y axis. * ``Z`` Z -- Z axis.
@@ -173,15 +173,15 @@
                   filepath: typing.Union[str, typing.Any] = "",
                   export_all: typing.Union[bool, typing.Any] = False,
                   modified: typing.Union[bool, typing.Any] = False,
                   mode: typing.Optional[typing.Any] = 'PNG',
                   size: typing.Optional[typing.Any] = (1024, 1024),
                   opacity: typing.Optional[typing.Any] = 0.25,
                   check_existing: typing.Union[bool, typing.Any] = True):
-    ''' Export UV layout to file :File: `addons/io_mesh_uv_layout/__init__.py\:118 <https://projects.blender.org/blender/blender-addons/addons/io_mesh_uv_layout/__init__.py#L118>`__
+    ''' Export UV layout to file :File: `addons/io_mesh_uv_layout/__init__.py\:120 <https://projects.blender.org/blender/blender-addons/addons/io_mesh_uv_layout/__init__.py#L120>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     :param export_all: All UVs, Export all UVs in this mesh (not just visible ones)
@@ -203,15 +203,15 @@
 
 def follow_active_quads(override_context: typing.
                         Union[typing.Dict, 'bpy.types.Context'] = None,
                         execution_context: typing.Union[str, int] = None,
                         undo: typing.Optional[bool] = None,
                         *,
                         mode: typing.Optional[typing.Any] = 'LENGTH_AVERAGE'):
-    ''' Follow UVs from active quads along continuous face loops :File: `startup/bl_operators/uvcalc_follow_active.py\:257 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/uvcalc_follow_active.py#L257>`__
+    ''' Follow UVs from active quads along continuous face loops :File: `startup/bl_operators/uvcalc_follow_active.py\:259 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/uvcalc_follow_active.py#L259>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param mode: Edge Length Mode, Method to space UV edge loops * ``EVEN`` Even -- Space all UVs evenly. * ``LENGTH`` Length -- Average space UVs edge length of each loop. * ``LENGTH_AVERAGE`` Length Average -- Average space UVs edge length of each loop.
     :type mode: typing.Optional[typing.Any]
     '''
@@ -243,15 +243,15 @@
                   undo: typing.Optional[bool] = None,
                   *,
                   PREF_CONTEXT: typing.Optional[typing.Any] = 'SEL_FACES',
                   PREF_PACK_IN_ONE: typing.Union[bool, typing.Any] = True,
                   PREF_NEW_UVLAYER: typing.Union[bool, typing.Any] = False,
                   PREF_BOX_DIV: typing.Optional[typing.Any] = 12,
                   PREF_MARGIN_DIV: typing.Optional[typing.Any] = 0.1):
-    ''' Pack each face's UVs into the UV bounds :File: `startup/bl_operators/uvcalc_lightmap.py\:630 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/uvcalc_lightmap.py#L630>`__
+    ''' Pack each face's UVs into the UV bounds :File: `startup/bl_operators/uvcalc_lightmap.py\:632 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/uvcalc_lightmap.py#L632>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param PREF_CONTEXT: Selection * ``SEL_FACES`` Selected Faces -- Space all UVs evenly. * ``ALL_FACES`` All Faces -- Average space UVs edge length of each loop.
     :type PREF_CONTEXT: typing.Optional[typing.Any]
     :param PREF_PACK_IN_ONE: Share Texture Space, Objects share texture space, map all objects into a single UV map
@@ -422,15 +422,15 @@
                            use_loc: typing.Union[bool, typing.Any] = True,
                            loc: typing.Optional[typing.Any] = (0.0, 0.0),
                            use_rot: typing.Union[bool, typing.Any] = True,
                            rot: typing.Optional[typing.Any] = 0.0,
                            use_scale: typing.Union[bool, typing.Any] = True,
                            scale_even: typing.Union[bool, typing.Any] = False,
                            scale: typing.Optional[typing.Any] = (1.0, 1.0)):
-    ''' Randomize the UV island's location, rotation, and scale :File: `startup/bl_operators/uvcalc_transform.py\:449 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/uvcalc_transform.py#L449>`__
+    ''' Randomize the UV island's location, rotation, and scale :File: `startup/bl_operators/uvcalc_transform.py\:451 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/uvcalc_transform.py#L451>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param random_seed: Random Seed, Seed value for the random generator
     :type random_seed: typing.Optional[typing.Any]
     :param use_loc: Randomize Location, Randomize the location values
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/view2d.py` & `fake-bpy-module-latest-20230616/bpy/ops/view2d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/view3d.py` & `fake-bpy-module-latest-20230616/bpy/ops/view3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
 def edit_mesh_extrude_individual_move(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         allow_navigation: typing.Union[bool, typing.Any] = False):
-    ''' Extrude each individual face separately along local normals :File: `startup/bl_operators/view3d.py\:27 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/view3d.py#L27>`__
+    ''' Extrude each individual face separately along local normals :File: `startup/bl_operators/view3d.py\:29 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/view3d.py#L29>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param allow_navigation: allow_navigation, Allow navigation
     :type allow_navigation: typing.Union[bool, typing.Any]
     '''
@@ -327,15 +327,15 @@
 def edit_mesh_extrude_manifold_normal(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         allow_navigation: typing.Union[bool, typing.Any] = False):
-    ''' Extrude manifold region along normals :File: `startup/bl_operators/view3d.py\:204 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/view3d.py#L204>`__
+    ''' Extrude manifold region along normals :File: `startup/bl_operators/view3d.py\:206 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/view3d.py#L206>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param allow_navigation: allow_navigation, Allow navigation
     :type allow_navigation: typing.Union[bool, typing.Any]
     '''
@@ -347,15 +347,15 @@
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         dissolve_and_intersect: typing.Union[bool, typing.Any] = False,
         allow_navigation: typing.Union[bool, typing.Any] = False):
-    ''' Extrude region together along the average normal :File: `startup/bl_operators/view3d.py\:157 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/view3d.py#L157>`__
+    ''' Extrude region together along the average normal :File: `startup/bl_operators/view3d.py\:159 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/view3d.py#L159>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param dissolve_and_intersect: dissolve_and_intersect, Dissolves adjacent faces and intersects new geometry
     :type dissolve_and_intersect: typing.Union[bool, typing.Any]
     :param allow_navigation: allow_navigation, Allow navigation
@@ -368,15 +368,15 @@
 def edit_mesh_extrude_move_shrink_fatten(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         allow_navigation: typing.Union[bool, typing.Any] = False):
-    ''' Extrude region together along local normals :File: `startup/bl_operators/view3d.py\:181 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/view3d.py#L181>`__
+    ''' Extrude region together along local normals :File: `startup/bl_operators/view3d.py\:183 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/view3d.py#L183>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param allow_navigation: allow_navigation, Allow navigation
     :type allow_navigation: typing.Union[bool, typing.Any]
     '''
@@ -998,15 +998,15 @@
 def transform_gizmo_set(override_context: typing.
                         Union[typing.Dict, 'bpy.types.Context'] = None,
                         execution_context: typing.Union[str, int] = None,
                         undo: typing.Optional[bool] = None,
                         *,
                         extend: typing.Union[bool, typing.Any] = False,
                         type: typing.Optional[typing.Any] = {}):
-    ''' Set the current transform gizmo :File: `startup/bl_operators/view3d.py\:247 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/view3d.py#L247>`__
+    ''' Set the current transform gizmo :File: `startup/bl_operators/view3d.py\:249 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/view3d.py#L249>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param extend: Extend
     :type extend: typing.Union[bool, typing.Any]
     :param type: Type
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/wm.py` & `fake-bpy-module-latest-20230616/bpy/ops/wm.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
                  execution_context: typing.Union[str, int] = None,
                  undo: typing.Optional[bool] = None,
                  *,
                  data_type: typing.Optional[typing.Any] = 'OBJECT',
                  data_source: typing.Optional[typing.Any] = 'SELECT',
                  actions: typing.Optional[bpy.types.bpy_prop_collection[
                      'bl_operators.wm.BatchRenameAction']] = None):
-    ''' Rename multiple items at once :File: `startup/bl_operators/wm.py\:3080 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L3080>`__
+    ''' Rename multiple items at once :File: `startup/bl_operators/wm.py\:3083 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L3083>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_type: Type, Type of data to rename
     :type data_type: typing.Optional[typing.Any]
     :param data_source: Source
@@ -425,15 +425,15 @@
 
 
 def blend_strings_utf8_validate(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Check and fix all strings in current .blend file to be valid UTF-8 Unicode (needed for some old, 2.4x area files) :File: `startup/bl_operators/file.py\:288 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/file.py#L288>`__
+    ''' Check and fix all strings in current .blend file to be valid UTF-8 Unicode (needed for some old, 2.4x area files) :File: `startup/bl_operators/file.py\:290 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/file.py#L290>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -788,15 +788,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         data_path_iter: typing.Union[str, typing.Any] = "",
         data_path_item: typing.Union[str, typing.Any] = "",
         type: typing.Optional[typing.Any] = 'TOGGLE'):
-    ''' Set boolean values for a collection of items :File: `startup/bl_operators/wm.py\:858 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L858>`__
+    ''' Set boolean values for a collection of items :File: `startup/bl_operators/wm.py\:861 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L861>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path_iter: data_path_iter, The data path relative to the context, must point to an iterable
     :type data_path_iter: typing.Union[str, typing.Any]
     :param data_path_item: data_path_item, The data path from each iterable to the value (int or float)
@@ -811,15 +811,15 @@
 def context_cycle_array(override_context: typing.
                         Union[typing.Dict, 'bpy.types.Context'] = None,
                         execution_context: typing.Union[str, int] = None,
                         undo: typing.Optional[bool] = None,
                         *,
                         data_path: typing.Union[str, typing.Any] = "",
                         reverse: typing.Union[bool, typing.Any] = False):
-    ''' Set a context array value (useful for cycling the active mesh edit mode) :File: `startup/bl_operators/wm.py\:661 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L661>`__
+    ''' Set a context array value (useful for cycling the active mesh edit mode) :File: `startup/bl_operators/wm.py\:664 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L664>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param reverse: Reverse, Cycle backwards
@@ -833,15 +833,15 @@
                        Union[typing.Dict, 'bpy.types.Context'] = None,
                        execution_context: typing.Union[str, int] = None,
                        undo: typing.Optional[bool] = None,
                        *,
                        data_path: typing.Union[str, typing.Any] = "",
                        reverse: typing.Union[bool, typing.Any] = False,
                        wrap: typing.Union[bool, typing.Any] = False):
-    ''' Toggle a context value :File: `startup/bl_operators/wm.py\:612 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L612>`__
+    ''' Toggle a context value :File: `startup/bl_operators/wm.py\:615 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L615>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param reverse: Reverse, Cycle backwards
@@ -857,15 +857,15 @@
                       Union[typing.Dict, 'bpy.types.Context'] = None,
                       execution_context: typing.Union[str, int] = None,
                       undo: typing.Optional[bool] = None,
                       *,
                       data_path: typing.Union[str, typing.Any] = "",
                       reverse: typing.Union[bool, typing.Any] = False,
                       wrap: typing.Union[bool, typing.Any] = False):
-    ''' Set a context value (useful for cycling active material, shape keys, groups, etc.) :File: `startup/bl_operators/wm.py\:572 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L572>`__
+    ''' Set a context value (useful for cycling active material, shape keys, groups, etc.) :File: `startup/bl_operators/wm.py\:575 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L575>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param reverse: Reverse, Cycle backwards
@@ -879,15 +879,15 @@
 
 def context_menu_enum(override_context: typing.
                       Union[typing.Dict, 'bpy.types.Context'] = None,
                       execution_context: typing.Union[str, int] = None,
                       undo: typing.Optional[bool] = None,
                       *,
                       data_path: typing.Union[str, typing.Any] = ""):
-    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/wm.py\:690 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L690>`__
+    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/wm.py\:693 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L693>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     '''
@@ -902,15 +902,15 @@
                         *,
                         data_path_iter: typing.Union[str, typing.Any] = "",
                         data_path_item: typing.Union[str, typing.Any] = "",
                         header_text: typing.Union[str, typing.Any] = "",
                         input_scale: typing.Optional[typing.Any] = 0.01,
                         invert: typing.Union[bool, typing.Any] = False,
                         initial_x: typing.Optional[typing.Any] = 0):
-    ''' Adjust arbitrary values with mouse input :File: `startup/bl_operators/wm.py\:995 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L995>`__
+    ''' Adjust arbitrary values with mouse input :File: `startup/bl_operators/wm.py\:998 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L998>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path_iter: data_path_iter, The data path relative to the context, must point to an iterable
     :type data_path_iter: typing.Union[str, typing.Any]
     :param data_path_item: data_path_item, The data path from each iterable to the value (int or float)
@@ -930,15 +930,15 @@
 
 def context_pie_enum(override_context: typing.
                      Union[typing.Dict, 'bpy.types.Context'] = None,
                      execution_context: typing.Union[str, int] = None,
                      undo: typing.Optional[bool] = None,
                      *,
                      data_path: typing.Union[str, typing.Any] = ""):
-    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/wm.py\:721 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L721>`__
+    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/wm.py\:724 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L724>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     '''
@@ -949,15 +949,15 @@
 def context_scale_float(override_context: typing.
                         Union[typing.Dict, 'bpy.types.Context'] = None,
                         execution_context: typing.Union[str, int] = None,
                         undo: typing.Optional[bool] = None,
                         *,
                         data_path: typing.Union[str, typing.Any] = "",
                         value: typing.Optional[typing.Any] = 1.0):
-    ''' Scale a float context value :File: `startup/bl_operators/wm.py\:331 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L331>`__
+    ''' Scale a float context value :File: `startup/bl_operators/wm.py\:334 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L334>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param value: Value, Assign value
@@ -971,15 +971,15 @@
                       Union[typing.Dict, 'bpy.types.Context'] = None,
                       execution_context: typing.Union[str, int] = None,
                       undo: typing.Optional[bool] = None,
                       *,
                       data_path: typing.Union[str, typing.Any] = "",
                       value: typing.Optional[typing.Any] = 1.0,
                       always_step: typing.Union[bool, typing.Any] = True):
-    ''' Scale an int context value :File: `startup/bl_operators/wm.py\:369 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L369>`__
+    ''' Scale an int context value :File: `startup/bl_operators/wm.py\:372 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L372>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param value: Value, Assign value
@@ -994,15 +994,15 @@
 def context_set_boolean(override_context: typing.
                         Union[typing.Dict, 'bpy.types.Context'] = None,
                         execution_context: typing.Union[str, int] = None,
                         undo: typing.Optional[bool] = None,
                         *,
                         data_path: typing.Union[str, typing.Any] = "",
                         value: typing.Union[bool, typing.Any] = True):
-    ''' Set a context value :File: `startup/bl_operators/wm.py\:260 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L260>`__
+    ''' Set a context value :File: `startup/bl_operators/wm.py\:263 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L263>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param value: Value, Assignment value
@@ -1015,15 +1015,15 @@
 def context_set_enum(override_context: typing.
                      Union[typing.Dict, 'bpy.types.Context'] = None,
                      execution_context: typing.Union[str, int] = None,
                      undo: typing.Optional[bool] = None,
                      *,
                      data_path: typing.Union[str, typing.Any] = "",
                      value: typing.Union[str, typing.Any] = ""):
-    ''' Set a context value :File: `startup/bl_operators/wm.py\:260 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L260>`__
+    ''' Set a context value :File: `startup/bl_operators/wm.py\:263 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L263>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param value: Value, Assignment value (as a string)
@@ -1037,15 +1037,15 @@
                       Union[typing.Dict, 'bpy.types.Context'] = None,
                       execution_context: typing.Union[str, int] = None,
                       undo: typing.Optional[bool] = None,
                       *,
                       data_path: typing.Union[str, typing.Any] = "",
                       value: typing.Optional[typing.Any] = 0.0,
                       relative: typing.Union[bool, typing.Any] = False):
-    ''' Set a context value :File: `startup/bl_operators/wm.py\:260 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L260>`__
+    ''' Set a context value :File: `startup/bl_operators/wm.py\:263 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L263>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param value: Value, Assignment value
@@ -1060,15 +1060,15 @@
 def context_set_id(override_context: typing.
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None,
                    *,
                    data_path: typing.Union[str, typing.Any] = "",
                    value: typing.Union[str, typing.Any] = ""):
-    ''' Set a context value to an ID data-block :File: `startup/bl_operators/wm.py\:802 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L802>`__
+    ''' Set a context value to an ID data-block :File: `startup/bl_operators/wm.py\:805 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L805>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param value: Value, Assign value
@@ -1082,15 +1082,15 @@
                     Union[typing.Dict, 'bpy.types.Context'] = None,
                     execution_context: typing.Union[str, int] = None,
                     undo: typing.Optional[bool] = None,
                     *,
                     data_path: typing.Union[str, typing.Any] = "",
                     value: typing.Optional[typing.Any] = 0,
                     relative: typing.Union[bool, typing.Any] = False):
-    ''' Set a context value :File: `startup/bl_operators/wm.py\:260 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L260>`__
+    ''' Set a context value :File: `startup/bl_operators/wm.py\:263 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L263>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param value: Value, Assign value
@@ -1105,15 +1105,15 @@
 def context_set_string(override_context: typing.
                        Union[typing.Dict, 'bpy.types.Context'] = None,
                        execution_context: typing.Union[str, int] = None,
                        undo: typing.Optional[bool] = None,
                        *,
                        data_path: typing.Union[str, typing.Any] = "",
                        value: typing.Union[str, typing.Any] = ""):
-    ''' Set a context value :File: `startup/bl_operators/wm.py\:260 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L260>`__
+    ''' Set a context value :File: `startup/bl_operators/wm.py\:263 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L263>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param value: Value, Assign value
@@ -1126,15 +1126,15 @@
 def context_set_value(override_context: typing.
                       Union[typing.Dict, 'bpy.types.Context'] = None,
                       execution_context: typing.Union[str, int] = None,
                       undo: typing.Optional[bool] = None,
                       *,
                       data_path: typing.Union[str, typing.Any] = "",
                       value: typing.Union[str, typing.Any] = ""):
-    ''' Set a context value :File: `startup/bl_operators/wm.py\:472 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L472>`__
+    ''' Set a context value :File: `startup/bl_operators/wm.py\:475 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L475>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param value: Value, Assignment value (as a string)
@@ -1147,15 +1147,15 @@
 def context_toggle(override_context: typing.
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None,
                    *,
                    data_path: typing.Union[str, typing.Any] = "",
                    module: typing.Union[str, typing.Any] = ""):
-    ''' Toggle a context value :File: `startup/bl_operators/wm.py\:496 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L496>`__
+    ''' Toggle a context value :File: `startup/bl_operators/wm.py\:499 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L499>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param module: Module, Optionally override the context with a module
@@ -1169,15 +1169,15 @@
                         Union[typing.Dict, 'bpy.types.Context'] = None,
                         execution_context: typing.Union[str, int] = None,
                         undo: typing.Optional[bool] = None,
                         *,
                         data_path: typing.Union[str, typing.Any] = "",
                         value_1: typing.Union[str, typing.Any] = "",
                         value_2: typing.Union[str, typing.Any] = ""):
-    ''' Toggle a context value :File: `startup/bl_operators/wm.py\:537 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L537>`__
+    ''' Toggle a context value :File: `startup/bl_operators/wm.py\:540 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L540>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Context Attributes, Context data-path (expanded using visible windows in the current .blend file)
     :type data_path: typing.Union[str, typing.Any]
     :param value_1: Value, Toggle enum
@@ -1209,15 +1209,15 @@
 
 def doc_view(override_context: typing.Union[typing.
                                             Dict, 'bpy.types.Context'] = None,
              execution_context: typing.Union[str, int] = None,
              undo: typing.Optional[bool] = None,
              *,
              doc_id: typing.Union[str, typing.Any] = ""):
-    ''' Open online reference docs in a web browser :File: `startup/bl_operators/wm.py\:1352 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L1352>`__
+    ''' Open online reference docs in a web browser :File: `startup/bl_operators/wm.py\:1355 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L1355>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param doc_id: Doc ID
     :type doc_id: typing.Union[str, typing.Any]
     '''
@@ -1227,15 +1227,15 @@
 
 def doc_view_manual(override_context: typing.
                     Union[typing.Dict, 'bpy.types.Context'] = None,
                     execution_context: typing.Union[str, int] = None,
                     undo: typing.Optional[bool] = None,
                     *,
                     doc_id: typing.Union[str, typing.Any] = ""):
-    ''' Load online manual :File: `startup/bl_operators/wm.py\:1324 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L1324>`__
+    ''' Load online manual :File: `startup/bl_operators/wm.py\:1327 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L1327>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param doc_id: Doc ID
     :type doc_id: typing.Union[str, typing.Any]
     '''
@@ -1260,15 +1260,15 @@
 
 def drop_blend_file(override_context: typing.
                     Union[typing.Dict, 'bpy.types.Context'] = None,
                     execution_context: typing.Union[str, int] = None,
                     undo: typing.Optional[bool] = None,
                     *,
                     filepath: typing.Union[str, typing.Any] = ""):
-    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/wm.py\:3311 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L3311>`__
+    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/wm.py\:3314 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L3314>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     '''
@@ -1572,15 +1572,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         name: typing.Union[str, typing.Any] = "",
         remove_name: typing.Union[bool, typing.Any] = False,
         remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove a theme preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove a theme preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
@@ -1597,15 +1597,15 @@
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         name: typing.Union[str, typing.Any] = "",
         remove_name: typing.Union[bool, typing.Any] = False,
         remove_active: typing.Union[bool, typing.Any] = False):
-    ''' Add or remove a Key-config Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove a Key-config Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
@@ -2304,15 +2304,15 @@
     pass
 
 
 def operator_cheat_sheet(override_context: typing.
                          Union[typing.Dict, 'bpy.types.Context'] = None,
                          execution_context: typing.Union[str, int] = None,
                          undo: typing.Optional[bool] = None):
-    ''' List all the operators in a text-block, useful for scripting :File: `startup/bl_operators/wm.py\:2168 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2168>`__
+    ''' List all the operators in a text-block, useful for scripting :File: `startup/bl_operators/wm.py\:2171 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2171>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -2335,15 +2335,15 @@
 def operator_pie_enum(override_context: typing.
                       Union[typing.Dict, 'bpy.types.Context'] = None,
                       execution_context: typing.Union[str, int] = None,
                       undo: typing.Optional[bool] = None,
                       *,
                       data_path: typing.Union[str, typing.Any] = "",
                       prop_string: typing.Union[str, typing.Any] = ""):
-    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/wm.py\:762 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L762>`__
+    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/wm.py\:765 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L765>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Operator, Operator name (in Python as string)
     :type data_path: typing.Union[str, typing.Any]
     :param prop_string: Property, Property name (as a string)
@@ -2358,15 +2358,15 @@
                         execution_context: typing.Union[str, int] = None,
                         undo: typing.Optional[bool] = None,
                         *,
                         name: typing.Union[str, typing.Any] = "",
                         remove_name: typing.Union[bool, typing.Any] = False,
                         remove_active: typing.Union[bool, typing.Any] = False,
                         operator: typing.Union[str, typing.Any] = ""):
-    ''' Add or remove an Operator Preset :File: `startup/bl_operators/presets.py\:73 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L73>`__
+    ''' Add or remove an Operator Preset :File: `startup/bl_operators/presets.py\:75 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/presets.py#L75>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Name, Name of the preset, used to make the path name
     :type name: typing.Union[str, typing.Any]
     :param remove_name: remove_name
@@ -2382,15 +2382,15 @@
 
 def owner_disable(override_context: typing.
                   Union[typing.Dict, 'bpy.types.Context'] = None,
                   execution_context: typing.Union[str, int] = None,
                   undo: typing.Optional[bool] = None,
                   *,
                   owner_id: typing.Union[str, typing.Any] = ""):
-    ''' Disable add-on for workspace :File: `startup/bl_operators/wm.py\:2216 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2216>`__
+    ''' Disable add-on for workspace :File: `startup/bl_operators/wm.py\:2219 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2219>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param owner_id: UI Tag
     :type owner_id: typing.Union[str, typing.Any]
     '''
@@ -2400,15 +2400,15 @@
 
 def owner_enable(override_context: typing.
                  Union[typing.Dict, 'bpy.types.Context'] = None,
                  execution_context: typing.Union[str, int] = None,
                  undo: typing.Optional[bool] = None,
                  *,
                  owner_id: typing.Union[str, typing.Any] = ""):
-    ''' Enable add-on for workspace :File: `startup/bl_operators/wm.py\:2201 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2201>`__
+    ''' Enable add-on for workspace :File: `startup/bl_operators/wm.py\:2204 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2204>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param owner_id: UI Tag
     :type owner_id: typing.Union[str, typing.Any]
     '''
@@ -2418,15 +2418,15 @@
 
 def path_open(override_context: typing.Union[typing.
                                              Dict, 'bpy.types.Context'] = None,
               execution_context: typing.Union[str, int] = None,
               undo: typing.Optional[bool] = None,
               *,
               filepath: typing.Union[str, typing.Any] = ""):
-    ''' Open a path in a file browser :File: `startup/bl_operators/wm.py\:1153 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L1153>`__
+    ''' Open a path in a file browser :File: `startup/bl_operators/wm.py\:1156 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L1156>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     '''
@@ -2671,15 +2671,15 @@
         filter_folder: typing.Union[bool, typing.Any] = True,
         use_scenes: typing.Union[bool, typing.Any] = True,
         use_collections: typing.Union[bool, typing.Any] = True,
         use_objects: typing.Union[bool, typing.Any] = True,
         use_intern_data: typing.Union[bool, typing.Any] = True,
         use_trusted: typing.Union[bool, typing.Any] = False,
         use_backups: typing.Union[bool, typing.Any] = True):
-    ''' Clear selected .blend file's previews :File: `startup/bl_operators/file.py\:203 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/file.py#L203>`__
+    ''' Clear selected .blend file's previews :File: `startup/bl_operators/file.py\:205 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/file.py#L205>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param files: files
     :type files: typing.Optional[bpy.types.bpy_prop_collection['bpy.types.OperatorFileListElement']]
     :param directory: directory
@@ -2718,15 +2718,15 @@
         filter_folder: typing.Union[bool, typing.Any] = True,
         use_scenes: typing.Union[bool, typing.Any] = True,
         use_collections: typing.Union[bool, typing.Any] = True,
         use_objects: typing.Union[bool, typing.Any] = True,
         use_intern_data: typing.Union[bool, typing.Any] = True,
         use_trusted: typing.Union[bool, typing.Any] = False,
         use_backups: typing.Union[bool, typing.Any] = True):
-    ''' Generate selected .blend file's previews :File: `startup/bl_operators/file.py\:93 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/file.py#L93>`__
+    ''' Generate selected .blend file's previews :File: `startup/bl_operators/file.py\:95 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/file.py#L95>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param files: Collection of file paths with common `directory` root
     :type files: typing.Optional[bpy.types.bpy_prop_collection['bpy.types.OperatorFileListElement']]
     :param directory: Root path of all files listed in `files` collection
@@ -2786,15 +2786,15 @@
 
 def properties_add(override_context: typing.
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None,
                    *,
                    data_path: typing.Union[str, typing.Any] = ""):
-    ''' Add your own property to the data-block :File: `startup/bl_operators/wm.py\:2060 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2060>`__
+    ''' Add your own property to the data-block :File: `startup/bl_operators/wm.py\:2063 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2063>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Property Edit, Property data_path edit
     :type data_path: typing.Union[str, typing.Any]
     '''
@@ -2804,15 +2804,15 @@
 
 def properties_context_change(override_context: typing.
                               Union[typing.Dict, 'bpy.types.Context'] = None,
                               execution_context: typing.Union[str, int] = None,
                               undo: typing.Optional[bool] = None,
                               *,
                               context: typing.Union[str, typing.Any] = ""):
-    ''' Jump to a different tab inside the properties editor :File: `startup/bl_operators/wm.py\:2103 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2103>`__
+    ''' Jump to a different tab inside the properties editor :File: `startup/bl_operators/wm.py\:2106 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2106>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param context: Context
     :type context: typing.Union[str, typing.Any]
     '''
@@ -2859,15 +2859,15 @@
         soft_min_float: typing.Optional[typing.Any] = -10000.0,
         soft_max_float: typing.Optional[typing.Any] = -10000.0,
         precision: typing.Optional[typing.Any] = 3,
         step_float: typing.Optional[typing.Any] = 0.1,
         subtype: typing.Union[str, int, typing.Any] = '',
         default_string: typing.Union[str, typing.Any] = "",
         eval_string: typing.Union[str, typing.Any] = ""):
-    ''' Change a custom property's type, or adjust how it is displayed in the interface :File: `startup/bl_operators/wm.py\:1802 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L1802>`__
+    ''' Change a custom property's type, or adjust how it is displayed in the interface :File: `startup/bl_operators/wm.py\:1805 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L1805>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Property Edit, Property data_path edit
     :type data_path: typing.Union[str, typing.Any]
     :param property_name: Property Name, Property name edit
@@ -2925,15 +2925,15 @@
                           Union[typing.Dict, 'bpy.types.Context'] = None,
                           execution_context: typing.Union[str, int] = None,
                           undo: typing.Optional[bool] = None,
                           *,
                           data_path: typing.Union[str, typing.Any] = "",
                           property_name: typing.Union[str, typing.Any] = "",
                           eval_string: typing.Union[str, typing.Any] = ""):
-    ''' Edit the value of a custom property :File: `startup/bl_operators/wm.py\:2016 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2016>`__
+    ''' Edit the value of a custom property :File: `startup/bl_operators/wm.py\:2019 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2019>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Property Edit, Property data_path edit
     :type data_path: typing.Union[str, typing.Any]
     :param property_name: Property Name, Property name edit
@@ -2948,15 +2948,15 @@
 def properties_remove(override_context: typing.
                       Union[typing.Dict, 'bpy.types.Context'] = None,
                       execution_context: typing.Union[str, int] = None,
                       undo: typing.Optional[bool] = None,
                       *,
                       data_path: typing.Union[str, typing.Any] = "",
                       property_name: typing.Union[str, typing.Any] = ""):
-    ''' Internal use (edit a property data_path) :File: `startup/bl_operators/wm.py\:2117 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2117>`__
+    ''' Internal use (edit a property data_path) :File: `startup/bl_operators/wm.py\:2120 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2120>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param data_path: Property Edit, Property data_path edit
     :type data_path: typing.Union[str, typing.Any]
     :param property_name: Property Name, Property name edit
@@ -3703,15 +3703,15 @@
 
 def sysinfo(override_context: typing.Union[typing.
                                            Dict, 'bpy.types.Context'] = None,
             execution_context: typing.Union[str, int] = None,
             undo: typing.Optional[bool] = None,
             *,
             filepath: typing.Union[str, typing.Any] = ""):
-    ''' Generate system information, saved into a text file :File: `startup/bl_operators/wm.py\:2146 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2146>`__
+    ''' Generate system information, saved into a text file :File: `startup/bl_operators/wm.py\:2149 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2149>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     '''
@@ -3724,15 +3724,15 @@
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None,
                    *,
                    name: typing.Union[str, typing.Any] = "",
                    cycle: typing.Union[bool, typing.Any] = False,
                    as_fallback: typing.Union[bool, typing.Any] = False,
                    space_type: typing.Optional[typing.Any] = 'EMPTY'):
-    ''' Set the tool by name (for keymaps) :File: `startup/bl_operators/wm.py\:2247 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2247>`__
+    ''' Set the tool by name (for keymaps) :File: `startup/bl_operators/wm.py\:2250 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2250>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param name: Identifier, Identifier of the tool
     :type name: typing.Union[str, typing.Any]
     :param cycle: Cycle, Cycle through tools in this group
@@ -3752,15 +3752,15 @@
                       undo: typing.Optional[bool] = None,
                       *,
                       index: typing.Optional[typing.Any] = 0,
                       cycle: typing.Union[bool, typing.Any] = False,
                       expand: typing.Union[bool, typing.Any] = True,
                       as_fallback: typing.Union[bool, typing.Any] = False,
                       space_type: typing.Optional[typing.Any] = 'EMPTY'):
-    ''' Set the tool by index (for keymaps) :File: `startup/bl_operators/wm.py\:2299 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2299>`__
+    ''' Set the tool by index (for keymaps) :File: `startup/bl_operators/wm.py\:2302 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2302>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param index: Index in Toolbar
     :type index: typing.Optional[typing.Any]
     :param cycle: Cycle, Cycle through tools in this group
@@ -3776,43 +3776,43 @@
     pass
 
 
 def toolbar(override_context: typing.Union[typing.
                                            Dict, 'bpy.types.Context'] = None,
             execution_context: typing.Union[str, int] = None,
             undo: typing.Optional[bool] = None):
-    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/wm.py\:2354 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2354>`__
+    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/wm.py\:2357 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2357>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def toolbar_fallback_pie(override_context: typing.
                          Union[typing.Dict, 'bpy.types.Context'] = None,
                          execution_context: typing.Union[str, int] = None,
                          undo: typing.Optional[bool] = None):
-    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/wm.py\:2378 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2378>`__
+    ''' Undocumented, consider `contributing <https://developer.blender.org/>`__. :File: `startup/bl_operators/wm.py\:2381 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2381>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def toolbar_prompt(override_context: typing.
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None):
-    ''' Leader key like functionality for accessing tools :File: `startup/bl_operators/wm.py\:2478 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2478>`__
+    ''' Leader key like functionality for accessing tools :File: `startup/bl_operators/wm.py\:2481 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L2481>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -3820,15 +3820,15 @@
 
 def url_open(override_context: typing.Union[typing.
                                             Dict, 'bpy.types.Context'] = None,
              execution_context: typing.Union[str, int] = None,
              undo: typing.Optional[bool] = None,
              *,
              url: typing.Union[str, typing.Any] = ""):
-    ''' Open a website in the web browser :File: `startup/bl_operators/wm.py\:1054 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L1054>`__
+    ''' Open a website in the web browser :File: `startup/bl_operators/wm.py\:1057 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L1057>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param url: URL, URL to open
     :type url: typing.Union[str, typing.Any]
     '''
@@ -3839,15 +3839,15 @@
 def url_open_preset(override_context: typing.
                     Union[typing.Dict, 'bpy.types.Context'] = None,
                     execution_context: typing.Union[str, int] = None,
                     undo: typing.Optional[bool] = None,
                     *,
                     type: typing.Union[str, int, typing.Any] = '',
                     id: typing.Union[str, typing.Any] = ""):
-    ''' Open a preset website in the web browser :File: `startup/bl_operators/wm.py\:1130 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L1130>`__
+    ''' Open a preset website in the web browser :File: `startup/bl_operators/wm.py\:1133 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/wm.py#L1133>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param type: Site
     :type type: typing.Union[str, int, typing.Any]
     :param id: Identifier, Optional identifier
```

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/workspace.py` & `fake-bpy-module-latest-20230616/bpy/ops/workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/ops/world.py` & `fake-bpy-module-latest-20230616/bpy/ops/world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/path.py` & `fake-bpy-module-latest-20230616/bpy/path.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/props.py` & `fake-bpy-module-latest-20230616/bpy/props.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/types.py` & `fake-bpy-module-latest-20230616/bpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,1055 +1,1055 @@
 00000000: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
 00000010: 7420 7479 7069 6e67 0a69 6d70 6f72 7420  t typing.import 
 00000020: 6d61 7468 7574 696c 730a 696d 706f 7274  mathutils.import
-00000030: 2062 7079 0a69 6d70 6f72 7420 626c 5f6f   bpy.import bl_o
-00000040: 7065 7261 746f 7273 2e70 7265 7365 7473  perators.presets
-00000050: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000060: 6f70 6572 7469 6573 5f64 6174 615f 706f  operties_data_po
-00000070: 696e 7463 6c6f 7564 0a69 6d70 6f72 7420  intcloud.import 
-00000080: 626c 5f75 690a 696d 706f 7274 2062 6c5f  bl_ui.import bl_
-00000090: 7569 2e73 7061 6365 5f69 6d61 6765 0a69  ui.space_image.i
-000000a0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-000000b0: 6572 7469 6573 5f64 6174 615f 6d65 7368  erties_data_mesh
-000000c0: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-000000d0: 746f 7273 2e74 6578 740a 696d 706f 7274  tors.text.import
-000000e0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-000000f0: 735f 776f 726c 640a 696d 706f 7274 2062  s_world.import b
-00000100: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000110: 636f 6c6c 6563 7469 6f6e 0a69 6d70 6f72  collection.impor
-00000120: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000130: 6573 5f64 6174 615f 6c69 6768 740a 696d  es_data_light.im
-00000140: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-00000150: 5f75 7365 7270 7265 660a 696d 706f 7274  _userpref.import
-00000160: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000170: 735f 6461 7461 5f6c 6967 6874 7072 6f62  s_data_lightprob
-00000180: 650a 696d 706f 7274 2062 6c5f 7569 2e70  e.import bl_ui.p
-00000190: 726f 7065 7274 6965 735f 6461 7461 5f73  roperties_data_s
-000001a0: 6861 6465 7266 780a 696d 706f 7274 2062  haderfx.import b
-000001b0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-000001c0: 6461 7461 5f6c 6174 7469 6365 0a69 6d70  data_lattice.imp
-000001d0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-000001e0: 7469 6573 5f64 6174 615f 6375 7276 650a  ties_data_curve.
-000001f0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000200: 7065 7274 6965 735f 7068 7973 6963 735f  perties_physics_
-00000210: 736f 6674 626f 6479 0a69 6d70 6f72 7420  softbody.import 
-00000220: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000230: 5f64 6174 615f 7370 6561 6b65 720a 696d  _data_speaker.im
-00000240: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000250: 7274 6965 735f 636f 6e73 7472 6169 6e74  rties_constraint
-00000260: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-00000270: 6163 655f 646f 7065 7368 6565 740a 696d  ace_dopesheet.im
-00000280: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000290: 7274 6965 735f 7068 7973 6963 735f 636f  rties_physics_co
-000002a0: 6d6d 6f6e 0a69 6d70 6f72 7420 626c 5f75  mmon.import bl_u
-000002b0: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
-000002c0: 7369 6373 5f66 6c75 6964 0a69 6d70 6f72  sics_fluid.impor
-000002d0: 7420 626c 5f6f 7065 7261 746f 7273 2e66  t bl_operators.f
-000002e0: 696c 650a 696d 706f 7274 2062 6c5f 7569  ile.import bl_ui
-000002f0: 2e73 7061 6365 5f74 6f6f 6c73 7973 7465  .space_toolsyste
-00000300: 6d5f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  m_common.import 
-00000310: 626c 5f75 692e 7370 6163 655f 7072 6f70  bl_ui.space_prop
-00000320: 6572 7469 6573 0a69 6d70 6f72 7420 626c  erties.import bl
-00000330: 5f6f 7065 7261 746f 7273 2e73 7072 6561  _operators.sprea
-00000340: 6473 6865 6574 0a69 6d70 6f72 7420 626c  dsheet.import bl
-00000350: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
-00000360: 6174 615f 6d65 7461 6261 6c6c 0a69 6d70  ata_metaball.imp
-00000370: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000380: 7469 6573 5f67 7265 6173 655f 7065 6e63  ties_grease_penc
-00000390: 696c 5f63 6f6d 6d6f 6e0a 696d 706f 7274  il_common.import
-000003a0: 2062 6c5f 7569 2e73 7061 6365 5f76 6965   bl_ui.space_vie
-000003b0: 7733 640a 696d 706f 7274 2062 6c5f 7569  w3d.import bl_ui
-000003c0: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
-000003d0: 5f63 7572 7665 730a 696d 706f 7274 2062  _curves.import b
+00000030: 2062 7079 0a69 6d70 6f72 7420 626c 5f75   bpy.import bl_u
+00000040: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000050: 615f 766f 6c75 6d65 0a69 6d70 6f72 7420  a_volume.import 
+00000060: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000070: 5f76 6965 775f 6c61 7965 720a 696d 706f  _view_layer.impo
+00000080: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000090: 6965 735f 7068 7973 6963 735f 6669 656c  ies_physics_fiel
+000000a0: 640a 696d 706f 7274 2062 6c5f 7569 2e73  d.import bl_ui.s
+000000b0: 7061 6365 5f69 6d61 6765 0a69 6d70 6f72  pace_image.impor
+000000c0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+000000d0: 6573 5f70 6879 7369 6373 5f64 796e 616d  es_physics_dynam
+000000e0: 6963 7061 696e 740a 696d 706f 7274 2062  icpaint.import b
+000000f0: 6c5f 7569 2e73 7061 6365 5f66 696c 6562  l_ui.space_fileb
+00000100: 726f 7773 6572 0a69 6d70 6f72 7420 626c  rowser.import bl
+00000110: 5f6f 7065 7261 746f 7273 2e73 7072 6561  _operators.sprea
+00000120: 6473 6865 6574 0a69 6d70 6f72 7420 626c  dsheet.import bl
+00000130: 5f75 692e 7072 6f70 6572 7469 6573 5f70  _ui.properties_p
+00000140: 6879 7369 6373 5f72 6967 6964 626f 6479  hysics_rigidbody
+00000150: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000160: 6f70 6572 7469 6573 5f70 6879 7369 6373  operties_physics
+00000170: 5f63 6f6d 6d6f 6e0a 696d 706f 7274 2062  _common.import b
+00000180: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000190: 7068 7973 6963 735f 7269 6769 6462 6f64  physics_rigidbod
+000001a0: 795f 636f 6e73 7472 6169 6e74 0a69 6d70  y_constraint.imp
+000001b0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+000001c0: 7469 6573 5f6d 6174 6572 6961 6c0a 696d  ties_material.im
+000001d0: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+000001e0: 5f74 6578 740a 696d 706f 7274 2062 6c5f  _text.import bl_
+000001f0: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
+00000200: 7973 6963 735f 636c 6f74 680a 696d 706f  ysics_cloth.impo
+00000210: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
+00000220: 7465 7874 0a69 6d70 6f72 7420 626c 5f75  text.import bl_u
+00000230: 692e 7072 6f70 6572 7469 6573 5f6d 6174  i.properties_mat
+00000240: 6572 6961 6c5f 6770 656e 6369 6c0a 696d  erial_gpencil.im
+00000250: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000260: 7274 6965 735f 7068 7973 6963 735f 736f  rties_physics_so
+00000270: 6674 626f 6479 0a69 6d70 6f72 7420 626c  ftbody.import bl
+00000280: 5f75 692e 7370 6163 655f 636c 6970 0a69  _ui.space_clip.i
+00000290: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+000002a0: 7273 2e77 6d0a 696d 706f 7274 2062 6c5f  rs.wm.import bl_
+000002b0: 7569 2e73 7061 6365 5f70 726f 7065 7274  ui.space_propert
+000002c0: 6965 730a 696d 706f 7274 2062 6c5f 7569  ies.import bl_ui
+000002d0: 2e73 7061 6365 5f73 7072 6561 6473 6865  .space_spreadshe
+000002e0: 6574 0a69 6d70 6f72 7420 626c 5f75 692e  et.import bl_ui.
+000002f0: 7370 6163 655f 7573 6572 7072 6566 0a69  space_userpref.i
+00000300: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000310: 6572 7469 6573 5f74 6578 7475 7265 0a69  erties_texture.i
+00000320: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+00000330: 7273 2e76 6965 7733 640a 696d 706f 7274  rs.view3d.import
+00000340: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000350: 735f 6461 7461 5f63 7572 7665 730a 696d  s_data_curves.im
+00000360: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000370: 7274 6965 735f 6461 7461 5f73 7065 616b  rties_data_speak
+00000380: 6572 0a69 6d70 6f72 7420 626c 5f75 692e  er.import bl_ui.
+00000390: 7370 6163 655f 7669 6577 3364 0a69 6d70  space_view3d.imp
+000003a0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+000003b0: 7669 6577 3364 5f74 6f6f 6c62 6172 0a69  view3d_toolbar.i
+000003c0: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+000003d0: 7273 2e66 696c 650a 696d 706f 7274 2062  rs.file.import b
 000003e0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-000003f0: 6461 7461 5f76 6f6c 756d 650a 696d 706f  data_volume.impo
+000003f0: 6461 7461 5f63 616d 6572 610a 696d 706f  data_camera.impo
 00000400: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000410: 6965 735f 6f62 6a65 6374 0a69 6d70 6f72  ies_object.impor
-00000420: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000430: 6573 5f64 6174 615f 6d6f 6469 6669 6572  es_data_modifier
-00000440: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-00000450: 6163 655f 6e6f 6465 0a69 6d70 6f72 7420  ace_node.import 
-00000460: 626c 5f75 692e 7370 6163 655f 7370 7265  bl_ui.space_spre
-00000470: 6164 7368 6565 740a 696d 706f 7274 2062  adsheet.import b
-00000480: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000490: 7068 7973 6963 735f 7269 6769 6462 6f64  physics_rigidbod
-000004a0: 790a 696d 706f 7274 2062 6c5f 7569 2e70  y.import bl_ui.p
-000004b0: 726f 7065 7274 6965 735f 6461 7461 5f67  roperties_data_g
-000004c0: 7065 6e63 696c 0a69 6d70 6f72 7420 626c  pencil.import bl
-000004d0: 5f6f 7065 7261 746f 7273 2e76 6965 7733  _operators.view3
-000004e0: 640a 696d 706f 7274 2062 6c5f 7569 2e73  d.import bl_ui.s
-000004f0: 7061 6365 5f6e 6c61 0a69 6d70 6f72 7420  pace_nla.import 
-00000500: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000510: 5f6d 6174 6572 6961 6c5f 6770 656e 6369  _material_gpenci
-00000520: 6c0a 696d 706f 7274 2062 6c5f 7569 2e67  l.import bl_ui.g
-00000530: 656e 6572 6963 5f75 695f 6c69 7374 0a69  eneric_ui_list.i
-00000540: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000550: 6572 7469 6573 5f70 6169 6e74 5f63 6f6d  erties_paint_com
-00000560: 6d6f 6e0a 696d 706f 7274 2062 6c5f 7569  mon.import bl_ui
-00000570: 2e73 7061 6365 5f74 6578 740a 696d 706f  .space_text.impo
-00000580: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000590: 6965 735f 6461 7461 5f65 6d70 7479 0a69  ies_data_empty.i
-000005a0: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-000005b0: 655f 7374 6174 7573 6261 720a 696d 706f  e_statusbar.impo
-000005c0: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
-000005d0: 7573 6572 7072 6566 0a69 6d70 6f72 7420  userpref.import 
-000005e0: 626c 5f75 692e 7370 6163 655f 6f75 746c  bl_ui.space_outl
-000005f0: 696e 6572 0a69 6d70 6f72 7420 626c 5f6f  iner.import bl_o
-00000600: 7065 7261 746f 7273 2e77 6d0a 696d 706f  perators.wm.impo
-00000610: 7274 2062 6c5f 7569 2e73 7061 6365 5f73  rt bl_ui.space_s
-00000620: 6571 7565 6e63 6572 0a69 6d70 6f72 7420  equencer.import 
-00000630: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000640: 5f72 656e 6465 720a 696d 706f 7274 2062  _render.import b
-00000650: 6c5f 6f70 6572 6174 6f72 732e 6e6f 6465  l_operators.node
-00000660: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-00000670: 746f 7273 2e63 6f6e 7374 7261 696e 740a  tors.constraint.
-00000680: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-00000690: 6365 5f63 6c69 700a 696d 706f 7274 2062  ce_clip.import b
-000006a0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-000006b0: 7068 7973 6963 735f 636c 6f74 680a 696d  physics_cloth.im
-000006c0: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-000006d0: 7274 6965 735f 6d61 7465 7269 616c 0a69  rties_material.i
-000006e0: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-000006f0: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00000700: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-00000710: 746f 7273 2e66 7265 6573 7479 6c65 0a69  tors.freestyle.i
-00000720: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
-00000730: 7273 2e61 6e69 6d0a 696d 706f 7274 2062  rs.anim.import b
-00000740: 6c5f 7569 2e73 7061 6365 5f74 696d 650a  l_ui.space_time.
-00000750: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-00000760: 6365 5f63 6f6e 736f 6c65 0a69 6d70 6f72  ce_console.impor
-00000770: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000780: 6573 5f74 6578 7475 7265 0a69 6d70 6f72  es_texture.impor
-00000790: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-000007a0: 6573 5f66 7265 6573 7479 6c65 0a69 6d70  es_freestyle.imp
-000007b0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-000007c0: 7469 6573 5f64 6174 615f 626f 6e65 0a69  ties_data_bone.i
-000007d0: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
-000007e0: 7273 2e6f 626a 6563 740a 696d 706f 7274  rs.object.import
-000007f0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000800: 735f 6f75 7470 7574 0a69 6d70 6f72 7420  s_output.import 
-00000810: 626c 5f75 692e 7370 6163 655f 746f 6f6c  bl_ui.space_tool
-00000820: 7379 7374 656d 5f74 6f6f 6c62 6172 0a69  system_toolbar.i
-00000830: 6d70 6f72 7420 626c 5f75 692e 6e6f 6465  mport bl_ui.node
-00000840: 5f61 6464 5f6d 656e 755f 6765 6f6d 6574  _add_menu_geomet
-00000850: 7279 0a69 6d70 6f72 7420 626c 5f75 692e  ry.import bl_ui.
-00000860: 7072 6f70 6572 7469 6573 5f70 6172 7469  properties_parti
-00000870: 636c 650a 696d 706f 7274 2062 6c5f 7569  cle.import bl_ui
-00000880: 2e70 726f 7065 7274 6965 735f 7068 7973  .properties_phys
-00000890: 6963 735f 6479 6e61 6d69 6370 6169 6e74  ics_dynamicpaint
-000008a0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-000008b0: 6f70 6572 7469 6573 5f77 6f72 6b73 7061  operties_workspa
-000008c0: 6365 0a69 6d70 6f72 7420 626c 5f75 692e  ce.import bl_ui.
-000008d0: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
-000008e0: 6373 5f66 6965 6c64 0a69 6d70 6f72 7420  cs_field.import 
-000008f0: 626c 5f6f 7065 7261 746f 7273 2e63 6c69  bl_operators.cli
-00000900: 700a 696d 706f 7274 2062 6c5f 7569 2e73  p.import bl_ui.s
-00000910: 7061 6365 5f67 7261 7068 0a69 6d70 6f72  pace_graph.impor
-00000920: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000930: 6573 5f64 6174 615f 6172 6d61 7475 7265  es_data_armature
-00000940: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000950: 6f70 6572 7469 6573 5f70 6879 7369 6373  operties_physics
-00000960: 5f72 6967 6964 626f 6479 5f63 6f6e 7374  _rigidbody_const
-00000970: 7261 696e 740a 696d 706f 7274 2062 6c5f  raint.import bl_
-00000980: 7569 2e73 7061 6365 5f66 696c 6562 726f  ui.space_filebro
-00000990: 7773 6572 0a69 6d70 6f72 7420 626c 5f75  wser.import bl_u
-000009a0: 692e 7370 6163 655f 696e 666f 0a69 6d70  i.space_info.imp
-000009b0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-000009c0: 7469 6573 5f6d 6173 6b5f 636f 6d6d 6f6e  ties_mask_common
-000009d0: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-000009e0: 6163 655f 746f 7062 6172 0a69 6d70 6f72  ace_topbar.impor
-000009f0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000a00: 6573 5f76 6965 775f 6c61 7965 720a 696d  es_view_layer.im
-00000a10: 706f 7274 2062 6c5f 6f70 6572 6174 6f72  port bl_operator
-00000a20: 732e 6173 7365 7473 0a69 6d70 6f72 7420  s.assets.import 
-00000a30: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000a40: 5f64 6174 615f 6361 6d65 7261 0a69 6d70  _data_camera.imp
-00000a50: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000a60: 7469 6573 5f73 6365 6e65 0a69 6d70 6f72  ties_scene.impor
-00000a70: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000a80: 6573 5f70 6879 7369 6373 5f67 656f 6d65  es_physics_geome
-00000a90: 7472 795f 6e6f 6465 730a 0a47 656e 6572  try_nodes..Gener
+00000410: 6965 735f 7068 7973 6963 735f 6765 6f6d  ies_physics_geom
+00000420: 6574 7279 5f6e 6f64 6573 0a69 6d70 6f72  etry_nodes.impor
+00000430: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+00000440: 6573 5f64 6174 615f 626f 6e65 0a69 6d70  es_data_bone.imp
+00000450: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
+00000460: 2e6f 626a 6563 740a 696d 706f 7274 2062  .object.import b
+00000470: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000480: 7061 696e 745f 636f 6d6d 6f6e 0a69 6d70  paint_common.imp
+00000490: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
+000004a0: 2e61 6e69 6d0a 696d 706f 7274 2062 6c5f  .anim.import bl_
+000004b0: 7569 2e73 7061 6365 5f74 696d 650a 696d  ui.space_time.im
+000004c0: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+000004d0: 7274 6965 735f 6461 7461 5f6c 6967 6874  rties_data_light
+000004e0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+000004f0: 6f70 6572 7469 6573 5f64 6174 615f 6c61  operties_data_la
+00000500: 7474 6963 650a 696d 706f 7274 2062 6c5f  ttice.import bl_
+00000510: 7569 2e73 7061 6365 5f74 6f6f 6c73 7973  ui.space_toolsys
+00000520: 7465 6d5f 746f 6f6c 6261 720a 696d 706f  tem_toolbar.impo
+00000530: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
+00000540: 6672 6565 7374 796c 650a 696d 706f 7274  freestyle.import
+00000550: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000560: 735f 7265 6e64 6572 0a69 6d70 6f72 7420  s_render.import 
+00000570: 626c 5f75 692e 7370 6163 655f 746f 6f6c  bl_ui.space_tool
+00000580: 7379 7374 656d 5f63 6f6d 6d6f 6e0a 696d  system_common.im
+00000590: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+000005a0: 7274 6965 735f 6461 7461 5f6d 6573 680a  rties_data_mesh.
+000005b0: 696d 706f 7274 2062 6c5f 7569 2e67 656e  import bl_ui.gen
+000005c0: 6572 6963 5f75 695f 6c69 7374 0a69 6d70  eric_ui_list.imp
+000005d0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+000005e0: 7469 6573 5f64 6174 615f 6d6f 6469 6669  ties_data_modifi
+000005f0: 6572 0a69 6d70 6f72 7420 626c 5f75 692e  er.import bl_ui.
+00000600: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
+00000610: 6172 6d61 7475 7265 0a69 6d70 6f72 7420  armature.import 
+00000620: 626c 5f75 692e 7370 6163 655f 7365 7175  bl_ui.space_sequ
+00000630: 656e 6365 720a 696d 706f 7274 2062 6c5f  encer.import bl_
+00000640: 7569 2e70 726f 7065 7274 6965 735f 636f  ui.properties_co
+00000650: 6e73 7472 6169 6e74 0a69 6d70 6f72 7420  nstraint.import 
+00000660: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000670: 5f64 6174 615f 6d65 7461 6261 6c6c 0a69  _data_metaball.i
+00000680: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000690: 6572 7469 6573 5f70 6879 7369 6373 5f66  erties_physics_f
+000006a0: 6c75 6964 0a69 6d70 6f72 7420 626c 5f75  luid.import bl_u
+000006b0: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+000006c0: 615f 706f 696e 7463 6c6f 7564 0a69 6d70  a_pointcloud.imp
+000006d0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+000006e0: 646f 7065 7368 6565 740a 696d 706f 7274  dopesheet.import
+000006f0: 2062 6c5f 7569 2e73 7061 6365 5f74 6f70   bl_ui.space_top
+00000700: 6261 720a 696d 706f 7274 2062 6c5f 7569  bar.import bl_ui
+00000710: 2e6e 6f64 655f 6164 645f 6d65 6e75 5f67  .node_add_menu_g
+00000720: 656f 6d65 7472 790a 696d 706f 7274 2062  eometry.import b
+00000730: 6c5f 7569 2e73 7061 6365 5f67 7261 7068  l_ui.space_graph
+00000740: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000750: 6f70 6572 7469 6573 5f67 7265 6173 655f  operties_grease_
+00000760: 7065 6e63 696c 5f63 6f6d 6d6f 6e0a 696d  pencil_common.im
+00000770: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000780: 7274 6965 735f 776f 726c 640a 696d 706f  rties_world.impo
+00000790: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000007a0: 6965 735f 776f 726b 7370 6163 650a 696d  ies_workspace.im
+000007b0: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+000007c0: 5f6e 6c61 0a69 6d70 6f72 7420 626c 5f6f  _nla.import bl_o
+000007d0: 7065 7261 746f 7273 2e61 7373 6574 730a  perators.assets.
+000007e0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+000007f0: 6365 5f73 7461 7475 7362 6172 0a69 6d70  ce_statusbar.imp
+00000800: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
+00000810: 2e6e 6f64 650a 696d 706f 7274 2062 6c5f  .node.import bl_
+00000820: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+00000830: 7461 5f73 6861 6465 7266 780a 696d 706f  ta_shaderfx.impo
+00000840: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000850: 6965 735f 6f75 7470 7574 0a69 6d70 6f72  ies_output.impor
+00000860: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+00000870: 6573 5f6d 6173 6b5f 636f 6d6d 6f6e 0a69  es_mask_common.i
+00000880: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000890: 6572 7469 6573 5f64 6174 615f 6c69 6768  erties_data_ligh
+000008a0: 7470 726f 6265 0a69 6d70 6f72 7420 626c  tprobe.import bl
+000008b0: 5f75 692e 7072 6f70 6572 7469 6573 5f63  _ui.properties_c
+000008c0: 6f6c 6c65 6374 696f 6e0a 696d 706f 7274  ollection.import
+000008d0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+000008e0: 735f 7363 656e 650a 696d 706f 7274 2062  s_scene.import b
+000008f0: 6c5f 7569 2e73 7061 6365 5f6f 7574 6c69  l_ui.space_outli
+00000900: 6e65 720a 696d 706f 7274 2062 6c5f 6f70  ner.import bl_op
+00000910: 6572 6174 6f72 732e 7072 6573 6574 730a  erators.presets.
+00000920: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+00000930: 6365 5f6e 6f64 650a 696d 706f 7274 2062  ce_node.import b
+00000940: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000950: 7061 7274 6963 6c65 0a69 6d70 6f72 7420  particle.import 
+00000960: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000970: 5f64 6174 615f 6770 656e 6369 6c0a 696d  _data_gpencil.im
+00000980: 706f 7274 2062 6c5f 6f70 6572 6174 6f72  port bl_operator
+00000990: 732e 636c 6970 0a69 6d70 6f72 7420 626c  s.clip.import bl
+000009a0: 5f6f 7065 7261 746f 7273 2e63 6f6e 7374  _operators.const
+000009b0: 7261 696e 740a 696d 706f 7274 2062 6c5f  raint.import bl_
+000009c0: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+000009d0: 7461 5f65 6d70 7479 0a69 6d70 6f72 7420  ta_empty.import 
+000009e0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+000009f0: 5f6f 626a 6563 740a 696d 706f 7274 2062  _object.import b
+00000a00: 6c5f 7569 2e73 7061 6365 5f69 6e66 6f0a  l_ui.space_info.
+00000a10: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+00000a20: 7065 7274 6965 735f 6672 6565 7374 796c  perties_freestyl
+00000a30: 650a 696d 706f 7274 2062 6c5f 6f70 6572  e.import bl_oper
+00000a40: 6174 6f72 732e 7573 6572 7072 6566 0a69  ators.userpref.i
+00000a50: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000a60: 6572 7469 6573 5f64 6174 615f 6375 7276  erties_data_curv
+00000a70: 650a 696d 706f 7274 2062 6c5f 7569 2e73  e.import bl_ui.s
+00000a80: 7061 6365 5f63 6f6e 736f 6c65 0a69 6d70  pace_console.imp
+00000a90: 6f72 7420 626c 5f75 690a 0a47 656e 6572  ort bl_ui..Gener
 00000aa0: 6963 5479 7065 203d 2074 7970 696e 672e  icType = typing.
 00000ab0: 5479 7065 5661 7228 2247 656e 6572 6963  TypeVar("Generic
 00000ac0: 5479 7065 2229 0a0a 0a63 6c61 7373 2062  Type")...class b
-00000ad0: 7079 5f70 726f 705f 636f 6c6c 6563 7469  py_prop_collecti
-00000ae0: 6f6e 2874 7970 696e 672e 4765 6e65 7269  on(typing.Generi
-00000af0: 635b 4765 6e65 7269 6354 7970 655d 293a  c[GenericType]):
-00000b00: 0a20 2020 2027 2727 2062 7569 6c74 2d69  .    ''' built-i
-00000b10: 6e20 636c 6173 7320 7573 6564 2066 6f72  n class used for
-00000b20: 2061 6c6c 2063 6f6c 6c65 6374 696f 6e73   all collections
-00000b30: 2e0a 2020 2020 2727 270a 0a20 2020 2064  ..    '''..    d
-00000b40: 6566 2066 696e 6428 7365 6c66 2c20 6b65  ef find(self, ke
-00000b50: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
-00000b60: 616c 5b73 7472 5d29 202d 3e20 696e 743a  al[str]) -> int:
-00000b70: 0a20 2020 2020 2020 2027 2727 2052 6574  .        ''' Ret
-00000b80: 7572 6e73 2074 6865 2069 6e64 6578 206f  urns the index o
-00000b90: 6620 6120 6b65 7920 696e 2061 2063 6f6c  f a key in a col
-00000ba0: 6c65 6374 696f 6e20 6f72 202d 3120 7768  lection or -1 wh
-00000bb0: 656e 206e 6f74 2066 6f75 6e64 2028 6d61  en not found (ma
-00000bc0: 7463 6865 7320 5079 7468 6f6e 2773 2073  tches Python's s
-00000bd0: 7472 696e 6720 6669 6e64 2066 756e 6374  tring find funct
-00000be0: 696f 6e20 6f66 2074 6865 2073 616d 6520  ion of the same 
-00000bf0: 6e61 6d65 292e 0a0a 2020 2020 2020 2020  name)...        
-00000c00: 3a70 6172 616d 206b 6579 3a20 5468 6520  :param key: The 
-00000c10: 6964 656e 7469 6669 6572 2066 6f72 2074  identifier for t
-00000c20: 6865 2063 6f6c 6c65 6374 696f 6e20 6d65  he collection me
-00000c30: 6d62 6572 2e0a 2020 2020 2020 2020 3a74  mber..        :t
-00000c40: 7970 6520 6b65 793a 2074 7970 696e 672e  ype key: typing.
-00000c50: 4f70 7469 6f6e 616c 5b73 7472 5d0a 2020  Optional[str].  
-00000c60: 2020 2020 2020 3a72 7479 7065 3a20 696e        :rtype: in
-00000c70: 740a 2020 2020 2020 2020 3a72 6574 7572  t.        :retur
-00000c80: 6e3a 2069 6e64 6578 206f 6620 7468 6520  n: index of the 
-00000c90: 6b65 792e 0a20 2020 2020 2020 2027 2727  key..        '''
-00000ca0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00000cb0: 2020 2064 6566 2066 6f72 6561 6368 5f67     def foreach_g
-00000cc0: 6574 2873 656c 662c 2061 7474 722c 2073  et(self, attr, s
-00000cd0: 6571 293a 0a20 2020 2020 2020 2027 2727  eq):.        '''
-00000ce0: 2054 6869 7320 6973 2061 2066 756e 6374   This is a funct
-00000cf0: 696f 6e20 746f 2067 6976 6520 6661 7374  ion to give fast
-00000d00: 2061 6363 6573 7320 746f 2061 7474 7269   access to attri
-00000d10: 6275 7465 7320 7769 7468 696e 2061 2063  butes within a c
-00000d20: 6f6c 6c65 6374 696f 6e2e 204f 6e6c 7920  ollection. Only 
-00000d30: 776f 726b 7320 666f 7220 2762 6173 6963  works for 'basic
-00000d40: 2074 7970 6527 2070 726f 7065 7274 6965   type' propertie
-00000d50: 7320 2862 6f6f 6c2c 2069 6e74 2061 6e64  s (bool, int and
-00000d60: 2066 6c6f 6174 2921 204d 756c 7469 2d64   float)! Multi-d
-00000d70: 696d 656e 7369 6f6e 616c 2061 7272 6179  imensional array
-00000d80: 7320 286c 696b 6520 6172 7261 7920 6f66  s (like array of
-00000d90: 2076 6563 746f 7273 2920 7769 6c6c 2062   vectors) will b
-00000da0: 6520 666c 6174 7465 6e65 6420 696e 746f  e flattened into
-00000db0: 2073 6571 2e0a 0a20 2020 2020 2020 2027   seq...        '
-00000dc0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-00000dd0: 0a20 2020 2064 6566 2066 6f72 6561 6368  .    def foreach
-00000de0: 5f73 6574 2873 656c 662c 2061 7474 722c  _set(self, attr,
-00000df0: 2073 6571 293a 0a20 2020 2020 2020 2027   seq):.        '
-00000e00: 2727 2054 6869 7320 6973 2061 2066 756e  '' This is a fun
-00000e10: 6374 696f 6e20 746f 2067 6976 6520 6661  ction to give fa
-00000e20: 7374 2061 6363 6573 7320 746f 2061 7474  st access to att
-00000e30: 7269 6275 7465 7320 7769 7468 696e 2061  ributes within a
-00000e40: 2063 6f6c 6c65 6374 696f 6e2e 204f 6e6c   collection. Onl
-00000e50: 7920 776f 726b 7320 666f 7220 2762 6173  y works for 'bas
-00000e60: 6963 2074 7970 6527 2070 726f 7065 7274  ic type' propert
-00000e70: 6965 7320 2862 6f6f 6c2c 2069 6e74 2061  ies (bool, int a
-00000e80: 6e64 2066 6c6f 6174 2921 2073 6571 206d  nd float)! seq m
-00000e90: 7573 7420 6265 2075 6e69 2d64 696d 656e  ust be uni-dimen
-00000ea0: 7369 6f6e 616c 2c20 6d75 6c74 692d 6469  sional, multi-di
-00000eb0: 6d65 6e73 696f 6e61 6c20 6172 7261 7973  mensional arrays
-00000ec0: 2028 6c69 6b65 2061 7272 6179 206f 6620   (like array of 
-00000ed0: 7665 6374 6f72 7329 2077 696c 6c20 6265  vectors) will be
-00000ee0: 2072 652d 6372 6561 7465 6420 6672 6f6d   re-created from
-00000ef0: 2069 742e 0a0a 2020 2020 2020 2020 2727   it...        ''
-00000f00: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00000f10: 2020 2020 6465 6620 6765 7428 7365 6c66      def get(self
-00000f20: 2c0a 2020 2020 2020 2020 2020 2020 6b65  ,.            ke
-00000f30: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
-00000f40: 616c 5b73 7472 5d2c 0a20 2020 2020 2020  al[str],.       
-00000f50: 2020 2020 2064 6566 6175 6c74 3a20 7479       default: ty
-00000f60: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-00000f70: 7069 6e67 2e41 6e79 5d20 3d20 4e6f 6e65  ping.Any] = None
-00000f80: 293a 0a20 2020 2020 2020 2027 2727 2052  ):.        ''' R
-00000f90: 6574 7572 6e73 2074 6865 2076 616c 7565  eturns the value
-00000fa0: 206f 6620 7468 6520 6974 656d 2061 7373   of the item ass
-00000fb0: 6967 6e65 6420 746f 206b 6579 206f 7220  igned to key or 
-00000fc0: 6465 6661 756c 7420 7768 656e 206e 6f74  default when not
-00000fd0: 2066 6f75 6e64 2028 6d61 7463 6865 7320   found (matches 
-00000fe0: 5079 7468 6f6e 2773 2064 6963 7469 6f6e  Python's diction
-00000ff0: 6172 7920 6675 6e63 7469 6f6e 206f 6620  ary function of 
-00001000: 7468 6520 7361 6d65 206e 616d 6529 2e0a  the same name)..
-00001010: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001020: 6b65 793a 2054 6865 2069 6465 6e74 6966  key: The identif
-00001030: 6965 7220 666f 7220 7468 6520 636f 6c6c  ier for the coll
-00001040: 6563 7469 6f6e 206d 656d 6265 722e 0a20  ection member.. 
-00001050: 2020 2020 2020 203a 7479 7065 206b 6579         :type key
-00001060: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00001070: 6c5b 7374 725d 0a20 2020 2020 2020 203a  l[str].        :
-00001080: 7061 7261 6d20 6465 6661 756c 743a 204f  param default: O
-00001090: 7074 696f 6e61 6c20 6172 6775 6d65 6e74  ptional argument
-000010a0: 2066 6f72 2074 6865 2076 616c 7565 2074   for the value t
-000010b0: 6f20 7265 7475 726e 2069 6620 2a6b 6579  o return if *key
-000010c0: 2a20 6973 206e 6f74 2066 6f75 6e64 2e0a  * is not found..
-000010d0: 2020 2020 2020 2020 3a74 7970 6520 6465          :type de
-000010e0: 6661 756c 743a 2074 7970 696e 672e 4f70  fault: typing.Op
-000010f0: 7469 6f6e 616c 5b74 7970 696e 672e 416e  tional[typing.An
-00001100: 795d 0a20 2020 2020 2020 2027 2727 0a20  y].        '''. 
-00001110: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00001120: 2064 6566 2069 7465 6d73 2873 656c 6629   def items(self)
-00001130: 202d 3e20 7479 7069 6e67 2e4c 6973 743a   -> typing.List:
-00001140: 0a20 2020 2020 2020 2027 2727 2052 6574  .        ''' Ret
-00001150: 7572 6e20 7468 6520 6964 656e 7469 6669  urn the identifi
-00001160: 6572 7320 6f66 2063 6f6c 6c65 6374 696f  ers of collectio
-00001170: 6e20 6d65 6d62 6572 7320 286d 6174 6368  n members (match
-00001180: 696e 6720 5079 7468 6f6e 2773 2064 6963  ing Python's dic
-00001190: 742e 6974 656d 7328 2920 6675 6e63 7469  t.items() functi
-000011a0: 6f6e 616c 6974 7929 2e0a 0a20 2020 2020  onality)...     
-000011b0: 2020 203a 7274 7970 653a 2074 7970 696e     :rtype: typin
-000011c0: 672e 4c69 7374 0a20 2020 2020 2020 203a  g.List.        :
-000011d0: 7265 7475 726e 3a20 286b 6579 2c20 7661  return: (key, va
-000011e0: 6c75 6529 2070 6169 7273 2066 6f72 2065  lue) pairs for e
-000011f0: 6163 6820 6d65 6d62 6572 206f 6620 7468  ach member of th
-00001200: 6973 2063 6f6c 6c65 6374 696f 6e2e 0a20  is collection.. 
-00001210: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00001220: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00001230: 206b 6579 7328 7365 6c66 2920 2d3e 2074   keys(self) -> t
-00001240: 7970 696e 672e 4c69 7374 5b73 7472 5d3a  yping.List[str]:
-00001250: 0a20 2020 2020 2020 2027 2727 2052 6574  .        ''' Ret
-00001260: 7572 6e20 7468 6520 6964 656e 7469 6669  urn the identifi
-00001270: 6572 7320 6f66 2063 6f6c 6c65 6374 696f  ers of collectio
-00001280: 6e20 6d65 6d62 6572 7320 286d 6174 6368  n members (match
-00001290: 696e 6720 5079 7468 6f6e 2773 2064 6963  ing Python's dic
-000012a0: 742e 6b65 7973 2829 2066 756e 6374 696f  t.keys() functio
-000012b0: 6e61 6c69 7479 292e 0a0a 2020 2020 2020  nality)...      
-000012c0: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
-000012d0: 2e4c 6973 745b 7374 725d 0a20 2020 2020  .List[str].     
-000012e0: 2020 203a 7265 7475 726e 3a20 7468 6520     :return: the 
-000012f0: 6964 656e 7469 6669 6572 7320 666f 7220  identifiers for 
-00001300: 6561 6368 206d 656d 6265 7220 6f66 2074  each member of t
-00001310: 6869 7320 636f 6c6c 6563 7469 6f6e 2e0a  his collection..
-00001320: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00001330: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00001340: 6620 7661 6c75 6573 2873 656c 6629 202d  f values(self) -
-00001350: 3e20 7479 7069 6e67 2e4c 6973 743a 0a20  > typing.List:. 
-00001360: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
-00001370: 6e20 7468 6520 7661 6c75 6573 206f 6620  n the values of 
-00001380: 636f 6c6c 6563 7469 6f6e 2028 6d61 7463  collection (matc
-00001390: 6869 6e67 2050 7974 686f 6e27 7320 6469  hing Python's di
-000013a0: 6374 2e76 616c 7565 7328 2920 6675 6e63  ct.values() func
-000013b0: 7469 6f6e 616c 6974 7929 2e0a 0a20 2020  tionality)...   
-000013c0: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
-000013d0: 696e 672e 4c69 7374 0a20 2020 2020 2020  ing.List.       
-000013e0: 203a 7265 7475 726e 3a20 7468 6520 6d65   :return: the me
-000013f0: 6d62 6572 7320 6f66 2074 6869 7320 636f  mbers of this co
-00001400: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
-00001410: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-00001420: 7373 0a0a 2020 2020 6465 6620 5f5f 6765  ss..    def __ge
-00001430: 7469 7465 6d5f 5f28 7365 6c66 2c20 6b65  titem__(self, ke
-00001440: 793a 2074 7970 696e 672e 556e 696f 6e5b  y: typing.Union[
-00001450: 696e 742c 2073 7472 5d29 202d 3e20 2747  int, str]) -> 'G
-00001460: 656e 6572 6963 5479 7065 273a 0a20 2020  enericType':.   
-00001470: 2020 2020 2027 2727 200a 0a20 2020 2020       ''' ..     
-00001480: 2020 203a 7061 7261 6d20 6b65 793a 200a     :param key: .
-00001490: 2020 2020 2020 2020 3a74 7970 6520 6b65          :type ke
-000014a0: 793a 2074 7970 696e 672e 556e 696f 6e5b  y: typing.Union[
-000014b0: 696e 742c 2073 7472 5d0a 2020 2020 2020  int, str].      
-000014c0: 2020 3a72 7479 7065 3a20 2747 656e 6572    :rtype: 'Gener
-000014d0: 6963 5479 7065 270a 2020 2020 2020 2020  icType'.        
-000014e0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-000014f0: 0a0a 2020 2020 6465 6620 5f5f 7365 7469  ..    def __seti
-00001500: 7465 6d5f 5f28 7365 6c66 2c20 6b65 793a  tem__(self, key:
-00001510: 2074 7970 696e 672e 556e 696f 6e5b 696e   typing.Union[in
-00001520: 742c 2073 7472 5d2c 2076 616c 7565 3a20  t, str], value: 
-00001530: 2747 656e 6572 6963 5479 7065 2729 3a0a  'GenericType'):.
-00001540: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
-00001550: 2020 2020 2020 3a70 6172 616d 206b 6579        :param key
-00001560: 3a20 0a20 2020 2020 2020 203a 7479 7065  : .        :type
-00001570: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
-00001580: 6f6e 5b69 6e74 2c20 7374 725d 0a20 2020  on[int, str].   
-00001590: 2020 2020 203a 7061 7261 6d20 7661 6c75       :param valu
-000015a0: 653a 200a 2020 2020 2020 2020 3a74 7970  e: .        :typ
-000015b0: 6520 7661 6c75 653a 2027 4765 6e65 7269  e value: 'Generi
-000015c0: 6354 7970 6527 0a20 2020 2020 2020 2027  cType'.        '
-000015d0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-000015e0: 0a20 2020 2064 6566 205f 5f64 656c 6974  .    def __delit
-000015f0: 656d 5f5f 2873 656c 662c 206b 6579 3a20  em__(self, key: 
-00001600: 7479 7069 6e67 2e55 6e69 6f6e 5b69 6e74  typing.Union[int
-00001610: 2c20 7374 725d 2920 2d3e 2027 4765 6e65  , str]) -> 'Gene
-00001620: 7269 6354 7970 6527 3a0a 2020 2020 2020  ricType':.      
-00001630: 2020 2727 2720 0a0a 2020 2020 2020 2020    ''' ..        
-00001640: 3a70 6172 616d 206b 6579 3a20 0a20 2020  :param key: .   
-00001650: 2020 2020 203a 7479 7065 206b 6579 3a20       :type key: 
-00001660: 7479 7069 6e67 2e55 6e69 6f6e 5b69 6e74  typing.Union[int
-00001670: 2c20 7374 725d 0a20 2020 2020 2020 203a  , str].        :
-00001680: 7274 7970 653a 2027 4765 6e65 7269 6354  rtype: 'GenericT
-00001690: 7970 6527 0a20 2020 2020 2020 2027 2727  ype'.        '''
-000016a0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-000016b0: 2020 2064 6566 205f 5f69 7465 725f 5f28     def __iter__(
-000016c0: 7365 6c66 2920 2d3e 2074 7970 696e 672e  self) -> typing.
-000016d0: 4974 6572 6174 6f72 5b27 4765 6e65 7269  Iterator['Generi
-000016e0: 6354 7970 6527 5d3a 0a20 2020 2020 2020  cType']:.       
-000016f0: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
-00001700: 7274 7970 653a 2074 7970 696e 672e 4974  rtype: typing.It
-00001710: 6572 6174 6f72 5b27 4765 6e65 7269 6354  erator['GenericT
-00001720: 7970 6527 5d0a 2020 2020 2020 2020 2727  ype'].        ''
-00001730: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00001740: 2020 2020 6465 6620 5f5f 6e65 7874 5f5f      def __next__
-00001750: 2873 656c 6629 202d 3e20 2747 656e 6572  (self) -> 'Gener
-00001760: 6963 5479 7065 273a 0a20 2020 2020 2020  icType':.       
-00001770: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
-00001780: 7274 7970 653a 2027 4765 6e65 7269 6354  rtype: 'GenericT
-00001790: 7970 6527 0a20 2020 2020 2020 2027 2727  ype'.        '''
-000017a0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-000017b0: 2020 2064 6566 205f 5f6c 656e 5f5f 2873     def __len__(s
-000017c0: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
-000017d0: 2020 2020 2027 2727 200a 0a20 2020 2020       ''' ..     
-000017e0: 2020 203a 7274 7970 653a 2069 6e74 0a20     :rtype: int. 
-000017f0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00001800: 2020 2070 6173 730a 0a0a 636c 6173 7320     pass...class 
-00001810: 6270 795f 7374 7275 6374 3a0a 2020 2020  bpy_struct:.    
-00001820: 2727 2720 6275 696c 742d 696e 2062 6173  ''' built-in bas
-00001830: 6520 636c 6173 7320 666f 7220 616c 6c20  e class for all 
-00001840: 636c 6173 7365 7320 696e 2062 7079 2e74  classes in bpy.t
-00001850: 7970 6573 2e0a 2020 2020 2727 270a 0a20  ypes..    '''.. 
-00001860: 2020 2069 645f 6461 7461 203d 204e 6f6e     id_data = Non
-00001870: 650a 2020 2020 2727 2720 5468 6520 6062  e.    ''' The `b
-00001880: 7079 2e74 7970 6573 2e49 4460 206f 626a  py.types.ID` obj
-00001890: 6563 7420 7468 6973 2064 6174 6162 6c6f  ect this datablo
-000018a0: 636b 2069 7320 6672 6f6d 206f 7220 4e6f  ck is from or No
-000018b0: 6e65 2c20 286e 6f74 2061 7661 696c 6162  ne, (not availab
-000018c0: 6c65 2066 6f72 2061 6c6c 2064 6174 6120  le for all data 
-000018d0: 7479 7065 7329 2727 270a 0a20 2020 2064  types)'''..    d
-000018e0: 6566 2061 735f 706f 696e 7465 7228 7365  ef as_pointer(se
-000018f0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-00001900: 2020 2020 2727 2720 5265 7475 726e 7320      ''' Returns 
-00001910: 7468 6520 6d65 6d6f 7279 2061 6464 7265  the memory addre
-00001920: 7373 2077 6869 6368 2068 6f6c 6473 2061  ss which holds a
-00001930: 2070 6f69 6e74 6572 2074 6f20 426c 656e   pointer to Blen
-00001940: 6465 7227 7320 696e 7465 726e 616c 2064  der's internal d
-00001950: 6174 610a 0a20 2020 2020 2020 203a 7274  ata..        :rt
-00001960: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
-00001970: 203a 7265 7475 726e 3a20 696e 7420 286d   :return: int (m
-00001980: 656d 6f72 7920 6164 6472 6573 7329 2e0a  emory address)..
-00001990: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000019a0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-000019b0: 6620 6472 6976 6572 5f61 6464 2873 656c  f driver_add(sel
-000019c0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-000019d0: 2020 2020 2020 7061 7468 3a20 7479 7069        path: typi
-000019e0: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-000019f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001a00: 2020 2020 2069 6e64 6578 3a20 7479 7069       index: typi
-00001a10: 6e67 2e4f 7074 696f 6e61 6c5b 696e 745d  ng.Optional[int]
-00001a20: 203d 202d 3129 202d 3e20 2746 4375 7276   = -1) -> 'FCurv
-00001a30: 6527 3a0a 2020 2020 2020 2020 2727 2720  e':.        ''' 
-00001a40: 4164 6473 2064 7269 7665 7228 7329 2074  Adds driver(s) t
-00001a50: 6f20 7468 6520 6769 7665 6e20 7072 6f70  o the given prop
-00001a60: 6572 7479 0a0a 2020 2020 2020 2020 3a70  erty..        :p
-00001a70: 6172 616d 2070 6174 683a 2070 6174 6820  aram path: path 
-00001a80: 746f 2074 6865 2070 726f 7065 7274 7920  to the property 
-00001a90: 746f 2064 7269 7665 2c20 616e 616c 6f67  to drive, analog
-00001aa0: 6f75 7320 746f 2074 6865 2066 6375 7276  ous to the fcurv
-00001ab0: 6527 7320 6461 7461 2070 6174 682e 0a20  e's data path.. 
-00001ac0: 2020 2020 2020 203a 7479 7065 2070 6174         :type pat
-00001ad0: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
-00001ae0: 616c 5b73 7472 5d0a 2020 2020 2020 2020  al[str].        
-00001af0: 3a70 6172 616d 2069 6e64 6578 3a20 6172  :param index: ar
-00001b00: 7261 7920 696e 6465 7820 6f66 2074 6865  ray index of the
-00001b10: 2070 726f 7065 7274 7920 6472 6976 652e   property drive.
-00001b20: 2044 6566 6175 6c74 7320 746f 202d 3120   Defaults to -1 
-00001b30: 666f 7220 616c 6c20 696e 6469 6365 7320  for all indices 
-00001b40: 6f72 2061 2073 696e 676c 6520 6368 616e  or a single chan
-00001b50: 6e65 6c20 6966 2074 6865 2070 726f 7065  nel if the prope
-00001b60: 7274 7920 6973 206e 6f74 2061 6e20 6172  rty is not an ar
-00001b70: 7261 792e 0a20 2020 2020 2020 203a 7479  ray..        :ty
-00001b80: 7065 2069 6e64 6578 3a20 7479 7069 6e67  pe index: typing
-00001b90: 2e4f 7074 696f 6e61 6c5b 696e 745d 0a20  .Optional[int]. 
-00001ba0: 2020 2020 2020 203a 7274 7970 653a 2027         :rtype: '
-00001bb0: 4643 7572 7665 270a 2020 2020 2020 2020  FCurve'.        
-00001bc0: 3a72 6574 7572 6e3a 2054 6865 2064 7269  :return: The dri
-00001bd0: 7665 7228 7329 2061 6464 6564 2e0a 2020  ver(s) added..  
-00001be0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00001bf0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00001c00: 6472 6976 6572 5f72 656d 6f76 6528 7365  driver_remove(se
-00001c10: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-00001c20: 2020 2020 2020 2020 2020 7061 7468 3a20            path: 
-00001c30: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00001c40: 7374 725d 2c0a 2020 2020 2020 2020 2020  str],.          
-00001c50: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-00001c60: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
-00001c70: 616c 5b69 6e74 5d20 3d20 2d31 2920 2d3e  al[int] = -1) ->
-00001c80: 2062 6f6f 6c3a 0a20 2020 2020 2020 2027   bool:.        '
-00001c90: 2727 2052 656d 6f76 6520 6472 6976 6572  '' Remove driver
-00001ca0: 2873 2920 6672 6f6d 2074 6865 2067 6976  (s) from the giv
-00001cb0: 656e 2070 726f 7065 7274 790a 0a20 2020  en property..   
-00001cc0: 2020 2020 203a 7061 7261 6d20 7061 7468       :param path
-00001cd0: 3a20 7061 7468 2074 6f20 7468 6520 7072  : path to the pr
-00001ce0: 6f70 6572 7479 2074 6f20 6472 6976 652c  operty to drive,
-00001cf0: 2061 6e61 6c6f 676f 7573 2074 6f20 7468   analogous to th
-00001d00: 6520 6663 7572 7665 2773 2064 6174 6120  e fcurve's data 
-00001d10: 7061 7468 2e0a 2020 2020 2020 2020 3a74  path..        :t
-00001d20: 7970 6520 7061 7468 3a20 7479 7069 6e67  ype path: typing
-00001d30: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
-00001d40: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
-00001d50: 6465 783a 2061 7272 6179 2069 6e64 6578  dex: array index
-00001d60: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
-00001d70: 2064 7269 7665 2e20 4465 6661 756c 7473   drive. Defaults
-00001d80: 2074 6f20 2d31 2066 6f72 2061 6c6c 2069   to -1 for all i
-00001d90: 6e64 6963 6573 206f 7220 6120 7369 6e67  ndices or a sing
-00001da0: 6c65 2063 6861 6e6e 656c 2069 6620 7468  le channel if th
-00001db0: 6520 7072 6f70 6572 7479 2069 7320 6e6f  e property is no
-00001dc0: 7420 616e 2061 7272 6179 2e0a 2020 2020  t an array..    
-00001dd0: 2020 2020 3a74 7970 6520 696e 6465 783a      :type index:
-00001de0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00001df0: 5b69 6e74 5d0a 2020 2020 2020 2020 3a72  [int].        :r
-00001e00: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
-00001e10: 2020 203a 7265 7475 726e 3a20 5375 6363     :return: Succ
-00001e20: 6573 7320 6f66 2064 7269 7665 7220 7265  ess of driver re
-00001e30: 6d6f 7661 6c2e 0a20 2020 2020 2020 2027  moval..        '
-00001e40: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-00001e50: 0a20 2020 2064 6566 2067 6574 2873 656c  .    def get(sel
-00001e60: 662c 0a20 2020 2020 2020 2020 2020 206b  f,.            k
-00001e70: 6579 3a20 7479 7069 6e67 2e4f 7074 696f  ey: typing.Optio
-00001e80: 6e61 6c5b 7374 725d 2c0a 2020 2020 2020  nal[str],.      
-00001e90: 2020 2020 2020 6465 6661 756c 743a 2074        default: t
-00001ea0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-00001eb0: 7970 696e 672e 416e 795d 203d 204e 6f6e  yping.Any] = Non
-00001ec0: 6529 3a0a 2020 2020 2020 2020 2727 2720  e):.        ''' 
-00001ed0: 5265 7475 726e 7320 7468 6520 7661 6c75  Returns the valu
-00001ee0: 6520 6f66 2074 6865 2063 7573 746f 6d20  e of the custom 
-00001ef0: 7072 6f70 6572 7479 2061 7373 6967 6e65  property assigne
-00001f00: 6420 746f 206b 6579 206f 7220 6465 6661  d to key or defa
-00001f10: 756c 7420 7768 656e 206e 6f74 2066 6f75  ult when not fou
-00001f20: 6e64 2028 6d61 7463 6865 7320 5079 7468  nd (matches Pyth
-00001f30: 6f6e 2773 2064 6963 7469 6f6e 6172 7920  on's dictionary 
-00001f40: 6675 6e63 7469 6f6e 206f 6620 7468 6520  function of the 
-00001f50: 7361 6d65 206e 616d 6529 2e0a 0a20 2020  same name)...   
-00001f60: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
-00001f70: 2054 6865 206b 6579 2061 7373 6f63 6961   The key associa
-00001f80: 7465 6420 7769 7468 2074 6865 2063 7573  ted with the cus
-00001f90: 746f 6d20 7072 6f70 6572 7479 2e0a 2020  tom property..  
-00001fa0: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
-00001fb0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00001fc0: 5b73 7472 5d0a 2020 2020 2020 2020 3a70  [str].        :p
-00001fd0: 6172 616d 2064 6566 6175 6c74 3a20 4f70  aram default: Op
-00001fe0: 7469 6f6e 616c 2061 7267 756d 656e 7420  tional argument 
-00001ff0: 666f 7220 7468 6520 7661 6c75 6520 746f  for the value to
-00002000: 2072 6574 7572 6e20 6966 202a 6b65 792a   return if *key*
-00002010: 2069 7320 6e6f 7420 666f 756e 642e 0a20   is not found.. 
-00002020: 2020 2020 2020 203a 7479 7065 2064 6566         :type def
-00002030: 6175 6c74 3a20 7479 7069 6e67 2e4f 7074  ault: typing.Opt
-00002040: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
-00002050: 5d0a 2020 2020 2020 2020 2727 270a 2020  ].        '''.  
-00002060: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00002070: 6465 6620 6964 5f70 726f 7065 7274 6965  def id_propertie
-00002080: 735f 636c 6561 7228 7365 6c66 293a 0a20  s_clear(self):. 
-00002090: 2020 2020 2020 2027 2727 200a 0a20 2020         ''' ..   
-000020a0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-000020b0: 2070 6173 730a 0a20 2020 2064 6566 2069   pass..    def i
-000020c0: 645f 7072 6f70 6572 7469 6573 5f65 6e73  d_properties_ens
-000020d0: 7572 6528 7365 6c66 2920 2d3e 2074 7970  ure(self) -> typ
-000020e0: 696e 672e 416e 793a 0a20 2020 2020 2020  ing.Any:.       
-000020f0: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
-00002100: 7274 7970 653a 2074 7970 696e 672e 416e  rtype: typing.An
-00002110: 790a 2020 2020 2020 2020 3a72 6574 7572  y.        :retur
-00002120: 6e3a 2074 6865 2070 6172 656e 7420 6772  n: the parent gr
-00002130: 6f75 7020 666f 7220 616e 2052 4e41 2073  oup for an RNA s
-00002140: 7472 7563 7427 7320 6375 7374 6f6d 2049  truct's custom I
-00002150: 4450 726f 7065 7274 6965 732e 0a20 2020  DProperties..   
-00002160: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00002170: 2070 6173 730a 0a20 2020 2064 6566 2069   pass..    def i
-00002180: 645f 7072 6f70 6572 7469 6573 5f75 6928  d_properties_ui(
-00002190: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
-000021a0: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-000021b0: 672e 416e 795d 2920 2d3e 2074 7970 696e  g.Any]) -> typin
-000021c0: 672e 416e 793a 0a20 2020 2020 2020 2027  g.Any:.        '
-000021d0: 2727 200a 0a20 2020 2020 2020 203a 7061  '' ..        :pa
-000021e0: 7261 6d20 6b65 793a 2020 5374 7269 6e67  ram key:  String
-000021f0: 206e 616d 6520 6f66 2074 6865 2070 726f   name of the pro
-00002200: 7065 7274 792e 0a20 2020 2020 2020 203a  perty..        :
-00002210: 7479 7065 206b 6579 3a20 7479 7069 6e67  type key: typing
-00002220: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-00002230: 2e41 6e79 5d0a 2020 2020 2020 2020 3a72  .Any].        :r
-00002240: 7479 7065 3a20 7479 7069 6e67 2e41 6e79  type: typing.Any
-00002250: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00002260: 3a20 5265 7475 726e 2061 6e20 6f62 6a65  : Return an obje
-00002270: 6374 2075 7365 6420 746f 206d 616e 6167  ct used to manag
-00002280: 6520 616e 2049 4450 726f 7065 7274 7927  e an IDProperty'
-00002290: 7320 5549 2064 6174 612e 0a20 2020 2020  s UI data..     
-000022a0: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
-000022b0: 6173 730a 0a20 2020 2064 6566 2069 735f  ass..    def is_
-000022c0: 7072 6f70 6572 7479 5f68 6964 6465 6e28  property_hidden(
-000022d0: 7365 6c66 2c20 7072 6f70 6572 7479 2920  self, property) 
-000022e0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-000022f0: 2027 2727 2043 6865 636b 2069 6620 6120   ''' Check if a 
-00002300: 7072 6f70 6572 7479 2069 7320 6869 6464  property is hidd
-00002310: 656e 2e0a 0a20 2020 2020 2020 203a 7274  en...        :rt
-00002320: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
-00002330: 2020 3a72 6574 7572 6e3a 2054 7275 6520    :return: True 
-00002340: 7768 656e 2074 6865 2070 726f 7065 7274  when the propert
-00002350: 7920 6973 2068 6964 6465 6e2e 0a20 2020  y is hidden..   
-00002360: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00002370: 2070 6173 730a 0a20 2020 2064 6566 2069   pass..    def i
-00002380: 735f 7072 6f70 6572 7479 5f6f 7665 7272  s_property_overr
-00002390: 6964 6162 6c65 5f6c 6962 7261 7279 2873  idable_library(s
-000023a0: 656c 662c 2070 726f 7065 7274 7929 202d  elf, property) -
-000023b0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-000023c0: 2727 2720 4368 6563 6b20 6966 2061 2070  ''' Check if a p
-000023d0: 726f 7065 7274 7920 6973 206f 7665 7272  roperty is overr
-000023e0: 6964 6162 6c65 2e0a 0a20 2020 2020 2020  idable...       
-000023f0: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
-00002400: 2020 2020 2020 3a72 6574 7572 6e3a 2054        :return: T
-00002410: 7275 6520 7768 656e 2074 6865 2070 726f  rue when the pro
-00002420: 7065 7274 7920 6973 206f 7665 7272 6964  perty is overrid
-00002430: 6162 6c65 2e0a 2020 2020 2020 2020 2727  able..        ''
-00002440: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00002450: 2020 2020 6465 6620 6973 5f70 726f 7065      def is_prope
-00002460: 7274 795f 7265 6164 6f6e 6c79 2873 656c  rty_readonly(sel
-00002470: 662c 2070 726f 7065 7274 7929 202d 3e20  f, property) -> 
-00002480: 626f 6f6c 3a0a 2020 2020 2020 2020 2727  bool:.        ''
-00002490: 2720 4368 6563 6b20 6966 2061 2070 726f  ' Check if a pro
-000024a0: 7065 7274 7920 6973 2072 6561 646f 6e6c  perty is readonl
-000024b0: 792e 0a0a 2020 2020 2020 2020 3a72 7479  y...        :rty
-000024c0: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
-000024d0: 203a 7265 7475 726e 3a20 5472 7565 2077   :return: True w
-000024e0: 6865 6e20 7468 6520 7072 6f70 6572 7479  hen the property
-000024f0: 2069 7320 7265 6164 6f6e 6c79 2028 6e6f   is readonly (no
-00002500: 7420 7772 6974 6162 6c65 292e 0a20 2020  t writable)..   
-00002510: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00002520: 2070 6173 730a 0a20 2020 2064 6566 2069   pass..    def i
-00002530: 735f 7072 6f70 6572 7479 5f73 6574 2873  s_property_set(s
-00002540: 656c 662c 2070 726f 7065 7274 792c 0a20  elf, property,. 
-00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002560: 2020 2020 2020 2067 686f 7374 3a20 7479         ghost: ty
-00002570: 7069 6e67 2e4f 7074 696f 6e61 6c5b 626f  ping.Optional[bo
-00002580: 6f6c 5d20 3d20 5472 7565 2920 2d3e 2062  ol] = True) -> b
-00002590: 6f6f 6c3a 0a20 2020 2020 2020 2027 2727  ool:.        '''
-000025a0: 2043 6865 636b 2069 6620 6120 7072 6f70   Check if a prop
-000025b0: 6572 7479 2069 7320 7365 742c 2075 7365  erty is set, use
-000025c0: 2066 6f72 2074 6573 7469 6e67 206f 7065   for testing ope
-000025d0: 7261 746f 7220 7072 6f70 6572 7469 6573  rator properties
-000025e0: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-000025f0: 6d20 6768 6f73 743a 2055 7365 6420 666f  m ghost: Used fo
-00002600: 7220 6f70 6572 6174 6f72 7320 7468 6174  r operators that
-00002610: 2072 652d 7275 6e20 7769 7468 2070 7265   re-run with pre
-00002620: 7669 6f75 7320 7365 7474 696e 6773 2e20  vious settings. 
-00002630: 496e 2074 6869 7320 6361 7365 2074 6865  In this case the
-00002640: 2070 726f 7065 7274 7920 6973 206e 6f74   property is not
-00002650: 206d 6172 6b65 6420 6173 2073 6574 2c20   marked as set, 
-00002660: 7965 7420 7468 6520 7661 6c75 6520 6672  yet the value fr
-00002670: 6f6d 2074 6865 2070 7265 7669 6f75 7320  om the previous 
-00002680: 6578 6563 7574 696f 6e20 6973 2075 7365  execution is use
-00002690: 642e 2049 6e20 7261 7265 2063 6173 6573  d. In rare cases
-000026a0: 2079 6f75 206d 6179 2077 616e 7420 746f   you may want to
-000026b0: 2073 6574 2074 6869 7320 6f70 7469 6f6e   set this option
-000026c0: 2074 6f20 6661 6c73 652e 0a20 2020 2020   to false..     
-000026d0: 2020 203a 7479 7065 2067 686f 7374 3a20     :type ghost: 
-000026e0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-000026f0: 626f 6f6c 5d0a 2020 2020 2020 2020 3a72  bool].        :r
-00002700: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
-00002710: 2020 203a 7265 7475 726e 3a20 5472 7565     :return: True
-00002720: 2077 6865 6e20 7468 6520 7072 6f70 6572   when the proper
-00002730: 7479 2068 6173 2062 6565 6e20 7365 742e  ty has been set.
-00002740: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00002750: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00002760: 6566 2069 7465 6d73 2873 656c 6629 202d  ef items(self) -
-00002770: 3e20 7479 7069 6e67 2e41 6e79 3a0a 2020  > typing.Any:.  
-00002780: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
-00002790: 7320 7468 6520 6974 656d 7320 6f66 2074  s the items of t
-000027a0: 6869 7320 6f62 6a65 6374 7320 6375 7374  his objects cust
-000027b0: 6f6d 2070 726f 7065 7274 6965 7320 286d  om properties (m
-000027c0: 6174 6368 6573 2050 7974 686f 6e27 7320  atches Python's 
-000027d0: 6469 6374 696f 6e61 7279 2066 756e 6374  dictionary funct
-000027e0: 696f 6e20 6f66 2074 6865 2073 616d 6520  ion of the same 
-000027f0: 6e61 6d65 292e 0a0a 2020 2020 2020 2020  name)...        
-00002800: 3a72 7479 7065 3a20 7479 7069 6e67 2e41  :rtype: typing.A
-00002810: 6e79 0a20 2020 2020 2020 203a 7265 7475  ny.        :retu
-00002820: 726e 3a20 6375 7374 6f6d 2070 726f 7065  rn: custom prope
-00002830: 7274 7920 6b65 792c 2076 616c 7565 2070  rty key, value p
-00002840: 6169 7273 2e0a 2020 2020 2020 2020 2727  airs..        ''
-00002850: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00002860: 2020 2020 6465 6620 6b65 7966 7261 6d65      def keyframe
-00002870: 5f64 656c 6574 6528 0a20 2020 2020 2020  _delete(.       
-00002880: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00002890: 2020 2020 2020 2064 6174 615f 7061 7468         data_path
-000028a0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-000028b0: 6c5b 7374 725d 2c0a 2020 2020 2020 2020  l[str],.        
-000028c0: 2020 2020 696e 6465 783a 2074 7970 696e      index: typin
-000028d0: 672e 4f70 7469 6f6e 616c 5b69 6e74 5d20  g.Optional[int] 
-000028e0: 3d20 2d31 2c0a 2020 2020 2020 2020 2020  = -1,.          
-000028f0: 2020 6672 616d 653a 2074 7970 696e 672e    frame: typing.
-00002900: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d20  Optional[float] 
-00002910: 3d20 2762 7079 2e63 6f6e 7465 7874 2e73  = 'bpy.context.s
-00002920: 6365 6e65 2e66 7261 6d65 5f63 7572 7265  cene.frame_curre
-00002930: 6e74 272c 0a20 2020 2020 2020 2020 2020  nt',.           
-00002940: 2067 726f 7570 3a20 7479 7069 6e67 2e4f   group: typing.O
-00002950: 7074 696f 6e61 6c5b 7374 725d 203d 2022  ptional[str] = "
-00002960: 2229 202d 3e20 626f 6f6c 3a0a 2020 2020  ") -> bool:.    
-00002970: 2020 2020 2727 2720 5265 6d6f 7665 2061      ''' Remove a
-00002980: 206b 6579 6672 616d 6520 6672 6f6d 2074   keyframe from t
-00002990: 6869 7320 7072 6f70 6572 7469 6573 2066  his properties f
-000029a0: 6375 7276 652e 0a0a 2020 2020 2020 2020  curve...        
-000029b0: 3a70 6172 616d 2064 6174 615f 7061 7468  :param data_path
-000029c0: 3a20 7061 7468 2074 6f20 7468 6520 7072  : path to the pr
-000029d0: 6f70 6572 7479 2074 6f20 7265 6d6f 7665  operty to remove
-000029e0: 2061 206b 6579 2c20 616e 616c 6f67 6f75   a key, analogou
-000029f0: 7320 746f 2074 6865 2066 6375 7276 6527  s to the fcurve'
-00002a00: 7320 6461 7461 2070 6174 682e 0a20 2020  s data path..   
-00002a10: 2020 2020 203a 7479 7065 2064 6174 615f       :type data_
-00002a20: 7061 7468 3a20 7479 7069 6e67 2e4f 7074  path: typing.Opt
-00002a30: 696f 6e61 6c5b 7374 725d 0a20 2020 2020  ional[str].     
-00002a40: 2020 203a 7061 7261 6d20 696e 6465 783a     :param index:
-00002a50: 2061 7272 6179 2069 6e64 6578 206f 6620   array index of 
-00002a60: 7468 6520 7072 6f70 6572 7479 2074 6f20  the property to 
-00002a70: 7265 6d6f 7665 2061 206b 6579 2e20 4465  remove a key. De
-00002a80: 6661 756c 7473 2074 6f20 2d31 2072 656d  faults to -1 rem
-00002a90: 6f76 696e 6720 616c 6c20 696e 6469 6365  oving all indice
-00002aa0: 7320 6f72 2061 2073 696e 676c 6520 6368  s or a single ch
-00002ab0: 616e 6e65 6c20 6966 2074 6865 2070 726f  annel if the pro
-00002ac0: 7065 7274 7920 6973 206e 6f74 2061 6e20  perty is not an 
-00002ad0: 6172 7261 792e 0a20 2020 2020 2020 203a  array..        :
-00002ae0: 7479 7065 2069 6e64 6578 3a20 7479 7069  type index: typi
-00002af0: 6e67 2e4f 7074 696f 6e61 6c5b 696e 745d  ng.Optional[int]
-00002b00: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00002b10: 6672 616d 653a 2054 6865 2066 7261 6d65  frame: The frame
-00002b20: 206f 6e20 7768 6963 6820 7468 6520 6b65   on which the ke
-00002b30: 7966 7261 6d65 2069 7320 6465 6c65 7465  yframe is delete
-00002b40: 642c 2064 6566 6175 6c74 696e 6720 746f  d, defaulting to
-00002b50: 2074 6865 2063 7572 7265 6e74 2066 7261   the current fra
-00002b60: 6d65 2e0a 2020 2020 2020 2020 3a74 7970  me..        :typ
-00002b70: 6520 6672 616d 653a 2074 7970 696e 672e  e frame: typing.
-00002b80: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d0a  Optional[float].
-00002b90: 2020 2020 2020 2020 3a70 6172 616d 2067          :param g
-00002ba0: 726f 7570 3a20 5468 6520 6e61 6d65 206f  roup: The name o
-00002bb0: 6620 7468 6520 6772 6f75 7020 7468 6520  f the group the 
-00002bc0: 462d 4375 7276 6520 7368 6f75 6c64 2062  F-Curve should b
-00002bd0: 6520 6164 6465 6420 746f 2069 6620 6974  e added to if it
-00002be0: 2064 6f65 736e 2774 2065 7869 7374 2079   doesn't exist y
-00002bf0: 6574 2e0a 2020 2020 2020 2020 3a74 7970  et..        :typ
-00002c00: 6520 6772 6f75 703a 2074 7970 696e 672e  e group: typing.
-00002c10: 4f70 7469 6f6e 616c 5b73 7472 5d0a 2020  Optional[str].  
-00002c20: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
-00002c30: 6f6c 0a20 2020 2020 2020 203a 7265 7475  ol.        :retu
-00002c40: 726e 3a20 5375 6363 6573 7320 6f66 206b  rn: Success of k
-00002c50: 6579 6672 616d 6520 6465 6c65 7469 6f6e  eyframe deletion
-00002c60: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00002c70: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00002c80: 6465 6620 6b65 7966 7261 6d65 5f69 6e73  def keyframe_ins
-00002c90: 6572 7428 0a20 2020 2020 2020 2020 2020  ert(.           
-00002ca0: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-00002cb0: 2020 2064 6174 615f 7061 7468 3a20 7479     data_path: ty
-00002cc0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-00002cd0: 725d 2c0a 2020 2020 2020 2020 2020 2020  r],.            
-00002ce0: 696e 6465 783a 2074 7970 696e 672e 4f70  index: typing.Op
-00002cf0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 2d31  tional[int] = -1
-00002d00: 2c0a 2020 2020 2020 2020 2020 2020 6672  ,.            fr
-00002d10: 616d 653a 2074 7970 696e 672e 4f70 7469  ame: typing.Opti
-00002d20: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 2762  onal[float] = 'b
-00002d30: 7079 2e63 6f6e 7465 7874 2e73 6365 6e65  py.context.scene
-00002d40: 2e66 7261 6d65 5f63 7572 7265 6e74 272c  .frame_current',
-00002d50: 0a20 2020 2020 2020 2020 2020 2067 726f  .            gro
-00002d60: 7570 3a20 7479 7069 6e67 2e4f 7074 696f  up: typing.Optio
-00002d70: 6e61 6c5b 7374 725d 203d 2022 222c 0a20  nal[str] = "",. 
-00002d80: 2020 2020 2020 2020 2020 206f 7074 696f             optio
-00002d90: 6e73 3a20 7479 7069 6e67 2e4f 7074 696f  ns: typing.Optio
-00002da0: 6e61 6c5b 7479 7069 6e67 2e41 6e79 5d20  nal[typing.Any] 
-00002db0: 3d20 2773 6574 2829 2729 202d 3e20 626f  = 'set()') -> bo
-00002dc0: 6f6c 3a0a 2020 2020 2020 2020 2727 2720  ol:.        ''' 
-00002dd0: 496e 7365 7274 2061 206b 6579 6672 616d  Insert a keyfram
-00002de0: 6520 6f6e 2074 6865 2070 726f 7065 7274  e on the propert
-00002df0: 7920 6769 7665 6e2c 2061 6464 696e 6720  y given, adding 
-00002e00: 6663 7572 7665 7320 616e 6420 616e 696d  fcurves and anim
-00002e10: 6174 696f 6e20 6461 7461 2077 6865 6e20  ation data when 
-00002e20: 6e65 6365 7373 6172 792e 2054 6869 7320  necessary. This 
-00002e30: 6973 2074 6865 206d 6f73 7420 7369 6d70  is the most simp
-00002e40: 6c65 2065 7861 6d70 6c65 206f 6620 696e  le example of in
-00002e50: 7365 7274 696e 6720 6120 6b65 7966 7261  serting a keyfra
-00002e60: 6d65 2066 726f 6d20 7079 7468 6f6e 2e20  me from python. 
-00002e70: 4e6f 7465 2074 6861 7420 7768 656e 206b  Note that when k
-00002e80: 6579 696e 6720 6461 7461 2070 6174 6873  eying data paths
-00002e90: 2077 6869 6368 2063 6f6e 7461 696e 206e   which contain n
-00002ea0: 6573 7465 6420 7072 6f70 6572 7469 6573  ested properties
-00002eb0: 2074 6869 7320 6d75 7374 2062 6520 646f   this must be do
-00002ec0: 6e65 2066 726f 6d20 7468 6520 6049 4460  ne from the `ID`
-00002ed0: 2073 7562 636c 6173 732c 2069 6e20 7468   subclass, in th
-00002ee0: 6973 2063 6173 6520 7468 6520 6041 726d  is case the `Arm
-00002ef0: 6174 7572 6560 2072 6174 6865 7220 7468  ature` rather th
-00002f00: 616e 2074 6865 2062 6f6e 652e 0a0a 2020  an the bone...  
-00002f10: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
-00002f20: 615f 7061 7468 3a20 7061 7468 2074 6f20  a_path: path to 
-00002f30: 7468 6520 7072 6f70 6572 7479 2074 6f20  the property to 
-00002f40: 6b65 792c 2061 6e61 6c6f 676f 7573 2074  key, analogous t
-00002f50: 6f20 7468 6520 6663 7572 7665 2773 2064  o the fcurve's d
-00002f60: 6174 6120 7061 7468 2e0a 2020 2020 2020  ata path..      
-00002f70: 2020 3a74 7970 6520 6461 7461 5f70 6174    :type data_pat
-00002f80: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
-00002f90: 616c 5b73 7472 5d0a 2020 2020 2020 2020  al[str].        
-00002fa0: 3a70 6172 616d 2069 6e64 6578 3a20 6172  :param index: ar
-00002fb0: 7261 7920 696e 6465 7820 6f66 2074 6865  ray index of the
-00002fc0: 2070 726f 7065 7274 7920 746f 206b 6579   property to key
-00002fd0: 2e20 4465 6661 756c 7473 2074 6f20 2d31  . Defaults to -1
-00002fe0: 2077 6869 6368 2077 696c 6c20 6b65 7920   which will key 
-00002ff0: 616c 6c20 696e 6469 6365 7320 6f72 2061  all indices or a
-00003000: 2073 696e 676c 6520 6368 616e 6e65 6c20   single channel 
-00003010: 6966 2074 6865 2070 726f 7065 7274 7920  if the property 
-00003020: 6973 206e 6f74 2061 6e20 6172 7261 792e  is not an array.
-00003030: 0a20 2020 2020 2020 203a 7479 7065 2069  .        :type i
-00003040: 6e64 6578 3a20 7479 7069 6e67 2e4f 7074  ndex: typing.Opt
-00003050: 696f 6e61 6c5b 696e 745d 0a20 2020 2020  ional[int].     
-00003060: 2020 203a 7061 7261 6d20 6672 616d 653a     :param frame:
-00003070: 2054 6865 2066 7261 6d65 206f 6e20 7768   The frame on wh
-00003080: 6963 6820 7468 6520 6b65 7966 7261 6d65  ich the keyframe
-00003090: 2069 7320 696e 7365 7274 6564 2c20 6465   is inserted, de
-000030a0: 6661 756c 7469 6e67 2074 6f20 7468 6520  faulting to the 
-000030b0: 6375 7272 656e 7420 6672 616d 652e 0a20  current frame.. 
-000030c0: 2020 2020 2020 203a 7479 7065 2066 7261         :type fra
-000030d0: 6d65 3a20 7479 7069 6e67 2e4f 7074 696f  me: typing.Optio
-000030e0: 6e61 6c5b 666c 6f61 745d 0a20 2020 2020  nal[float].     
-000030f0: 2020 203a 7061 7261 6d20 6772 6f75 703a     :param group:
-00003100: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
-00003110: 2067 726f 7570 2074 6865 2046 2d43 7572   group the F-Cur
-00003120: 7665 2073 686f 756c 6420 6265 2061 6464  ve should be add
-00003130: 6564 2074 6f20 6966 2069 7420 646f 6573  ed to if it does
-00003140: 6e27 7420 6578 6973 7420 7965 742e 0a20  n't exist yet.. 
-00003150: 2020 2020 2020 203a 7479 7065 2067 726f         :type gro
-00003160: 7570 3a20 7479 7069 6e67 2e4f 7074 696f  up: typing.Optio
-00003170: 6e61 6c5b 7374 725d 0a20 2020 2020 2020  nal[str].       
-00003180: 203a 7061 7261 6d20 666c 6167 3a20 0a20   :param flag: . 
-00003190: 2020 2020 2020 203a 7479 7065 2066 6c61         :type fla
-000031a0: 673a 2074 7970 696e 672e 4f70 7469 6f6e  g: typing.Option
-000031b0: 616c 5b74 7970 696e 672e 5365 745d 0a20  al[typing.Set]. 
-000031c0: 2020 2020 2020 203a 7061 7261 6d20 6f70         :param op
-000031d0: 7469 6f6e 733a 2020 2d20 6060 494e 5345  tions:  - ``INSE
-000031e0: 5254 4b45 595f 4e45 4544 4544 6060 204f  RTKEY_NEEDED`` O
-000031f0: 6e6c 7920 696e 7365 7274 206b 6579 6672  nly insert keyfr
-00003200: 616d 6573 2077 6865 7265 2074 6865 7927  ames where they'
-00003210: 7265 206e 6565 6465 6420 696e 2074 6865  re needed in the
-00003220: 2072 656c 6576 616e 7420 462d 4375 7276   relevant F-Curv
-00003230: 6573 2e20 2d20 6060 494e 5345 5254 4b45  es. - ``INSERTKE
-00003240: 595f 5649 5355 414c 6060 2049 6e73 6572  Y_VISUAL`` Inser
-00003250: 7420 6b65 7966 7261 6d65 7320 6261 7365  t keyframes base
-00003260: 6420 6f6e 2027 7669 7375 616c 2074 7261  d on 'visual tra
-00003270: 6e73 666f 726d 7327 2e20 2d20 6060 494e  nsforms'. - ``IN
-00003280: 5345 5254 4b45 595f 5859 5a5f 544f 5f52  SERTKEY_XYZ_TO_R
-00003290: 4742 6060 2043 6f6c 6f72 2066 6f72 206e  GB`` Color for n
-000032a0: 6577 6c79 2061 6464 6564 2074 7261 6e73  ewly added trans
-000032b0: 666f 726d 6174 696f 6e20 462d 4375 7276  formation F-Curv
-000032c0: 6573 2028 4c6f 6361 7469 6f6e 2c20 526f  es (Location, Ro
-000032d0: 7461 7469 6f6e 2c20 5363 616c 6529 2069  tation, Scale) i
-000032e0: 7320 6261 7365 6420 6f6e 2074 6865 2074  s based on the t
-000032f0: 7261 6e73 666f 726d 2061 7869 732e 202d  ransform axis. -
-00003300: 2060 6049 4e53 4552 544b 4559 5f52 4550   ``INSERTKEY_REP
-00003310: 4c41 4345 6060 204f 6e6c 7920 7265 706c  LACE`` Only repl
-00003320: 6163 6520 616c 7265 6164 7920 6578 6973  ace already exis
-00003330: 7469 6e67 206b 6579 6672 616d 6573 2e20  ting keyframes. 
-00003340: 2d20 6060 494e 5345 5254 4b45 595f 4156  - ``INSERTKEY_AV
-00003350: 4149 4c41 424c 4560 6020 4f6e 6c79 2069  AILABLE`` Only i
-00003360: 6e73 6572 7420 696e 746f 2061 6c72 6561  nsert into alrea
-00003370: 6479 2065 7869 7374 696e 6720 462d 4375  dy existing F-Cu
-00003380: 7276 6573 2e20 2d20 6060 494e 5345 5254  rves. - ``INSERT
-00003390: 4b45 595f 4359 434c 455f 4157 4152 4560  KEY_CYCLE_AWARE`
-000033a0: 6020 5461 6b65 2063 7963 6c69 6320 6578  ` Take cyclic ex
-000033b0: 7472 6170 6f6c 6174 696f 6e20 696e 746f  trapolation into
-000033c0: 2061 6363 6f75 6e74 2028 4379 636c 652d   account (Cycle-
-000033d0: 4177 6172 6520 4b65 7969 6e67 206f 7074  Aware Keying opt
-000033e0: 696f 6e29 2e0a 2020 2020 2020 2020 3a74  ion)..        :t
-000033f0: 7970 6520 6f70 7469 6f6e 733a 2074 7970  ype options: typ
-00003400: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
-00003410: 696e 672e 416e 795d 0a20 2020 2020 2020  ing.Any].       
-00003420: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
-00003430: 2020 2020 2020 3a72 6574 7572 6e3a 2053        :return: S
-00003440: 7563 6365 7373 206f 6620 6b65 7966 7261  uccess of keyfra
-00003450: 6d65 2069 6e73 6572 7469 6f6e 2e0a 2020  me insertion..  
-00003460: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00003470: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00003480: 6b65 7973 2873 656c 6629 202d 3e20 7479  keys(self) -> ty
-00003490: 7069 6e67 2e41 6e79 3a0a 2020 2020 2020  ping.Any:.      
-000034a0: 2020 2727 2720 5265 7475 726e 7320 7468    ''' Returns th
-000034b0: 6520 6b65 7973 206f 6620 7468 6973 206f  e keys of this o
-000034c0: 626a 6563 7473 2063 7573 746f 6d20 7072  bjects custom pr
-000034d0: 6f70 6572 7469 6573 2028 6d61 7463 6865  operties (matche
-000034e0: 7320 5079 7468 6f6e 2773 2064 6963 7469  s Python's dicti
-000034f0: 6f6e 6172 7920 6675 6e63 7469 6f6e 206f  onary function o
-00003500: 6620 7468 6520 7361 6d65 206e 616d 6529  f the same name)
-00003510: 2e0a 0a20 2020 2020 2020 203a 7274 7970  ...        :rtyp
-00003520: 653a 2074 7970 696e 672e 416e 790a 2020  e: typing.Any.  
-00003530: 2020 2020 2020 3a72 6574 7572 6e3a 2063        :return: c
-00003540: 7573 746f 6d20 7072 6f70 6572 7479 206b  ustom property k
-00003550: 6579 732e 0a20 2020 2020 2020 2027 2727  eys..        '''
-00003560: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00003570: 2020 2064 6566 2070 6174 685f 6672 6f6d     def path_from
-00003580: 5f69 6428 7365 6c66 2c20 7072 6f70 6572  _id(self, proper
-00003590: 7479 3a20 7479 7069 6e67 2e4f 7074 696f  ty: typing.Optio
-000035a0: 6e61 6c5b 7374 725d 203d 2022 2229 202d  nal[str] = "") -
-000035b0: 3e20 7374 723a 0a20 2020 2020 2020 2027  > str:.        '
-000035c0: 2727 2052 6574 7572 6e73 2074 6865 2064  '' Returns the d
-000035d0: 6174 6120 7061 7468 2066 726f 6d20 7468  ata path from th
-000035e0: 6520 4944 2074 6f20 7468 6973 206f 626a  e ID to this obj
-000035f0: 6563 7420 2873 7472 696e 6729 2e0a 0a20  ect (string)... 
-00003600: 2020 2020 2020 203a 7061 7261 6d20 7072         :param pr
-00003610: 6f70 6572 7479 3a20 4f70 7469 6f6e 616c  operty: Optional
-00003620: 2070 726f 7065 7274 7920 6e61 6d65 2077   property name w
-00003630: 6869 6368 2063 616e 2062 6520 7573 6564  hich can be used
-00003640: 2069 6620 7468 6520 7061 7468 2069 7320   if the path is 
-00003650: 746f 2061 2070 726f 7065 7274 7920 6f66  to a property of
-00003660: 2074 6869 7320 6f62 6a65 6374 2e0a 2020   this object..  
-00003670: 2020 2020 2020 3a74 7970 6520 7072 6f70        :type prop
-00003680: 6572 7479 3a20 7479 7069 6e67 2e4f 7074  erty: typing.Opt
-00003690: 696f 6e61 6c5b 7374 725d 0a20 2020 2020  ional[str].     
-000036a0: 2020 203a 7274 7970 653a 2073 7472 0a20     :rtype: str. 
-000036b0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-000036c0: 6062 7079 2e74 7970 6573 2e62 7079 5f73  `bpy.types.bpy_s
-000036d0: 7472 7563 742e 6964 5f64 6174 6160 2074  truct.id_data` t
-000036e0: 6f20 7468 6973 2073 7472 7563 7420 616e  o this struct an
-000036f0: 6420 7072 6f70 6572 7479 2028 7768 656e  d property (when
-00003700: 2067 6976 656e 292e 0a20 2020 2020 2020   given)..       
-00003710: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00003720: 730a 0a20 2020 2064 6566 2070 6174 685f  s..    def path_
-00003730: 7265 736f 6c76 6528 7365 6c66 2c0a 2020  resolve(self,.  
-00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003750: 2020 2070 6174 683a 2074 7970 696e 672e     path: typing.
-00003760: 4f70 7469 6f6e 616c 5b73 7472 5d2c 0a20  Optional[str],. 
-00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 2020 2020 636f 6572 6365 3a20 7479 7069      coerce: typi
-00003790: 6e67 2e4f 7074 696f 6e61 6c5b 626f 6f6c  ng.Optional[bool
-000037a0: 5d20 3d20 5472 7565 293a 0a20 2020 2020  ] = True):.     
-000037b0: 2020 2027 2727 2052 6574 7572 6e73 2074     ''' Returns t
-000037c0: 6865 2070 726f 7065 7274 7920 6672 6f6d  he property from
-000037d0: 2074 6865 2070 6174 682c 2072 6169 7365   the path, raise
-000037e0: 2061 6e20 6578 6365 7074 696f 6e20 7768   an exception wh
-000037f0: 656e 206e 6f74 2066 6f75 6e64 2e0a 0a20  en not found... 
-00003800: 2020 2020 2020 203a 7061 7261 6d20 7061         :param pa
-00003810: 7468 3a20 7061 7468 2077 6869 6368 2074  th: path which t
-00003820: 6869 7320 7072 6f70 6572 7479 2072 6573  his property res
-00003830: 6f6c 7665 732e 0a20 2020 2020 2020 203a  olves..        :
-00003840: 7479 7065 2070 6174 683a 2074 7970 696e  type path: typin
-00003850: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
-00003860: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-00003870: 6f65 7263 653a 206f 7074 696f 6e61 6c20  oerce: optional 
-00003880: 6172 6775 6d65 6e74 2c20 7768 656e 2054  argument, when T
-00003890: 7275 652c 2074 6865 2070 726f 7065 7274  rue, the propert
-000038a0: 7920 7769 6c6c 2062 6520 636f 6e76 6572  y will be conver
-000038b0: 7465 6420 696e 746f 2069 7473 2050 7974  ted into its Pyt
-000038c0: 686f 6e20 7265 7072 6573 656e 7461 7469  hon representati
-000038d0: 6f6e 2e0a 2020 2020 2020 2020 3a74 7970  on..        :typ
-000038e0: 6520 636f 6572 6365 3a20 7479 7069 6e67  e coerce: typing
-000038f0: 2e4f 7074 696f 6e61 6c5b 626f 6f6c 5d0a  .Optional[bool].
-00003900: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00003910: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00003920: 6620 706f 7028 7365 6c66 2c0a 2020 2020  f pop(self,.    
-00003930: 2020 2020 2020 2020 6b65 793a 2074 7970          key: typ
-00003940: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-00003950: 5d2c 0a20 2020 2020 2020 2020 2020 2064  ],.            d
-00003960: 6566 6175 6c74 3a20 7479 7069 6e67 2e4f  efault: typing.O
-00003970: 7074 696f 6e61 6c5b 7479 7069 6e67 2e41  ptional[typing.A
-00003980: 6e79 5d20 3d20 4e6f 6e65 293a 0a20 2020  ny] = None):.   
-00003990: 2020 2020 2027 2727 2052 656d 6f76 6520       ''' Remove 
-000039a0: 616e 6420 7265 7475 726e 2074 6865 2076  and return the v
-000039b0: 616c 7565 206f 6620 7468 6520 6375 7374  alue of the cust
-000039c0: 6f6d 2070 726f 7065 7274 7920 6173 7369  om property assi
-000039d0: 676e 6564 2074 6f20 6b65 7920 6f72 2064  gned to key or d
-000039e0: 6566 6175 6c74 2077 6865 6e20 6e6f 7420  efault when not 
-000039f0: 666f 756e 6420 286d 6174 6368 6573 2050  found (matches P
-00003a00: 7974 686f 6e27 7320 6469 6374 696f 6e61  ython's dictiona
-00003a10: 7279 2066 756e 6374 696f 6e20 6f66 2074  ry function of t
-00003a20: 6865 2073 616d 6520 6e61 6d65 292e 0a0a  he same name)...
-00003a30: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
-00003a40: 6579 3a20 5468 6520 6b65 7920 6173 736f  ey: The key asso
-00003a50: 6369 6174 6564 2077 6974 6820 7468 6520  ciated with the 
-00003a60: 6375 7374 6f6d 2070 726f 7065 7274 792e  custom property.
-00003a70: 0a20 2020 2020 2020 203a 7479 7065 206b  .        :type k
-00003a80: 6579 3a20 7479 7069 6e67 2e4f 7074 696f  ey: typing.Optio
-00003a90: 6e61 6c5b 7374 725d 0a20 2020 2020 2020  nal[str].       
-00003aa0: 203a 7061 7261 6d20 6465 6661 756c 743a   :param default:
-00003ab0: 204f 7074 696f 6e61 6c20 6172 6775 6d65   Optional argume
-00003ac0: 6e74 2066 6f72 2074 6865 2076 616c 7565  nt for the value
-00003ad0: 2074 6f20 7265 7475 726e 2069 6620 2a6b   to return if *k
-00003ae0: 6579 2a20 6973 206e 6f74 2066 6f75 6e64  ey* is not found
-00003af0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00003b00: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
-00003b10: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-00003b20: 416e 795d 0a20 2020 2020 2020 2027 2727  Any].        '''
-00003b30: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00003b40: 2020 2064 6566 2070 726f 7065 7274 795f     def property_
-00003b50: 6f76 6572 7269 6461 626c 655f 6c69 6272  overridable_libr
-00003b60: 6172 795f 7365 7428 7365 6c66 2c20 7072  ary_set(self, pr
-00003b70: 6f70 6572 7479 2c20 6f76 6572 7269 6461  operty, overrida
-00003b80: 626c 6529 202d 3e20 626f 6f6c 3a0a 2020  ble) -> bool:.  
-00003b90: 2020 2020 2020 2727 2720 4465 6669 6e65        ''' Define
-00003ba0: 2061 2070 726f 7065 7274 7920 6173 206f   a property as o
-00003bb0: 7665 7272 6964 6162 6c65 206f 7220 6e6f  verridable or no
-00003bc0: 7420 286f 6e6c 7920 666f 7220 6375 7374  t (only for cust
-00003bd0: 6f6d 2070 726f 7065 7274 6965 7321 292e  om properties!).
-00003be0: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-00003bf0: 3a20 626f 6f6c 0a20 2020 2020 2020 203a  : bool.        :
-00003c00: 7265 7475 726e 3a20 5472 7565 2077 6865  return: True whe
-00003c10: 6e20 7468 6520 6f76 6572 7269 6461 626c  n the overridabl
-00003c20: 6520 7374 6174 7573 206f 6620 7468 6520  e status of the 
-00003c30: 7072 6f70 6572 7479 2077 6173 2073 7563  property was suc
-00003c40: 6365 7373 6675 6c6c 7920 7365 742e 0a20  cessfully set.. 
-00003c50: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00003c60: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00003c70: 2070 726f 7065 7274 795f 756e 7365 7428   property_unset(
-00003c80: 7365 6c66 2c20 7072 6f70 6572 7479 293a  self, property):
-00003c90: 0a20 2020 2020 2020 2027 2727 2055 6e73  .        ''' Uns
-00003ca0: 6574 2061 2070 726f 7065 7274 792c 2077  et a property, w
-00003cb0: 696c 6c20 7573 6520 6465 6661 756c 7420  ill use default 
-00003cc0: 7661 6c75 6520 6166 7465 7277 6172 642e  value afterward.
-00003cd0: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00003ce0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00003cf0: 6465 6620 7479 7065 5f72 6563 6173 7428  def type_recast(
-00003d00: 7365 6c66 2920 2d3e 2027 6270 795f 7374  self) -> 'bpy_st
-00003d10: 7275 6374 273a 0a20 2020 2020 2020 2027  ruct':.        '
-00003d20: 2727 2052 6574 7572 6e20 6120 6e65 7720  '' Return a new 
-00003d30: 696e 7374 616e 6365 2c20 7468 6973 2069  instance, this i
-00003d40: 7320 6e65 6564 6564 2062 6563 6175 7365  s needed because
-00003d50: 2074 7970 6573 2073 7563 6820 6173 2074   types such as t
-00003d60: 6578 7475 7265 7320 6361 6e20 6265 2063  extures can be c
-00003d70: 6861 6e67 6564 2061 7420 7275 6e74 696d  hanged at runtim
-00003d80: 652e 0a0a 2020 2020 2020 2020 3a72 7479  e...        :rty
-00003d90: 7065 3a20 2762 7079 5f73 7472 7563 7427  pe: 'bpy_struct'
-00003da0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00003db0: 3a20 6120 6e65 7720 696e 7374 616e 6365  : a new instance
-00003dc0: 206f 6620 7468 6973 206f 626a 6563 7420   of this object 
-00003dd0: 7769 7468 2074 6865 2074 7970 6520 696e  with the type in
-00003de0: 6974 6961 6c69 7a65 6420 6167 6169 6e2e  itialized again.
-00003df0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00003e00: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00003e10: 6566 2076 616c 7565 7328 7365 6c66 2920  ef values(self) 
-00003e20: 2d3e 2074 7970 696e 672e 416e 793a 0a20  -> typing.Any:. 
-00003e30: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
-00003e40: 6e73 2074 6865 2076 616c 7565 7320 6f66  ns the values of
-00003e50: 2074 6869 7320 6f62 6a65 6374 7320 6375   this objects cu
-00003e60: 7374 6f6d 2070 726f 7065 7274 6965 7320  stom properties 
-00003e70: 286d 6174 6368 6573 2050 7974 686f 6e27  (matches Python'
-00003e80: 7320 6469 6374 696f 6e61 7279 2066 756e  s dictionary fun
-00003e90: 6374 696f 6e20 6f66 2074 6865 2073 616d  ction of the sam
-00003ea0: 6520 6e61 6d65 292e 0a0a 2020 2020 2020  e name)...      
-00003eb0: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
-00003ec0: 2e41 6e79 0a20 2020 2020 2020 203a 7265  .Any.        :re
-00003ed0: 7475 726e 3a20 6375 7374 6f6d 2070 726f  turn: custom pro
-00003ee0: 7065 7274 7920 7661 6c75 6573 2e0a 2020  perty values..  
-00003ef0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00003f00: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00003f10: 5f5f 6765 7469 7465 6d5f 5f28 7365 6c66  __getitem__(self
-00003f20: 2c20 6b65 793a 2074 7970 696e 672e 556e  , key: typing.Un
-00003f30: 696f 6e5b 696e 742c 2073 7472 5d29 202d  ion[int, str]) -
-00003f40: 3e20 2774 7970 696e 672e 416e 7927 3a0a  > 'typing.Any':.
-00003f50: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
-00003f60: 2020 2020 2020 3a70 6172 616d 206b 6579        :param key
-00003f70: 3a20 0a20 2020 2020 2020 203a 7479 7065  : .        :type
-00003f80: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
-00003f90: 6f6e 5b69 6e74 2c20 7374 725d 0a20 2020  on[int, str].   
-00003fa0: 2020 2020 203a 7274 7970 653a 2027 7479       :rtype: 'ty
-00003fb0: 7069 6e67 2e41 6e79 270a 2020 2020 2020  ping.Any'.      
-00003fc0: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-00003fd0: 7373 0a0a 2020 2020 6465 6620 5f5f 7365  ss..    def __se
-00003fe0: 7469 7465 6d5f 5f28 7365 6c66 2c20 6b65  titem__(self, ke
-00003ff0: 793a 2074 7970 696e 672e 556e 696f 6e5b  y: typing.Union[
-00004000: 696e 742c 2073 7472 5d2c 2076 616c 7565  int, str], value
-00004010: 3a20 2774 7970 696e 672e 416e 7927 293a  : 'typing.Any'):
-00004020: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
-00004030: 2020 2020 2020 203a 7061 7261 6d20 6b65         :param ke
-00004040: 793a 200a 2020 2020 2020 2020 3a74 7970  y: .        :typ
-00004050: 6520 6b65 793a 2074 7970 696e 672e 556e  e key: typing.Un
-00004060: 696f 6e5b 696e 742c 2073 7472 5d0a 2020  ion[int, str].  
-00004070: 2020 2020 2020 3a70 6172 616d 2076 616c        :param val
-00004080: 7565 3a20 0a20 2020 2020 2020 203a 7479  ue: .        :ty
-00004090: 7065 2076 616c 7565 3a20 2774 7970 696e  pe value: 'typin
-000040a0: 672e 416e 7927 0a20 2020 2020 2020 2027  g.Any'.        '
-000040b0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-000040c0: 0a20 2020 2064 6566 205f 5f64 656c 6974  .    def __delit
-000040d0: 656d 5f5f 2873 656c 662c 206b 6579 3a20  em__(self, key: 
-000040e0: 7479 7069 6e67 2e55 6e69 6f6e 5b69 6e74  typing.Union[int
-000040f0: 2c20 7374 725d 2920 2d3e 2027 7479 7069  , str]) -> 'typi
-00004100: 6e67 2e41 6e79 273a 0a20 2020 2020 2020  ng.Any':.       
-00004110: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
-00004120: 7061 7261 6d20 6b65 793a 200a 2020 2020  param key: .    
-00004130: 2020 2020 3a74 7970 6520 6b65 793a 2074      :type key: t
-00004140: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
-00004150: 2073 7472 5d0a 2020 2020 2020 2020 3a72   str].        :r
-00004160: 7479 7065 3a20 2774 7970 696e 672e 416e  type: 'typing.An
-00004170: 7927 0a20 2020 2020 2020 2027 2727 0a20  y'.        '''. 
+00000ad0: 7079 5f73 7472 7563 743a 0a20 2020 2027  py_struct:.    '
+00000ae0: 2727 2062 7569 6c74 2d69 6e20 6261 7365  '' built-in base
+00000af0: 2063 6c61 7373 2066 6f72 2061 6c6c 2063   class for all c
+00000b00: 6c61 7373 6573 2069 6e20 6270 792e 7479  lasses in bpy.ty
+00000b10: 7065 732e 0a20 2020 2027 2727 0a0a 2020  pes..    '''..  
+00000b20: 2020 6964 5f64 6174 6120 3d20 4e6f 6e65    id_data = None
+00000b30: 0a20 2020 2027 2727 2054 6865 2060 6270  .    ''' The `bp
+00000b40: 792e 7479 7065 732e 4944 6020 6f62 6a65  y.types.ID` obje
+00000b50: 6374 2074 6869 7320 6461 7461 626c 6f63  ct this databloc
+00000b60: 6b20 6973 2066 726f 6d20 6f72 204e 6f6e  k is from or Non
+00000b70: 652c 2028 6e6f 7420 6176 6169 6c61 626c  e, (not availabl
+00000b80: 6520 666f 7220 616c 6c20 6461 7461 2074  e for all data t
+00000b90: 7970 6573 2927 2727 0a0a 2020 2020 6465  ypes)'''..    de
+00000ba0: 6620 6173 5f70 6f69 6e74 6572 2873 656c  f as_pointer(sel
+00000bb0: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+00000bc0: 2020 2027 2727 2052 6574 7572 6e73 2074     ''' Returns t
+00000bd0: 6865 206d 656d 6f72 7920 6164 6472 6573  he memory addres
+00000be0: 7320 7768 6963 6820 686f 6c64 7320 6120  s which holds a 
+00000bf0: 706f 696e 7465 7220 746f 2042 6c65 6e64  pointer to Blend
+00000c00: 6572 2773 2069 6e74 6572 6e61 6c20 6461  er's internal da
+00000c10: 7461 0a0a 2020 2020 2020 2020 3a72 7479  ta..        :rty
+00000c20: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
+00000c30: 3a72 6574 7572 6e3a 2069 6e74 2028 6d65  :return: int (me
+00000c40: 6d6f 7279 2061 6464 7265 7373 292e 0a20  mory address).. 
+00000c50: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00000c60: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00000c70: 2064 7269 7665 725f 6164 6428 7365 6c66   driver_add(self
+00000c80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000c90: 2020 2020 2070 6174 683a 2074 7970 696e       path: typin
+00000ca0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d2c  g.Optional[str],
+00000cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000cc0: 2020 2020 696e 6465 783a 2074 7970 696e      index: typin
+00000cd0: 672e 4f70 7469 6f6e 616c 5b69 6e74 5d20  g.Optional[int] 
+00000ce0: 3d20 2d31 2920 2d3e 2027 4643 7572 7665  = -1) -> 'FCurve
+00000cf0: 273a 0a20 2020 2020 2020 2027 2727 2041  ':.        ''' A
+00000d00: 6464 7320 6472 6976 6572 2873 2920 746f  dds driver(s) to
+00000d10: 2074 6865 2067 6976 656e 2070 726f 7065   the given prope
+00000d20: 7274 790a 0a20 2020 2020 2020 203a 7061  rty..        :pa
+00000d30: 7261 6d20 7061 7468 3a20 7061 7468 2074  ram path: path t
+00000d40: 6f20 7468 6520 7072 6f70 6572 7479 2074  o the property t
+00000d50: 6f20 6472 6976 652c 2061 6e61 6c6f 676f  o drive, analogo
+00000d60: 7573 2074 6f20 7468 6520 6663 7572 7665  us to the fcurve
+00000d70: 2773 2064 6174 6120 7061 7468 2e0a 2020  's data path..  
+00000d80: 2020 2020 2020 3a74 7970 6520 7061 7468        :type path
+00000d90: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00000da0: 6c5b 7374 725d 0a20 2020 2020 2020 203a  l[str].        :
+00000db0: 7061 7261 6d20 696e 6465 783a 2061 7272  param index: arr
+00000dc0: 6179 2069 6e64 6578 206f 6620 7468 6520  ay index of the 
+00000dd0: 7072 6f70 6572 7479 2064 7269 7665 2e20  property drive. 
+00000de0: 4465 6661 756c 7473 2074 6f20 2d31 2066  Defaults to -1 f
+00000df0: 6f72 2061 6c6c 2069 6e64 6963 6573 206f  or all indices o
+00000e00: 7220 6120 7369 6e67 6c65 2063 6861 6e6e  r a single chann
+00000e10: 656c 2069 6620 7468 6520 7072 6f70 6572  el if the proper
+00000e20: 7479 2069 7320 6e6f 7420 616e 2061 7272  ty is not an arr
+00000e30: 6179 2e0a 2020 2020 2020 2020 3a74 7970  ay..        :typ
+00000e40: 6520 696e 6465 783a 2074 7970 696e 672e  e index: typing.
+00000e50: 4f70 7469 6f6e 616c 5b69 6e74 5d0a 2020  Optional[int].  
+00000e60: 2020 2020 2020 3a72 7479 7065 3a20 2746        :rtype: 'F
+00000e70: 4375 7276 6527 0a20 2020 2020 2020 203a  Curve'.        :
+00000e80: 7265 7475 726e 3a20 5468 6520 6472 6976  return: The driv
+00000e90: 6572 2873 2920 6164 6465 642e 0a20 2020  er(s) added..   
+00000ea0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00000eb0: 2070 6173 730a 0a20 2020 2064 6566 2064   pass..    def d
+00000ec0: 7269 7665 725f 7265 6d6f 7665 2873 656c  river_remove(sel
+00000ed0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+00000ee0: 2020 2020 2020 2020 2070 6174 683a 2074           path: t
+00000ef0: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
+00000f00: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
+00000f10: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+00000f20: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00000f30: 6c5b 696e 745d 203d 202d 3129 202d 3e20  l[int] = -1) -> 
+00000f40: 626f 6f6c 3a0a 2020 2020 2020 2020 2727  bool:.        ''
+00000f50: 2720 5265 6d6f 7665 2064 7269 7665 7228  ' Remove driver(
+00000f60: 7329 2066 726f 6d20 7468 6520 6769 7665  s) from the give
+00000f70: 6e20 7072 6f70 6572 7479 0a0a 2020 2020  n property..    
+00000f80: 2020 2020 3a70 6172 616d 2070 6174 683a      :param path:
+00000f90: 2070 6174 6820 746f 2074 6865 2070 726f   path to the pro
+00000fa0: 7065 7274 7920 746f 2064 7269 7665 2c20  perty to drive, 
+00000fb0: 616e 616c 6f67 6f75 7320 746f 2074 6865  analogous to the
+00000fc0: 2066 6375 7276 6527 7320 6461 7461 2070   fcurve's data p
+00000fd0: 6174 682e 0a20 2020 2020 2020 203a 7479  ath..        :ty
+00000fe0: 7065 2070 6174 683a 2074 7970 696e 672e  pe path: typing.
+00000ff0: 4f70 7469 6f6e 616c 5b73 7472 5d0a 2020  Optional[str].  
+00001000: 2020 2020 2020 3a70 6172 616d 2069 6e64        :param ind
+00001010: 6578 3a20 6172 7261 7920 696e 6465 7820  ex: array index 
+00001020: 6f66 2074 6865 2070 726f 7065 7274 7920  of the property 
+00001030: 6472 6976 652e 2044 6566 6175 6c74 7320  drive. Defaults 
+00001040: 746f 202d 3120 666f 7220 616c 6c20 696e  to -1 for all in
+00001050: 6469 6365 7320 6f72 2061 2073 696e 676c  dices or a singl
+00001060: 6520 6368 616e 6e65 6c20 6966 2074 6865  e channel if the
+00001070: 2070 726f 7065 7274 7920 6973 206e 6f74   property is not
+00001080: 2061 6e20 6172 7261 792e 0a20 2020 2020   an array..     
+00001090: 2020 203a 7479 7065 2069 6e64 6578 3a20     :type index: 
+000010a0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+000010b0: 696e 745d 0a20 2020 2020 2020 203a 7274  int].        :rt
+000010c0: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+000010d0: 2020 3a72 6574 7572 6e3a 2053 7563 6365    :return: Succe
+000010e0: 7373 206f 6620 6472 6976 6572 2072 656d  ss of driver rem
+000010f0: 6f76 616c 2e0a 2020 2020 2020 2020 2727  oval..        ''
+00001100: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00001110: 2020 2020 6465 6620 6765 7428 7365 6c66      def get(self
+00001120: 2c0a 2020 2020 2020 2020 2020 2020 6b65  ,.            ke
+00001130: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
+00001140: 616c 5b73 7472 5d2c 0a20 2020 2020 2020  al[str],.       
+00001150: 2020 2020 2064 6566 6175 6c74 3a20 7479       default: ty
+00001160: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+00001170: 7069 6e67 2e41 6e79 5d20 3d20 4e6f 6e65  ping.Any] = None
+00001180: 293a 0a20 2020 2020 2020 2027 2727 2052  ):.        ''' R
+00001190: 6574 7572 6e73 2074 6865 2076 616c 7565  eturns the value
+000011a0: 206f 6620 7468 6520 6375 7374 6f6d 2070   of the custom p
+000011b0: 726f 7065 7274 7920 6173 7369 676e 6564  roperty assigned
+000011c0: 2074 6f20 6b65 7920 6f72 2064 6566 6175   to key or defau
+000011d0: 6c74 2077 6865 6e20 6e6f 7420 666f 756e  lt when not foun
+000011e0: 6420 286d 6174 6368 6573 2050 7974 686f  d (matches Pytho
+000011f0: 6e27 7320 6469 6374 696f 6e61 7279 2066  n's dictionary f
+00001200: 756e 6374 696f 6e20 6f66 2074 6865 2073  unction of the s
+00001210: 616d 6520 6e61 6d65 292e 0a0a 2020 2020  ame name)...    
+00001220: 2020 2020 3a70 6172 616d 206b 6579 3a20      :param key: 
+00001230: 5468 6520 6b65 7920 6173 736f 6369 6174  The key associat
+00001240: 6564 2077 6974 6820 7468 6520 6375 7374  ed with the cust
+00001250: 6f6d 2070 726f 7065 7274 792e 0a20 2020  om property..   
+00001260: 2020 2020 203a 7479 7065 206b 6579 3a20       :type key: 
+00001270: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00001280: 7374 725d 0a20 2020 2020 2020 203a 7061  str].        :pa
+00001290: 7261 6d20 6465 6661 756c 743a 204f 7074  ram default: Opt
+000012a0: 696f 6e61 6c20 6172 6775 6d65 6e74 2066  ional argument f
+000012b0: 6f72 2074 6865 2076 616c 7565 2074 6f20  or the value to 
+000012c0: 7265 7475 726e 2069 6620 2a6b 6579 2a20  return if *key* 
+000012d0: 6973 206e 6f74 2066 6f75 6e64 2e0a 2020  is not found..  
+000012e0: 2020 2020 2020 3a74 7970 6520 6465 6661        :type defa
+000012f0: 756c 743a 2074 7970 696e 672e 4f70 7469  ult: typing.Opti
+00001300: 6f6e 616c 5b74 7970 696e 672e 416e 795d  onal[typing.Any]
+00001310: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00001320: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00001330: 6566 2069 645f 7072 6f70 6572 7469 6573  ef id_properties
+00001340: 5f63 6c65 6172 2873 656c 6629 3a0a 2020  _clear(self):.  
+00001350: 2020 2020 2020 2727 2720 0a0a 2020 2020        ''' ..    
+00001360: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00001370: 7061 7373 0a0a 2020 2020 6465 6620 6964  pass..    def id
+00001380: 5f70 726f 7065 7274 6965 735f 656e 7375  _properties_ensu
+00001390: 7265 2873 656c 6629 202d 3e20 7479 7069  re(self) -> typi
+000013a0: 6e67 2e41 6e79 3a0a 2020 2020 2020 2020  ng.Any:.        
+000013b0: 2727 2720 0a0a 2020 2020 2020 2020 3a72  ''' ..        :r
+000013c0: 7479 7065 3a20 7479 7069 6e67 2e41 6e79  type: typing.Any
+000013d0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+000013e0: 3a20 7468 6520 7061 7265 6e74 2067 726f  : the parent gro
+000013f0: 7570 2066 6f72 2061 6e20 524e 4120 7374  up for an RNA st
+00001400: 7275 6374 2773 2063 7573 746f 6d20 4944  ruct's custom ID
+00001410: 5072 6f70 6572 7469 6573 2e0a 2020 2020  Properties..    
+00001420: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00001430: 7061 7373 0a0a 2020 2020 6465 6620 6964  pass..    def id
+00001440: 5f70 726f 7065 7274 6965 735f 7569 2873  _properties_ui(s
+00001450: 656c 662c 206b 6579 3a20 7479 7069 6e67  elf, key: typing
+00001460: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+00001470: 2e41 6e79 5d29 202d 3e20 7479 7069 6e67  .Any]) -> typing
+00001480: 2e41 6e79 3a0a 2020 2020 2020 2020 2727  .Any:.        ''
+00001490: 2720 0a0a 2020 2020 2020 2020 3a70 6172  ' ..        :par
+000014a0: 616d 206b 6579 3a20 2053 7472 696e 6720  am key:  String 
+000014b0: 6e61 6d65 206f 6620 7468 6520 7072 6f70  name of the prop
+000014c0: 6572 7479 2e0a 2020 2020 2020 2020 3a74  erty..        :t
+000014d0: 7970 6520 6b65 793a 2074 7970 696e 672e  ype key: typing.
+000014e0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+000014f0: 416e 795d 0a20 2020 2020 2020 203a 7274  Any].        :rt
+00001500: 7970 653a 2074 7970 696e 672e 416e 790a  ype: typing.Any.
+00001510: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00001520: 2052 6574 7572 6e20 616e 206f 626a 6563   Return an objec
+00001530: 7420 7573 6564 2074 6f20 6d61 6e61 6765  t used to manage
+00001540: 2061 6e20 4944 5072 6f70 6572 7479 2773   an IDProperty's
+00001550: 2055 4920 6461 7461 2e0a 2020 2020 2020   UI data..      
+00001560: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00001570: 7373 0a0a 2020 2020 6465 6620 6973 5f70  ss..    def is_p
+00001580: 726f 7065 7274 795f 6869 6464 656e 2873  roperty_hidden(s
+00001590: 656c 662c 2070 726f 7065 7274 7929 202d  elf, property) -
+000015a0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+000015b0: 2727 2720 4368 6563 6b20 6966 2061 2070  ''' Check if a p
+000015c0: 726f 7065 7274 7920 6973 2068 6964 6465  roperty is hidde
+000015d0: 6e2e 0a0a 2020 2020 2020 2020 3a72 7479  n...        :rty
+000015e0: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
+000015f0: 203a 7265 7475 726e 3a20 5472 7565 2077   :return: True w
+00001600: 6865 6e20 7468 6520 7072 6f70 6572 7479  hen the property
+00001610: 2069 7320 6869 6464 656e 2e0a 2020 2020   is hidden..    
+00001620: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00001630: 7061 7373 0a0a 2020 2020 6465 6620 6973  pass..    def is
+00001640: 5f70 726f 7065 7274 795f 6f76 6572 7269  _property_overri
+00001650: 6461 626c 655f 6c69 6272 6172 7928 7365  dable_library(se
+00001660: 6c66 2c20 7072 6f70 6572 7479 2920 2d3e  lf, property) ->
+00001670: 2062 6f6f 6c3a 0a20 2020 2020 2020 2027   bool:.        '
+00001680: 2727 2043 6865 636b 2069 6620 6120 7072  '' Check if a pr
+00001690: 6f70 6572 7479 2069 7320 6f76 6572 7269  operty is overri
+000016a0: 6461 626c 652e 0a0a 2020 2020 2020 2020  dable...        
+000016b0: 3a72 7479 7065 3a20 626f 6f6c 0a20 2020  :rtype: bool.   
+000016c0: 2020 2020 203a 7265 7475 726e 3a20 5472       :return: Tr
+000016d0: 7565 2077 6865 6e20 7468 6520 7072 6f70  ue when the prop
+000016e0: 6572 7479 2069 7320 6f76 6572 7269 6461  erty is overrida
+000016f0: 626c 652e 0a20 2020 2020 2020 2027 2727  ble..        '''
+00001700: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00001710: 2020 2064 6566 2069 735f 7072 6f70 6572     def is_proper
+00001720: 7479 5f72 6561 646f 6e6c 7928 7365 6c66  ty_readonly(self
+00001730: 2c20 7072 6f70 6572 7479 2920 2d3e 2062  , property) -> b
+00001740: 6f6f 6c3a 0a20 2020 2020 2020 2027 2727  ool:.        '''
+00001750: 2043 6865 636b 2069 6620 6120 7072 6f70   Check if a prop
+00001760: 6572 7479 2069 7320 7265 6164 6f6e 6c79  erty is readonly
+00001770: 2e0a 0a20 2020 2020 2020 203a 7274 7970  ...        :rtyp
+00001780: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+00001790: 3a72 6574 7572 6e3a 2054 7275 6520 7768  :return: True wh
+000017a0: 656e 2074 6865 2070 726f 7065 7274 7920  en the property 
+000017b0: 6973 2072 6561 646f 6e6c 7920 286e 6f74  is readonly (not
+000017c0: 2077 7269 7461 626c 6529 2e0a 2020 2020   writable)..    
+000017d0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+000017e0: 7061 7373 0a0a 2020 2020 6465 6620 6973  pass..    def is
+000017f0: 5f70 726f 7065 7274 795f 7365 7428 7365  _property_set(se
+00001800: 6c66 2c20 7072 6f70 6572 7479 2c0a 2020  lf, property,.  
+00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001820: 2020 2020 2020 6768 6f73 743a 2074 7970        ghost: typ
+00001830: 696e 672e 4f70 7469 6f6e 616c 5b62 6f6f  ing.Optional[boo
+00001840: 6c5d 203d 2054 7275 6529 202d 3e20 626f  l] = True) -> bo
+00001850: 6f6c 3a0a 2020 2020 2020 2020 2727 2720  ol:.        ''' 
+00001860: 4368 6563 6b20 6966 2061 2070 726f 7065  Check if a prope
+00001870: 7274 7920 6973 2073 6574 2c20 7573 6520  rty is set, use 
+00001880: 666f 7220 7465 7374 696e 6720 6f70 6572  for testing oper
+00001890: 6174 6f72 2070 726f 7065 7274 6965 732e  ator properties.
+000018a0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000018b0: 2067 686f 7374 3a20 5573 6564 2066 6f72   ghost: Used for
+000018c0: 206f 7065 7261 746f 7273 2074 6861 7420   operators that 
+000018d0: 7265 2d72 756e 2077 6974 6820 7072 6576  re-run with prev
+000018e0: 696f 7573 2073 6574 7469 6e67 732e 2049  ious settings. I
+000018f0: 6e20 7468 6973 2063 6173 6520 7468 6520  n this case the 
+00001900: 7072 6f70 6572 7479 2069 7320 6e6f 7420  property is not 
+00001910: 6d61 726b 6564 2061 7320 7365 742c 2079  marked as set, y
+00001920: 6574 2074 6865 2076 616c 7565 2066 726f  et the value fro
+00001930: 6d20 7468 6520 7072 6576 696f 7573 2065  m the previous e
+00001940: 7865 6375 7469 6f6e 2069 7320 7573 6564  xecution is used
+00001950: 2e20 496e 2072 6172 6520 6361 7365 7320  . In rare cases 
+00001960: 796f 7520 6d61 7920 7761 6e74 2074 6f20  you may want to 
+00001970: 7365 7420 7468 6973 206f 7074 696f 6e20  set this option 
+00001980: 746f 2066 616c 7365 2e0a 2020 2020 2020  to false..      
+00001990: 2020 3a74 7970 6520 6768 6f73 743a 2074    :type ghost: t
+000019a0: 7970 696e 672e 4f70 7469 6f6e 616c 5b62  yping.Optional[b
+000019b0: 6f6f 6c5d 0a20 2020 2020 2020 203a 7274  ool].        :rt
+000019c0: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+000019d0: 2020 3a72 6574 7572 6e3a 2054 7275 6520    :return: True 
+000019e0: 7768 656e 2074 6865 2070 726f 7065 7274  when the propert
+000019f0: 7920 6861 7320 6265 656e 2073 6574 2e0a  y has been set..
+00001a00: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00001a10: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+00001a20: 6620 6974 656d 7328 7365 6c66 2920 2d3e  f items(self) ->
+00001a30: 2074 7970 696e 672e 416e 793a 0a20 2020   typing.Any:.   
+00001a40: 2020 2020 2027 2727 2052 6574 7572 6e73       ''' Returns
+00001a50: 2074 6865 2069 7465 6d73 206f 6620 7468   the items of th
+00001a60: 6973 206f 626a 6563 7473 2063 7573 746f  is objects custo
+00001a70: 6d20 7072 6f70 6572 7469 6573 2028 6d61  m properties (ma
+00001a80: 7463 6865 7320 5079 7468 6f6e 2773 2064  tches Python's d
+00001a90: 6963 7469 6f6e 6172 7920 6675 6e63 7469  ictionary functi
+00001aa0: 6f6e 206f 6620 7468 6520 7361 6d65 206e  on of the same n
+00001ab0: 616d 6529 2e0a 0a20 2020 2020 2020 203a  ame)...        :
+00001ac0: 7274 7970 653a 2074 7970 696e 672e 416e  rtype: typing.An
+00001ad0: 790a 2020 2020 2020 2020 3a72 6574 7572  y.        :retur
+00001ae0: 6e3a 2063 7573 746f 6d20 7072 6f70 6572  n: custom proper
+00001af0: 7479 206b 6579 2c20 7661 6c75 6520 7061  ty key, value pa
+00001b00: 6972 732e 0a20 2020 2020 2020 2027 2727  irs..        '''
+00001b10: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00001b20: 2020 2064 6566 206b 6579 6672 616d 655f     def keyframe_
+00001b30: 6465 6c65 7465 280a 2020 2020 2020 2020  delete(.        
+00001b40: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00001b50: 2020 2020 2020 6461 7461 5f70 6174 683a        data_path:
+00001b60: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00001b70: 5b73 7472 5d2c 0a20 2020 2020 2020 2020  [str],.         
+00001b80: 2020 2069 6e64 6578 3a20 7479 7069 6e67     index: typing
+00001b90: 2e4f 7074 696f 6e61 6c5b 696e 745d 203d  .Optional[int] =
+00001ba0: 202d 312c 0a20 2020 2020 2020 2020 2020   -1,.           
+00001bb0: 2066 7261 6d65 3a20 7479 7069 6e67 2e4f   frame: typing.O
+00001bc0: 7074 696f 6e61 6c5b 666c 6f61 745d 203d  ptional[float] =
+00001bd0: 2027 6270 792e 636f 6e74 6578 742e 7363   'bpy.context.sc
+00001be0: 656e 652e 6672 616d 655f 6375 7272 656e  ene.frame_curren
+00001bf0: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
+00001c00: 6772 6f75 703a 2074 7970 696e 672e 4f70  group: typing.Op
+00001c10: 7469 6f6e 616c 5b73 7472 5d20 3d20 2222  tional[str] = ""
+00001c20: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00001c30: 2020 2027 2727 2052 656d 6f76 6520 6120     ''' Remove a 
+00001c40: 6b65 7966 7261 6d65 2066 726f 6d20 7468  keyframe from th
+00001c50: 6973 2070 726f 7065 7274 6965 7320 6663  is properties fc
+00001c60: 7572 7665 2e0a 0a20 2020 2020 2020 203a  urve...        :
+00001c70: 7061 7261 6d20 6461 7461 5f70 6174 683a  param data_path:
+00001c80: 2070 6174 6820 746f 2074 6865 2070 726f   path to the pro
+00001c90: 7065 7274 7920 746f 2072 656d 6f76 6520  perty to remove 
+00001ca0: 6120 6b65 792c 2061 6e61 6c6f 676f 7573  a key, analogous
+00001cb0: 2074 6f20 7468 6520 6663 7572 7665 2773   to the fcurve's
+00001cc0: 2064 6174 6120 7061 7468 2e0a 2020 2020   data path..    
+00001cd0: 2020 2020 3a74 7970 6520 6461 7461 5f70      :type data_p
+00001ce0: 6174 683a 2074 7970 696e 672e 4f70 7469  ath: typing.Opti
+00001cf0: 6f6e 616c 5b73 7472 5d0a 2020 2020 2020  onal[str].      
+00001d00: 2020 3a70 6172 616d 2069 6e64 6578 3a20    :param index: 
+00001d10: 6172 7261 7920 696e 6465 7820 6f66 2074  array index of t
+00001d20: 6865 2070 726f 7065 7274 7920 746f 2072  he property to r
+00001d30: 656d 6f76 6520 6120 6b65 792e 2044 6566  emove a key. Def
+00001d40: 6175 6c74 7320 746f 202d 3120 7265 6d6f  aults to -1 remo
+00001d50: 7669 6e67 2061 6c6c 2069 6e64 6963 6573  ving all indices
+00001d60: 206f 7220 6120 7369 6e67 6c65 2063 6861   or a single cha
+00001d70: 6e6e 656c 2069 6620 7468 6520 7072 6f70  nnel if the prop
+00001d80: 6572 7479 2069 7320 6e6f 7420 616e 2061  erty is not an a
+00001d90: 7272 6179 2e0a 2020 2020 2020 2020 3a74  rray..        :t
+00001da0: 7970 6520 696e 6465 783a 2074 7970 696e  ype index: typin
+00001db0: 672e 4f70 7469 6f6e 616c 5b69 6e74 5d0a  g.Optional[int].
+00001dc0: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
+00001dd0: 7261 6d65 3a20 5468 6520 6672 616d 6520  rame: The frame 
+00001de0: 6f6e 2077 6869 6368 2074 6865 206b 6579  on which the key
+00001df0: 6672 616d 6520 6973 2064 656c 6574 6564  frame is deleted
+00001e00: 2c20 6465 6661 756c 7469 6e67 2074 6f20  , defaulting to 
+00001e10: 7468 6520 6375 7272 656e 7420 6672 616d  the current fram
+00001e20: 652e 0a20 2020 2020 2020 203a 7479 7065  e..        :type
+00001e30: 2066 7261 6d65 3a20 7479 7069 6e67 2e4f   frame: typing.O
+00001e40: 7074 696f 6e61 6c5b 666c 6f61 745d 0a20  ptional[float]. 
+00001e50: 2020 2020 2020 203a 7061 7261 6d20 6772         :param gr
+00001e60: 6f75 703a 2054 6865 206e 616d 6520 6f66  oup: The name of
+00001e70: 2074 6865 2067 726f 7570 2074 6865 2046   the group the F
+00001e80: 2d43 7572 7665 2073 686f 756c 6420 6265  -Curve should be
+00001e90: 2061 6464 6564 2074 6f20 6966 2069 7420   added to if it 
+00001ea0: 646f 6573 6e27 7420 6578 6973 7420 7965  doesn't exist ye
+00001eb0: 742e 0a20 2020 2020 2020 203a 7479 7065  t..        :type
+00001ec0: 2067 726f 7570 3a20 7479 7069 6e67 2e4f   group: typing.O
+00001ed0: 7074 696f 6e61 6c5b 7374 725d 0a20 2020  ptional[str].   
+00001ee0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+00001ef0: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
+00001f00: 6e3a 2053 7563 6365 7373 206f 6620 6b65  n: Success of ke
+00001f10: 7966 7261 6d65 2064 656c 6574 696f 6e2e  yframe deletion.
+00001f20: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00001f30: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00001f40: 6566 206b 6579 6672 616d 655f 696e 7365  ef keyframe_inse
+00001f50: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
+00001f60: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00001f70: 2020 6461 7461 5f70 6174 683a 2074 7970    data_path: typ
+00001f80: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+00001f90: 5d2c 0a20 2020 2020 2020 2020 2020 2069  ],.            i
+00001fa0: 6e64 6578 3a20 7479 7069 6e67 2e4f 7074  ndex: typing.Opt
+00001fb0: 696f 6e61 6c5b 696e 745d 203d 202d 312c  ional[int] = -1,
+00001fc0: 0a20 2020 2020 2020 2020 2020 2066 7261  .            fra
+00001fd0: 6d65 3a20 7479 7069 6e67 2e4f 7074 696f  me: typing.Optio
+00001fe0: 6e61 6c5b 666c 6f61 745d 203d 2027 6270  nal[float] = 'bp
+00001ff0: 792e 636f 6e74 6578 742e 7363 656e 652e  y.context.scene.
+00002000: 6672 616d 655f 6375 7272 656e 7427 2c0a  frame_current',.
+00002010: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
+00002020: 703a 2074 7970 696e 672e 4f70 7469 6f6e  p: typing.Option
+00002030: 616c 5b73 7472 5d20 3d20 2222 2c0a 2020  al[str] = "",.  
+00002040: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
+00002050: 733a 2074 7970 696e 672e 4f70 7469 6f6e  s: typing.Option
+00002060: 616c 5b74 7970 696e 672e 416e 795d 203d  al[typing.Any] =
+00002070: 2027 7365 7428 2927 2920 2d3e 2062 6f6f   'set()') -> boo
+00002080: 6c3a 0a20 2020 2020 2020 2027 2727 2049  l:.        ''' I
+00002090: 6e73 6572 7420 6120 6b65 7966 7261 6d65  nsert a keyframe
+000020a0: 206f 6e20 7468 6520 7072 6f70 6572 7479   on the property
+000020b0: 2067 6976 656e 2c20 6164 6469 6e67 2066   given, adding f
+000020c0: 6375 7276 6573 2061 6e64 2061 6e69 6d61  curves and anima
+000020d0: 7469 6f6e 2064 6174 6120 7768 656e 206e  tion data when n
+000020e0: 6563 6573 7361 7279 2e20 5468 6973 2069  ecessary. This i
+000020f0: 7320 7468 6520 6d6f 7374 2073 696d 706c  s the most simpl
+00002100: 6520 6578 616d 706c 6520 6f66 2069 6e73  e example of ins
+00002110: 6572 7469 6e67 2061 206b 6579 6672 616d  erting a keyfram
+00002120: 6520 6672 6f6d 2070 7974 686f 6e2e 204e  e from python. N
+00002130: 6f74 6520 7468 6174 2077 6865 6e20 6b65  ote that when ke
+00002140: 7969 6e67 2064 6174 6120 7061 7468 7320  ying data paths 
+00002150: 7768 6963 6820 636f 6e74 6169 6e20 6e65  which contain ne
+00002160: 7374 6564 2070 726f 7065 7274 6965 7320  sted properties 
+00002170: 7468 6973 206d 7573 7420 6265 2064 6f6e  this must be don
+00002180: 6520 6672 6f6d 2074 6865 2060 4944 6020  e from the `ID` 
+00002190: 7375 6263 6c61 7373 2c20 696e 2074 6869  subclass, in thi
+000021a0: 7320 6361 7365 2074 6865 2060 4172 6d61  s case the `Arma
+000021b0: 7475 7265 6020 7261 7468 6572 2074 6861  ture` rather tha
+000021c0: 6e20 7468 6520 626f 6e65 2e0a 0a20 2020  n the bone...   
+000021d0: 2020 2020 203a 7061 7261 6d20 6461 7461       :param data
+000021e0: 5f70 6174 683a 2070 6174 6820 746f 2074  _path: path to t
+000021f0: 6865 2070 726f 7065 7274 7920 746f 206b  he property to k
+00002200: 6579 2c20 616e 616c 6f67 6f75 7320 746f  ey, analogous to
+00002210: 2074 6865 2066 6375 7276 6527 7320 6461   the fcurve's da
+00002220: 7461 2070 6174 682e 0a20 2020 2020 2020  ta path..       
+00002230: 203a 7479 7065 2064 6174 615f 7061 7468   :type data_path
+00002240: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00002250: 6c5b 7374 725d 0a20 2020 2020 2020 203a  l[str].        :
+00002260: 7061 7261 6d20 696e 6465 783a 2061 7272  param index: arr
+00002270: 6179 2069 6e64 6578 206f 6620 7468 6520  ay index of the 
+00002280: 7072 6f70 6572 7479 2074 6f20 6b65 792e  property to key.
+00002290: 2044 6566 6175 6c74 7320 746f 202d 3120   Defaults to -1 
+000022a0: 7768 6963 6820 7769 6c6c 206b 6579 2061  which will key a
+000022b0: 6c6c 2069 6e64 6963 6573 206f 7220 6120  ll indices or a 
+000022c0: 7369 6e67 6c65 2063 6861 6e6e 656c 2069  single channel i
+000022d0: 6620 7468 6520 7072 6f70 6572 7479 2069  f the property i
+000022e0: 7320 6e6f 7420 616e 2061 7272 6179 2e0a  s not an array..
+000022f0: 2020 2020 2020 2020 3a74 7970 6520 696e          :type in
+00002300: 6465 783a 2074 7970 696e 672e 4f70 7469  dex: typing.Opti
+00002310: 6f6e 616c 5b69 6e74 5d0a 2020 2020 2020  onal[int].      
+00002320: 2020 3a70 6172 616d 2066 7261 6d65 3a20    :param frame: 
+00002330: 5468 6520 6672 616d 6520 6f6e 2077 6869  The frame on whi
+00002340: 6368 2074 6865 206b 6579 6672 616d 6520  ch the keyframe 
+00002350: 6973 2069 6e73 6572 7465 642c 2064 6566  is inserted, def
+00002360: 6175 6c74 696e 6720 746f 2074 6865 2063  aulting to the c
+00002370: 7572 7265 6e74 2066 7261 6d65 2e0a 2020  urrent frame..  
+00002380: 2020 2020 2020 3a74 7970 6520 6672 616d        :type fram
+00002390: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
+000023a0: 616c 5b66 6c6f 6174 5d0a 2020 2020 2020  al[float].      
+000023b0: 2020 3a70 6172 616d 2067 726f 7570 3a20    :param group: 
+000023c0: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+000023d0: 6772 6f75 7020 7468 6520 462d 4375 7276  group the F-Curv
+000023e0: 6520 7368 6f75 6c64 2062 6520 6164 6465  e should be adde
+000023f0: 6420 746f 2069 6620 6974 2064 6f65 736e  d to if it doesn
+00002400: 2774 2065 7869 7374 2079 6574 2e0a 2020  't exist yet..  
+00002410: 2020 2020 2020 3a74 7970 6520 6772 6f75        :type grou
+00002420: 703a 2074 7970 696e 672e 4f70 7469 6f6e  p: typing.Option
+00002430: 616c 5b73 7472 5d0a 2020 2020 2020 2020  al[str].        
+00002440: 3a70 6172 616d 2066 6c61 673a 200a 2020  :param flag: .  
+00002450: 2020 2020 2020 3a74 7970 6520 666c 6167        :type flag
+00002460: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00002470: 6c5b 7479 7069 6e67 2e53 6574 5d0a 2020  l[typing.Set].  
+00002480: 2020 2020 2020 3a70 6172 616d 206f 7074        :param opt
+00002490: 696f 6e73 3a20 202d 2060 6049 4e53 4552  ions:  - ``INSER
+000024a0: 544b 4559 5f4e 4545 4445 4460 6020 4f6e  TKEY_NEEDED`` On
+000024b0: 6c79 2069 6e73 6572 7420 6b65 7966 7261  ly insert keyfra
+000024c0: 6d65 7320 7768 6572 6520 7468 6579 2772  mes where they'r
+000024d0: 6520 6e65 6564 6564 2069 6e20 7468 6520  e needed in the 
+000024e0: 7265 6c65 7661 6e74 2046 2d43 7572 7665  relevant F-Curve
+000024f0: 732e 202d 2060 6049 4e53 4552 544b 4559  s. - ``INSERTKEY
+00002500: 5f56 4953 5541 4c60 6020 496e 7365 7274  _VISUAL`` Insert
+00002510: 206b 6579 6672 616d 6573 2062 6173 6564   keyframes based
+00002520: 206f 6e20 2776 6973 7561 6c20 7472 616e   on 'visual tran
+00002530: 7366 6f72 6d73 272e 202d 2060 6049 4e53  sforms'. - ``INS
+00002540: 4552 544b 4559 5f58 595a 5f54 4f5f 5247  ERTKEY_XYZ_TO_RG
+00002550: 4260 6020 436f 6c6f 7220 666f 7220 6e65  B`` Color for ne
+00002560: 776c 7920 6164 6465 6420 7472 616e 7366  wly added transf
+00002570: 6f72 6d61 7469 6f6e 2046 2d43 7572 7665  ormation F-Curve
+00002580: 7320 284c 6f63 6174 696f 6e2c 2052 6f74  s (Location, Rot
+00002590: 6174 696f 6e2c 2053 6361 6c65 2920 6973  ation, Scale) is
+000025a0: 2062 6173 6564 206f 6e20 7468 6520 7472   based on the tr
+000025b0: 616e 7366 6f72 6d20 6178 6973 2e20 2d20  ansform axis. - 
+000025c0: 6060 494e 5345 5254 4b45 595f 5245 504c  ``INSERTKEY_REPL
+000025d0: 4143 4560 6020 4f6e 6c79 2072 6570 6c61  ACE`` Only repla
+000025e0: 6365 2061 6c72 6561 6479 2065 7869 7374  ce already exist
+000025f0: 696e 6720 6b65 7966 7261 6d65 732e 202d  ing keyframes. -
+00002600: 2060 6049 4e53 4552 544b 4559 5f41 5641   ``INSERTKEY_AVA
+00002610: 494c 4142 4c45 6060 204f 6e6c 7920 696e  ILABLE`` Only in
+00002620: 7365 7274 2069 6e74 6f20 616c 7265 6164  sert into alread
+00002630: 7920 6578 6973 7469 6e67 2046 2d43 7572  y existing F-Cur
+00002640: 7665 732e 202d 2060 6049 4e53 4552 544b  ves. - ``INSERTK
+00002650: 4559 5f43 5943 4c45 5f41 5741 5245 6060  EY_CYCLE_AWARE``
+00002660: 2054 616b 6520 6379 636c 6963 2065 7874   Take cyclic ext
+00002670: 7261 706f 6c61 7469 6f6e 2069 6e74 6f20  rapolation into 
+00002680: 6163 636f 756e 7420 2843 7963 6c65 2d41  account (Cycle-A
+00002690: 7761 7265 204b 6579 696e 6720 6f70 7469  ware Keying opti
+000026a0: 6f6e 292e 0a20 2020 2020 2020 203a 7479  on)..        :ty
+000026b0: 7065 206f 7074 696f 6e73 3a20 7479 7069  pe options: typi
+000026c0: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
+000026d0: 6e67 2e41 6e79 5d0a 2020 2020 2020 2020  ng.Any].        
+000026e0: 3a72 7479 7065 3a20 626f 6f6c 0a20 2020  :rtype: bool.   
+000026f0: 2020 2020 203a 7265 7475 726e 3a20 5375       :return: Su
+00002700: 6363 6573 7320 6f66 206b 6579 6672 616d  ccess of keyfram
+00002710: 6520 696e 7365 7274 696f 6e2e 0a20 2020  e insertion..   
+00002720: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00002730: 2070 6173 730a 0a20 2020 2064 6566 206b   pass..    def k
+00002740: 6579 7328 7365 6c66 2920 2d3e 2074 7970  eys(self) -> typ
+00002750: 696e 672e 416e 793a 0a20 2020 2020 2020  ing.Any:.       
+00002760: 2027 2727 2052 6574 7572 6e73 2074 6865   ''' Returns the
+00002770: 206b 6579 7320 6f66 2074 6869 7320 6f62   keys of this ob
+00002780: 6a65 6374 7320 6375 7374 6f6d 2070 726f  jects custom pro
+00002790: 7065 7274 6965 7320 286d 6174 6368 6573  perties (matches
+000027a0: 2050 7974 686f 6e27 7320 6469 6374 696f   Python's dictio
+000027b0: 6e61 7279 2066 756e 6374 696f 6e20 6f66  nary function of
+000027c0: 2074 6865 2073 616d 6520 6e61 6d65 292e   the same name).
+000027d0: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+000027e0: 3a20 7479 7069 6e67 2e41 6e79 0a20 2020  : typing.Any.   
+000027f0: 2020 2020 203a 7265 7475 726e 3a20 6375       :return: cu
+00002800: 7374 6f6d 2070 726f 7065 7274 7920 6b65  stom property ke
+00002810: 7973 2e0a 2020 2020 2020 2020 2727 270a  ys..        '''.
+00002820: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00002830: 2020 6465 6620 7061 7468 5f66 726f 6d5f    def path_from_
+00002840: 6964 2873 656c 662c 2070 726f 7065 7274  id(self, propert
+00002850: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
+00002860: 616c 5b73 7472 5d20 3d20 2222 2920 2d3e  al[str] = "") ->
+00002870: 2073 7472 3a0a 2020 2020 2020 2020 2727   str:.        ''
+00002880: 2720 5265 7475 726e 7320 7468 6520 6461  ' Returns the da
+00002890: 7461 2070 6174 6820 6672 6f6d 2074 6865  ta path from the
+000028a0: 2049 4420 746f 2074 6869 7320 6f62 6a65   ID to this obje
+000028b0: 6374 2028 7374 7269 6e67 292e 0a0a 2020  ct (string)...  
+000028c0: 2020 2020 2020 3a70 6172 616d 2070 726f        :param pro
+000028d0: 7065 7274 793a 204f 7074 696f 6e61 6c20  perty: Optional 
+000028e0: 7072 6f70 6572 7479 206e 616d 6520 7768  property name wh
+000028f0: 6963 6820 6361 6e20 6265 2075 7365 6420  ich can be used 
+00002900: 6966 2074 6865 2070 6174 6820 6973 2074  if the path is t
+00002910: 6f20 6120 7072 6f70 6572 7479 206f 6620  o a property of 
+00002920: 7468 6973 206f 626a 6563 742e 0a20 2020  this object..   
+00002930: 2020 2020 203a 7479 7065 2070 726f 7065       :type prope
+00002940: 7274 793a 2074 7970 696e 672e 4f70 7469  rty: typing.Opti
+00002950: 6f6e 616c 5b73 7472 5d0a 2020 2020 2020  onal[str].      
+00002960: 2020 3a72 7479 7065 3a20 7374 720a 2020    :rtype: str.  
+00002970: 2020 2020 2020 3a72 6574 7572 6e3a 2060        :return: `
+00002980: 6270 792e 7479 7065 732e 6270 795f 7374  bpy.types.bpy_st
+00002990: 7275 6374 2e69 645f 6461 7461 6020 746f  ruct.id_data` to
+000029a0: 2074 6869 7320 7374 7275 6374 2061 6e64   this struct and
+000029b0: 2070 726f 7065 7274 7920 2877 6865 6e20   property (when 
+000029c0: 6769 7665 6e29 2e0a 2020 2020 2020 2020  given)..        
+000029d0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+000029e0: 0a0a 2020 2020 6465 6620 7061 7468 5f72  ..    def path_r
+000029f0: 6573 6f6c 7665 2873 656c 662c 0a20 2020  esolve(self,.   
+00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a10: 2020 7061 7468 3a20 7479 7069 6e67 2e4f    path: typing.O
+00002a20: 7074 696f 6e61 6c5b 7374 725d 2c0a 2020  ptional[str],.  
+00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a40: 2020 2063 6f65 7263 653a 2074 7970 696e     coerce: typin
+00002a50: 672e 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  g.Optional[bool]
+00002a60: 203d 2054 7275 6529 3a0a 2020 2020 2020   = True):.      
+00002a70: 2020 2727 2720 5265 7475 726e 7320 7468    ''' Returns th
+00002a80: 6520 7072 6f70 6572 7479 2066 726f 6d20  e property from 
+00002a90: 7468 6520 7061 7468 2c20 7261 6973 6520  the path, raise 
+00002aa0: 616e 2065 7863 6570 7469 6f6e 2077 6865  an exception whe
+00002ab0: 6e20 6e6f 7420 666f 756e 642e 0a0a 2020  n not found...  
+00002ac0: 2020 2020 2020 3a70 6172 616d 2070 6174        :param pat
+00002ad0: 683a 2070 6174 6820 7768 6963 6820 7468  h: path which th
+00002ae0: 6973 2070 726f 7065 7274 7920 7265 736f  is property reso
+00002af0: 6c76 6573 2e0a 2020 2020 2020 2020 3a74  lves..        :t
+00002b00: 7970 6520 7061 7468 3a20 7479 7069 6e67  ype path: typing
+00002b10: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
+00002b20: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
+00002b30: 6572 6365 3a20 6f70 7469 6f6e 616c 2061  erce: optional a
+00002b40: 7267 756d 656e 742c 2077 6865 6e20 5472  rgument, when Tr
+00002b50: 7565 2c20 7468 6520 7072 6f70 6572 7479  ue, the property
+00002b60: 2077 696c 6c20 6265 2063 6f6e 7665 7274   will be convert
+00002b70: 6564 2069 6e74 6f20 6974 7320 5079 7468  ed into its Pyth
+00002b80: 6f6e 2072 6570 7265 7365 6e74 6174 696f  on representatio
+00002b90: 6e2e 0a20 2020 2020 2020 203a 7479 7065  n..        :type
+00002ba0: 2063 6f65 7263 653a 2074 7970 696e 672e   coerce: typing.
+00002bb0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 0a20  Optional[bool]. 
+00002bc0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00002bd0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00002be0: 2070 6f70 2873 656c 662c 0a20 2020 2020   pop(self,.     
+00002bf0: 2020 2020 2020 206b 6579 3a20 7479 7069         key: typi
+00002c00: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00002c10: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
+00002c20: 6661 756c 743a 2074 7970 696e 672e 4f70  fault: typing.Op
+00002c30: 7469 6f6e 616c 5b74 7970 696e 672e 416e  tional[typing.An
+00002c40: 795d 203d 204e 6f6e 6529 3a0a 2020 2020  y] = None):.    
+00002c50: 2020 2020 2727 2720 5265 6d6f 7665 2061      ''' Remove a
+00002c60: 6e64 2072 6574 7572 6e20 7468 6520 7661  nd return the va
+00002c70: 6c75 6520 6f66 2074 6865 2063 7573 746f  lue of the custo
+00002c80: 6d20 7072 6f70 6572 7479 2061 7373 6967  m property assig
+00002c90: 6e65 6420 746f 206b 6579 206f 7220 6465  ned to key or de
+00002ca0: 6661 756c 7420 7768 656e 206e 6f74 2066  fault when not f
+00002cb0: 6f75 6e64 2028 6d61 7463 6865 7320 5079  ound (matches Py
+00002cc0: 7468 6f6e 2773 2064 6963 7469 6f6e 6172  thon's dictionar
+00002cd0: 7920 6675 6e63 7469 6f6e 206f 6620 7468  y function of th
+00002ce0: 6520 7361 6d65 206e 616d 6529 2e0a 0a20  e same name)... 
+00002cf0: 2020 2020 2020 203a 7061 7261 6d20 6b65         :param ke
+00002d00: 793a 2054 6865 206b 6579 2061 7373 6f63  y: The key assoc
+00002d10: 6961 7465 6420 7769 7468 2074 6865 2063  iated with the c
+00002d20: 7573 746f 6d20 7072 6f70 6572 7479 2e0a  ustom property..
+00002d30: 2020 2020 2020 2020 3a74 7970 6520 6b65          :type ke
+00002d40: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
+00002d50: 616c 5b73 7472 5d0a 2020 2020 2020 2020  al[str].        
+00002d60: 3a70 6172 616d 2064 6566 6175 6c74 3a20  :param default: 
+00002d70: 4f70 7469 6f6e 616c 2061 7267 756d 656e  Optional argumen
+00002d80: 7420 666f 7220 7468 6520 7661 6c75 6520  t for the value 
+00002d90: 746f 2072 6574 7572 6e20 6966 202a 6b65  to return if *ke
+00002da0: 792a 2069 7320 6e6f 7420 666f 756e 642e  y* is not found.
+00002db0: 0a20 2020 2020 2020 203a 7479 7065 2064  .        :type d
+00002dc0: 6566 6175 6c74 3a20 7479 7069 6e67 2e4f  efault: typing.O
+00002dd0: 7074 696f 6e61 6c5b 7479 7069 6e67 2e41  ptional[typing.A
+00002de0: 6e79 5d0a 2020 2020 2020 2020 2727 270a  ny].        '''.
+00002df0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00002e00: 2020 6465 6620 7072 6f70 6572 7479 5f6f    def property_o
+00002e10: 7665 7272 6964 6162 6c65 5f6c 6962 7261  verridable_libra
+00002e20: 7279 5f73 6574 2873 656c 662c 2070 726f  ry_set(self, pro
+00002e30: 7065 7274 792c 206f 7665 7272 6964 6162  perty, overridab
+00002e40: 6c65 2920 2d3e 2062 6f6f 6c3a 0a20 2020  le) -> bool:.   
+00002e50: 2020 2020 2027 2727 2044 6566 696e 6520       ''' Define 
+00002e60: 6120 7072 6f70 6572 7479 2061 7320 6f76  a property as ov
+00002e70: 6572 7269 6461 626c 6520 6f72 206e 6f74  erridable or not
+00002e80: 2028 6f6e 6c79 2066 6f72 2063 7573 746f   (only for custo
+00002e90: 6d20 7072 6f70 6572 7469 6573 2129 2e0a  m properties!)..
+00002ea0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00002eb0: 2062 6f6f 6c0a 2020 2020 2020 2020 3a72   bool.        :r
+00002ec0: 6574 7572 6e3a 2054 7275 6520 7768 656e  eturn: True when
+00002ed0: 2074 6865 206f 7665 7272 6964 6162 6c65   the overridable
+00002ee0: 2073 7461 7475 7320 6f66 2074 6865 2070   status of the p
+00002ef0: 726f 7065 7274 7920 7761 7320 7375 6363  roperty was succ
+00002f00: 6573 7366 756c 6c79 2073 6574 2e0a 2020  essfully set..  
+00002f10: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00002f20: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00002f30: 7072 6f70 6572 7479 5f75 6e73 6574 2873  property_unset(s
+00002f40: 656c 662c 2070 726f 7065 7274 7929 3a0a  elf, property):.
+00002f50: 2020 2020 2020 2020 2727 2720 556e 7365          ''' Unse
+00002f60: 7420 6120 7072 6f70 6572 7479 2c20 7769  t a property, wi
+00002f70: 6c6c 2075 7365 2064 6566 6175 6c74 2076  ll use default v
+00002f80: 616c 7565 2061 6674 6572 7761 7264 2e0a  alue afterward..
+00002f90: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00002fa0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00002fb0: 6566 2074 7970 655f 7265 6361 7374 2873  ef type_recast(s
+00002fc0: 656c 6629 202d 3e20 2762 7079 5f73 7472  elf) -> 'bpy_str
+00002fd0: 7563 7427 3a0a 2020 2020 2020 2020 2727  uct':.        ''
+00002fe0: 2720 5265 7475 726e 2061 206e 6577 2069  ' Return a new i
+00002ff0: 6e73 7461 6e63 652c 2074 6869 7320 6973  nstance, this is
+00003000: 206e 6565 6465 6420 6265 6361 7573 6520   needed because 
+00003010: 7479 7065 7320 7375 6368 2061 7320 7465  types such as te
+00003020: 7874 7572 6573 2063 616e 2062 6520 6368  xtures can be ch
+00003030: 616e 6765 6420 6174 2072 756e 7469 6d65  anged at runtime
+00003040: 2e0a 0a20 2020 2020 2020 203a 7274 7970  ...        :rtyp
+00003050: 653a 2027 6270 795f 7374 7275 6374 270a  e: 'bpy_struct'.
+00003060: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00003070: 2061 206e 6577 2069 6e73 7461 6e63 6520   a new instance 
+00003080: 6f66 2074 6869 7320 6f62 6a65 6374 2077  of this object w
+00003090: 6974 6820 7468 6520 7479 7065 2069 6e69  ith the type ini
+000030a0: 7469 616c 697a 6564 2061 6761 696e 2e0a  tialized again..
+000030b0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+000030c0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+000030d0: 6620 7661 6c75 6573 2873 656c 6629 202d  f values(self) -
+000030e0: 3e20 7479 7069 6e67 2e41 6e79 3a0a 2020  > typing.Any:.  
+000030f0: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
+00003100: 7320 7468 6520 7661 6c75 6573 206f 6620  s the values of 
+00003110: 7468 6973 206f 626a 6563 7473 2063 7573  this objects cus
+00003120: 746f 6d20 7072 6f70 6572 7469 6573 2028  tom properties (
+00003130: 6d61 7463 6865 7320 5079 7468 6f6e 2773  matches Python's
+00003140: 2064 6963 7469 6f6e 6172 7920 6675 6e63   dictionary func
+00003150: 7469 6f6e 206f 6620 7468 6520 7361 6d65  tion of the same
+00003160: 206e 616d 6529 2e0a 0a20 2020 2020 2020   name)...       
+00003170: 203a 7274 7970 653a 2074 7970 696e 672e   :rtype: typing.
+00003180: 416e 790a 2020 2020 2020 2020 3a72 6574  Any.        :ret
+00003190: 7572 6e3a 2063 7573 746f 6d20 7072 6f70  urn: custom prop
+000031a0: 6572 7479 2076 616c 7565 732e 0a20 2020  erty values..   
+000031b0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+000031c0: 2070 6173 730a 0a20 2020 2064 6566 205f   pass..    def _
+000031d0: 5f67 6574 6974 656d 5f5f 2873 656c 662c  _getitem__(self,
+000031e0: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
+000031f0: 6f6e 5b69 6e74 2c20 7374 725d 2920 2d3e  on[int, str]) ->
+00003200: 2027 7479 7069 6e67 2e41 6e79 273a 0a20   'typing.Any':. 
+00003210: 2020 2020 2020 2027 2727 200a 0a20 2020         ''' ..   
+00003220: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
+00003230: 200a 2020 2020 2020 2020 3a74 7970 6520   .        :type 
+00003240: 6b65 793a 2074 7970 696e 672e 556e 696f  key: typing.Unio
+00003250: 6e5b 696e 742c 2073 7472 5d0a 2020 2020  n[int, str].    
+00003260: 2020 2020 3a72 7479 7065 3a20 2774 7970      :rtype: 'typ
+00003270: 696e 672e 416e 7927 0a20 2020 2020 2020  ing.Any'.       
+00003280: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00003290: 730a 0a20 2020 2064 6566 205f 5f73 6574  s..    def __set
+000032a0: 6974 656d 5f5f 2873 656c 662c 206b 6579  item__(self, key
+000032b0: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b69  : typing.Union[i
+000032c0: 6e74 2c20 7374 725d 2c20 7661 6c75 653a  nt, str], value:
+000032d0: 2027 7479 7069 6e67 2e41 6e79 2729 3a0a   'typing.Any'):.
+000032e0: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
+000032f0: 2020 2020 2020 3a70 6172 616d 206b 6579        :param key
+00003300: 3a20 0a20 2020 2020 2020 203a 7479 7065  : .        :type
+00003310: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
+00003320: 6f6e 5b69 6e74 2c20 7374 725d 0a20 2020  on[int, str].   
+00003330: 2020 2020 203a 7061 7261 6d20 7661 6c75       :param valu
+00003340: 653a 200a 2020 2020 2020 2020 3a74 7970  e: .        :typ
+00003350: 6520 7661 6c75 653a 2027 7479 7069 6e67  e value: 'typing
+00003360: 2e41 6e79 270a 2020 2020 2020 2020 2727  .Any'.        ''
+00003370: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00003380: 2020 2020 6465 6620 5f5f 6465 6c69 7465      def __delite
+00003390: 6d5f 5f28 7365 6c66 2c20 6b65 793a 2074  m__(self, key: t
+000033a0: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+000033b0: 2073 7472 5d29 202d 3e20 2774 7970 696e   str]) -> 'typin
+000033c0: 672e 416e 7927 3a0a 2020 2020 2020 2020  g.Any':.        
+000033d0: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
+000033e0: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
+000033f0: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
+00003400: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
+00003410: 7374 725d 0a20 2020 2020 2020 203a 7274  str].        :rt
+00003420: 7970 653a 2027 7479 7069 6e67 2e41 6e79  ype: 'typing.Any
+00003430: 270a 2020 2020 2020 2020 2727 270a 2020  '.        '''.  
+00003440: 2020 2020 2020 7061 7373 0a0a 0a63 6c61        pass...cla
+00003450: 7373 2062 7079 5f70 726f 705f 636f 6c6c  ss bpy_prop_coll
+00003460: 6563 7469 6f6e 2874 7970 696e 672e 4765  ection(typing.Ge
+00003470: 6e65 7269 635b 4765 6e65 7269 6354 7970  neric[GenericTyp
+00003480: 655d 293a 0a20 2020 2027 2727 2062 7569  e]):.    ''' bui
+00003490: 6c74 2d69 6e20 636c 6173 7320 7573 6564  lt-in class used
+000034a0: 2066 6f72 2061 6c6c 2063 6f6c 6c65 6374   for all collect
+000034b0: 696f 6e73 2e0a 2020 2020 2727 270a 0a20  ions..    '''.. 
+000034c0: 2020 2064 6566 2066 696e 6428 7365 6c66     def find(self
+000034d0: 2c20 6b65 793a 2074 7970 696e 672e 4f70  , key: typing.Op
+000034e0: 7469 6f6e 616c 5b73 7472 5d29 202d 3e20  tional[str]) -> 
+000034f0: 696e 743a 0a20 2020 2020 2020 2027 2727  int:.        '''
+00003500: 2052 6574 7572 6e73 2074 6865 2069 6e64   Returns the ind
+00003510: 6578 206f 6620 6120 6b65 7920 696e 2061  ex of a key in a
+00003520: 2063 6f6c 6c65 6374 696f 6e20 6f72 202d   collection or -
+00003530: 3120 7768 656e 206e 6f74 2066 6f75 6e64  1 when not found
+00003540: 2028 6d61 7463 6865 7320 5079 7468 6f6e   (matches Python
+00003550: 2773 2073 7472 696e 6720 6669 6e64 2066  's string find f
+00003560: 756e 6374 696f 6e20 6f66 2074 6865 2073  unction of the s
+00003570: 616d 6520 6e61 6d65 292e 0a0a 2020 2020  ame name)...    
+00003580: 2020 2020 3a70 6172 616d 206b 6579 3a20      :param key: 
+00003590: 5468 6520 6964 656e 7469 6669 6572 2066  The identifier f
+000035a0: 6f72 2074 6865 2063 6f6c 6c65 6374 696f  or the collectio
+000035b0: 6e20 6d65 6d62 6572 2e0a 2020 2020 2020  n member..      
+000035c0: 2020 3a74 7970 6520 6b65 793a 2074 7970    :type key: typ
+000035d0: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+000035e0: 5d0a 2020 2020 2020 2020 3a72 7479 7065  ].        :rtype
+000035f0: 3a20 696e 740a 2020 2020 2020 2020 3a72  : int.        :r
+00003600: 6574 7572 6e3a 2069 6e64 6578 206f 6620  eturn: index of 
+00003610: 7468 6520 6b65 792e 0a20 2020 2020 2020  the key..       
+00003620: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00003630: 730a 0a20 2020 2064 6566 2066 6f72 6561  s..    def forea
+00003640: 6368 5f67 6574 2873 656c 662c 2061 7474  ch_get(self, att
+00003650: 722c 2073 6571 293a 0a20 2020 2020 2020  r, seq):.       
+00003660: 2027 2727 2054 6869 7320 6973 2061 2066   ''' This is a f
+00003670: 756e 6374 696f 6e20 746f 2067 6976 6520  unction to give 
+00003680: 6661 7374 2061 6363 6573 7320 746f 2061  fast access to a
+00003690: 7474 7269 6275 7465 7320 7769 7468 696e  ttributes within
+000036a0: 2061 2063 6f6c 6c65 6374 696f 6e2e 204f   a collection. O
+000036b0: 6e6c 7920 776f 726b 7320 666f 7220 2762  nly works for 'b
+000036c0: 6173 6963 2074 7970 6527 2070 726f 7065  asic type' prope
+000036d0: 7274 6965 7320 2862 6f6f 6c2c 2069 6e74  rties (bool, int
+000036e0: 2061 6e64 2066 6c6f 6174 2921 204d 756c   and float)! Mul
+000036f0: 7469 2d64 696d 656e 7369 6f6e 616c 2061  ti-dimensional a
+00003700: 7272 6179 7320 286c 696b 6520 6172 7261  rrays (like arra
+00003710: 7920 6f66 2076 6563 746f 7273 2920 7769  y of vectors) wi
+00003720: 6c6c 2062 6520 666c 6174 7465 6e65 6420  ll be flattened 
+00003730: 696e 746f 2073 6571 2e0a 0a20 2020 2020  into seq...     
+00003740: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
+00003750: 6173 730a 0a20 2020 2064 6566 2066 6f72  ass..    def for
+00003760: 6561 6368 5f73 6574 2873 656c 662c 2061  each_set(self, a
+00003770: 7474 722c 2073 6571 293a 0a20 2020 2020  ttr, seq):.     
+00003780: 2020 2027 2727 2054 6869 7320 6973 2061     ''' This is a
+00003790: 2066 756e 6374 696f 6e20 746f 2067 6976   function to giv
+000037a0: 6520 6661 7374 2061 6363 6573 7320 746f  e fast access to
+000037b0: 2061 7474 7269 6275 7465 7320 7769 7468   attributes with
+000037c0: 696e 2061 2063 6f6c 6c65 6374 696f 6e2e  in a collection.
+000037d0: 204f 6e6c 7920 776f 726b 7320 666f 7220   Only works for 
+000037e0: 2762 6173 6963 2074 7970 6527 2070 726f  'basic type' pro
+000037f0: 7065 7274 6965 7320 2862 6f6f 6c2c 2069  perties (bool, i
+00003800: 6e74 2061 6e64 2066 6c6f 6174 2921 2073  nt and float)! s
+00003810: 6571 206d 7573 7420 6265 2075 6e69 2d64  eq must be uni-d
+00003820: 696d 656e 7369 6f6e 616c 2c20 6d75 6c74  imensional, mult
+00003830: 692d 6469 6d65 6e73 696f 6e61 6c20 6172  i-dimensional ar
+00003840: 7261 7973 2028 6c69 6b65 2061 7272 6179  rays (like array
+00003850: 206f 6620 7665 6374 6f72 7329 2077 696c   of vectors) wil
+00003860: 6c20 6265 2072 652d 6372 6561 7465 6420  l be re-created 
+00003870: 6672 6f6d 2069 742e 0a0a 2020 2020 2020  from it...      
+00003880: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00003890: 7373 0a0a 2020 2020 6465 6620 6765 7428  ss..    def get(
+000038a0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+000038b0: 2020 6b65 793a 2074 7970 696e 672e 4f70    key: typing.Op
+000038c0: 7469 6f6e 616c 5b73 7472 5d2c 0a20 2020  tional[str],.   
+000038d0: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+000038e0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+000038f0: 6c5b 7479 7069 6e67 2e41 6e79 5d20 3d20  l[typing.Any] = 
+00003900: 4e6f 6e65 293a 0a20 2020 2020 2020 2027  None):.        '
+00003910: 2727 2052 6574 7572 6e73 2074 6865 2076  '' Returns the v
+00003920: 616c 7565 206f 6620 7468 6520 6974 656d  alue of the item
+00003930: 2061 7373 6967 6e65 6420 746f 206b 6579   assigned to key
+00003940: 206f 7220 6465 6661 756c 7420 7768 656e   or default when
+00003950: 206e 6f74 2066 6f75 6e64 2028 6d61 7463   not found (matc
+00003960: 6865 7320 5079 7468 6f6e 2773 2064 6963  hes Python's dic
+00003970: 7469 6f6e 6172 7920 6675 6e63 7469 6f6e  tionary function
+00003980: 206f 6620 7468 6520 7361 6d65 206e 616d   of the same nam
+00003990: 6529 2e0a 0a20 2020 2020 2020 203a 7061  e)...        :pa
+000039a0: 7261 6d20 6b65 793a 2054 6865 2069 6465  ram key: The ide
+000039b0: 6e74 6966 6965 7220 666f 7220 7468 6520  ntifier for the 
+000039c0: 636f 6c6c 6563 7469 6f6e 206d 656d 6265  collection membe
+000039d0: 722e 0a20 2020 2020 2020 203a 7479 7065  r..        :type
+000039e0: 206b 6579 3a20 7479 7069 6e67 2e4f 7074   key: typing.Opt
+000039f0: 696f 6e61 6c5b 7374 725d 0a20 2020 2020  ional[str].     
+00003a00: 2020 203a 7061 7261 6d20 6465 6661 756c     :param defaul
+00003a10: 743a 204f 7074 696f 6e61 6c20 6172 6775  t: Optional argu
+00003a20: 6d65 6e74 2066 6f72 2074 6865 2076 616c  ment for the val
+00003a30: 7565 2074 6f20 7265 7475 726e 2069 6620  ue to return if 
+00003a40: 2a6b 6579 2a20 6973 206e 6f74 2066 6f75  *key* is not fou
+00003a50: 6e64 2e0a 2020 2020 2020 2020 3a74 7970  nd..        :typ
+00003a60: 6520 6465 6661 756c 743a 2074 7970 696e  e default: typin
+00003a70: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00003a80: 672e 416e 795d 0a20 2020 2020 2020 2027  g.Any].        '
+00003a90: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00003aa0: 0a20 2020 2064 6566 2069 7465 6d73 2873  .    def items(s
+00003ab0: 656c 6629 202d 3e20 7479 7069 6e67 2e4c  elf) -> typing.L
+00003ac0: 6973 743a 0a20 2020 2020 2020 2027 2727  ist:.        '''
+00003ad0: 2052 6574 7572 6e20 7468 6520 6964 656e   Return the iden
+00003ae0: 7469 6669 6572 7320 6f66 2063 6f6c 6c65  tifiers of colle
+00003af0: 6374 696f 6e20 6d65 6d62 6572 7320 286d  ction members (m
+00003b00: 6174 6368 696e 6720 5079 7468 6f6e 2773  atching Python's
+00003b10: 2064 6963 742e 6974 656d 7328 2920 6675   dict.items() fu
+00003b20: 6e63 7469 6f6e 616c 6974 7929 2e0a 0a20  nctionality)... 
+00003b30: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
+00003b40: 7970 696e 672e 4c69 7374 0a20 2020 2020  yping.List.     
+00003b50: 2020 203a 7265 7475 726e 3a20 286b 6579     :return: (key
+00003b60: 2c20 7661 6c75 6529 2070 6169 7273 2066  , value) pairs f
+00003b70: 6f72 2065 6163 6820 6d65 6d62 6572 206f  or each member o
+00003b80: 6620 7468 6973 2063 6f6c 6c65 6374 696f  f this collectio
+00003b90: 6e2e 0a20 2020 2020 2020 2027 2727 0a20  n..        '''. 
+00003ba0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00003bb0: 2064 6566 206b 6579 7328 7365 6c66 2920   def keys(self) 
+00003bc0: 2d3e 2074 7970 696e 672e 4c69 7374 5b73  -> typing.List[s
+00003bd0: 7472 5d3a 0a20 2020 2020 2020 2027 2727  tr]:.        '''
+00003be0: 2052 6574 7572 6e20 7468 6520 6964 656e   Return the iden
+00003bf0: 7469 6669 6572 7320 6f66 2063 6f6c 6c65  tifiers of colle
+00003c00: 6374 696f 6e20 6d65 6d62 6572 7320 286d  ction members (m
+00003c10: 6174 6368 696e 6720 5079 7468 6f6e 2773  atching Python's
+00003c20: 2064 6963 742e 6b65 7973 2829 2066 756e   dict.keys() fun
+00003c30: 6374 696f 6e61 6c69 7479 292e 0a0a 2020  ctionality)...  
+00003c40: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
+00003c50: 7069 6e67 2e4c 6973 745b 7374 725d 0a20  ping.List[str]. 
+00003c60: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00003c70: 7468 6520 6964 656e 7469 6669 6572 7320  the identifiers 
+00003c80: 666f 7220 6561 6368 206d 656d 6265 7220  for each member 
+00003c90: 6f66 2074 6869 7320 636f 6c6c 6563 7469  of this collecti
+00003ca0: 6f6e 2e0a 2020 2020 2020 2020 2727 270a  on..        '''.
+00003cb0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00003cc0: 2020 6465 6620 7661 6c75 6573 2873 656c    def values(sel
+00003cd0: 6629 202d 3e20 7479 7069 6e67 2e4c 6973  f) -> typing.Lis
+00003ce0: 743a 0a20 2020 2020 2020 2027 2727 2052  t:.        ''' R
+00003cf0: 6574 7572 6e20 7468 6520 7661 6c75 6573  eturn the values
+00003d00: 206f 6620 636f 6c6c 6563 7469 6f6e 2028   of collection (
+00003d10: 6d61 7463 6869 6e67 2050 7974 686f 6e27  matching Python'
+00003d20: 7320 6469 6374 2e76 616c 7565 7328 2920  s dict.values() 
+00003d30: 6675 6e63 7469 6f6e 616c 6974 7929 2e0a  functionality)..
+00003d40: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00003d50: 2074 7970 696e 672e 4c69 7374 0a20 2020   typing.List.   
+00003d60: 2020 2020 203a 7265 7475 726e 3a20 7468       :return: th
+00003d70: 6520 6d65 6d62 6572 7320 6f66 2074 6869  e members of thi
+00003d80: 7320 636f 6c6c 6563 7469 6f6e 2e0a 2020  s collection..  
+00003d90: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00003da0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00003db0: 5f5f 6765 7469 7465 6d5f 5f28 7365 6c66  __getitem__(self
+00003dc0: 2c20 6b65 793a 2074 7970 696e 672e 556e  , key: typing.Un
+00003dd0: 696f 6e5b 696e 742c 2073 7472 5d29 202d  ion[int, str]) -
+00003de0: 3e20 2747 656e 6572 6963 5479 7065 273a  > 'GenericType':
+00003df0: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
+00003e00: 2020 2020 2020 203a 7061 7261 6d20 6b65         :param ke
+00003e10: 793a 200a 2020 2020 2020 2020 3a74 7970  y: .        :typ
+00003e20: 6520 6b65 793a 2074 7970 696e 672e 556e  e key: typing.Un
+00003e30: 696f 6e5b 696e 742c 2073 7472 5d0a 2020  ion[int, str].  
+00003e40: 2020 2020 2020 3a72 7479 7065 3a20 2747        :rtype: 'G
+00003e50: 656e 6572 6963 5479 7065 270a 2020 2020  enericType'.    
+00003e60: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00003e70: 7061 7373 0a0a 2020 2020 6465 6620 5f5f  pass..    def __
+00003e80: 7365 7469 7465 6d5f 5f28 7365 6c66 2c20  setitem__(self, 
+00003e90: 6b65 793a 2074 7970 696e 672e 556e 696f  key: typing.Unio
+00003ea0: 6e5b 696e 742c 2073 7472 5d2c 2076 616c  n[int, str], val
+00003eb0: 7565 3a20 2747 656e 6572 6963 5479 7065  ue: 'GenericType
+00003ec0: 2729 3a0a 2020 2020 2020 2020 2727 2720  '):.        ''' 
+00003ed0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00003ee0: 206b 6579 3a20 0a20 2020 2020 2020 203a   key: .        :
+00003ef0: 7479 7065 206b 6579 3a20 7479 7069 6e67  type key: typing
+00003f00: 2e55 6e69 6f6e 5b69 6e74 2c20 7374 725d  .Union[int, str]
+00003f10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00003f20: 7661 6c75 653a 200a 2020 2020 2020 2020  value: .        
+00003f30: 3a74 7970 6520 7661 6c75 653a 2027 4765  :type value: 'Ge
+00003f40: 6e65 7269 6354 7970 6527 0a20 2020 2020  nericType'.     
+00003f50: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
+00003f60: 6173 730a 0a20 2020 2064 6566 205f 5f64  ass..    def __d
+00003f70: 656c 6974 656d 5f5f 2873 656c 662c 206b  elitem__(self, k
+00003f80: 6579 3a20 7479 7069 6e67 2e55 6e69 6f6e  ey: typing.Union
+00003f90: 5b69 6e74 2c20 7374 725d 2920 2d3e 2027  [int, str]) -> '
+00003fa0: 4765 6e65 7269 6354 7970 6527 3a0a 2020  GenericType':.  
+00003fb0: 2020 2020 2020 2727 2720 0a0a 2020 2020        ''' ..    
+00003fc0: 2020 2020 3a70 6172 616d 206b 6579 3a20      :param key: 
+00003fd0: 0a20 2020 2020 2020 203a 7479 7065 206b  .        :type k
+00003fe0: 6579 3a20 7479 7069 6e67 2e55 6e69 6f6e  ey: typing.Union
+00003ff0: 5b69 6e74 2c20 7374 725d 0a20 2020 2020  [int, str].     
+00004000: 2020 203a 7274 7970 653a 2027 4765 6e65     :rtype: 'Gene
+00004010: 7269 6354 7970 6527 0a20 2020 2020 2020  ricType'.       
+00004020: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00004030: 730a 0a20 2020 2064 6566 205f 5f69 7465  s..    def __ite
+00004040: 725f 5f28 7365 6c66 2920 2d3e 2074 7970  r__(self) -> typ
+00004050: 696e 672e 4974 6572 6174 6f72 5b27 4765  ing.Iterator['Ge
+00004060: 6e65 7269 6354 7970 6527 5d3a 0a20 2020  nericType']:.   
+00004070: 2020 2020 2027 2727 200a 0a20 2020 2020       ''' ..     
+00004080: 2020 203a 7274 7970 653a 2074 7970 696e     :rtype: typin
+00004090: 672e 4974 6572 6174 6f72 5b27 4765 6e65  g.Iterator['Gene
+000040a0: 7269 6354 7970 6527 5d0a 2020 2020 2020  ricType'].      
+000040b0: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+000040c0: 7373 0a0a 2020 2020 6465 6620 5f5f 6e65  ss..    def __ne
+000040d0: 7874 5f5f 2873 656c 6629 202d 3e20 2747  xt__(self) -> 'G
+000040e0: 656e 6572 6963 5479 7065 273a 0a20 2020  enericType':.   
+000040f0: 2020 2020 2027 2727 200a 0a20 2020 2020       ''' ..     
+00004100: 2020 203a 7274 7970 653a 2027 4765 6e65     :rtype: 'Gene
+00004110: 7269 6354 7970 6527 0a20 2020 2020 2020  ricType'.       
+00004120: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00004130: 730a 0a20 2020 2064 6566 205f 5f6c 656e  s..    def __len
+00004140: 5f5f 2873 656c 6629 202d 3e20 696e 743a  __(self) -> int:
+00004150: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
+00004160: 2020 2020 2020 203a 7274 7970 653a 2069         :rtype: i
+00004170: 6e74 0a20 2020 2020 2020 2027 2727 0a20  nt.        '''. 
 00004180: 2020 2020 2020 2070 6173 730a 0a0a 636c         pass...cl
 00004190: 6173 7320 6270 795f 7072 6f70 5f61 7272  ass bpy_prop_arr
 000041a0: 6179 2874 7970 696e 672e 4765 6e65 7269  ay(typing.Generi
 000041b0: 635b 4765 6e65 7269 6354 7970 655d 293a  c[GenericType]):
 000041c0: 0a20 2020 2064 6566 2066 6f72 6561 6368  .    def foreach
 000041d0: 5f67 6574 2873 656c 662c 2061 7474 722c  _get(self, attr,
 000041e0: 2073 6571 293a 0a20 2020 2020 2020 2027   seq):.        '
@@ -10285,27 +10285,27 @@
 000282c0: 6571 7565 6e63 655b 274b 6579 6672 616d  equence['Keyfram
 000282d0: 6527 5d0a 2020 2020 2727 270a 0a20 2020  e'].    '''..   
 000282e0: 2075 695f 6c69 7374 3a20 2755 494c 6973   ui_list: 'UILis
 000282f0: 7427 203d 204e 6f6e 650a 2020 2020 2727  t' = None.    ''
 00028300: 2720 0a0a 2020 2020 3a74 7970 653a 2027  ' ..    :type: '
 00028310: 5549 4c69 7374 270a 2020 2020 2727 270a  UIList'.    '''.
 00028320: 0a20 2020 2070 726f 7065 7274 793a 2074  .    property: t
-00028330: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
-00028340: 2073 7472 2c20 2749 4427 5d20 3d20 4e6f   str, 'ID'] = No
+00028330: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
+00028340: 2069 6e74 2c20 2749 4427 5d20 3d20 4e6f   int, 'ID'] = No
 00028350: 6e65 0a20 2020 2027 2727 2047 6574 2074  ne.    ''' Get t
 00028360: 6865 2070 726f 7065 7274 7920 6173 736f  he property asso
 00028370: 6369 6174 6564 2077 6974 6820 6120 686f  ciated with a ho
 00028380: 7665 7265 6420 6275 7474 6f6e 2e20 5265  vered button. Re
 00028390: 7475 726e 7320 6120 7475 706c 6520 6f66  turns a tuple of
 000283a0: 2074 6865 2064 6174 6162 6c6f 636b 2c20   the datablock, 
 000283b0: 6461 7461 2070 6174 6820 746f 2074 6865  data path to the
 000283c0: 2070 726f 7065 7274 792c 2061 6e64 2061   property, and a
 000283d0: 7272 6179 2069 6e64 6578 2e0a 0a20 2020  rray index...   
 000283e0: 203a 7479 7065 3a20 7479 7069 6e67 2e55   :type: typing.U
-000283f0: 6e69 6f6e 5b69 6e74 2c20 7374 722c 2027  nion[int, str, '
+000283f0: 6e69 6f6e 5b73 7472 2c20 696e 742c 2027  nion[str, int, '
 00028400: 4944 275d 0a20 2020 2027 2727 0a0a 2020  ID'].    '''..  
 00028410: 2020 6564 6974 5f74 6578 743a 2027 5465    edit_text: 'Te
 00028420: 7874 2720 3d20 4e6f 6e65 0a20 2020 2027  xt' = None.    '
 00028430: 2727 200a 0a20 2020 203a 7479 7065 3a20  '' ..    :type: 
 00028440: 2754 6578 7427 0a20 2020 2027 2727 0a0a  'Text'.    '''..
 00028450: 2020 2020 6465 6620 6576 616c 7561 7465      def evaluate
 00028460: 645f 6465 7073 6772 6170 685f 6765 7428  d_depsgraph_get(
@@ -23284,17 +23284,17 @@
 0005af30: 6576 656e 743a 2027 4576 656e 7427 2c0a  event: 'Event',.
 0005af40: 2020 2020 2020 2020 2020 2020 2020 7477                tw
 0005af50: 6561 6b3a 2074 7970 696e 672e 556e 696f  eak: typing.Unio
 0005af60: 6e5b 7479 7069 6e67 2e53 6574 5b73 7472  n[typing.Set[str
 0005af70: 5d2c 2074 7970 696e 672e 5365 745b 696e  ], typing.Set[in
 0005af80: 745d 5d0a 2020 2020 2020 2020 2020 2020  t]].            
 0005af90: 2020 2920 2d3e 2074 7970 696e 672e 556e    ) -> typing.Un
-0005afa0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b69  ion[typing.Set[i
-0005afb0: 6e74 5d2c 2074 7970 696e 672e 5365 745b  nt], typing.Set[
-0005afc0: 7374 725d 5d3a 0a20 2020 2020 2020 2027  str]]:.        '
+0005afa0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b73  ion[typing.Set[s
+0005afb0: 7472 5d2c 2074 7970 696e 672e 5365 745b  tr], typing.Set[
+0005afc0: 696e 745d 5d3a 0a20 2020 2020 2020 2027  int]]:.        '
 0005afd0: 2727 200a 0a20 2020 2020 2020 203a 7061  '' ..        :pa
 0005afe0: 7261 6d20 636f 6e74 6578 743a 200a 2020  ram context: .  
 0005aff0: 2020 2020 2020 3a74 7970 6520 636f 6e74        :type cont
 0005b000: 6578 743a 2027 436f 6e74 6578 7427 0a20  ext: 'Context'. 
 0005b010: 2020 2020 2020 203a 7061 7261 6d20 6576         :param ev
 0005b020: 656e 743a 200a 2020 2020 2020 2020 3a74  ent: .        :t
 0005b030: 7970 6520 6576 656e 743a 2027 4576 656e  ype event: 'Even
@@ -23302,43 +23302,43 @@
 0005b050: 6d20 7477 6561 6b3a 2054 7765 616b 0a20  m tweak: Tweak. 
 0005b060: 2020 2020 2020 203a 7479 7065 2074 7765         :type twe
 0005b070: 616b 3a20 7479 7069 6e67 2e55 6e69 6f6e  ak: typing.Union
 0005b080: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
 0005b090: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
 0005b0a0: 5d5d 0a20 2020 2020 2020 203a 7274 7970  ]].        :rtyp
 0005b0b0: 653a 2074 7970 696e 672e 556e 696f 6e5b  e: typing.Union[
-0005b0c0: 7479 7069 6e67 2e53 6574 5b69 6e74 5d2c  typing.Set[int],
-0005b0d0: 2074 7970 696e 672e 5365 745b 7374 725d   typing.Set[str]
+0005b0c0: 7479 7069 6e67 2e53 6574 5b73 7472 5d2c  typing.Set[str],
+0005b0d0: 2074 7970 696e 672e 5365 745b 696e 745d   typing.Set[int]
 0005b0e0: 5d0a 2020 2020 2020 2020 3a72 6574 7572  ].        :retur
 0005b0f0: 6e3a 2072 6573 756c 740a 2020 2020 2020  n: result.      
 0005b100: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
 0005b110: 7373 0a0a 2020 2020 6465 6620 7365 7475  ss..    def setu
 0005b120: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
 0005b130: 2027 2727 200a 0a20 2020 2020 2020 2027   ''' ..        '
 0005b140: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
 0005b150: 0a20 2020 2064 6566 2069 6e76 6f6b 6528  .    def invoke(
 0005b160: 7365 6c66 2c20 636f 6e74 6578 743a 2027  self, context: '
 0005b170: 436f 6e74 6578 7427 2c20 6576 656e 743a  Context', event:
 0005b180: 2027 4576 656e 7427 0a20 2020 2020 2020   'Event'.       
 0005b190: 2020 2020 2020 2020 2920 2d3e 2074 7970          ) -> typ
 0005b1a0: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
-0005b1b0: 2e53 6574 5b69 6e74 5d2c 2074 7970 696e  .Set[int], typin
-0005b1c0: 672e 5365 745b 7374 725d 5d3a 0a20 2020  g.Set[str]]:.   
+0005b1b0: 2e53 6574 5b73 7472 5d2c 2074 7970 696e  .Set[str], typin
+0005b1c0: 672e 5365 745b 696e 745d 5d3a 0a20 2020  g.Set[int]]:.   
 0005b1d0: 2020 2020 2027 2727 200a 0a20 2020 2020       ''' ..     
 0005b1e0: 2020 203a 7061 7261 6d20 636f 6e74 6578     :param contex
 0005b1f0: 743a 200a 2020 2020 2020 2020 3a74 7970  t: .        :typ
 0005b200: 6520 636f 6e74 6578 743a 2027 436f 6e74  e context: 'Cont
 0005b210: 6578 7427 0a20 2020 2020 2020 203a 7061  ext'.        :pa
 0005b220: 7261 6d20 6576 656e 743a 200a 2020 2020  ram event: .    
 0005b230: 2020 2020 3a74 7970 6520 6576 656e 743a      :type event:
 0005b240: 2027 4576 656e 7427 0a20 2020 2020 2020   'Event'.       
 0005b250: 203a 7274 7970 653a 2074 7970 696e 672e   :rtype: typing.
 0005b260: 556e 696f 6e5b 7479 7069 6e67 2e53 6574  Union[typing.Set
-0005b270: 5b69 6e74 5d2c 2074 7970 696e 672e 5365  [int], typing.Se
-0005b280: 745b 7374 725d 5d0a 2020 2020 2020 2020  t[str]].        
+0005b270: 5b73 7472 5d2c 2074 7970 696e 672e 5365  [str], typing.Se
+0005b280: 745b 696e 745d 5d0a 2020 2020 2020 2020  t[int]].        
 0005b290: 3a72 6574 7572 6e3a 2072 6573 756c 740a  :return: result.
 0005b2a0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
 0005b2b0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
 0005b2c0: 6620 6578 6974 2873 656c 662c 2063 6f6e  f exit(self, con
 0005b2d0: 7465 7874 3a20 2743 6f6e 7465 7874 272c  text: 'Context',
 0005b2e0: 2063 616e 6365 6c3a 2074 7970 696e 672e   cancel: typing.
 0005b2f0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 293a  Optional[bool]):
@@ -27421,24 +27421,24 @@
 0006b1c0: 672e 416e 795d 203d 204e 6f6e 650a 2020  g.Any] = None.  
 0006b1d0: 2020 2727 2720 0a0a 2020 2020 3a74 7970    ''' ..    :typ
 0006b1e0: 653a 2074 7970 696e 672e 556e 696f 6e5b  e: typing.Union[
 0006b1f0: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
 0006b200: 0a20 2020 2027 2727 0a0a 2020 2020 626c  .    '''..    bl
 0006b210: 5f6f 7074 696f 6e73 3a20 7479 7069 6e67  _options: typing
 0006b220: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-0006b230: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
-0006b240: 6574 5b73 7472 5d5d 203d 204e 6f6e 650a  et[str]] = None.
+0006b230: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
+0006b240: 6574 5b69 6e74 5d5d 203d 204e 6f6e 650a  et[int]] = None.
 0006b250: 2020 2020 2727 2720 4b65 7969 6e67 2053      ''' Keying S
 0006b260: 6574 206f 7074 696f 6e73 2074 6f20 7573  et options to us
 0006b270: 6520 7768 656e 2069 6e73 6572 7469 6e67  e when inserting
 0006b280: 206b 6579 6672 616d 6573 0a0a 2020 2020   keyframes..    
 0006b290: 3a74 7970 653a 2074 7970 696e 672e 556e  :type: typing.Un
-0006b2a0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b69  ion[typing.Set[i
-0006b2b0: 6e74 5d2c 2074 7970 696e 672e 5365 745b  nt], typing.Set[
-0006b2c0: 7374 725d 5d0a 2020 2020 2727 270a 0a20  str]].    '''.. 
+0006b2a0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b73  ion[typing.Set[s
+0006b2b0: 7472 5d2c 2074 7970 696e 672e 5365 745b  tr], typing.Set[
+0006b2c0: 696e 745d 5d0a 2020 2020 2727 270a 0a20  int]].    '''.. 
 0006b2d0: 2020 2064 6566 2070 6f6c 6c28 7365 6c66     def poll(self
 0006b2e0: 2c20 636f 6e74 6578 743a 2074 7970 696e  , context: typin
 0006b2f0: 672e 4f70 7469 6f6e 616c 5b27 436f 6e74  g.Optional['Cont
 0006b300: 6578 7427 5d29 3a0a 2020 2020 2020 2020  ext']):.        
 0006b310: 2727 2720 5465 7374 2069 6620 4b65 7969  ''' Test if Keyi
 0006b320: 6e67 2053 6574 2063 616e 2062 6520 7573  ng Set can be us
 0006b330: 6564 206f 7220 6e6f 740a 0a20 2020 2020  ed or not..     
@@ -28181,23 +28181,23 @@
 0006e140: 7472 2c20 7479 7069 6e67 2e41 6e79 5d20  tr, typing.Any] 
 0006e150: 3d20 4e6f 6e65 0a20 2020 2027 2727 200a  = None.    ''' .
 0006e160: 0a20 2020 203a 7479 7065 3a20 7479 7069  .    :type: typi
 0006e170: 6e67 2e55 6e69 6f6e 5b73 7472 2c20 7479  ng.Union[str, ty
 0006e180: 7069 6e67 2e41 6e79 5d0a 2020 2020 2727  ping.Any].    ''
 0006e190: 270a 0a20 2020 2062 6c5f 6f70 7469 6f6e  '..    bl_option
 0006e1a0: 733a 2074 7970 696e 672e 556e 696f 6e5b  s: typing.Union[
-0006e1b0: 7479 7069 6e67 2e53 6574 5b69 6e74 5d2c  typing.Set[int],
-0006e1c0: 2074 7970 696e 672e 5365 745b 7374 725d   typing.Set[str]
+0006e1b0: 7479 7069 6e67 2e53 6574 5b73 7472 5d2c  typing.Set[str],
+0006e1c0: 2074 7970 696e 672e 5365 745b 696e 745d   typing.Set[int]
 0006e1d0: 5d20 3d20 4e6f 6e65 0a20 2020 2027 2727  ] = None.    '''
 0006e1e0: 204f 7074 696f 6e73 2066 6f72 2074 6869   Options for thi
 0006e1f0: 7320 6f70 6572 6174 6f72 2074 7970 650a  s operator type.
 0006e200: 0a20 2020 203a 7479 7065 3a20 7479 7069  .    :type: typi
 0006e210: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-0006e220: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
-0006e230: 2e53 6574 5b73 7472 5d5d 0a20 2020 2027  .Set[str]].    '
+0006e220: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
+0006e230: 2e53 6574 5b69 6e74 5d5d 0a20 2020 2027  .Set[int]].    '
 0006e240: 2727 0a0a 2020 2020 626c 5f74 7261 6e73  ''..    bl_trans
 0006e250: 6c61 7469 6f6e 5f63 6f6e 7465 7874 3a20  lation_context: 
 0006e260: 7479 7069 6e67 2e55 6e69 6f6e 5b73 7472  typing.Union[str
 0006e270: 2c20 7479 7069 6e67 2e41 6e79 5d20 3d20  , typing.Any] = 
 0006e280: 4e6f 6e65 0a20 2020 2027 2727 200a 0a20  None.    ''' .. 
 0006e290: 2020 203a 7479 7065 3a20 7479 7069 6e67     :type: typing
 0006e2a0: 2e55 6e69 6f6e 5b73 7472 2c20 7479 7069  .Union[str, typi
@@ -28232,27 +28232,27 @@
 0006e470: 6174 6f72 5072 6f70 6572 7469 6573 2720  atorProperties' 
 0006e480: 3d20 4e6f 6e65 0a20 2020 2027 2727 200a  = None.    ''' .
 0006e490: 0a20 2020 203a 7479 7065 3a20 274f 7065  .    :type: 'Ope
 0006e4a0: 7261 746f 7250 726f 7065 7274 6965 7327  ratorProperties'
 0006e4b0: 0a20 2020 2027 2727 0a0a 2020 2020 6465  .    '''..    de
 0006e4c0: 6620 7265 706f 7274 2873 656c 662c 2074  f report(self, t
 0006e4d0: 7970 653a 2074 7970 696e 672e 556e 696f  ype: typing.Unio
-0006e4e0: 6e5b 7479 7069 6e67 2e53 6574 5b69 6e74  n[typing.Set[int
-0006e4f0: 5d2c 2074 7970 696e 672e 5365 745b 7374  ], typing.Set[st
-0006e500: 725d 5d2c 0a20 2020 2020 2020 2020 2020  r]],.           
+0006e4e0: 6e5b 7479 7069 6e67 2e53 6574 5b73 7472  n[typing.Set[str
+0006e4f0: 5d2c 2074 7970 696e 672e 5365 745b 696e  ], typing.Set[in
+0006e500: 745d 5d2c 0a20 2020 2020 2020 2020 2020  t]],.           
 0006e510: 2020 2020 6d65 7373 6167 653a 2074 7970      message: typ
 0006e520: 696e 672e 556e 696f 6e5b 7374 722c 2074  ing.Union[str, t
 0006e530: 7970 696e 672e 416e 795d 293a 0a20 2020  yping.Any]):.   
 0006e540: 2020 2020 2027 2727 2072 6570 6f72 740a       ''' report.
 0006e550: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
 0006e560: 7479 7065 3a20 5479 7065 0a20 2020 2020  type: Type.     
 0006e570: 2020 203a 7479 7065 2074 7970 653a 2074     :type type: t
 0006e580: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
-0006e590: 6e67 2e53 6574 5b69 6e74 5d2c 2074 7970  ng.Set[int], typ
-0006e5a0: 696e 672e 5365 745b 7374 725d 5d0a 2020  ing.Set[str]].  
+0006e590: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
+0006e5a0: 696e 672e 5365 745b 696e 745d 5d0a 2020  ing.Set[int]].  
 0006e5b0: 2020 2020 2020 3a70 6172 616d 206d 6573        :param mes
 0006e5c0: 7361 6765 3a20 5265 706f 7274 204d 6573  sage: Report Mes
 0006e5d0: 7361 6765 0a20 2020 2020 2020 203a 7479  sage.        :ty
 0006e5e0: 7065 206d 6573 7361 6765 3a20 7479 7069  pe message: typi
 0006e5f0: 6e67 2e55 6e69 6f6e 5b73 7472 2c20 7479  ng.Union[str, ty
 0006e600: 7069 6e67 2e41 6e79 5d0a 2020 2020 2020  ping.Any].      
 0006e610: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
@@ -36236,23 +36236,23 @@
 0008d8b0: 6e5b 7374 722c 2074 7970 696e 672e 416e  n[str, typing.An
 0008d8c0: 795d 203d 204e 6f6e 650a 2020 2020 2727  y] = None.    ''
 0008d8d0: 2720 0a0a 2020 2020 3a74 7970 653a 2074  ' ..    :type: t
 0008d8e0: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
 0008d8f0: 2074 7970 696e 672e 416e 795d 0a20 2020   typing.Any].   
 0008d900: 2027 2727 0a0a 2020 2020 626c 5f6f 7074   '''..    bl_opt
 0008d910: 696f 6e73 3a20 7479 7069 6e67 2e55 6e69  ions: typing.Uni
-0008d920: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
-0008d930: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
-0008d940: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
+0008d920: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
+0008d930: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
+0008d940: 6e74 5d5d 203d 204e 6f6e 650a 2020 2020  nt]] = None.    
 0008d950: 2727 2720 4f70 7469 6f6e 7320 666f 7220  ''' Options for 
 0008d960: 7468 6973 206f 7065 7261 746f 7220 7479  this operator ty
 0008d970: 7065 0a0a 2020 2020 3a74 7970 653a 2074  pe..    :type: t
 0008d980: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
-0008d990: 6e67 2e53 6574 5b69 6e74 5d2c 2074 7970  ng.Set[int], typ
-0008d9a0: 696e 672e 5365 745b 7374 725d 5d0a 2020  ing.Set[str]].  
+0008d990: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
+0008d9a0: 696e 672e 5365 745b 696e 745d 5d0a 2020  ing.Set[int]].  
 0008d9b0: 2020 2727 270a 0a20 2020 2062 6c5f 7472    '''..    bl_tr
 0008d9c0: 616e 736c 6174 696f 6e5f 636f 6e74 6578  anslation_contex
 0008d9d0: 743a 2074 7970 696e 672e 556e 696f 6e5b  t: typing.Union[
 0008d9e0: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
 0008d9f0: 203d 204e 6f6e 650a 2020 2020 2727 2720   = None.    ''' 
 0008da00: 0a0a 2020 2020 3a74 7970 653a 2074 7970  ..    :type: typ
 0008da10: 696e 672e 556e 696f 6e5b 7374 722c 2074  ing.Union[str, t
@@ -36319,27 +36319,27 @@
 0008dde0: 6572 7479 2077 6865 6e20 6578 7061 6e64  erty when expand
 0008ddf0: 696e 6720 616e 206f 7065 7261 746f 7220  ing an operator 
 0008de00: 696e 746f 2061 206d 656e 752e 0a0a 2020  into a menu...  
 0008de10: 2020 3a74 7970 653a 2073 7472 0a20 2020    :type: str.   
 0008de20: 2027 2727 0a0a 2020 2020 6465 6620 7265   '''..    def re
 0008de30: 706f 7274 2873 656c 662c 2074 7970 653a  port(self, type:
 0008de40: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-0008de50: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
-0008de60: 7970 696e 672e 5365 745b 7374 725d 5d2c  yping.Set[str]],
+0008de50: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
+0008de60: 7970 696e 672e 5365 745b 696e 745d 5d2c  yping.Set[int]],
 0008de70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0008de80: 6d65 7373 6167 653a 2074 7970 696e 672e  message: typing.
 0008de90: 556e 696f 6e5b 7374 722c 2074 7970 696e  Union[str, typin
 0008dea0: 672e 416e 795d 293a 0a20 2020 2020 2020  g.Any]):.       
 0008deb0: 2027 2727 2072 6570 6f72 740a 0a20 2020   ''' report..   
 0008dec0: 2020 2020 203a 7061 7261 6d20 7479 7065       :param type
 0008ded0: 3a20 5479 7065 0a20 2020 2020 2020 203a  : Type.        :
 0008dee0: 7479 7065 2074 7970 653a 2074 7970 696e  type type: typin
 0008def0: 672e 556e 696f 6e5b 7479 7069 6e67 2e53  g.Union[typing.S
-0008df00: 6574 5b69 6e74 5d2c 2074 7970 696e 672e  et[int], typing.
-0008df10: 5365 745b 7374 725d 5d0a 2020 2020 2020  Set[str]].      
+0008df00: 6574 5b73 7472 5d2c 2074 7970 696e 672e  et[str], typing.
+0008df10: 5365 745b 696e 745d 5d0a 2020 2020 2020  Set[int]].      
 0008df20: 2020 3a70 6172 616d 206d 6573 7361 6765    :param message
 0008df30: 3a20 5265 706f 7274 204d 6573 7361 6765  : Report Message
 0008df40: 0a20 2020 2020 2020 203a 7479 7065 206d  .        :type m
 0008df50: 6573 7361 6765 3a20 7479 7069 6e67 2e55  essage: typing.U
 0008df60: 6e69 6f6e 5b73 7472 2c20 7479 7069 6e67  nion[str, typing
 0008df70: 2e41 6e79 5d0a 2020 2020 2020 2020 2727  .Any].        ''
 0008df80: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
@@ -36364,26 +36364,26 @@
 0008e0b0: 6f6e 7465 7874 270a 2020 2020 2020 2020  ontext'.        
 0008e0c0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
 0008e0d0: 0a0a 2020 2020 6465 6620 6578 6563 7574  ..    def execut
 0008e0e0: 6528 7365 6c66 2c20 636f 6e74 6578 743a  e(self, context:
 0008e0f0: 2027 436f 6e74 6578 7427 0a20 2020 2020   'Context'.     
 0008e100: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
 0008e110: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
-0008e120: 696e 672e 5365 745b 696e 745d 2c20 7479  ing.Set[int], ty
-0008e130: 7069 6e67 2e53 6574 5b73 7472 5d5d 3a0a  ping.Set[str]]:.
+0008e120: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
+0008e130: 7069 6e67 2e53 6574 5b69 6e74 5d5d 3a0a  ping.Set[int]]:.
 0008e140: 2020 2020 2020 2020 2727 2720 4578 6563          ''' Exec
 0008e150: 7574 6520 7468 6520 6f70 6572 6174 6f72  ute the operator
 0008e160: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
 0008e170: 2063 6f6e 7465 7874 3a20 0a20 2020 2020   context: .     
 0008e180: 2020 203a 7479 7065 2063 6f6e 7465 7874     :type context
 0008e190: 3a20 2743 6f6e 7465 7874 270a 2020 2020  : 'Context'.    
 0008e1a0: 2020 2020 3a72 7479 7065 3a20 7479 7069      :rtype: typi
 0008e1b0: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-0008e1c0: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
-0008e1d0: 2e53 6574 5b73 7472 5d5d 0a20 2020 2020  .Set[str]].     
+0008e1c0: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
+0008e1d0: 2e53 6574 5b69 6e74 5d5d 0a20 2020 2020  .Set[int]].     
 0008e1e0: 2020 203a 7265 7475 726e 3a20 7265 7375     :return: resu
 0008e1f0: 6c74 0a20 2020 2020 2020 2027 2727 0a20  lt.        '''. 
 0008e200: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
 0008e210: 2064 6566 2063 6865 636b 2873 656c 662c   def check(self,
 0008e220: 2063 6f6e 7465 7874 3a20 2743 6f6e 7465   context: 'Conte
 0008e230: 7874 2729 202d 3e20 626f 6f6c 3a0a 2020  xt') -> bool:.  
 0008e240: 2020 2020 2020 2727 2720 4368 6563 6b20        ''' Check 
@@ -36401,53 +36401,53 @@
 0008e300: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
 0008e310: 0a0a 2020 2020 6465 6620 696e 766f 6b65  ..    def invoke
 0008e320: 2873 656c 662c 2063 6f6e 7465 7874 3a20  (self, context: 
 0008e330: 2743 6f6e 7465 7874 272c 2065 7665 6e74  'Context', event
 0008e340: 3a20 2745 7665 6e74 270a 2020 2020 2020  : 'Event'.      
 0008e350: 2020 2020 2020 2020 2029 202d 3e20 7479           ) -> ty
 0008e360: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-0008e370: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
-0008e380: 6e67 2e53 6574 5b73 7472 5d5d 3a0a 2020  ng.Set[str]]:.  
+0008e370: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
+0008e380: 6e67 2e53 6574 5b69 6e74 5d5d 3a0a 2020  ng.Set[int]]:.  
 0008e390: 2020 2020 2020 2727 2720 496e 766f 6b65        ''' Invoke
 0008e3a0: 2074 6865 206f 7065 7261 746f 720a 0a20   the operator.. 
 0008e3b0: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
 0008e3c0: 6e74 6578 743a 200a 2020 2020 2020 2020  ntext: .        
 0008e3d0: 3a74 7970 6520 636f 6e74 6578 743a 2027  :type context: '
 0008e3e0: 436f 6e74 6578 7427 0a20 2020 2020 2020  Context'.       
 0008e3f0: 203a 7061 7261 6d20 6576 656e 743a 200a   :param event: .
 0008e400: 2020 2020 2020 2020 3a74 7970 6520 6576          :type ev
 0008e410: 656e 743a 2027 4576 656e 7427 0a20 2020  ent: 'Event'.   
 0008e420: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
 0008e430: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
-0008e440: 2e53 6574 5b69 6e74 5d2c 2074 7970 696e  .Set[int], typin
-0008e450: 672e 5365 745b 7374 725d 5d0a 2020 2020  g.Set[str]].    
+0008e440: 2e53 6574 5b73 7472 5d2c 2074 7970 696e  .Set[str], typin
+0008e450: 672e 5365 745b 696e 745d 5d0a 2020 2020  g.Set[int]].    
 0008e460: 2020 2020 3a72 6574 7572 6e3a 2072 6573      :return: res
 0008e470: 756c 740a 2020 2020 2020 2020 2727 270a  ult.        '''.
 0008e480: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
 0008e490: 2020 6465 6620 6d6f 6461 6c28 7365 6c66    def modal(self
 0008e4a0: 2c20 636f 6e74 6578 743a 2027 436f 6e74  , context: 'Cont
 0008e4b0: 6578 7427 2c20 6576 656e 743a 2027 4576  ext', event: 'Ev
 0008e4c0: 656e 7427 0a20 2020 2020 2020 2020 2020  ent'.           
 0008e4d0: 2020 2029 202d 3e20 7479 7069 6e67 2e55     ) -> typing.U
 0008e4e0: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-0008e4f0: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
-0008e500: 5b73 7472 5d5d 3a0a 2020 2020 2020 2020  [str]]:.        
+0008e4f0: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
+0008e500: 5b69 6e74 5d5d 3a0a 2020 2020 2020 2020  [int]]:.        
 0008e510: 2727 2720 4d6f 6461 6c20 6f70 6572 6174  ''' Modal operat
 0008e520: 6f72 2066 756e 6374 696f 6e0a 0a20 2020  or function..   
 0008e530: 2020 2020 203a 7061 7261 6d20 636f 6e74       :param cont
 0008e540: 6578 743a 200a 2020 2020 2020 2020 3a74  ext: .        :t
 0008e550: 7970 6520 636f 6e74 6578 743a 2027 436f  ype context: 'Co
 0008e560: 6e74 6578 7427 0a20 2020 2020 2020 203a  ntext'.        :
 0008e570: 7061 7261 6d20 6576 656e 743a 200a 2020  param event: .  
 0008e580: 2020 2020 2020 3a74 7970 6520 6576 656e        :type even
 0008e590: 743a 2027 4576 656e 7427 0a20 2020 2020  t: 'Event'.     
 0008e5a0: 2020 203a 7274 7970 653a 2074 7970 696e     :rtype: typin
 0008e5b0: 672e 556e 696f 6e5b 7479 7069 6e67 2e53  g.Union[typing.S
-0008e5c0: 6574 5b69 6e74 5d2c 2074 7970 696e 672e  et[int], typing.
-0008e5d0: 5365 745b 7374 725d 5d0a 2020 2020 2020  Set[str]].      
+0008e5c0: 6574 5b73 7472 5d2c 2074 7970 696e 672e  et[str], typing.
+0008e5d0: 5365 745b 696e 745d 5d0a 2020 2020 2020  Set[int]].      
 0008e5e0: 2020 3a72 6574 7572 6e3a 2072 6573 756c    :return: resul
 0008e5f0: 740a 2020 2020 2020 2020 2727 270a 2020  t.        '''.  
 0008e600: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
 0008e610: 6465 6620 6472 6177 2873 656c 662c 2063  def draw(self, c
 0008e620: 6f6e 7465 7874 3a20 2743 6f6e 7465 7874  ontext: 'Context
 0008e630: 2729 3a0a 2020 2020 2020 2020 2727 2720  '):.        ''' 
 0008e640: 4472 6177 2066 756e 6374 696f 6e20 666f  Draw function fo
@@ -46313,29 +46313,29 @@
 000b4e80: 2020 3a74 7970 6520 6d65 6d6f 7279 5f70    :type memory_p
 000b4e90: 6561 6b3a 2074 7970 696e 672e 4f70 7469  eak: typing.Opti
 000b4ea0: 6f6e 616c 5b74 7970 696e 672e 416e 795d  onal[typing.Any]
 000b4eb0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
 000b4ec0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
 000b4ed0: 6566 2072 6570 6f72 7428 7365 6c66 2c20  ef report(self, 
 000b4ee0: 7479 7065 3a20 7479 7069 6e67 2e55 6e69  type: typing.Uni
-000b4ef0: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
-000b4f00: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
-000b4f10: 7472 5d5d 2c0a 2020 2020 2020 2020 2020  tr]],.          
+000b4ef0: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
+000b4f00: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
+000b4f10: 6e74 5d5d 2c0a 2020 2020 2020 2020 2020  nt]],.          
 000b4f20: 2020 2020 206d 6573 7361 6765 3a20 7479       message: ty
 000b4f30: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
 000b4f40: 7479 7069 6e67 2e41 6e79 5d29 3a0a 2020  typing.Any]):.  
 000b4f50: 2020 2020 2020 2727 2720 5265 706f 7274        ''' Report
 000b4f60: 2069 6e66 6f2c 2077 6172 6e69 6e67 206f   info, warning o
 000b4f70: 7220 6572 726f 7220 6d65 7373 6167 6573  r error messages
 000b4f80: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
 000b4f90: 2074 7970 653a 2054 7970 650a 2020 2020   type: Type.    
 000b4fa0: 2020 2020 3a74 7970 6520 7479 7065 3a20      :type type: 
 000b4fb0: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
-000b4fc0: 696e 672e 5365 745b 696e 745d 2c20 7479  ing.Set[int], ty
-000b4fd0: 7069 6e67 2e53 6574 5b73 7472 5d5d 0a20  ping.Set[str]]. 
+000b4fc0: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
+000b4fd0: 7069 6e67 2e53 6574 5b69 6e74 5d5d 0a20  ping.Set[int]]. 
 000b4fe0: 2020 2020 2020 203a 7061 7261 6d20 6d65         :param me
 000b4ff0: 7373 6167 653a 2052 6570 6f72 7420 4d65  ssage: Report Me
 000b5000: 7373 6167 650a 2020 2020 2020 2020 3a74  ssage.        :t
 000b5010: 7970 6520 6d65 7373 6167 653a 2074 7970  ype message: typ
 000b5020: 696e 672e 556e 696f 6e5b 7374 722c 2074  ing.Union[str, t
 000b5030: 7970 696e 672e 416e 795d 0a20 2020 2020  yping.Any].     
 000b5040: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
@@ -66047,22 +66047,22 @@
 00101fe0: 6573 2077 6974 6820 7468 6520 6375 7272  es with the curr
 00101ff0: 656e 746c 7920 6469 7370 6c61 7965 6420  ently displayed 
 00102000: 696d 6167 6520 6173 7369 676e 6564 0a0a  image assigned..
 00102010: 2020 2020 3a74 7970 653a 2062 6f6f 6c0a      :type: bool.
 00102020: 2020 2020 2727 270a 0a20 2020 2073 6e61      '''..    sna
 00102030: 705f 656c 656d 656e 7473 3a20 7479 7069  p_elements: typi
 00102040: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-00102050: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
-00102060: 2e53 6574 5b73 7472 5d5d 203d 204e 6f6e  .Set[str]] = Non
+00102050: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
+00102060: 2e53 6574 5b69 6e74 5d5d 203d 204e 6f6e  .Set[int]] = Non
 00102070: 650a 2020 2020 2727 2720 5479 7065 206f  e.    ''' Type o
 00102080: 6620 656c 656d 656e 7420 746f 2073 6e61  f element to sna
 00102090: 7020 746f 0a0a 2020 2020 3a74 7970 653a  p to..    :type:
 001020a0: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-001020b0: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
-001020c0: 7970 696e 672e 5365 745b 7374 725d 5d0a  yping.Set[str]].
+001020b0: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
+001020c0: 7970 696e 672e 5365 745b 696e 745d 5d0a  yping.Set[int]].
 001020d0: 2020 2020 2727 270a 0a20 2020 2073 6e61      '''..    sna
 001020e0: 705f 656c 656d 656e 7473 5f62 6173 653a  p_elements_base:
 001020f0: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
 00102100: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
 00102110: 7970 696e 672e 5365 745b 696e 745d 5d20  yping.Set[int]] 
 00102120: 3d20 4e6f 6e65 0a20 2020 2027 2727 2054  = None.    ''' T
 00102130: 7970 6520 6f66 2065 6c65 6d65 6e74 2066  ype of element f
@@ -107778,16 +107778,16 @@
 001a5010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 001a5020: 2020 2020 2020 2020 2020 2020 6576 656e              even
 001a5030: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
 001a5040: 616c 5b27 4576 656e 7427 5d0a 2020 2020  al['Event'].    
 001a5050: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a5060: 2020 2020 2020 2029 202d 3e20 7479 7069         ) -> typi
 001a5070: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-001a5080: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
-001a5090: 2e53 6574 5b73 7472 5d5d 3a0a 2020 2020  .Set[str]]:.    
+001a5080: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
+001a5090: 2e53 6574 5b69 6e74 5d5d 3a0a 2020 2020  .Set[int]]:.    
 001a50a0: 2020 2020 2727 2720 4f70 6572 6174 6f72      ''' Operator
 001a50b0: 2070 6f70 7570 2069 6e76 6f6b 6520 2873   popup invoke (s
 001a50c0: 686f 7720 6f70 6572 6174 6f72 2070 726f  how operator pro
 001a50d0: 7065 7274 6965 7320 616e 6420 6578 6563  perties and exec
 001a50e0: 7574 6520 6974 2061 7574 6f6d 6174 6963  ute it automatic
 001a50f0: 616c 6c79 206f 6e20 6368 616e 6765 7329  ally on changes)
 001a5100: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
@@ -107799,16 +107799,16 @@
 001a5160: 2020 2020 2020 2020 3a70 6172 616d 2065          :param e
 001a5170: 7665 6e74 3a20 4576 656e 740a 2020 2020  vent: Event.    
 001a5180: 2020 2020 3a74 7970 6520 6576 656e 743a      :type event:
 001a5190: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
 001a51a0: 5b27 4576 656e 7427 5d0a 2020 2020 2020  ['Event'].      
 001a51b0: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
 001a51c0: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-001a51d0: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
-001a51e0: 6574 5b73 7472 5d5d 0a20 2020 2020 2020  et[str]].       
+001a51d0: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
+001a51e0: 6574 5b69 6e74 5d5d 0a20 2020 2020 2020  et[int]].       
 001a51f0: 203a 7265 7475 726e 3a20 7265 7375 6c74   :return: result
 001a5200: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
 001a5210: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
 001a5220: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
 001a5230: 6465 6620 696e 766f 6b65 5f70 726f 7073  def invoke_props
 001a5240: 5f64 6961 6c6f 6728 0a20 2020 2020 2020  _dialog(.       
 001a5250: 2020 2020 2063 6c73 2c0a 2020 2020 2020       cls,.      
@@ -107816,16 +107816,16 @@
 001a5270: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
 001a5280: 274f 7065 7261 746f 7227 5d2c 0a20 2020  'Operator'],.   
 001a5290: 2020 2020 2020 2020 2077 6964 7468 3a20           width: 
 001a52a0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
 001a52b0: 7479 7069 6e67 2e41 6e79 5d20 3d20 3330  typing.Any] = 30
 001a52c0: 300a 2020 2020 2920 2d3e 2074 7970 696e  0.    ) -> typin
 001a52d0: 672e 556e 696f 6e5b 7479 7069 6e67 2e53  g.Union[typing.S
-001a52e0: 6574 5b69 6e74 5d2c 2074 7970 696e 672e  et[int], typing.
-001a52f0: 5365 745b 7374 725d 5d3a 0a20 2020 2020  Set[str]]:.     
+001a52e0: 6574 5b73 7472 5d2c 2074 7970 696e 672e  et[str], typing.
+001a52f0: 5365 745b 696e 745d 5d3a 0a20 2020 2020  Set[int]]:.     
 001a5300: 2020 2027 2727 204f 7065 7261 746f 7220     ''' Operator 
 001a5310: 6469 616c 6f67 2028 6e6f 6e2d 6175 746f  dialog (non-auto
 001a5320: 6578 6563 2070 6f70 7570 2920 696e 766f  exec popup) invo
 001a5330: 6b65 2028 7368 6f77 206f 7065 7261 746f  ke (show operato
 001a5340: 7220 7072 6f70 6572 7469 6573 2061 6e64  r properties and
 001a5350: 206f 6e6c 7920 6578 6563 7574 6520 6974   only execute it
 001a5360: 206f 6e20 636c 6963 6b20 6f6e 204f 4b20   on click on OK 
@@ -107839,16 +107839,16 @@
 001a53e0: 7061 7261 6d20 7769 6474 683a 2057 6964  param width: Wid
 001a53f0: 7468 206f 6620 7468 6520 706f 7075 700a  th of the popup.
 001a5400: 2020 2020 2020 2020 3a74 7970 6520 7769          :type wi
 001a5410: 6474 683a 2074 7970 696e 672e 4f70 7469  dth: typing.Opti
 001a5420: 6f6e 616c 5b74 7970 696e 672e 416e 795d  onal[typing.Any]
 001a5430: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
 001a5440: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-001a5450: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
-001a5460: 7970 696e 672e 5365 745b 7374 725d 5d0a  yping.Set[str]].
+001a5450: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
+001a5460: 7970 696e 672e 5365 745b 696e 745d 5d0a  yping.Set[int]].
 001a5470: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
 001a5480: 2072 6573 756c 740a 2020 2020 2020 2020   result.        
 001a5490: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
 001a54a0: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
 001a54b0: 6f64 0a20 2020 2064 6566 2069 6e76 6f6b  od.    def invok
 001a54c0: 655f 7365 6172 6368 5f70 6f70 7570 2863  e_search_popup(c
 001a54d0: 6c73 2c20 6f70 6572 6174 6f72 3a20 7479  ls, operator: ty
@@ -107881,16 +107881,16 @@
 001a5680: 4f70 6572 6174 6f72 275d 2c0a 2020 2020  Operator'],.    
 001a5690: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a56a0: 2077 6964 7468 3a20 7479 7069 6e67 2e4f   width: typing.O
 001a56b0: 7074 696f 6e61 6c5b 7479 7069 6e67 2e41  ptional[typing.A
 001a56c0: 6e79 5d20 3d20 3330 300a 2020 2020 2020  ny] = 300.      
 001a56d0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
 001a56e0: 202d 3e20 7479 7069 6e67 2e55 6e69 6f6e   -> typing.Union
-001a56f0: 5b74 7970 696e 672e 5365 745b 696e 745d  [typing.Set[int]
-001a5700: 2c20 7479 7069 6e67 2e53 6574 5b73 7472  , typing.Set[str
+001a56f0: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
+001a5700: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
 001a5710: 5d5d 3a0a 2020 2020 2020 2020 2727 2720  ]]:.        ''' 
 001a5720: 4f70 6572 6174 6f72 2070 6f70 7570 2069  Operator popup i
 001a5730: 6e76 6f6b 6520 286f 6e6c 7920 7368 6f77  nvoke (only show
 001a5740: 7320 6f70 6572 6174 6f72 2773 2070 726f  s operator's pro
 001a5750: 7065 7274 6965 732c 2077 6974 686f 7574  perties, without
 001a5760: 2065 7865 6375 7469 6e67 2069 7429 0a0a   executing it)..
 001a5770: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
@@ -107903,32 +107903,32 @@
 001a57e0: 7468 3a20 5769 6474 6820 6f66 2074 6865  th: Width of the
 001a57f0: 2070 6f70 7570 0a20 2020 2020 2020 203a   popup.        :
 001a5800: 7479 7065 2077 6964 7468 3a20 7479 7069  type width: typi
 001a5810: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
 001a5820: 6e67 2e41 6e79 5d0a 2020 2020 2020 2020  ng.Any].        
 001a5830: 3a72 7479 7065 3a20 7479 7069 6e67 2e55  :rtype: typing.U
 001a5840: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-001a5850: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
-001a5860: 5b73 7472 5d5d 0a20 2020 2020 2020 203a  [str]].        :
+001a5850: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
+001a5860: 5b69 6e74 5d5d 0a20 2020 2020 2020 203a  [int]].        :
 001a5870: 7265 7475 726e 3a20 7265 7375 6c74 0a20  return: result. 
 001a5880: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
 001a5890: 2020 2070 6173 730a 0a20 2020 2040 636c     pass..    @cl
 001a58a0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
 001a58b0: 6620 696e 766f 6b65 5f63 6f6e 6669 726d  f invoke_confirm
 001a58c0: 2863 6c73 2c20 6f70 6572 6174 6f72 3a20  (cls, operator: 
 001a58d0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
 001a58e0: 274f 7065 7261 746f 7227 5d2c 0a20 2020  'Operator'],.   
 001a58f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a5900: 2020 2020 6576 656e 743a 2074 7970 696e      event: typin
 001a5910: 672e 4f70 7469 6f6e 616c 5b27 4576 656e  g.Optional['Even
 001a5920: 7427 5d0a 2020 2020 2020 2020 2020 2020  t'].            
 001a5930: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
 001a5940: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
-001a5950: 696e 672e 5365 745b 696e 745d 2c20 7479  ing.Set[int], ty
-001a5960: 7069 6e67 2e53 6574 5b73 7472 5d5d 3a0a  ping.Set[str]]:.
+001a5950: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
+001a5960: 7069 6e67 2e53 6574 5b69 6e74 5d5d 3a0a  ping.Set[int]]:.
 001a5970: 2020 2020 2020 2020 2727 2720 4f70 6572          ''' Oper
 001a5980: 6174 6f72 2063 6f6e 6669 726d 6174 696f  ator confirmatio
 001a5990: 6e20 706f 7075 7020 286f 6e6c 7920 746f  n popup (only to
 001a59a0: 206c 6574 2075 7365 7220 636f 6e66 6972   let user confir
 001a59b0: 6d20 7468 6520 6578 6563 7574 696f 6e2c  m the execution,
 001a59c0: 206e 6f20 6f70 6572 6174 6f72 2070 726f   no operator pro
 001a59d0: 7065 7274 6965 7320 7368 6f77 6e29 0a0a  perties shown)..
@@ -107941,16 +107941,16 @@
 001a5a40: 2020 2020 2020 3a70 6172 616d 2065 7665        :param eve
 001a5a50: 6e74 3a20 4576 656e 740a 2020 2020 2020  nt: Event.      
 001a5a60: 2020 3a74 7970 6520 6576 656e 743a 2074    :type event: t
 001a5a70: 7970 696e 672e 4f70 7469 6f6e 616c 5b27  yping.Optional['
 001a5a80: 4576 656e 7427 5d0a 2020 2020 2020 2020  Event'].        
 001a5a90: 3a72 7479 7065 3a20 7479 7069 6e67 2e55  :rtype: typing.U
 001a5aa0: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-001a5ab0: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
-001a5ac0: 5b73 7472 5d5d 0a20 2020 2020 2020 203a  [str]].        :
+001a5ab0: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
+001a5ac0: 5b69 6e74 5d5d 0a20 2020 2020 2020 203a  [int]].        :
 001a5ad0: 7265 7475 726e 3a20 7265 7375 6c74 0a20  return: result. 
 001a5ae0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
 001a5af0: 2020 2070 6173 730a 0a20 2020 2040 636c     pass..    @cl
 001a5b00: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
 001a5b10: 6620 706f 706d 656e 755f 6265 6769 6e5f  f popmenu_begin_
 001a5b20: 5f69 6e74 6572 6e61 6c28 636c 732c 0a20  _internal(cls,. 
 001a5b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
@@ -113286,22 +113286,22 @@
 001ba850: 6d65 7472 7920 746f 2066 6f72 6d20 706c  metry to form pl
 001ba860: 616e 6172 2070 6f6c 7967 6f6e 732e 0a0a  anar polygons...
 001ba870: 2020 2020 3a74 7970 653a 2074 7970 696e      :type: typin
 001ba880: 672e 556e 696f 6e5b 7374 722c 2069 6e74  g.Union[str, int
 001ba890: 5d0a 2020 2020 2727 270a 0a20 2020 2064  ].    '''..    d
 001ba8a0: 656c 696d 6974 3a20 7479 7069 6e67 2e55  elimit: typing.U
 001ba8b0: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-001ba8c0: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
-001ba8d0: 5b73 7472 5d5d 203d 204e 6f6e 650a 2020  [str]] = None.  
+001ba8c0: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
+001ba8d0: 5b69 6e74 5d5d 203d 204e 6f6e 650a 2020  [int]] = None.  
 001ba8e0: 2020 2727 2720 4c69 6d69 7420 6d65 7267    ''' Limit merg
 001ba8f0: 696e 6720 6765 6f6d 6574 7279 0a0a 2020  ing geometry..  
 001ba900: 2020 3a74 7970 653a 2074 7970 696e 672e    :type: typing.
 001ba910: 556e 696f 6e5b 7479 7069 6e67 2e53 6574  Union[typing.Set
-001ba920: 5b69 6e74 5d2c 2074 7970 696e 672e 5365  [int], typing.Se
-001ba930: 745b 7374 725d 5d0a 2020 2020 2727 270a  t[str]].    '''.
+001ba920: 5b73 7472 5d2c 2074 7970 696e 672e 5365  [str], typing.Se
+001ba930: 745b 696e 745d 5d0a 2020 2020 2727 270a  t[int]].    '''.
 001ba940: 0a20 2020 2066 6163 655f 636f 756e 743a  .    face_count:
 001ba950: 2069 6e74 203d 204e 6f6e 650a 2020 2020   int = None.    
 001ba960: 2727 2720 5468 6520 6375 7272 656e 7420  ''' The current 
 001ba970: 6e75 6d62 6572 206f 6620 6661 6365 7320  number of faces 
 001ba980: 696e 2074 6865 2064 6563 696d 6174 6564  in the decimated
 001ba990: 206d 6573 680a 0a20 2020 203a 7479 7065   mesh..    :type
 001ba9a0: 3a20 696e 740a 2020 2020 2727 270a 0a20  : int.    '''.. 
@@ -114569,21 +114569,21 @@
 001bf880: 5061 7468 2074 6f20 6578 7465 726e 616c  Path to external
 001bf890: 2064 6973 706c 6163 656d 656e 7473 2066   displacements f
 001bf8a0: 696c 650a 0a20 2020 203a 7479 7065 3a20  ile..    :type: 
 001bf8b0: 7479 7069 6e67 2e55 6e69 6f6e 5b73 7472  typing.Union[str
 001bf8c0: 2c20 7479 7069 6e67 2e41 6e79 5d0a 2020  , typing.Any].  
 001bf8d0: 2020 2727 270a 0a20 2020 2066 6c69 705f    '''..    flip_
 001bf8e0: 6178 6973 3a20 7479 7069 6e67 2e55 6e69  axis: typing.Uni
-001bf8f0: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
-001bf900: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
-001bf910: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
+001bf8f0: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
+001bf900: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
+001bf910: 6e74 5d5d 203d 204e 6f6e 650a 2020 2020  nt]] = None.    
 001bf920: 2727 2720 0a0a 2020 2020 3a74 7970 653a  ''' ..    :type:
 001bf930: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-001bf940: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
-001bf950: 7970 696e 672e 5365 745b 7374 725d 5d0a  yping.Set[str]].
+001bf940: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
+001bf950: 7970 696e 672e 5365 745b 696e 745d 5d0a  yping.Set[int]].
 001bf960: 2020 2020 2727 270a 0a20 2020 2066 6f72      '''..    for
 001bf970: 7761 7264 5f61 7869 733a 2074 7970 696e  ward_axis: typin
 001bf980: 672e 556e 696f 6e5b 7374 722c 2069 6e74  g.Union[str, int
 001bf990: 5d20 3d20 4e6f 6e65 0a20 2020 2027 2727  ] = None.    '''
 001bf9a0: 200a 0a20 2020 203a 7479 7065 3a20 7479   ..    :type: ty
 001bf9b0: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
 001bf9c0: 696e 745d 0a20 2020 2027 2727 0a0a 2020  int].    '''..
```

### Comparing `fake-bpy-module-latest-20230615/bpy/utils/__init__.py` & `fake-bpy-module-latest-20230616/bpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/utils/previews.py` & `fake-bpy-module-latest-20230616/bpy/utils/previews.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy/utils/units.py` & `fake-bpy-module-latest-20230616/bpy/utils/units.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy_extras/anim_utils.py` & `fake-bpy-module-latest-20230616/bpy_extras/anim_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     '''
 
     pass
 
 
 def bake_action_objects_iter(
         object_action_pairs: typing.
-        Union['bpy.types.Object', 'bpy.types.Action', 'bpy.types.Sequence'],
+        Union['bpy.types.Sequence', 'bpy.types.Action', 'bpy.types.Object'],
         **kwargs):
     ''' An coroutine that bakes actions for multiple objects.
 
     :param object_action_pairs: Sequence of object action tuples, action is the destination for the baked data. When None a new action will be created.
-    :type object_action_pairs: typing.Union['bpy.types.Object', 'bpy.types.Action', 'bpy.types.Sequence']
+    :type object_action_pairs: typing.Union['bpy.types.Sequence', 'bpy.types.Action', 'bpy.types.Object']
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230615/bpy_extras/image_utils.py` & `fake-bpy-module-latest-20230616/bpy_extras/image_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy_extras/io_utils.py` & `fake-bpy-module-latest-20230616/bpy_extras/io_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy_extras/mesh_utils.py` & `fake-bpy-module-latest-20230616/bpy_extras/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy_extras/node_shader_utils.py` & `fake-bpy-module-latest-20230616/bpy_extras/node_shader_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy_extras/object_utils.py` & `fake-bpy-module-latest-20230616/bpy_extras/object_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy_extras/view3d_utils.py` & `fake-bpy-module-latest-20230616/bpy_extras/view3d_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy_extras/wm_utils/progress_report.py` & `fake-bpy-module-latest-20230616/bpy_extras/wm_utils/progress_report.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/bpy_types.py` & `fake-bpy-module-latest-20230616/bpy_types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/fake_bpy_module_latest.egg-info/PKG-INFO` & `fake-bpy-module-latest-20230616/fake_bpy_module_latest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230615
+Version: 20230616
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230615/fake_bpy_module_latest.egg-info/SOURCES.txt` & `fake-bpy-module-latest-20230616/fake_bpy_module_latest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/freestyle/chainingiterators.py` & `fake-bpy-module-latest-20230616/freestyle/chainingiterators.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/freestyle/functions.py` & `fake-bpy-module-latest-20230616/freestyle/functions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/freestyle/predicates.py` & `fake-bpy-module-latest-20230616/freestyle/predicates.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/freestyle/shaders.py` & `fake-bpy-module-latest-20230616/freestyle/shaders.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/freestyle/types.py` & `fake-bpy-module-latest-20230616/freestyle/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/freestyle/utils/ContextFunctions.py` & `fake-bpy-module-latest-20230616/freestyle/utils/ContextFunctions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/freestyle/utils/__init__.py` & `fake-bpy-module-latest-20230616/freestyle/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/gpu/capabilities.py` & `fake-bpy-module-latest-20230616/gpu/capabilities.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/gpu/matrix.py` & `fake-bpy-module-latest-20230616/gpu/matrix.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/gpu/platform.py` & `fake-bpy-module-latest-20230616/gpu/platform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/gpu/shader.py` & `fake-bpy-module-latest-20230616/gpu/shader.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/gpu/state.py` & `fake-bpy-module-latest-20230616/gpu/state.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/gpu/texture.py` & `fake-bpy-module-latest-20230616/gpu/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/gpu/types.py` & `fake-bpy-module-latest-20230616/gpu/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/gpu_extras/batch.py` & `fake-bpy-module-latest-20230616/gpu_extras/batch.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/gpu_extras/presets.py` & `fake-bpy-module-latest-20230616/gpu_extras/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/idprop/types.py` & `fake-bpy-module-latest-20230616/idprop/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/imbuf/__init__.py` & `fake-bpy-module-latest-20230616/imbuf/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/imbuf/types.py` & `fake-bpy-module-latest-20230616/imbuf/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/keyingsets_builtins.py` & `fake-bpy-module-latest-20230616/keyingsets_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/keyingsets_utils.py` & `fake-bpy-module-latest-20230616/keyingsets_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/mathutils/__init__.py` & `fake-bpy-module-latest-20230616/mathutils/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import typing
+from . import kdtree
+from . import noise
 from . import bvhtree
 from . import interpolate
-from . import kdtree
 from . import geometry
-from . import noise
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class Color:
     ''' This object gives access to Colors in Blender. Most colors returned by Blender APIs are in scene linear color space, as defined by the OpenColorIO configuration. The notable exception is user interface theming colors, which are in sRGB color space. :arg rgb: (r, g, b) color values :type rgb: 3d vector
     '''
```

### Comparing `fake-bpy-module-latest-20230615/mathutils/bvhtree.py` & `fake-bpy-module-latest-20230616/mathutils/bvhtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/mathutils/geometry.py` & `fake-bpy-module-latest-20230616/mathutils/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/mathutils/kdtree.py` & `fake-bpy-module-latest-20230616/mathutils/kdtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/mathutils/noise.py` & `fake-bpy-module-latest-20230616/mathutils/noise.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/nodeitems_builtins.py` & `fake-bpy-module-latest-20230616/nodeitems_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/nodeitems_utils.py` & `fake-bpy-module-latest-20230616/nodeitems_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/rna_info.py` & `fake-bpy-module-latest-20230616/rna_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/rna_keymap_ui.py` & `fake-bpy-module-latest-20230616/rna_keymap_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/rna_prop_ui.py` & `fake-bpy-module-latest-20230616/rna_prop_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/rna_xml.py` & `fake-bpy-module-latest-20230616/rna_xml.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230615/setup.py` & `fake-bpy-module-latest-20230616/setup.py`

 * *Files identical despite different names*

