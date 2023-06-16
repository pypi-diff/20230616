# Comparing `tmp/unfolded.map-sdk-1.8.1.tar.gz` & `tmp/unfolded.map-sdk-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unfolded.map-sdk-1.8.1.tar", last modified: Wed May 17 15:25:46 2023, max compression
+gzip compressed data, was "unfolded.map-sdk-1.8.2.tar", last modified: Fri Jun 16 21:09:44 2023, max compression
```

## Comparing `unfolded.map-sdk-1.8.1.tar` & `unfolded.map-sdk-1.8.2.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.857122 unfolded.map-sdk-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-17 15:25:46.857122 unfolded.map-sdk-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.833121 unfolded.map-sdk-1.8.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.833121 unfolded.map-sdk-1.8.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.837122 unfolded.map-sdk-1.8.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    25658 2023-05-17 15:22:32.000000 unfolded.map-sdk-1.8.1/docs/source/_static/embed-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.837122 unfolded.map-sdk-1.8.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/scripts/rename_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-17 15:25:46.857122 unfolded.map-sdk-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.841122 unfolded.map-sdk-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.841122 unfolded.map-sdk-1.8.1/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/api/test_dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/api/test_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/api/test_layer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/api/test_map_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.845121 unfolded.map-sdk-1.8.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/fixtures/dataset_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.833121 unfolded.map-sdk-1.8.1/tests/fixtures/raster/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.845121 unfolded.map-sdk-1.8.1/tests/fixtures/raster/collection/
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.845121 unfolded.map-sdk-1.8.1/tests/fixtures/raster/item/
--rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/fixtures/raster/item/sentinel-2-l2a.json
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/fixtures/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.845121 unfolded.map-sdk-1.8.1/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/mocks/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.833121 unfolded.map-sdk-1.8.1/tests/snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.833121 unfolded.map-sdk-1.8.1/tests/snapshots/test_html_map/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.845121 unfolded.map-sdk-1.8.1/tests/snapshots/test_html_map/test_iframe_template_rendering/
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.845121 unfolded.map-sdk-1.8.1/tests/snapshots/test_html_map/test_template_rendering/
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/snapshots/test_html_map/test_template_rendering/map.html
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/test_html_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/test_nbextension_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/test_subclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/test_widget_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.845121 unfolded.map-sdk-1.8.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tests/utils/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.833121 unfolded.map-sdk-1.8.1/unfolded/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.849121 unfolded.map-sdk-1.8.1/unfolded/map_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.849121 unfolded.map-sdk-1.8.1/unfolded/map_sdk/_poll_v56/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/_poll_v56/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/_poll_v56/_async_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/_poll_v56/_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/_poll_v56/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.853122 unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/create_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/event_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17979 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/layer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21910 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/map_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/colab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.853122 unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-17 15:25:46.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.853122 unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-17 15:25:46.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/4.c6720f8df23b707b3655.js
--rw-r--r--   0 runner    (1001) docker     (123)    17474 2023-05-17 15:25:46.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/480.232c2d64243946e2f053.js
--rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-05-17 15:25:46.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/568.9ca15b62cee6758f82c8.js
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-17 15:25:46.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/747.488cf0ee36d815959581.js
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-17 15:25:46.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/remoteEntry.7fae4787113bb153082a.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-17 15:25:44.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-17 15:25:46.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.853122 unfolded.map-sdk-1.8.1/unfolded/map_sdk/map/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/map/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/map/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/map/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.853122 unfolded.map-sdk-1.8.1/unfolded/map_sdk/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-05-17 15:25:39.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/nbextension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.853122 unfolded.map-sdk-1.8.1/unfolded/map_sdk/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/templates/html_map_sdk.j2
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/transfer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.857122 unfolded.map-sdk-1.8.1/unfolded/map_sdk/transport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/transport/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/transport/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/transport/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.857122 unfolded.map-sdk-1.8.1/unfolded/map_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/utils/action_type_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/utils/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded/map_sdk/utils/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:25:46.849121 unfolded.map-sdk-1.8.1/unfolded.map_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-17 15:25:46.000000 unfolded.map-sdk-1.8.1/unfolded.map_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-17 15:25:46.000000 unfolded.map-sdk-1.8.1/unfolded.map_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:25:46.000000 unfolded.map-sdk-1.8.1/unfolded.map_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-17 15:25:46.000000 unfolded.map-sdk-1.8.1/unfolded.map_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 15:25:46.000000 unfolded.map-sdk-1.8.1/unfolded.map_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/unfolded.map_sdk.json
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-17 15:15:28.000000 unfolded.map-sdk-1.8.1/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.856611 unfolded.map-sdk-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-16 21:09:44.856611 unfolded.map-sdk-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.832611 unfolded.map-sdk-1.8.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.832611 unfolded.map-sdk-1.8.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.836611 unfolded.map-sdk-1.8.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    25658 2023-06-16 21:05:07.000000 unfolded.map-sdk-1.8.2/docs/source/_static/embed-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.836611 unfolded.map-sdk-1.8.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/scripts/rename_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-16 21:09:44.856611 unfolded.map-sdk-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.840611 unfolded.map-sdk-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.840611 unfolded.map-sdk-1.8.2/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/api/test_dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/api/test_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/api/test_layer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/api/test_map_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.840611 unfolded.map-sdk-1.8.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/fixtures/dataset_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.832611 unfolded.map-sdk-1.8.2/tests/fixtures/raster/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.840611 unfolded.map-sdk-1.8.2/tests/fixtures/raster/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.840611 unfolded.map-sdk-1.8.2/tests/fixtures/raster/item/
+-rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/fixtures/raster/item/sentinel-2-l2a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/fixtures/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.840611 unfolded.map-sdk-1.8.2/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/mocks/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.832611 unfolded.map-sdk-1.8.2/tests/snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.832611 unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.844611 unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/test_iframe_template_rendering/
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.844611 unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/test_template_rendering/
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/test_template_rendering/map.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/test_html_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/test_nbextension_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/test_subclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/test_widget_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.844611 unfolded.map-sdk-1.8.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tests/utils/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.832611 unfolded.map-sdk-1.8.2/unfolded/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.844611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.844611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/_async_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.848611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/create_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/event_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17979 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/layer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21910 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/map_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/colab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.848611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.852611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/4.2f5ebe11a5669cad3275.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17474 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/480.25ce0490671eeeb9f120.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/568.caff7d3d72d44ec36b9e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/747.488cf0ee36d815959581.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/remoteEntry.1f1edfc58c4b1a509424.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-16 21:09:42.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.852611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.852611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-06-16 21:09:38.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.852611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/templates/html_map_sdk.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/transfer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.856611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.856611 unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/action_type_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:09:44.844611 unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 21:09:44.000000 unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/unfolded.map_sdk.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-16 20:58:32.000000 unfolded.map-sdk-1.8.2/webpack.config.js
```

### Comparing `unfolded.map-sdk-1.8.1/MANIFEST.in` & `unfolded.map-sdk-1.8.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/PKG-INFO` & `unfolded.map-sdk-1.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfolded.map-sdk
-Version: 1.8.1
+Version: 1.8.2
 Summary: Jupyter Widget for Foursquare Studio Maps
 Author: Foursquare Labs
 Author-email: info-studio@foursquare.com
 License: (c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `unfolded.map-sdk-1.8.1/docs/source/_static/embed-bundle.js` & `unfolded.map-sdk-1.8.2/docs/source/_static/embed-bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -576,15 +576,15 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.1","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.1","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+                e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.2","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.2","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
             }
         },
         n = {};
 
     function a(e) {
         var s = n[e];
         if (void 0 !== s) return s.exports;
```

### Comparing `unfolded.map-sdk-1.8.1/package.json` & `unfolded.map-sdk-1.8.2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9623015873015872%*

 * *Differences: {"'dependencies'": "{'@unfolded/map-sdk': '^1.8.2'}", "'version'": "'1.8.2'"}*

```diff
@@ -5,15 +5,15 @@
     },
     "dependencies": {
         "@aws-amplify/core": "^4.2.9",
         "@jupyter-widgets/base": "^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0",
         "@jupyterlab/rendermime-interfaces": "^1.3.0 || ^2.0.0 || ^3.0.0",
         "@lumino/application": "^1.16.0",
         "@lumino/widgets": "^1.30.0",
-        "@unfolded/map-sdk": "^1.8.1",
+        "@unfolded/map-sdk": "^1.8.2",
         "aws-sdk": "^2.988.0",
         "csstype": "^3.1.0",
         "global": "^4.3.0"
     },
     "description": "JavaScript bindings for Unfolded's Jupyter Map SDK",
     "devDependencies": {
         "@jupyterlab/builder": "^3.0.0",
@@ -76,12 +76,12 @@
         "typecheck": "tsc",
         "typescript": "yarn run -T tsc --noEmit",
         "watch": "npm-run-all -p watch:*",
         "watch:lib": "yarn run -T tsc -w",
         "watch:nbextension": "webpack --watch --mode development"
     },
     "types": "lib/index.d.ts",
-    "version": "1.8.1",
+    "version": "1.8.2",
     "volta": {
         "extends": "../../../package.json"
     }
 }
```

### Comparing `unfolded.map-sdk-1.8.1/scripts/rename_package.py` & `unfolded.map-sdk-1.8.2/scripts/rename_package.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/setup.cfg` & `unfolded.map-sdk-1.8.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.8.1
+current_version = 1.8.2
 commit = True
 message = chore(map-sdk): Bump version {current_version} → {new_version}
 tag = False
 tag_name = map-sdk/{new_version}
 
 [bdist_wheel]
 universal = 1
```

### Comparing `unfolded.map-sdk-1.8.1/setup.py` & `unfolded.map-sdk-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/_utils.py` & `unfolded.map-sdk-1.8.2/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/api/test_dataset_api.py` & `unfolded.map-sdk-1.8.2/tests/api/test_dataset_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/api/test_filter_api.py` & `unfolded.map-sdk-1.8.2/tests/api/test_filter_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/api/test_layer_api.py` & `unfolded.map-sdk-1.8.2/tests/api/test_layer_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/api/test_map_api.py` & `unfolded.map-sdk-1.8.2/tests/api/test_map_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/conftest.py` & `unfolded.map-sdk-1.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/fixtures/dataset_api.py` & `unfolded.map-sdk-1.8.2/tests/fixtures/dataset_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json` & `unfolded.map-sdk-1.8.2/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/fixtures/raster/item/sentinel-2-l2a.json` & `unfolded.map-sdk-1.8.2/tests/fixtures/raster/item/sentinel-2-l2a.json`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/fixtures/test_data.py` & `unfolded.map-sdk-1.8.2/tests/fixtures/test_data.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/mocks/transport.py` & `unfolded.map-sdk-1.8.2/tests/mocks/transport.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html` & `unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/snapshots/test_html_map/test_template_rendering/map.html` & `unfolded.map-sdk-1.8.2/tests/snapshots/test_html_map/test_template_rendering/map.html`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/test_html_map.py` & `unfolded.map-sdk-1.8.2/tests/test_html_map.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/test_serialization.py` & `unfolded.map-sdk-1.8.2/tests/test_serialization.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,16 @@
     Dataset,
     LocalDataset,
     RasterTileDataset,
     RasterTileLocalItemMetadata,
     VectorTileDataset,
     VectorTileLocalMetadata,
 )
+from unfolded.map_sdk.api.enums import ActionType
+from unfolded.map_sdk.utils.serialization import FUNCTION_MAPPING
 
 from .fixtures.dataset_api import (
     LOCAL_RESPONSE,
     RASTER_TILE_RESPONSE,
     VECTOR_TILE_RESPONSE,
 )
 
@@ -27,7 +29,21 @@
         vector_tile_dataset = parse_obj_as(Dataset, VECTOR_TILE_RESPONSE)
         assert isinstance(vector_tile_dataset, VectorTileDataset)
         assert isinstance(vector_tile_dataset.metadata, VectorTileLocalMetadata)
 
         raster_tile_dataset = parse_obj_as(Dataset, RASTER_TILE_RESPONSE)
         assert isinstance(raster_tile_dataset, RasterTileDataset)
         assert isinstance(raster_tile_dataset.metadata, RasterTileLocalItemMetadata)
+
+
+class TestFunctionMapping:
+    """Tests relating to the function mapping we maintain for the HTML map"""
+
+    def test_function_mapping(self):
+
+        for key in ActionType:
+            # Event handler actions are not translated to Javascript
+            if key not in [
+                ActionType.SET_EVENT_HANDLERS,
+                ActionType.REMOVE_EVENT_HANDLERS,
+            ]:
+                assert key in FUNCTION_MAPPING
```

### Comparing `unfolded.map-sdk-1.8.1/tests/test_subclass.py` & `unfolded.map-sdk-1.8.2/tests/test_subclass.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/test_widget_map.py` & `unfolded.map-sdk-1.8.2/tests/test_widget_map.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tests/utils/test_validators.py` & `unfolded.map-sdk-1.8.2/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/tsconfig.json` & `unfolded.map-sdk-1.8.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/__init__.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/_poll.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/_poll_v56/_async_thread.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/_async_thread.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/_poll_v56/_poll.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/_poll_v56/_poll.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/base.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/base.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/create_map.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/create_map.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/dataset_api.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/dataset_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/enums.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/enums.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/event_api.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/event_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/filter_api.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/filter_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/layer_api.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/layer_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/api/map_api.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/api/map_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/environment.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/environment.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/package.json` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9617063492063492%*

 * *Differences: {"'dependencies'": "{'@unfolded/map-sdk': '^1.8.2'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.1f1edfc58c4b1a509424.js'}}",*

 * * "'version'": "'1.8.2'"}*

```diff
@@ -5,15 +5,15 @@
     },
     "dependencies": {
         "@aws-amplify/core": "^4.2.9",
         "@jupyter-widgets/base": "^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0",
         "@jupyterlab/rendermime-interfaces": "^1.3.0 || ^2.0.0 || ^3.0.0",
         "@lumino/application": "^1.16.0",
         "@lumino/widgets": "^1.30.0",
-        "@unfolded/map-sdk": "^1.8.1",
+        "@unfolded/map-sdk": "^1.8.2",
         "aws-sdk": "^2.988.0",
         "csstype": "^3.1.0",
         "global": "^4.3.0"
     },
     "description": "JavaScript bindings for Unfolded's Jupyter Map SDK",
     "devDependencies": {
         "@jupyterlab/builder": "^3.0.0",
@@ -35,15 +35,15 @@
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.7fae4787113bb153082a.js",
+            "load": "static/remoteEntry.1f1edfc58c4b1a509424.js",
             "mimeExtension": "./mimeExtension"
         },
         "extension": "lib/plugin",
         "mimeExtension": "lib/javascript-renderer-extension.js",
         "outputDir": "unfolded/map_sdk/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
@@ -81,12 +81,12 @@
         "typecheck": "tsc",
         "typescript": "yarn run -T tsc --noEmit",
         "watch": "npm-run-all -p watch:*",
         "watch:lib": "yarn run -T tsc -w",
         "watch:nbextension": "webpack --watch --mode development"
     },
     "types": "lib/index.d.ts",
-    "version": "1.8.1",
+    "version": "1.8.2",
     "volta": {
         "extends": "../../../package.json"
     }
 }
```

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/4.c6720f8df23b707b3655.js` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/4.2f5ebe11a5669cad3275.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -29,15 +29,15 @@
                     d((o = o.apply(e, n || [])).next())
                 }))
             };
             Object.defineProperty(n, "__esModule", {
                 value: !0
             }), n.unfoldedRendererFactory = void 0;
             const s = t(832),
-                r = t(641),
+                r = t(413),
                 i = "application/geo+json",
                 a = "text/csv",
                 d = [i, a];
             class u extends s.Widget {
                 constructor(e) {
                     super(), this.addClass("unfolded-rendermime"), this.options = e
                 }
```

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/480.232c2d64243946e2f053.js` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/480.25ce0490671eeeb9f120.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -337,15 +337,15 @@
                     d((s = s.apply(e, t || [])).next())
                 }))
             };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.UnfoldedMapView = void 0;
             const a = n(565),
-                i = n(641);
+                i = n(413);
             n(204);
             const r = "unfolded-widget";
             class o extends a.DOMWidgetView {
                 initialize() {
                     return s(this, void 0, void 0, (function*() {
                         const e = {
                             style: this.model.style(),
@@ -547,11 +547,11 @@
                         n = d
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.1","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.1","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+            e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.2","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.2","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
         }
     }
 ]);
```

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/568.9ca15b62cee6758f82c8.js` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/568.caff7d3d72d44ec36b9e.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -288,15 +288,15 @@
                     d((s = s.apply(e, t || [])).next())
                 }))
             };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.UnfoldedMapView = void 0;
             const a = n(565),
-                i = n(641);
+                i = n(413);
             n(204);
             const r = "unfolded-widget";
             class o extends a.DOMWidgetView {
                 initialize() {
                     return s(this, void 0, void 0, (function*() {
                         const e = {
                             style: this.model.style(),
@@ -498,11 +498,11 @@
                         n = d
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.1","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.1","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+            e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.2","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.2","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
         }
     }
 ]);
```

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/747.488cf0ee36d815959581.js` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/747.488cf0ee36d815959581.js`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/remoteEntry.7fae4787113bb153082a.js` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/remoteEntry.1f1edfc58c4b1a509424.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,88 +1,88 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, d, l, f, s, p, c, h, v, m, b, g = {
+    var e, r, t, n, a, o, i, u, d, f, l, s, p, c, h, v, m, g, b = {
             768: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(641), t.e(568)]).then((() => () => t(568))),
-                        "./extension": () => Promise.all([t.e(641), t.e(565), t.e(480)]).then((() => () => t(480))),
-                        "./mimeExtension": () => Promise.all([t.e(641), t.e(4)]).then((() => () => t(4)))
+                        "./index": () => Promise.all([t.e(413), t.e(568)]).then((() => () => t(568))),
+                        "./extension": () => Promise.all([t.e(413), t.e(565), t.e(480)]).then((() => () => t(480))),
+                        "./mimeExtension": () => Promise.all([t.e(413), t.e(4)]).then((() => () => t(4)))
                     },
-                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    o = (e, r) => {
                         if (t.S) {
                             var n = t.S.default,
-                                o = "default";
+                                a = "default";
                             if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[o] = e, t.I(o, r)
+                            return t.S[a] = e, t.I(a, r)
                         }
                     };
                 t.d(r, {
-                    get: () => o,
-                    init: () => a
+                    get: () => a,
+                    init: () => o
                 })
             }
         },
         y = {};
 
     function w(e) {
         var r = y[e];
         if (void 0 !== r) return r.exports;
         var t = y[e] = {
             id: e,
             exports: {}
         };
-        return g[e].call(t.exports, t, t.exports, w), t.exports
+        return b[e].call(t.exports, t, t.exports, w), t.exports
     }
-    w.m = g, w.c = y, w.d = (e, r) => {
+    w.m = b, w.c = y, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        4: "c6720f8df23b707b3655",
-        480: "232c2d64243946e2f053",
+        4: "2f5ebe11a5669cad3275",
+        413: "813f632371f69f38335a",
+        480: "25ce0490671eeeb9f120",
         565: "6aa0248333a228f5539f",
-        568: "9ca15b62cee6758f82c8",
-        641: "8b842d53a48dc0d64d26",
+        568: "caff7d3d72d44ec36b9e",
         747: "488cf0ee36d815959581"
     } [e] + ".js?v=" + {
-        4: "c6720f8df23b707b3655",
-        480: "232c2d64243946e2f053",
+        4: "2f5ebe11a5669cad3275",
+        413: "813f632371f69f38335a",
+        480: "25ce0490671eeeb9f120",
         565: "6aa0248333a228f5539f",
-        568: "9ca15b62cee6758f82c8",
-        641: "8b842d53a48dc0d64d26",
+        568: "caff7d3d72d44ec36b9e",
         747: "488cf0ee36d815959581"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@unfolded/jupyter-map-sdk:", w.l = (t, n, o, a) => {
+    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@unfolded/jupyter-map-sdk:", w.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
-            if (void 0 !== o)
-                for (var d = document.getElementsByTagName("script"), l = 0; l < d.length; l++) {
-                    var f = d[l];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+            if (void 0 !== a)
+                for (var d = document.getElementsByTagName("script"), f = 0; f < d.length; f++) {
+                    var l = d[f];
+                    if (l.getAttribute("src") == t || l.getAttribute("data-webpack") == r + a) {
+                        i = l;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var s = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
-                    var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
+                    var a = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
         }
@@ -94,31 +94,31 @@
         })
     }, (() => {
         w.S = {};
         var e = {},
             r = {};
         w.I = (t, n) => {
             n || (n = []);
-            var o = r[t];
-            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
-                if (n.push(o), e[t]) return e[t];
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
+                if (n.push(a), e[t]) return e[t];
                 w.o(w.S, t) || (w.S[t] = {});
-                var a = w.S[t],
+                var o = w.S[t],
                     i = "@unfolded/jupyter-map-sdk",
                     u = (e, r, t, n) => {
-                        var o = a[e] = a[e] || {},
-                            u = o[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
+                        var a = o[e] = o[e] || {},
+                            u = a[r];
+                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     d = [];
-                return "default" === t && (u("@unfolded/jupyter-map-sdk", "1.8.1", (() => Promise.all([w.e(641), w.e(568)]).then((() => () => w(568))))), u("@unfolded/map-sdk", "1.8.1", (() => w.e(747).then((() => () => w(747)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@unfolded/jupyter-map-sdk", "1.8.2", (() => Promise.all([w.e(413), w.e(568)]).then((() => () => w(568))))), u("@unfolded/map-sdk", "1.8.2", (() => w.e(747).then((() => () => w(747)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -132,160 +132,160 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var o = e[n],
-                a = (typeof o)[0];
-            if (n >= r.length) return "u" == a;
+            var a = e[n],
+                o = (typeof a)[0];
+            if (n >= r.length) return "u" == o;
             var i = r[n],
                 u = (typeof i)[0];
-            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
-            if ("o" != a && "u" != a && o != i) return o < i;
+            if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
+            if ("o" != o && "u" != o && a != i) return a < i;
             n++
         }
-    }, o = e => {
+    }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
-        for (a = 1; a < e.length; a++) {
-            var u = e[a];
-            i.push(0 === u ? "not(" + d() + ")" : 1 === u ? "(" + d() + " || " + d() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+        for (o = 1; o < e.length; o++) {
+            var u = e[o];
+            i.push(0 === u ? "not(" + d() + ")" : 1 === u ? "(" + d() + " || " + d() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
         }
         return d();
 
         function d() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                o = n < 0;
-            o && (n = -n - 1);
+                a = n < 0;
+            a && (n = -n - 1);
             for (var i = 0, u = 1, d = !0;; u++, i++) {
-                var l, f, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(l = r[i]))[0])) return !d || ("u" == s ? u > n && !o : "" == s != o);
-                if ("u" == f) {
+                var f, l, s = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (l = (typeof(f = r[i]))[0])) return !d || ("u" == s ? u > n && !a : "" == s != a);
+                if ("u" == l) {
                     if (!d || "u" != s) return !1
                 } else if (d)
-                    if (s == f)
+                    if (s == l)
                         if (u <= n) {
-                            if (l != e[u]) return !1
+                            if (f != e[u]) return !1
                         } else {
-                            if (o ? l > e[u] : l < e[u]) return !1;
-                            l != e[u] && (d = !1)
+                            if (a ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (d = !1)
                         }
                 else if ("s" != s && "n" != s) {
-                    if (o || u <= n) return !1;
+                    if (a || u <= n) return !1;
                     d = !1, u--
                 } else {
-                    if (u <= n || f < s != o) return !1;
+                    if (u <= n || l < s != a) return !1;
                     d = !1
                 } else "s" != s && "n" != s && (d = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
-        var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(d(e, t, o, n)), s(e[t][o])
-    }, f = (e, r, t) => {
-        var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, s = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, o) {
-        var a = w.I(r);
-        return a && a.then ? a.then(e.bind(e, r, w.S[r], t, n, o)) : e(r, w.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), h = p(((e, r, t, n, o) => {
-        var a = r && w.o(r, t) && f(r, t, n);
-        return a ? s(a) : o()
+    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
+        var a = u(e, t);
+        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(d(e, t, a, n)), s(e[t][a])
+    }, l = (e, r, t) => {
+        var a = e[r];
+        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+    }, s = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, a) {
+        var o = w.I(r);
+        return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), h = p(((e, r, t, n, a) => {
+        var o = r && w.o(r, t) && l(r, t, n);
+        return o ? s(o) : a()
     })), v = {}, m = {
-        641: () => h("default", "@unfolded/map-sdk", [1, 1, 8, 1], (() => w.e(747).then((() => () => w(747))))),
+        413: () => h("default", "@unfolded/map-sdk", [1, 1, 8, 2], (() => w.e(747).then((() => () => w(747))))),
         565: () => c("default", "@jupyter-widgets/base", [, [1, 4, 0, 0],
             [1, 3, 0, 0],
             [1, 2, 0, 0],
             [1, 1, 1, 10], 1, 1, 1
         ]),
         832: () => c("default", "@lumino/widgets", [1, 1, 37, 2])
-    }, b = {
+    }, g = {
         4: [832],
+        413: [413],
         565: [565],
-        568: [565],
-        641: [641]
+        568: [565]
     }, w.f.consumes = (e, r) => {
-        w.o(b, e) && b[e].forEach((e => {
+        w.o(g, e) && g[e].forEach((e => {
             if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
                 },
                 n = r => {
                     delete v[e], w.m[e] = t => {
                         throw delete w.c[e], r
                     }
                 };
             try {
-                var o = m[e]();
-                o.then ? r.push(v[e] = o.then(t).catch(n)) : t(o)
+                var a = m[e]();
+                a.then ? r.push(v[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             754: 0
         };
         w.f.j = (r, t) => {
             var n = w.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (/^(565|641)$/.test(r)) e[r] = 0;
+                else if (/^(413|565)$/.test(r)) e[r] = 0;
             else {
-                var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                t.push(n[2] = o);
-                var a = w.p + w.u(r),
+                var a = new Promise(((t, a) => n = e[r] = [t, a]));
+                t.push(n[2] = a);
+                var o = w.p + w.u(r),
                     i = new Error;
-                w.l(a, (t => {
+                w.l(o, (t => {
                     if (w.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var o = t && ("load" === t.type ? "missing" : t.type),
-                            a = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                        var a = t && ("load" === t.type ? "missing" : t.type),
+                            o = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var n, o, [a, i, u] = t,
+                var n, a, [o, i, u] = t,
                     d = 0;
-                if (a.some((r => 0 !== e[r]))) {
+                if (o.some((r => 0 !== e[r]))) {
                     for (n in i) w.o(i, n) && (w.m[n] = i[n]);
                     u && u(w)
                 }
-                for (r && r(t); d < a.length; d++) o = a[d], w.o(e, o) && e[o] && e[o][0](), e[a[d]] = 0
+                for (r && r(t); d < o.length; d++) a = o[d], w.o(e, a) && e[a] && e[a][0](), e[o[d]] = 0
             },
             t = self.webpackChunk_unfolded_jupyter_map_sdk = self.webpackChunk_unfolded_jupyter_map_sdk || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var k = w(768);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@unfolded/jupyter-map-sdk"] = k
 })();
```

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/labextension/static/third-party-licenses.json` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '1.8.2'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "UNLICENSED",
             "name": "@unfolded/map-sdk",
-            "versionInfo": "1.8.1"
+            "versionInfo": "1.8.2"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "3.6.0"
         },
```

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/map/base.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/base.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/map/html.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/html.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/map/widget.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/map/widget.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/nbextension/index.js` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -597,15 +597,15 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.1","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.1","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+                e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.2","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.2","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
             }
         },
         n = {};
 
     function a(e) {
         var s = n[e];
         if (void 0 !== s) return s.exports;
```

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/poll.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/poll.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/templates/html_map_sdk.j2` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/templates/html_map_sdk.j2`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/transfer_utils.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/transfer_utils.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/transport/base.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/base.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/transport/html.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/html.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/transport/widget.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/transport/widget.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/types.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/types.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/utils/action_type_mapping.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/action_type_mapping.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,26 +9,30 @@
     ActionType.SET_VIEW: "setView",
     ActionType.GET_VIEW_LIMITS: "getViewLimits",
     ActionType.SET_VIEW_LIMITS: "setViewLimits",
     ActionType.GET_MAP_CONTROL_VISIBILITY: "getMapControlVisibility",
     ActionType.SET_MAP_CONTROL_VISIBILITY: "setMapControlVisibility",
     ActionType.GET_SPLIT_MODE: "getSplitMode",
     ActionType.SET_SPLIT_MODE: "setSplitMode",
+    ActionType.GET_MAP_CONFIG: "getMapConfig",
+    ActionType.SET_MAP_CONFIG: "setMapConfig",
+    ActionType.GET_MAP_STYLES: "getMapStyles",
     ActionType.SET_THEME: "setUiTheme",
     # Filter API
     ActionType.GET_FILTERS: "getFilters",
     ActionType.GET_FILTER_BY_ID: "getFilterById",
     ActionType.ADD_FILTER: "addFilter",
     ActionType.UPDATE_FILTER: "updateFilter",
     ActionType.REMOVE_FILTER: "removeFilter",
     ActionType.UPDATE_TIMELINE: "updateTimeline",
     # Datasets API
     ActionType.GET_DATASETS: "getDatasets",
     ActionType.GET_DATASET_BY_ID: "getDatasetById",
     ActionType.ADD_DATASET: "addDataset",
+    ActionType.ADD_TILE_DATASET: "addTileDataset",
     ActionType.UPDATE_DATASET: "updateDataset",
     ActionType.REMOVE_DATASET: "removeDataset",
     ActionType.REPLACE_DATASET: "replaceDataset",
     ActionType.GET_DATASET_WITH_DATA: "getDatasetWithData",
     # Layer API
     ActionType.GET_LAYERS: "getLayers",
     ActionType.GET_LAYER_BY_ID: "getLayerById",
```

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/utils/encoders.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/utils/serialization.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded/map_sdk/utils/validators.py` & `unfolded.map-sdk-1.8.2/unfolded/map_sdk/utils/validators.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.8.1/unfolded.map_sdk.egg-info/PKG-INFO` & `unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfolded.map-sdk
-Version: 1.8.1
+Version: 1.8.2
 Summary: Jupyter Widget for Foursquare Studio Maps
 Author: Foursquare Labs
 Author-email: info-studio@foursquare.com
 License: (c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `unfolded.map-sdk-1.8.1/unfolded.map_sdk.egg-info/SOURCES.txt` & `unfolded.map-sdk-1.8.2/unfolded.map_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -59,19 +59,19 @@
 unfolded/map_sdk/api/dataset_api.py
 unfolded/map_sdk/api/enums.py
 unfolded/map_sdk/api/event_api.py
 unfolded/map_sdk/api/filter_api.py
 unfolded/map_sdk/api/layer_api.py
 unfolded/map_sdk/api/map_api.py
 unfolded/map_sdk/labextension/package.json
-unfolded/map_sdk/labextension/static/4.c6720f8df23b707b3655.js
-unfolded/map_sdk/labextension/static/480.232c2d64243946e2f053.js
-unfolded/map_sdk/labextension/static/568.9ca15b62cee6758f82c8.js
+unfolded/map_sdk/labextension/static/4.2f5ebe11a5669cad3275.js
+unfolded/map_sdk/labextension/static/480.25ce0490671eeeb9f120.js
+unfolded/map_sdk/labextension/static/568.caff7d3d72d44ec36b9e.js
 unfolded/map_sdk/labextension/static/747.488cf0ee36d815959581.js
-unfolded/map_sdk/labextension/static/remoteEntry.7fae4787113bb153082a.js
+unfolded/map_sdk/labextension/static/remoteEntry.1f1edfc58c4b1a509424.js
 unfolded/map_sdk/labextension/static/style.js
 unfolded/map_sdk/labextension/static/third-party-licenses.json
 unfolded/map_sdk/map/__init__.py
 unfolded/map_sdk/map/base.py
 unfolded/map_sdk/map/html.py
 unfolded/map_sdk/map/widget.py
 unfolded/map_sdk/nbextension/extension.js
```

### Comparing `unfolded.map-sdk-1.8.1/webpack.config.js` & `unfolded.map-sdk-1.8.2/webpack.config.js`

 * *Files identical despite different names*

