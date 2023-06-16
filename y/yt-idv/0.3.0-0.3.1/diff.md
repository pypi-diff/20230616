# Comparing `tmp/yt_idv-0.3.0.tar.gz` & `tmp/yt_idv-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_idv-0.3.0.tar", last modified: Wed Apr 12 17:34:33 2023, max compression
+gzip compressed data, was "yt_idv-0.3.1.tar", last modified: Fri Jun 16 20:14:50 2023, max compression
```

## Comparing `yt_idv-0.3.0.tar` & `yt_idv-0.3.1.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:33.822305 yt_idv-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-12 17:34:19.000000 yt_idv-0.3.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-12 17:34:19.000000 yt_idv-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 17:34:19.000000 yt_idv-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-12 17:34:19.000000 yt_idv-0.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-12 17:34:19.000000 yt_idv-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-12 17:34:19.000000 yt_idv-0.3.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-12 17:34:19.000000 yt_idv-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-12 17:34:19.000000 yt_idv-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-12 17:34:19.000000 yt_idv-0.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-12 17:34:33.822305 yt_idv-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-12 17:34:19.000000 yt_idv-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:33.810305 yt_idv-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5222 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/scene.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/yt_idv.cameras.rst
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/yt_idv.misc.rst
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/yt_idv.rendering_contexts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/yt_idv.scene_annotations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/yt_idv.scene_components.rst
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/yt_idv.scene_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 17:34:19.000000 yt_idv-0.3.0/docs/yt_idv.scene_graph.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:33.810305 yt_idv-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-12 17:34:19.000000 yt_idv-0.3.0/examples/amr_offscreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-12 17:34:19.000000 yt_idv-0.3.0/examples/amr_osmesa.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-12 17:34:19.000000 yt_idv-0.3.0/examples/amr_volume_rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-12 17:34:19.000000 yt_idv-0.3.0/examples/amr_volume_rendering_with_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-12 17:34:19.000000 yt_idv-0.3.0/examples/grid_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-12 17:34:19.000000 yt_idv-0.3.0/examples/hires_galaxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-12 17:34:19.000000 yt_idv-0.3.0/examples/idv_widget.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-12 17:34:19.000000 yt_idv-0.3.0/examples/mesh_render.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 17:34:19.000000 yt_idv-0.3.0/examples/octree_volume_rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-12 17:34:19.000000 yt_idv-0.3.0/examples/particle_rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-12 17:34:19.000000 yt_idv-0.3.0/examples/sph_rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-12 17:34:19.000000 yt_idv-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-12 17:34:33.822305 yt_idv-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-12 17:34:19.000000 yt_idv-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:33.810305 yt_idv-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 17:34:19.000000 yt_idv-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-12 17:34:19.000000 yt_idv-0.3.0/tests/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-12 17:34:19.000000 yt_idv-0.3.0/tests/test_yt_idv.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-12 17:34:19.000000 yt_idv-0.3.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:33.814305 yt_idv-0.3.0/yt_idv/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:33.814305 yt_idv-0.3.0/yt_idv/cameras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/cameras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/cameras/base_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/cameras/trackball_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/gui_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/opengl_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:33.814305 yt_idv-0.3.0/yt_idv/rendering_contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/rendering_contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/rendering_contexts/base_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/rendering_contexts/base_offscreen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/rendering_contexts/egl_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/rendering_contexts/osmesa_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/rendering_contexts/pyglet_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:33.814305 yt_idv-0.3.0/yt_idv/scene_annotations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_annotations/base_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_annotations/block_outline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_annotations/box.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_annotations/grid_outlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_annotations/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:33.818305 yt_idv-0.3.0/yt_idv/scene_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_components/base_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_components/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_components/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_components/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_components/octree_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_components/particles.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_components/rgba.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_components/sph_particles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:33.818305 yt_idv-0.3.0/yt_idv/scene_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_data/base_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_data/block_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_data/box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_data/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_data/grid_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_data/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_data/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_data/octree_block_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_data/particle_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_data/rgba.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_data/text_characters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/scene_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shader_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:33.822305 yt_idv-0.3.0/yt_idv/shaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/apply_colormap.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/block_outline.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/constant.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/constant_rgba.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/default.vert.glsl
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/draw_colormap.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/draw_lines.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/draw_lines.vert.glsl
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/expand_1d.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/field_value.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/grid_expand.geom.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/grid_position.vert.glsl
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/header.inc.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/isocontour.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/known_uniforms.inc.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/max_intensity.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/mesh.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/mesh.vert.glsl
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/noop.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/octree_position.vert.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/particle.vert.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/particle_expand.geom.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/passthrough.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/passthrough.vert.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/projection.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/ray_tracing.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/shaderlist.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/slice_sample.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/sph_kernel.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/textoverlay.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/textoverlay.vert.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/shaders/transfer_function.frag.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/simple_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/traitlets_support.py
--rw-r--r--   0 runner    (1001) docker     (123)   877930 2023-04-12 17:34:33.000000 yt_idv-0.3.0/yt_idv/utilities.c
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/utilities.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 17:34:19.000000 yt_idv-0.3.0/yt_idv/yt_idv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:34:33.814305 yt_idv-0.3.0/yt_idv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-12 17:34:33.000000 yt_idv-0.3.0/yt_idv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-12 17:34:33.000000 yt_idv-0.3.0/yt_idv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:34:33.000000 yt_idv-0.3.0/yt_idv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 17:34:33.000000 yt_idv-0.3.0/yt_idv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:34:33.000000 yt_idv-0.3.0/yt_idv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 17:34:33.000000 yt_idv-0.3.0/yt_idv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 17:34:33.000000 yt_idv-0.3.0/yt_idv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:50.322816 yt_idv-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-16 20:14:32.000000 yt_idv-0.3.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-16 20:14:32.000000 yt_idv-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-16 20:14:32.000000 yt_idv-0.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-16 20:14:32.000000 yt_idv-0.3.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-16 20:14:32.000000 yt_idv-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-16 20:14:32.000000 yt_idv-0.3.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-16 20:14:32.000000 yt_idv-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-16 20:14:32.000000 yt_idv-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-16 20:14:32.000000 yt_idv-0.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-16 20:14:50.322816 yt_idv-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-16 20:14:32.000000 yt_idv-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:50.306816 yt_idv-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5222 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/scene.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/yt_idv.cameras.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/yt_idv.misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/yt_idv.rendering_contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/yt_idv.scene_annotations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/yt_idv.scene_components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/yt_idv.scene_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 20:14:32.000000 yt_idv-0.3.1/docs/yt_idv.scene_graph.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:50.306816 yt_idv-0.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-16 20:14:32.000000 yt_idv-0.3.1/examples/amr_offscreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 20:14:32.000000 yt_idv-0.3.1/examples/amr_osmesa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-16 20:14:32.000000 yt_idv-0.3.1/examples/amr_volume_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-16 20:14:32.000000 yt_idv-0.3.1/examples/amr_volume_rendering_with_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-16 20:14:32.000000 yt_idv-0.3.1/examples/grid_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-16 20:14:32.000000 yt_idv-0.3.1/examples/hires_galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-16 20:14:32.000000 yt_idv-0.3.1/examples/idv_widget.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-16 20:14:32.000000 yt_idv-0.3.1/examples/mesh_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 20:14:32.000000 yt_idv-0.3.1/examples/octree_volume_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 20:14:32.000000 yt_idv-0.3.1/examples/particle_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-16 20:14:32.000000 yt_idv-0.3.1/examples/sph_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-16 20:14:32.000000 yt_idv-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-16 20:14:50.322816 yt_idv-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-16 20:14:32.000000 yt_idv-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:50.306816 yt_idv-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 20:14:32.000000 yt_idv-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-16 20:14:32.000000 yt_idv-0.3.1/tests/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-16 20:14:32.000000 yt_idv-0.3.1/tests/test_yt_idv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-16 20:14:32.000000 yt_idv-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:50.310816 yt_idv-0.3.1/yt_idv/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:50.310816 yt_idv-0.3.1/yt_idv/cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/cameras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/cameras/base_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/cameras/trackball_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/gui_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17482 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/opengl_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:50.310816 yt_idv-0.3.1/yt_idv/rendering_contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/rendering_contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/rendering_contexts/base_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/rendering_contexts/base_offscreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/rendering_contexts/egl_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/rendering_contexts/osmesa_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/rendering_contexts/pyglet_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:50.310816 yt_idv-0.3.1/yt_idv/scene_annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_annotations/base_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_annotations/block_outline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_annotations/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_annotations/grid_outlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_annotations/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:50.314816 yt_idv-0.3.1/yt_idv/scene_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18173 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_components/base_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_components/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_components/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_components/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_components/octree_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_components/particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_components/rgba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_components/sph_particles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:50.314816 yt_idv-0.3.1/yt_idv/scene_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_data/base_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_data/block_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_data/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_data/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_data/grid_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_data/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_data/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_data/octree_block_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_data/particle_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_data/rgba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_data/text_characters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/scene_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13508 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shader_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:50.322816 yt_idv-0.3.1/yt_idv/shaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/apply_colormap.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/block_outline.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/constant.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/constant_rgba.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/default.vert.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/draw_colormap.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/draw_lines.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/draw_lines.vert.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/expand_1d.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/field_value.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/grid_expand.geom.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/grid_position.vert.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/header.inc.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/isocontour.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/known_uniforms.inc.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/max_intensity.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/mesh.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/mesh.vert.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/noop.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/octree_position.vert.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/particle.vert.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/particle_expand.geom.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/passthrough.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/passthrough.vert.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/projection.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/ray_tracing.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/shaderlist.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/slice_sample.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/sph_kernel.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/textoverlay.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/textoverlay.vert.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/shaders/transfer_function.frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/simple_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/traitlets_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)   878535 2023-06-16 20:14:49.000000 yt_idv-0.3.1/yt_idv/utilities.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/utilities.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 20:14:32.000000 yt_idv-0.3.1/yt_idv/yt_idv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:14:50.310816 yt_idv-0.3.1/yt_idv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-16 20:14:50.000000 yt_idv-0.3.1/yt_idv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-16 20:14:50.000000 yt_idv-0.3.1/yt_idv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:14:50.000000 yt_idv-0.3.1/yt_idv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 20:14:50.000000 yt_idv-0.3.1/yt_idv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:14:49.000000 yt_idv-0.3.1/yt_idv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-16 20:14:50.000000 yt_idv-0.3.1/yt_idv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 20:14:50.000000 yt_idv-0.3.1/yt_idv.egg-info/top_level.txt
```

### Comparing `yt_idv-0.3.0/.pre-commit-config.yaml` & `yt_idv-0.3.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
 -   repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v2.2.0
+    rev: v2.3.0
     hooks:
     - id: setup-cfg-fmt
       args: [
         --include-version-classifiers,
         --max-py-version=3.10,
       ]
 -   repo: https://github.com/pre-commit/pre-commit-hooks
@@ -13,15 +13,15 @@
     - id: trailing-whitespace
     - id: end-of-file-fixer
     - id: no-commit-to-branch
     - id: check-shebang-scripts-are-executable
     - id: check-executables-have-shebangs
     - id: check-yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.6.0
     hooks:
     - id: pyupgrade
       args: [--py37-plus]
 -   repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
     - id: black-jupyter
```

### Comparing `yt_idv-0.3.0/.readthedocs.yml` & `yt_idv-0.3.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/CONTRIBUTING.md` & `yt_idv-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/LICENSE` & `yt_idv-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/MANIFEST.in` & `yt_idv-0.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/Makefile` & `yt_idv-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/PKG-INFO` & `yt_idv-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt_idv
-Version: 0.3.0
+Version: 0.3.1
 Summary: Interactive Volume Rendering for yt
 Home-page: https://github.com/yt-project/yt_idv
 Author: Matthew Turk
 Author-email: matthewturk@gmail.com
 License: BSD-3-Clause
 Keywords: yt_idv
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,20 +25,22 @@
 
 # interactive volume rendering for yt
 
 [![](https://img.shields.io/pypi/v/yt_idv.svg)](https://pypi.python.org/pypi/yt_idv)
 
 [![Doc Status](https://readthedocs.org/projects/yt-idv/badge/?version=latest)](https://yt-idv.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/yt-project/yt_idv/main.svg)](https://results.pre-commit.ci/latest/github/yt-project/yt_idv/main)
+[![Run tests](https://github.com/yt-project/yt_idv/actions/workflows/build-test.yaml/badge.svg)](https://github.com/yt-project/yt_idv/actions/workflows/build-test.yaml)
 
 This package provides interactive visualization using OpenGL for datasets
 loaded in yt.  It is written to provide both scripting and interactive access.
 
 * Free software: BSD license
 * Documentation: https://yt-idv.readthedocs.io.
+* Source code: https://github.com/yt-project/yt_idv
 
 ![example of using yt_idv](https://i.imgur.com/Q4XPNZw.gif)
 
 ## Features
 
 * Rendering of multi-resolution (AMR) volume data
 * Rendering of unstructured mesh data
```

### Comparing `yt_idv-0.3.0/README.md` & `yt_idv-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # interactive volume rendering for yt
 
 [![](https://img.shields.io/pypi/v/yt_idv.svg)](https://pypi.python.org/pypi/yt_idv)
 
 [![Doc Status](https://readthedocs.org/projects/yt-idv/badge/?version=latest)](https://yt-idv.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/yt-project/yt_idv/main.svg)](https://results.pre-commit.ci/latest/github/yt-project/yt_idv/main)
+[![Run tests](https://github.com/yt-project/yt_idv/actions/workflows/build-test.yaml/badge.svg)](https://github.com/yt-project/yt_idv/actions/workflows/build-test.yaml)
 
 This package provides interactive visualization using OpenGL for datasets
 loaded in yt.  It is written to provide both scripting and interactive access.
 
 * Free software: BSD license
 * Documentation: https://yt-idv.readthedocs.io.
+* Source code: https://github.com/yt-project/yt_idv
 
 ![example of using yt_idv](https://i.imgur.com/Q4XPNZw.gif)
 
 ## Features
 
 * Rendering of multi-resolution (AMR) volume data
 * Rendering of unstructured mesh data
```

### Comparing `yt_idv-0.3.0/docs/Makefile` & `yt_idv-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/docs/conf.py` & `yt_idv-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/docs/examples.rst` & `yt_idv-0.3.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/docs/installation.rst` & `yt_idv-0.3.1/docs/installation.rst`

 * *Files 27% similar despite different names*

```diff
@@ -43,9 +43,30 @@
 Once you have a copy of the source, you can install it with:
 
 .. code-block:: console
 
     $ python setup.py install
 
 
+Extra steps for linux
+---------------------
+
+A number of linux distros (Ubuntu 21+, Fedora 34+) have switched the default graphics backend from Xorg to Wayland.
+
+To Use yt_idv on these linux distributions, you may need enforce Xorg usage, which you can do in several ways:
+
+1. Log into an Xorg session. For Ubuntu, you can still select to launch an Xorg session on the login screen (see `here <https://askubuntu.com/a/961345>`_).
+
+OR
+
+2. Set the ``PYOPENGL_PLATFORM`` environment variable to ``"gdx"``.  In a bash shell:
+
+.. code-block:: console
+
+   $ export PYOPENGL_PLATFORM="gdx"
+
+To avoid having to set this variable each time, you can add the above line to your ``.bashrc`` or ``.bash_aliases`` file.
+
+See `Issue 81 <https://github.com/yt-project/yt_idv/issues/81>`_ for more information.
+
 .. _Github repo: https://github.com/yt-project/yt_idv
 .. _tarball: https://github.com/yt-project/yt_idv/tarball/master
```

### Comparing `yt_idv-0.3.0/docs/make.bat` & `yt_idv-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/docs/scene.rst` & `yt_idv-0.3.1/docs/scene.rst`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/docs/usage.rst` & `yt_idv-0.3.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/docs/yt_idv.rendering_contexts.rst` & `yt_idv-0.3.1/docs/yt_idv.rendering_contexts.rst`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 .. autofunction:: yt_idv.rendering_contexts.render_context
 
 .. autoclass:: yt_idv.rendering_contexts.pyglet_context.PygletRenderingContext
    :members:
    :undoc-members:
    :show-inheritance:
 
-.. autoclass:: yt_idv.rendering_contexts.egl_context.OSMesaRenderingContext
+.. autoclass:: yt_idv.rendering_contexts.osmesa_context.OSMesaRenderingContext
    :members:
    :undoc-members:
    :show-inheritance:
 
 .. autoclass:: yt_idv.rendering_contexts.egl_context.EGLRenderingContext
    :members:
    :undoc-members:
```

### Comparing `yt_idv-0.3.0/examples/amr_volume_rendering_with_curves.py` & `yt_idv-0.3.1/examples/amr_volume_rendering_with_curves.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,22 +37,24 @@
 sg = rc.add_scene(ds, "density", no_ghost=True)
 
 
 # add a single streamline as a single curve
 curved = CurveData()
 curved.add_data(streamlines.streamlines[0])
 curve_render = CurveRendering(data=curved, curve_rgba=(1.0, 0.0, 0.0, 1.0))
+curve_render.display_name = "single streamline"
 rc.scene.data_objects.append(curved)
 rc.scene.components.append(curve_render)
 
 # add the remaining streamlines as a collection of curves
 curve_collection = CurveCollection()
 for stream in streamlines.streamlines[1:]:
     stream = stream[np.all(stream != 0.0, axis=1)]
     curve_collection.add_curve(stream)
 curve_collection.add_data()  # call add_data() after done adding curves
 
 cc_render = CurveCollectionRendering(data=curve_collection)
+cc_render.display_name = "multiple streamlines"
 rc.scene.data_objects.append(curve_collection)
 rc.scene.components.append(cc_render)
 
 rc.run()
```

### Comparing `yt_idv-0.3.0/examples/grid_positions.py` & `yt_idv-0.3.1/examples/grid_positions.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/examples/hires_galaxy.py` & `yt_idv-0.3.1/examples/hires_galaxy.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/examples/idv_widget.ipynb` & `yt_idv-0.3.1/examples/idv_widget.ipynb`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/examples/mesh_render.py` & `yt_idv-0.3.1/examples/mesh_render.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/examples/octree_volume_rendering.py` & `yt_idv-0.3.1/examples/octree_volume_rendering.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 dd = ds.all_data()
 
 rc = yt_idv.render_context(height=800, width=800, gui=True)
 sg = rc.add_scene(ds, None, no_ghost=True)
 
 odata = OctreeBlockCollection(data_source=dd)
 odata.add_data("density")
-oren = OctreeBlockRendering(data=odata)
+oren = OctreeBlockRendering(data=odata, display_name="density")
 
 sg.data_objects.append(odata)
 sg.components.append(oren)
 
 rc.run()
```

### Comparing `yt_idv-0.3.0/examples/sph_rendering.py` & `yt_idv-0.3.1/examples/sph_rendering.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/setup.cfg` & `yt_idv-0.3.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = yt_idv
-version = 0.3.0
+version = 0.3.1
 description = Interactive Volume Rendering for yt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yt-project/yt_idv
 author = Matthew Turk
 author_email = matthewturk@gmail.com
 license = BSD-3-Clause
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `yt_idv-0.3.0/tests/test_yt_idv.py` & `yt_idv-0.3.1/tests/test_yt_idv.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,7 +107,12 @@
     image_store(osmesa_empty)
     text.origin = (0.0, 0.0)
     text.text = "S 1.0"
     image_store(osmesa_empty)
     text.text = "S 2.0"
     text.scale = 2.0
     image_store(osmesa_empty)
+
+
+def test_isocontour_functionality(osmesa_fake_amr, image_store):
+    osmesa_fake_amr.scene.components[0].render_method = "isocontours"
+    image_store(osmesa_fake_amr)
```

### Comparing `yt_idv-0.3.0/yt_idv/cameras/base_camera.py` & `yt_idv-0.3.1/yt_idv/cameras/base_camera.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/cameras/trackball_camera.py` & `yt_idv-0.3.1/yt_idv/cameras/trackball_camera.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/constants.py` & `yt_idv-0.3.1/yt_idv/constants.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/opengl_support.py` & `yt_idv-0.3.1/yt_idv/opengl_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,15 @@
     def _viewport_default(self):
         # origin_x, origin_y, width, height
         return tuple(GL.glGetIntegerv(GL.GL_VIEWPORT))
 
     @traitlets.observe("viewport")
     def _viewport_changed(self, change):
         # we just need to disable the initialized value here
-        self.initalized = False
+        self.initialized = False
 
     @traitlets.default("fb_id")
     def _fb_id_default(self):
         return GL.glGenFramebuffers(1)
 
     @traitlets.default("rb_id")
     def _rb_id_default(self):
```

### Comparing `yt_idv-0.3.0/yt_idv/rendering_contexts/base_offscreen.py` & `yt_idv-0.3.1/yt_idv/rendering_contexts/base_offscreen.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/rendering_contexts/egl_context.py` & `yt_idv-0.3.1/yt_idv/rendering_contexts/egl_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 from OpenGL import EGL, GL
 
 from .base_offscreen import OffscreenRenderingContext
 
 
 class EGLRenderingContext(OffscreenRenderingContext):
-    """Rendering context using EGL (experimental)
+    """Offscreen rendering context using EGL (experimental)
 
     Parameters
     ----------
     width : int, optional
         The width of the off-screen buffer window.  For performance reasons it
         is recommended to use values that are natural powers of 2.
```

### Comparing `yt_idv-0.3.0/yt_idv/rendering_contexts/osmesa_context.py` & `yt_idv-0.3.1/yt_idv/rendering_contexts/osmesa_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 import numpy as np
 from OpenGL import GL, osmesa
 
 from .base_offscreen import OffscreenRenderingContext
 
 
 class OSMesaRenderingContext(OffscreenRenderingContext):
-    """Rendering context using OSMesa (experimental)"""
+    """Offscreen rendering context using OSMesa (experimental)
+
+    Parameters
+    ----------
+    width : int, optional
+        The width of the off-screen buffer window.  For performance reasons it
+        is recommended to use values that are natural powers of 2.
+
+    height : int, optional
+        The height of the off-screen buffer window.  For performance reasons it
+        it is recommended to use values that are natural powers of 2.
+
+    """
 
     def __init__(self, width=1024, height=1024, **kwargs):
         super().__init__(width, height, **kwargs)
         self.osmesa = osmesa
         # Now we create our necessary bits.
         config_attribs = np.array(
             [
```

### Comparing `yt_idv-0.3.0/yt_idv/rendering_contexts/pyglet_context.py` & `yt_idv-0.3.1/yt_idv/rendering_contexts/pyglet_context.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/scene_annotations/block_outline.py` & `yt_idv-0.3.1/yt_idv/scene_annotations/block_outline.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/scene_annotations/box.py` & `yt_idv-0.3.1/yt_idv/scene_annotations/box.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/scene_annotations/grid_outlines.py` & `yt_idv-0.3.1/yt_idv/scene_annotations/grid_outlines.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/scene_annotations/text.py` & `yt_idv-0.3.1/yt_idv/scene_annotations/text.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/scene_components/base_component.py` & `yt_idv-0.3.1/yt_idv/scene_components/base_component.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,16 +25,19 @@
 class SceneComponent(traitlets.HasTraits):
     data = traitlets.Instance(SceneData)
     base_quad = traitlets.Instance(SceneData)
     name = "undefined"
     priority = traitlets.CInt(0)
     visible = traitlets.Bool(True)
     use_db = traitlets.Bool(False)  # use depth buffer
-    iso_tolerance = traitlets.CFloat(0.025)
-    iso_layers = traitlets.List()
+    iso_tolerance = traitlets.CFloat(-1)  # the tolerance for finding isocontours
+    iso_tol_is_pct = traitlets.Bool(False)  # if True, the tolerance is a fraction
+    iso_log = traitlets.Bool(True)  # if True, iso values are base 10 exponents
+    iso_layers = traitlets.List()  # the target values for isocontours
+    iso_layers_alpha = traitlets.List()  # the transparency of isocontours
     display_bounds = traitlets.Tuple(
         traitlets.CFloat(),
         traitlets.CFloat(),
         traitlets.CFloat(),
         traitlets.CFloat(),
         default_value=(0.0, 1.0, 0.0, 1.0),
     )
@@ -50,14 +53,16 @@
     colormap = traitlets.Instance(ColormapTexture)
     _program1 = traitlets.Instance(ShaderProgram, allow_none=True)
     _program2 = traitlets.Instance(ShaderProgram, allow_none=True)
     _program1_invalid = True
     _program2_invalid = True
     _cmap_bounds_invalid = True
 
+    display_name = traitlets.Unicode(allow_none=True)
+
     # These attributes are
     cmap_min = traitlets.CFloat(None, allow_none=True)
     cmap_max = traitlets.CFloat(None, allow_none=True)
     cmap_log = traitlets.Bool(True)
     scale = traitlets.CFloat(1.0)
 
     @traitlets.observe("display_bounds")
@@ -73,31 +78,18 @@
         new_height = change["new"][3] - change["new"][2]
         if old_width != new_width or old_height != new_height:
             self.fb = Framebuffer()
 
     def render_gui(self, imgui, renderer, scene):
         changed, self.visible = imgui.checkbox("Visible", self.visible)
         _, self.use_db = imgui.checkbox("Depth Buffer", self.use_db)
-        changed = changed or _
         _ = add_popup_help(
             imgui, "If checked, will render the depth buffer of the current view."
         )
         changed = changed or _
-        _, self.iso_tolerance = imgui.slider_float(
-            "Isocontour Tolerance", self.iso_tolerance, 0.0, 0.1
-        )
-        changed = changed or _
-
-        if self.render_method == "isocontours":
-            if imgui.button("Add Layer"):
-                if len(self.iso_layers) < 32:
-                    changed = True
-                    self.iso_layers.append(0.0)
-            _ = self._construct_isolayer_table(imgui)
-            changed = changed or _
 
         if imgui.button("Recompile Shader"):
             changed = self._recompile_shader()
         _, cmap_index = imgui.listbox(
             "Colormap", _cmaps.index(self.colormap.colormap_name), _cmaps
         )
         if _:
@@ -113,16 +105,40 @@
         changed = changed or _
         if imgui.button("Reset Colorbounds"):
             self._cmap_bounds_invalid = True
             changed = True
         _ = add_popup_help(imgui, "Click to reset the colorbounds of the current view.")
         changed = changed or _
 
+        if self.render_method == "isocontours":
+            _ = self._render_isolayer_inputs(imgui)
+            changed = changed or _
+
         return changed
 
+    @traitlets.observe("iso_log")
+    def _switch_iso_log(self, change):
+        # if iso_log, then the user is setting 10**x, otherwise they are setting
+        # x directly. So when toggling this checkbox we convert the existing
+        # values between the two forms.
+        if change["old"]:
+            # if True, we were taking the log, but now are not:
+            self.iso_tolerance = 10**self.iso_tolerance
+            new_iso_layers = [10**iso_val for iso_val in self.iso_layers]
+            self.iso_layers = new_iso_layers
+        else:
+            # we were not taking the log but now we are, so convert to the exponent
+            self.iso_tolerance = np.log10(self.iso_tolerance)
+            new_iso_layers = [np.log10(iso_val) for iso_val in self.iso_layers]
+            self.iso_layers = new_iso_layers
+
+    @traitlets.default("display_name")
+    def _default_display_name(self):
+        return self.name
+
     @traitlets.default("render_method")
     def _default_render_method(self):
         return default_shader_combos[self.name]
 
     @traitlets.observe("render_method")
     def _change_render_method(self, change):
         new_combo = component_shaders[self.name][change["new"]]
@@ -135,14 +151,15 @@
 
     @traitlets.observe("render_method")
     def _add_initial_isolayer(self, change):
         # this adds an initial isocontour entry when the render method
         # switches to isocontours and if there are no layers yet.
         if change["new"] == "isocontours" and len(self.iso_layers) == 0:
             self.iso_layers.append(0.0)
+            self.iso_layers_alpha.append(1.0)
 
     @traitlets.default("fb")
     def _fb_default(self):
         return Framebuffer()
 
     @traitlets.observe("fragment_shader")
     def _change_fragment(self, change):
@@ -232,33 +249,39 @@
             # The vertex shader will always be the same.
             # The fragment shader will change based on whether we are
             # colormapping or not.
             self._program2 = ShaderProgram(self.colormap_vertex, self.colormap_fragment)
             self._program2_invalid = False
         return self._program2
 
+    def _set_iso_uniforms(self, p):
+        # these could be handled better by watching traits.
+        p._set_uniform("iso_num_layers", int(len(self.iso_layers)))
+        isolayervals = self._get_sanitized_iso_layers()
+        p._set_uniform("iso_layers", isolayervals)
+        p._set_uniform("iso_layer_tol", self._get_sanitized_iso_tol())
+        avals = np.zeros((32,), dtype="float32")
+        avals[: len(self.iso_layers)] = np.array(self.iso_layers_alpha)
+        p._set_uniform("iso_alphas", avals)
+        p._set_uniform("iso_min", float(self.data.min_val))
+        p._set_uniform("iso_max", float(self.data.max_val))
+
     def run_program(self, scene):
         # Store this info, because we need to render into a framebuffer that is the
         # right size.
         x0, y0, w, h = GL.glGetIntegerv(GL.GL_VIEWPORT)
         GL.glViewport(0, 0, w, h)
         if not self.visible:
             return
         with self.fb.bind(True):
             with self.program1.enable() as p:
                 scene.camera._set_uniforms(scene, p)
                 self._set_uniforms(scene, p)
-                p._set_uniform("iso_tolerance", float(self.iso_tolerance))
-                p._set_uniform("iso_num_layers", int(len(self.iso_layers)))
-                v = np.zeros(32, dtype="float32")
-                v[: len(self.iso_layers)] = self._get_sanitized_iso_layers()
-                p._set_uniform("iso_layers", v)
-                p._set_uniform("iso_log", bool(self.cmap_log))
-                p._set_uniform("iso_min", float(self.data.min_val))
-                p._set_uniform("iso_max", float(self.data.max_val))
+                if self.render_method == "isocontours":
+                    self._set_iso_uniforms(p)
                 with self.data.vertex_array.bind(p):
                     self.draw(scene, p)
 
         if self._cmap_bounds_invalid:
             self._reset_cmap_bounds()
 
         with self.colormap.bind(0):
@@ -279,16 +302,72 @@
                             # the framebuffer
                             GL.glViewport(x0, y0, w, h)
                             GL.glDrawArrays(GL.GL_TRIANGLES, 0, 6)
 
     def draw(self, scene, program):
         raise NotImplementedError
 
-    def _get_sanitized_iso_layers(self):
-        return self.iso_layers
+    def _get_sanitized_iso_layers(self, normalize=True):
+        # returns an array of the isocontour layer values, padded with 0s out
+        # to max number of contours (32).
+        iso_vals = np.asarray(self.iso_layers)
+        if self.iso_log:
+            iso_vals = 10**iso_vals
+
+        if normalize:
+            iso_vals = self.data._normalize_by_min_max(iso_vals)
+
+        full_array = np.zeros(32, dtype="float32")
+        full_array[: len(self.iso_layers)] = iso_vals
+        return full_array
+
+    def _get_sanitized_iso_tol(self):
+        # isocontour selection conditions:
+        #
+        # absolute difference
+        #   d - c <= eps
+        # or percent difference
+        #   (d - c) / c * 100 <= eps_pct
+        #
+        # where d is a raw data value, c is the target isocontour, eps
+        # is an absolute difference, eps_f is a percent difference
+        #
+        # The data textures available on the shaders are normalized values:
+        #   d_ = (d - min) / (max - min)
+        # where max and min are the global min and max values across the entire
+        # volume (e.g., over all blocks, not within a block)
+        #
+        # So in terms of normalized values, the absoulte difference condition
+        # becomes
+        #   d_ - c_ <= eps / (max - min)
+        # where c_ is the target value normalized in the same way as d_.
+        #
+        # And the percent difference becomes
+        #   (d_ - c_) * (max - min) / c * 100 <= eps_pct
+        #       or
+        #   d_ - c_ <= eps_pct / 100 * c / (max - min)
+        # so that the allowed tolerance is a function of the raw target value
+        # and so will vary with each layer.
+
+        if self.iso_log:
+            # the tol value is an exponent, convert
+            tol = 10 ** float(self.iso_tolerance)
+        else:
+            tol = float(self.iso_tolerance)
+        # always normalize tolerance
+        tol = tol / self.data.val_range
+
+        if self.iso_tol_is_pct:
+            # tolerance depends on the layer value
+            tol = tol * 0.01
+            raw_layers = self._get_sanitized_iso_layers(normalize=False)
+            final_tol = raw_layers * tol
+        else:
+            final_tol = np.full((32,), tol, dtype="float32")
+        return final_tol
 
     def _recompile_shader(self) -> bool:
         # removes existing shaders, invalidates shader programs
         shaders = (
             "vertex_shader",
             "geometry_shader",
             "fragment_shader",
@@ -298,27 +377,76 @@
         for shader_name in shaders:
             s = getattr(self, shader_name, None)
             if s:
                 s.delete_shader()
         self._program1_invalid = self._program2_invalid = True
         return True
 
+    def _render_isolayer_inputs(self, imgui) -> bool:
+        changed = False
+        if imgui.tree_node("Isocontours"):
+            _, self.iso_log = imgui.checkbox("set exponent", self.iso_log)
+            _ = add_popup_help(
+                imgui, "If checked, will treat isocontour values as base-10 exponents."
+            )
+            changed = changed or _
+
+            imgui.columns(2, "iso_tol_cols", False)
+
+            _, self.iso_tolerance = imgui.input_float(
+                "tol",
+                self.iso_tolerance,
+                flags=imgui.INPUT_TEXT_ENTER_RETURNS_TRUE,
+            )
+            _ = add_popup_help(imgui, "The tolerance for selecting an isocontour.")
+            changed = changed or _
+
+            imgui.next_column()
+            _, self.iso_tol_is_pct = imgui.checkbox("%", self.iso_tol_is_pct)
+            _ = add_popup_help(imgui, "If checked, the tolerance is a percent.")
+            changed = changed or _
+            imgui.columns(1)
+
+            if imgui.button("Add Layer"):
+                if len(self.iso_layers) < 32:
+                    changed = True
+                    self.iso_layers.append(0.0)
+                    self.iso_layers_alpha.append(1.0)
+            _ = self._construct_isolayer_table(imgui)
+            changed = changed or _
+            imgui.tree_pop()
+        return changed
+
     def _construct_isolayer_table(self, imgui) -> bool:
-        imgui.columns(2, "iso_layers_cols", False)
+        imgui.columns(3, "iso_layers_cols", False)
+
         i = 0
         changed = False
         while i < len(self.iso_layers):
             _, self.iso_layers[i] = imgui.input_float(
-                "Layer " + str(i + 1),
+                f"Layer {i + 1}",
                 self.iso_layers[i],
                 flags=imgui.INPUT_TEXT_ENTER_RETURNS_TRUE,
             )
+            _ = add_popup_help(imgui, "The value of the isocontour layer.")
+            changed = changed or _
+
+            imgui.next_column()
+            _, self.iso_layers_alpha[i] = imgui.input_float(
+                f"alpha {i}",
+                self.iso_layers_alpha[i],
+                flags=imgui.INPUT_TEXT_ENTER_RETURNS_TRUE,
+            )
+            _ = add_popup_help(imgui, "The opacity of the isocontour layer.")
+            changed = changed or _
+
             imgui.next_column()
             if imgui.button("Remove##rl" + str(i + 1)):
                 self.iso_layers.pop(i)
+                self.iso_layers_alpha.pop(i)
                 i -= 1
                 _ = True
             changed = changed or _
             imgui.next_column()
             i += 1
         imgui.columns(1)
```

### Comparing `yt_idv-0.3.0/yt_idv/scene_components/blocks.py` & `yt_idv-0.3.1/yt_idv/scene_components/blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from math import ceil, floor, log10
+from math import ceil, floor
 
 import numpy as np
 import traitlets
 from OpenGL import GL
 
 from yt_idv.gui_support import add_popup_help
 from yt_idv.opengl_support import TransferFunctionTexture
@@ -137,31 +137,15 @@
                 with tex.bind(target=0):
                     with bitmap_tex.bind(target=1):
                         GL.glDrawArrays(GL.GL_POINTS, tex_ind * each, each)
 
     def _set_uniforms(self, scene, shader_program):
         shader_program._set_uniform("box_width", self.box_width)
         shader_program._set_uniform("sample_factor", self.sample_factor)
-        shader_program._set_uniform("ds_tex", 0)
+        shader_program._set_uniform("ds_tex", np.array([0, 0, 0, 0, 0, 0]))
         shader_program._set_uniform("bitmap_tex", 1)
         shader_program._set_uniform("tf_tex", 2)
         shader_program._set_uniform("tf_min", self.tf_min)
         shader_program._set_uniform("tf_max", self.tf_max)
         shader_program._set_uniform("tf_log", float(self.tf_log))
         shader_program._set_uniform("slice_normal", np.array(self.slice_normal))
         shader_program._set_uniform("slice_position", np.array(self.slice_position))
-
-    def _get_sanitized_iso_layers(self):
-        # return the sanitized layers
-
-        # pull extrema from `BlockCollection`, these are extrema across all blocks
-        data_min = self.data.min_val
-        data_max = self.data.max_val
-        if self.cmap_log:
-            data_min = log10(data_min)
-            data_max = log10(data_max)
-
-        # apply the same scaling as in `self.data._load_textures()`
-        normalized_isovals = [
-            (iso_val - data_min) / (data_max - data_min) for iso_val in self.iso_layers
-        ]
-        return normalized_isovals
```

### Comparing `yt_idv-0.3.0/yt_idv/scene_components/curves.py` & `yt_idv-0.3.1/yt_idv/scene_components/curves.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class CurveRendering(SceneComponent):
     """
     A class that renders user-specified curves.
     """
 
     name = "curve_rendering"
-    data = traitlets.Instance(CurveData)
+    data = traitlets.Instance(CurveData, help="The curve data.")
     line_width = traitlets.CFloat(1.0)
     curve_rgba = traitlets.Tuple((1.0, 1.0, 1.0, 1.0), trait=traitlets.CFloat())
     priority = 10
 
     def render_gui(self, imgui, renderer, scene):
         changed, self.visible = imgui.checkbox("Visible", self.visible)
```

### Comparing `yt_idv-0.3.0/yt_idv/scene_components/octree_blocks.py` & `yt_idv-0.3.1/yt_idv/scene_components/octree_blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,13 +123,13 @@
                             GL.GL_TRIANGLE_STRIP, 0, each, shape, start
                         )
                         start += shape
 
     def _set_uniforms(self, scene, shader_program):
         shader_program._set_uniform("box_width", self.box_width)
         shader_program._set_uniform("sample_factor", self.sample_factor)
-        shader_program._set_uniform("ds_tex", 0)
+        shader_program._set_uniform("ds_tex", np.array([0, 0, 0, 0, 0, 0]))
         shader_program._set_uniform("bitmap_tex", 1)
         shader_program._set_uniform("tf_tex", 2)
         shader_program._set_uniform("tf_min", self.tf_min)
         shader_program._set_uniform("tf_max", self.tf_max)
         shader_program._set_uniform("tf_log", float(self.tf_log))
```

### Comparing `yt_idv-0.3.0/yt_idv/scene_components/particles.py` & `yt_idv-0.3.1/yt_idv/scene_components/particles.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/scene_components/rgba.py` & `yt_idv-0.3.1/yt_idv/scene_components/rgba.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/scene_components/sph_particles.py` & `yt_idv-0.3.1/yt_idv/scene_components/sph_particles.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/scene_data/block_collection.py` & `yt_idv-0.3.1/yt_idv/scene_data/block_collection.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,18 +75,19 @@
             self.max_val = self.max_val.d
 
         LE = np.array([b.LeftEdge for i, b in self.blocks.values()]).min(axis=0)
         RE = np.array([b.RightEdge for i, b in self.blocks.values()]).max(axis=0)
         self.diagonal = np.sqrt(((RE - LE) ** 2).sum())
         # Now we set up our buffer
         vert = np.array(vert, dtype="f4")
-        dx = np.array(dx, dtype="f4")
-        le = np.array(le, dtype="f4")
-        re = np.array(re, dtype="f4")
-
+        units = self.data_source.ds.units
+        ratio = (units.code_length / units.unitary).base_value
+        dx = np.array(dx, dtype="f4") * ratio
+        le = np.array(le, dtype="f4") * ratio
+        re = np.array(re, dtype="f4") * ratio
         self.vertex_array.attributes.append(
             VertexAttribute(name="model_vertex", data=vert)
         )
         self.vertex_array.attributes.append(VertexAttribute(name="in_dx", data=dx))
         self.vertex_array.attributes.append(
             VertexAttribute(name="in_left_edge", data=le)
         )
@@ -118,16 +119,15 @@
 
     def _load_textures(self):
         for block_id in sorted(self.blocks):
             vbo_i, block = self.blocks[block_id]
             n_data = np.abs(block.my_data[0]).copy(order="F").astype("float32").d
             # Avoid setting to NaNs
             if self.max_val != self.min_val:
-                n_data = (n_data - self.min_val) / (
-                    self.max_val - self.min_val
-                )  # * self.diagonal)
+                n_data = self._normalize_by_min_max(n_data)
+
             data_tex = Texture3D(data=n_data)
             bitmap_tex = Texture3D(
                 data=block.source_mask * 255, min_filter="nearest", mag_filter="nearest"
             )
             self.texture_objects[vbo_i] = data_tex
             self.bitmap_objects[vbo_i] = bitmap_tex
```

### Comparing `yt_idv-0.3.0/yt_idv/scene_data/box.py` & `yt_idv-0.3.1/yt_idv/scene_data/box.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/scene_data/curve.py` & `yt_idv-0.3.1/yt_idv/scene_data/curve.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,24 +3,38 @@
 from traittypes import Array
 
 from yt_idv.opengl_support import VertexArray, VertexAttribute
 from yt_idv.scene_data.base_data import SceneData
 
 
 class CurveData(SceneData):
+    """
+    Data component for a single curve.
+    """
+
     name = "curve_data"
     data = Array()
     n_vertices = traitlets.CInt()
 
     @traitlets.default("vertex_array")
     def _default_vertex_array(self):
         va = VertexArray(name="vertices")
         return va
 
     def add_data(self, curve):
+        """
+        add curve data
+
+        Parameters
+        ----------
+        curve: ArrayLike
+            an array of shape (N, 3) specifying the position (in x, y, z) of
+            N points.
+
+        """
         # curve is a collection of ndarray of points
         assert curve.shape[0] > 1  # a curve needs at least 2 points
         assert curve.shape[1] == 3  # a curve needs at least 3 dimensions
 
         # add the singleton 4th dim
         data = np.ones((curve.shape[0], 4))
         data[:, 0:3] = curve
@@ -33,19 +47,32 @@
         )
 
         self.vertex_array.indices = np.arange(0, self.n_vertices).astype("uint32")
         self.size = self.n_vertices
 
 
 class CurveCollection(CurveData):
+    """Data component for a collection of curves"""
+
     name = "curve_collection"
     data = Array()
     n_vertices = traitlets.CInt()
 
     def add_curve(self, curve):
+        """
+        add a single curve to the collection
+
+        Parameters
+        ----------
+        curve: ArrayLike
+            an array of shape (N, 3) specifying the position (in x, y, z) of
+            N points.
+
+        """
+
         # curve is a collection of ndarray of points
         assert curve.shape[0] > 1  # a curve needs at least 2 points
         assert curve.shape[1] == 3  # a curve needs at least 3 dimensions
 
         # double up the indices to use GL_LINES
         index_range = np.arange(0, curve.shape[0])
         line_indices = np.column_stack([index_range, index_range]).ravel()[1:-1]
@@ -54,14 +81,17 @@
 
         if self.data.shape:
             self.data = np.concatenate([self.data, data])
         else:
             self.data = data
 
     def add_data(self):
+        """
+        finalize the current collection of curves.
+        """
         self.n_vertices = self.data.shape[0]
 
         self.vertex_array.attributes.append(
             VertexAttribute(name="model_vertex", data=self.data.astype("f4"))
         )
 
         self.vertex_array.indices = np.arange(0, self.n_vertices).astype("uint32")
```

### Comparing `yt_idv-0.3.0/yt_idv/scene_data/line.py` & `yt_idv-0.3.1/yt_idv/scene_data/line.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/scene_data/mesh.py` & `yt_idv-0.3.1/yt_idv/scene_data/mesh.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,16 @@
             mesh_id = int(ftype[-1])
         except ValueError:
             mesh_id = 0
 
         mesh = data_source.ds.index.meshes[mesh_id - 1]
         offset = mesh._index_offset
         vertices = mesh.connectivity_coords
+        if hasattr(vertices, "in_units"):
+            vertices = vertices.in_units("unitary")
         indices = mesh.connectivity_indices - offset
 
         data = data_source[field]
 
         return triangulate_mesh(vertices, data, indices)
 
     def add_data(self, field):
```

### Comparing `yt_idv-0.3.0/yt_idv/scene_data/octree_block_collection.py` & `yt_idv-0.3.1/yt_idv/scene_data/octree_block_collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         """
         ds = self.data_source.ds
         ds.index._identify_base_chunk(self.data_source)
         left_edges = []
         right_edges = []
         dx = []
         data = []
+        units = self.data_source.ds.units
+        ratio = (units.code_length / units.unitary).base_value
 
         for obj in self.data_source._current_chunk.objs:
             bs = OctreeSubsetBlockSlice(obj, ds)
             LE = bs._fcoords[0, 0, 0, :, :].d - bs._fwidth[0, 0, 0, :, :].d * 0.5
             RE = bs._fcoords[-1, -1, -1, :, :].d + bs._fwidth[-1, -1, -1, :, :].d * 0.5
             dx.append(bs._fwidth[-1, -1, -1, :, :].d)
             left_edges.append(LE)
@@ -53,17 +55,17 @@
             data.append(
                 np.concatenate(
                     [d[:, :, :, i] for i in range(d.shape[-1])], axis=2
                 ).copy(order="C")
             )
 
         # Let's reshape ...
-        left_edges = np.concatenate(left_edges, axis=0).astype("f4")
-        right_edges = np.concatenate(right_edges, axis=0).astype("f4")
-        dx = np.concatenate(dx, axis=0).astype("f4")
+        left_edges = np.concatenate(left_edges, axis=0).astype("f4") * ratio
+        right_edges = np.concatenate(right_edges, axis=0).astype("f4") * ratio
+        dx = np.concatenate(dx, axis=0).astype("f4") * ratio
         data = np.concatenate(data, axis=-1).astype("f4")
         data = data.reshape((3, 3, -1))
 
         self.min_val = np.nanmin(data)
         self.max_val = np.nanmax(data)
 
         if hasattr(self.min_val, "in_units"):
```

### Comparing `yt_idv-0.3.0/yt_idv/scene_data/particle_positions.py` & `yt_idv-0.3.1/yt_idv/scene_data/particle_positions.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/scene_data/rgba.py` & `yt_idv-0.3.1/yt_idv/scene_data/rgba.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/scene_data/text_characters.py` & `yt_idv-0.3.1/yt_idv/scene_data/text_characters.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/scene_graph.py` & `yt_idv-0.3.1/yt_idv/scene_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 from yt_idv.scene_data.base_data import SceneData
 from yt_idv.scene_data.block_collection import BlockCollection
 from yt_idv.scene_data.box import BoxData
 from yt_idv.scene_data.text_characters import TextCharacters
 
 
 class SceneGraph(traitlets.HasTraits):
+    """
+    The SceneGraph controls the data of a rendering context
+    including the data itself as well as annotations and camera controls.
+
+    """
+
     components = traitlets.List(
         trait=traitlets.Instance(SceneComponent), default_value=[]
     )
     annotations = traitlets.List(
         trait=traitlets.Instance(SceneAnnotation), default_value=[]
     )
     data_objects = traitlets.List(trait=traitlets.Instance(SceneData), default_value=[])
```

### Comparing `yt_idv-0.3.0/yt_idv/shader_objects.py` & `yt_idv-0.3.1/yt_idv/shader_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,53 +260,61 @@
     blend_func_separate = traitlets.Tuple(
         GLValue(),
         GLValue(),
         GLValue(),
         GLValue(),
         default_value=("none", "none", "none", "none"),
     )
+    preprocessor_defs = traitlets.List(trait=traitlets.Tuple)
 
     def _get_source(self, source):
         if ";" in source:
             # This is probably safe, right?  Enh, probably.
             return source
         # What this does is concatenate multiple (if available) source files.
         # This gets around GLSL's composition issues, which means we can have
         # functions that get called at each step in a ray tracing process, for
         # instance, that can still share ray tracing code between multiple
         # files.
         if not isinstance(source, (tuple, list)):
             source = (source,)
         source = (
-            "header.inc.glsl",
-            "known_uniforms.inc.glsl",
-        ) + tuple(source)
+            ("header.inc.glsl",)
+            + tuple(self.preprocessor_defs)
+            + ("known_uniforms.inc.glsl",)
+            + tuple(source)
+        )
         full_source = []
         for fn in source:
+            if isinstance(fn, tuple):
+                full_source.append(f"#define {fn[0]} {fn[1]}\n")
+                continue
             if os.path.isfile(fn):
                 sh_directory = ""
             else:
                 sh_directory = os.path.join(os.path.dirname(__file__), "shaders")
             fn = os.path.join(sh_directory, fn)
             if not os.path.isfile(fn):
                 raise YTInvalidShaderType(fn)
             full_source.append(open(fn).read())
         return "\n\n".join(full_source)
 
     def _enable_null_shader(self):
         source = _NULL_SOURCES[self.shader_type]
         self.compile(source=source)
 
-    def compile(self, source=None, parameters=None):
+    @property
+    def defines(self):
+        return "\n".join([f"#define {var}" for var in self.preprocessor_defs])
+
+    def compile(self, source=None):
         if source is None:
             source = self.source
             if source is None:
                 raise RuntimeError
-        if parameters is not None:
-            raise NotImplementedError
         source = self._get_source(source)
         shader_type_enum = getattr(GL, f"GL_{self.shader_type.upper()}_SHADER")
         shader = GL.glCreateShader(shader_type_enum)
         # We could do templating here if we wanted.
         self.shader_source = source
         GL.glShaderSource(shader, source)
         GL.glCompileShader(shader)
```

### Comparing `yt_idv-0.3.0/yt_idv/shaders/block_outline.frag.glsl` & `yt_idv-0.3.1/yt_idv/shaders/block_outline.frag.glsl`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/shaders/default.vert.glsl` & `yt_idv-0.3.1/yt_idv/shaders/default.vert.glsl`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/shaders/grid_expand.geom.glsl` & `yt_idv-0.3.1/yt_idv/shaders/grid_expand.geom.glsl`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/shaders/grid_position.vert.glsl` & `yt_idv-0.3.1/yt_idv/shaders/grid_position.vert.glsl`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/shaders/isocontour.frag.glsl` & `yt_idv-0.3.1/yt_idv/shaders/isocontour.frag.glsl`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     ivec3 texsize = textureSize(tex, 0); // lod (mipmap level) always 0?
     return (tex_curr_pos * texsize + texture_offset) / texsize;
 }
 
 bool sample_texture(vec3 tex_curr_pos, inout vec4 curr_color, float tdelta,
                     float t, vec3 dir)
 {
-    vec3 offset_pos = get_offset_texture_position(ds_tex, tex_curr_pos);
-    vec3 tex_sample = texture(ds_tex, offset_pos).rgb;
+    vec3 offset_pos = get_offset_texture_position(ds_tex[0], tex_curr_pos);
+    vec3 tex_sample = texture(ds_tex[0], offset_pos).rgb;
     vec3 offset_bmap_pos = get_offset_texture_position(bitmap_tex, tex_curr_pos);
     float map_sample = texture(bitmap_tex, offset_bmap_pos).r;
     if ((map_sample > 0.0) && (length(curr_color.rgb) < length(tex_sample))) {
         curr_color = vec4(tex_sample, 1.0);
     }
     return bool(map_sample > 0.0);
 }
@@ -100,39 +100,37 @@
     bool ever_sampled = false;
 
     vec4 v_clip_coord;
     float f_ndc_depth;
     float depth = 1.0;
 
     ray_position = p0;
-
-    // precomputed so we don't need to call log 4 times per sample.
-    float log_iso_min = log(iso_min);
-    float log_iso_range = log(iso_max)-log(iso_min);
+    float data_value = 0.0;
     bool is_layer = false;
 
     while(t <= t1) {
         tex_curr_pos = (ray_position - left_edge) / range;  // Scale from 0 .. 1
         // But, we actually need it to be 0 + normalized dx/2 to 1 - normalized dx/2
         tex_curr_pos = (tex_curr_pos * (1.0 - ndx)) + ndx/2.0;
 
         sampled = sample_texture(tex_curr_pos, curr_color, tdelta, t, dir);
 
         if (sampled) {
             ever_sampled = true;
             v_clip_coord = projection * modelview * vec4(ray_position, 1.0);
             f_ndc_depth = v_clip_coord.z / v_clip_coord.w;
             depth = min(depth, (1.0 - 0.0) * 0.5 * f_ndc_depth + (1.0 + 0.0) * 0.5);
-            float color_len = length(curr_color.rgb);
-            if (iso_log) {
-                color_len = (log((iso_max - iso_min) * color_len + iso_min) - log_iso_min) / log_iso_range;
-            }
+            data_value = curr_color.r;  // ds texture stores data in r channel
+            // note that these texture values are already normalized. i.e.,
+            // current_data_value = (raw block value - iso_min) / (iso_range);
+            // the iso_layer values below also come in already normalized.
             for (int i = 0; i < iso_num_layers; i++) {
-                if (abs(color_len - iso_layers[i]) <= iso_tolerance) {
+                if (abs(data_value - iso_layers[i]) <= iso_layer_tol[i]) {
                     is_layer = true;
+                    curr_color.a = iso_alphas[i];
                     break;
                 }
             }
             if (is_layer) {
                 break;
             }
         }
```

### Comparing `yt_idv-0.3.0/yt_idv/shaders/known_uniforms.inc.glsl` & `yt_idv-0.3.1/yt_idv/shaders/known_uniforms.inc.glsl`

 * *Files 4% similar despite different names*

```diff
@@ -42,25 +42,23 @@
 
 // textures we tend to use
 uniform sampler1D cm_tex;
 uniform sampler2D db_tex;
 uniform sampler2D fb_tex;
 uniform sampler2D tf_tex;
 uniform sampler3D bitmap_tex;
-uniform sampler3D ds_tex;
+uniform sampler3D ds_tex[6];
 
 // ray tracing control
 uniform float sample_factor;
 
 // depth buffer control
 uniform bool use_db;
 
 // curve drawing control
 uniform vec4 curve_rgba;
 
 // isocontour control
-uniform float iso_tolerance;
 uniform int iso_num_layers;
 uniform float iso_layers[32];
-uniform bool iso_log;
-uniform float iso_min;
-uniform float iso_max;
+uniform float iso_layer_tol[32];
+uniform float iso_alphas[32];
```

### Comparing `yt_idv-0.3.0/yt_idv/shaders/max_intensity.frag.glsl` & `yt_idv-0.3.1/yt_idv/shaders/max_intensity.frag.glsl`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 bool sample_texture(vec3 tex_curr_pos, inout vec4 curr_color, float tdelta,
                     float t, vec3 dir)
 {
 
-    vec3 offset_pos = get_offset_texture_position(ds_tex, tex_curr_pos);
-    vec3 tex_sample = texture(ds_tex, offset_pos).rgb;
+    vec3 offset_pos = get_offset_texture_position(ds_tex[0], tex_curr_pos);
+    vec3 tex_sample = texture(ds_tex[0], offset_pos).rgb;
     vec3 offset_bmap_pos = get_offset_texture_position(bitmap_tex, tex_curr_pos);
     float map_sample = texture(bitmap_tex, offset_bmap_pos).r;
     if ((map_sample > 0.0) && (length(curr_color.rgb) < length(tex_sample))) {
         curr_color = vec4(tex_sample, 1.0);
     }
     return bool(map_sample > 0.0);
 }
```

### Comparing `yt_idv-0.3.0/yt_idv/shaders/octree_position.vert.glsl` & `yt_idv-0.3.1/yt_idv/shaders/octree_position.vert.glsl`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/shaders/particle.vert.glsl` & `yt_idv-0.3.1/yt_idv/shaders/particle.vert.glsl`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/shaders/particle_expand.geom.glsl` & `yt_idv-0.3.1/yt_idv/shaders/particle_expand.geom.glsl`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/shaders/projection.frag.glsl` & `yt_idv-0.3.1/yt_idv/shaders/projection.frag.glsl`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 bool sample_texture(vec3 tex_curr_pos, inout vec4 curr_color, float tdelta,
                     float t, vec3 dir) {
 
-    vec3 offset_pos = get_offset_texture_position(ds_tex, tex_curr_pos);
-    vec3 tex_sample = texture(ds_tex, offset_pos).rgb;
+    vec3 offset_pos = get_offset_texture_position(ds_tex[0], tex_curr_pos);
+    vec3 tex_sample = texture(ds_tex[0], offset_pos).rgb;
     vec3 offset_bmap_pos = get_offset_texture_position(bitmap_tex, tex_curr_pos);
     float map_sample = texture(bitmap_tex, offset_bmap_pos).r;
     if (map_sample > 0.0) {
         float val = length(tdelta * dir) * tex_sample.r + curr_color.r;
         curr_color = vec4(val, val, val, 1.0);
     }
     return bool(map_sample > 0.0);
```

### Comparing `yt_idv-0.3.0/yt_idv/shaders/ray_tracing.frag.glsl` & `yt_idv-0.3.1/yt_idv/shaders/ray_tracing.frag.glsl`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/shaders/shaderlist.yaml` & `yt_idv-0.3.1/yt_idv/shaders/shaderlist.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
       - one minus src alpha
       blend_equation: func add
     isocontour:
       info: A first pass fragment shader that renders isocontour layers.
       source: isocontour.frag.glsl
       blend_func:
       - src alpha
-      - dst alpha
+      - one minus src alpha
       blend_equation: func add
     max_intensity:
       info: A first pass fragment shader that computes Maximum Intensity Projection
         of the data. See :ref:`projection-types` for more information.
       source:
       - ray_tracing.frag.glsl
       - max_intensity.frag.glsl
```

### Comparing `yt_idv-0.3.0/yt_idv/shaders/slice_sample.frag.glsl` & `yt_idv-0.3.1/yt_idv/shaders/slice_sample.frag.glsl`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/shaders/textoverlay.vert.glsl` & `yt_idv-0.3.1/yt_idv/shaders/textoverlay.vert.glsl`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/shaders/transfer_function.frag.glsl` & `yt_idv-0.3.1/yt_idv/shaders/transfer_function.frag.glsl`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     float tp = tf_max;
     vec4 tf_sample;
 
     vec3 offset_bmap_pos = get_offset_texture_position(bitmap_tex, tex_curr_pos);
     float map_sample = texture(bitmap_tex, offset_bmap_pos).r;
     if (!(map_sample > 0.0)) return false;
 
-    vec3 offset_pos = get_offset_texture_position(ds_tex, tex_curr_pos);
-    float tex_sample = texture(ds_tex, offset_pos).r;
+    vec3 offset_pos = get_offset_texture_position(ds_tex[0], tex_curr_pos);
+    float tex_sample = texture(ds_tex[0], offset_pos).r;
 
     if (tf_log > 0.5) {
        if(tex_sample <= 0.0) return false;
        tex_sample = log(tex_sample);
        tm = log(tm);
        tp = log(tp);
     }
```

### Comparing `yt_idv-0.3.0/yt_idv/simple_gui.py` & `yt_idv-0.3.1/yt_idv/simple_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                     )
                     self.snapshot_count += 1
                 imgui.tree_pop()
             _ = self.render_camera(scene)
             changed = changed or _
             # imgui.show_style_editor()
             for i, element in enumerate(scene):
-                if imgui.tree_node(f"element {i + 1}: {element.name}"):
+                if imgui.tree_node(f"element {i + 1}: {element.display_name}"):
                     changed = changed or element.render_gui(imgui, self.renderer, scene)
                     imgui.tree_pop()
             self.window._do_update = self.window._do_update or changed
             imgui.end()
         imgui.render()
         self.renderer.render(imgui.get_draw_data())
```

### Comparing `yt_idv-0.3.0/yt_idv/traitlets_support.py` & `yt_idv-0.3.1/yt_idv/traitlets_support.py`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv/utilities.c` & `yt_idv-0.3.1/yt_idv/utilities.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "yt_idv.utilities",
         "sources": [
@@ -18,16 +18,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -87,16 +87,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1102,195 +1106,195 @@
   Py_ssize_t shape[8];
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1321,42 +1325,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2021,30 +2025,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -3490,15 +3494,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_q1.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3507,29 +3511,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3540,15 +3544,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3557,29 +3561,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3590,15 +3594,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3607,29 +3611,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3640,15 +3644,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3657,29 +3661,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3690,15 +3694,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3707,29 +3711,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3740,212 +3744,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":868
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":869
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":869
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":870
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":870
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":868
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":872
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":873
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":873
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":874
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":875
+    /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":875
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":874
+    /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":876
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":876
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":872
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":880
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3961,15 +3965,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":881
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3977,53 +3981,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":882
+      /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":882
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 882, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":881
+      /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":883
+    /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":883
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 883, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":884
+      /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 884, __pyx_L5_except_error)
@@ -4031,30 +4035,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 884, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":881
+    /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":880
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4069,15 +4073,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":886
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4093,15 +4097,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":887
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4109,53 +4113,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":888
+      /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":888
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 888, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":887
+      /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":889
+    /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":889
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 889, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":890
+      /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 890, __pyx_L5_except_error)
@@ -4163,30 +4167,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 890, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":887
+    /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":886
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4201,15 +4205,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":892
+/* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4225,15 +4229,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":893
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4241,53 +4245,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":894
+      /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":894
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 894, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":893
+      /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":895
+    /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":895
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 895, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":896
+      /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":896
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 896, __pyx_L5_except_error)
@@ -4295,30 +4299,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 896, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":893
+    /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":892
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -17916,15 +17920,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -18038,15 +18042,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -18302,15 +18306,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -18451,15 +18455,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -18644,26 +18648,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":884
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 884, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-zu6up402/lib/python3.9/site-packages/numpy/__init__.pxd":890
+  /* "../../../../../tmp/build-env-bw9kipj5/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 890, __pyx_L1_error)
@@ -19069,40 +19073,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 764, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 764, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -21913,18 +21906,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -21970,22 +21963,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -22958,15 +22951,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -23154,15 +23147,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -23426,15 +23419,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `yt_idv-0.3.0/yt_idv/utilities.pyx` & `yt_idv-0.3.1/yt_idv/utilities.pyx`

 * *Files identical despite different names*

### Comparing `yt_idv-0.3.0/yt_idv.egg-info/PKG-INFO` & `yt_idv-0.3.1/yt_idv.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-idv
-Version: 0.3.0
+Version: 0.3.1
 Summary: Interactive Volume Rendering for yt
 Home-page: https://github.com/yt-project/yt_idv
 Author: Matthew Turk
 Author-email: matthewturk@gmail.com
 License: BSD-3-Clause
 Keywords: yt_idv
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,20 +25,22 @@
 
 # interactive volume rendering for yt
 
 [![](https://img.shields.io/pypi/v/yt_idv.svg)](https://pypi.python.org/pypi/yt_idv)
 
 [![Doc Status](https://readthedocs.org/projects/yt-idv/badge/?version=latest)](https://yt-idv.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/yt-project/yt_idv/main.svg)](https://results.pre-commit.ci/latest/github/yt-project/yt_idv/main)
+[![Run tests](https://github.com/yt-project/yt_idv/actions/workflows/build-test.yaml/badge.svg)](https://github.com/yt-project/yt_idv/actions/workflows/build-test.yaml)
 
 This package provides interactive visualization using OpenGL for datasets
 loaded in yt.  It is written to provide both scripting and interactive access.
 
 * Free software: BSD license
 * Documentation: https://yt-idv.readthedocs.io.
+* Source code: https://github.com/yt-project/yt_idv
 
 ![example of using yt_idv](https://i.imgur.com/Q4XPNZw.gif)
 
 ## Features
 
 * Rendering of multi-resolution (AMR) volume data
 * Rendering of unstructured mesh data
```

### Comparing `yt_idv-0.3.0/yt_idv.egg-info/SOURCES.txt` & `yt_idv-0.3.1/yt_idv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

