# Comparing `tmp/deeplake-3.6.3.tar.gz` & `tmp/deeplake-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.6.3.tar", last modified: Tue Jun 13 18:21:09 2023, max compression
+gzip compressed data, was "deeplake-3.6.4.tar", last modified: Fri Jun 16 18:26:43 2023, max compression
```

## Comparing `deeplake-3.6.3.tar` & `deeplake-3.6.4.tar`

### file list

```diff
@@ -1,398 +1,398 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.146204 deeplake-3.6.3/
--rw-r--r--   0 root         (0) root         (0)    15975 2023-06-13 18:19:49.000000 deeplake-3.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-13 18:19:49.000000 deeplake-3.6.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    26080 2023-06-13 18:21:09.146204 deeplake-3.6.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25351 2023-06-13 18:19:49.000000 deeplake-3.6.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.116204 deeplake-3.6.3/deeplake/
--rw-r--r--   0 root         (0) root         (0)     2662 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    96883 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4693 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/info.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/link.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/api/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 root         (0) root         (0)    85180 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_events.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    25678 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_link.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_linking.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 root         (0) root         (0)     7900 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_none.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 root         (0) root         (0)    10559 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_pop.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)    18863 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_reset.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_text.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 root         (0) root         (0)     7499 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_video.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tiled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/auto/structured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/structured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/structured/base.py
--rw-r--r--   0 root         (0) root         (0)     6666 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/auto/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7975 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 root         (0) root         (0)    12440 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/auto/unstructured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/auto/unstructured/coco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 root         (0) root         (0)     6693 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4514 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 root         (0) root         (0)    12937 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/cli/auth.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/cli/commands.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/cli/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19099 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/client/config.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/client/log.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/client/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/client/utils.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/compression.py
--rw-r--r--   0 root         (0) root         (0)     7332 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/chunk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24150 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)   113519 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)    39478 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compute/process.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compute/provider.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compute/ray.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compute/serial.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compute/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/dataset/
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171829 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    15422 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11965 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5265 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 root         (0) root         (0)     4769 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/index/
--rw-r--r--   0 root         (0) root         (0)      138 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/index/index.py
--rw-r--r--   0 root         (0) root         (0)    19800 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/io.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/ipc.py
--rw-r--r--   0 root         (0) root         (0)    13074 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/link_creds.py
--rw-r--r--   0 root         (0) root         (0)    15995 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/linked_sample.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/meta/
--rw-r--r--   0 root         (0) root         (0)       97 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/meta/encode/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25591 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 root         (0) root         (0)    13495 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/meta/encode/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     7515 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/meta.py
--rw-r--r--   0 root         (0) root         (0)    13344 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/partial_reader.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/partial_sample.py
--rw-r--r--   0 root         (0) root         (0)     5269 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/polygon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/query/
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/query/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)    14326 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/query/filter.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/query/query.py
--rw-r--r--   0 root         (0) root         (0)    20658 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/sample.py
--rw-r--r--   0 root         (0) root         (0)    22849 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/storage/
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13705 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/azure.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 root         (0) root         (0)    19080 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/gcs.py
--rw-r--r--   0 root         (0) root         (0)    13053 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/google_drive.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/local.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/memory.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/provider.py
--rw-r--r--   0 root         (0) root         (0)    25799 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/s3.py
--rw-r--r--   0 root         (0) root         (0)    50140 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7485 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tensor_link.py
--rw-r--r--   0 root         (0) root         (0)     5152 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_compression.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     4312 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_locking.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/tiling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/transform/
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51556 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/transform/test_transform.py
--rw-r--r--   0 root         (0) root         (0)    29645 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/transform/transform.py
--rw-r--r--   0 root         (0) root         (0)     5860 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/
--rw-r--r--   0 root         (0) root         (0)      611 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24105 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/deeplake_vectorstore.py
--rw-r--r--   0 root         (0) root         (0)    30234 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/test_deeplake_vectorstore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/dataset/
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11211 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    10090 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/filter/
--rw-r--r--   0 root         (0) root         (0)      286 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/filter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/filter/filter.py
--rw-r--r--   0 root         (0) root         (0)     3542 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/filter/test_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4510 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/query.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/test_indra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
--rw-r--r--   0 root         (0) root         (0)      275 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/
--rw-r--r--   0 root         (0) root         (0)       93 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6455 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
--rw-r--r--   0 root         (0) root         (0)     5014 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/vector_search.py
--rw-r--r--   0 root         (0) root         (0)     9551 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/utils.py
--rw-r--r--   0 root         (0) root         (0)     3399 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/version_control/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 root         (0) root         (0)    19869 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 root         (0) root         (0)    84800 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/enterprise/
--rw-r--r--   0 root         (0) root         (0)      257 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 root         (0) root         (0)    29584 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 root         (0) root         (0)    25897 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/test_query.py
--rw-r--r--   0 root         (0) root         (0)    22353 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/util.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/hooks.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/htype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/integrations/
--rw-r--r--   0 root         (0) root         (0)       99 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/integrations/huggingface/
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5503 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/integrations/mmdet/
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62754 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 root         (0) root         (0)     4739 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/integrations/pytorch/
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9862 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 root         (0) root         (0)     7140 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 root         (0) root         (0)     6919 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/integrations/tf/
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/tf/common.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/integrations/wandb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/requirements/
--rw-r--r--   0 root         (0) root         (0)      476 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/requirements/common.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/requirements/plugins.txt
--rw-r--r--   0 root         (0) root         (0)      304 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/requirements/tests.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2554 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/client_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     4015 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 root         (0) root         (0)    16165 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/path_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2735 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.146204 deeplake-3.6.3/deeplake/util/
--rw-r--r--   0 root         (0) root         (0)       86 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/access_method.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/agreement.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/array_list.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/auto.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/bugout_reporter.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/bugout_token.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/cache_chain.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/casting.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/check_installation.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/check_latest_version.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     4597 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/class_label.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/compression.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/compute.py
--rw-r--r--   0 root         (0) root         (0)     5404 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/dataset.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/delete_entry.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/diff.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/downsample.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/empty_sample.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/encoder.py
--rw-r--r--   0 root         (0) root         (0)    34773 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/exif.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/from_tfds.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/generate_id.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/hash.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/htype.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/image.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/invalid_view_op.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/iteration_warning.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/join_chunks.py
--rw-r--r--   0 root         (0) root         (0)     6422 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/json.py
--rw-r--r--   0 root         (0) root         (0)     7261 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/keys.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/link.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/logging.py
--rw-r--r--   0 root         (0) root         (0)    37497 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/merge.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/modified.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.146204 deeplake-3.6.3/deeplake/util/object_3d/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 root         (0) root         (0)    10213 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 root         (0) root         (0)     3986 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/path.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/pretty_print.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/remove_cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     4204 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/spinner.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/split.py
--rw-r--r--   0 root         (0) root         (0)     8435 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/storage.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tag.py
--rw-r--r--   0 root         (0) root         (0)     1390 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tensor_db.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.146204 deeplake-3.6.3/deeplake/util/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_auto.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_tensor_db.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/threading.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/token.py
--rw-r--r--   0 root         (0) root         (0)    25235 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/transform.py
--rw-r--r--   0 root         (0) root         (0)    31615 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/version_control.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/video.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.146204 deeplake-3.6.3/deeplake/visualizer/
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.116204 deeplake-3.6.3/deeplake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    26080 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12677 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1075 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-06-13 18:21:09.146204 deeplake-3.6.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3357 2023-06-13 18:19:49.000000 deeplake-3.6.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-06-16 18:24:57.000000 deeplake-3.6.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-16 18:24:57.000000 deeplake-3.6.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    26080 2023-06-16 18:26:43.728096 deeplake-3.6.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25351 2023-06-16 18:24:57.000000 deeplake-3.6.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99372 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    85180 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    25678 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     7900 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    18863 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7499 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     7081 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    13490 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19099 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     7387 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   113519 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171829 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    15422 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11965 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5265 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    19800 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    13074 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    15995 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13344 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    20658 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    22849 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13705 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/azure.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    19080 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    25799 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    50140 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7485 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51556 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    29645 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5860 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25170 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/deeplake_vectorstore.py
+-rw-r--r--   0 root         (0) root         (0)    35113 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/test_deeplake_vectorstore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/dataset/
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12673 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10090 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/filter/
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/filter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/filter/filter.py
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/filter/test_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4510 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/query.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/test_indra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6564 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
+-rw-r--r--   0 root         (0) root         (0)     5040 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/vector_search.py
+-rw-r--r--   0 root         (0) root         (0)    11940 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/vectorstore/vector_search/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19869 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    29584 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    25897 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22353 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62754 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.718096 deeplake-3.6.4/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9862 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      304 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     4015 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    16165 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    34773 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37497 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     8435 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    25235 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31615 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.728096 deeplake-3.6.4/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-06-16 18:24:57.000000 deeplake-3.6.4/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 18:26:43.708096 deeplake-3.6.4/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    26080 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12677 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-16 18:26:43.000000 deeplake-3.6.4/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-16 18:26:43.728096 deeplake-3.6.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-06-16 18:24:57.000000 deeplake-3.6.4/setup.py
```

### Comparing `deeplake-3.6.3/LICENSE` & `deeplake-3.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/PKG-INFO` & `deeplake-3.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.6.3
+Version: 3.6.4
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.6.3 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.4 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
 Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
```

### Comparing `deeplake-3.6.3/README.md` & `deeplake-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/__init__.py` & `deeplake-3.6.4/deeplake/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.6.3"
+__version__ = "3.6.4"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
 deeplake_reporter.system_report(publish=True)
```

### Comparing `deeplake-3.6.3/deeplake/api/dataset.py` & `deeplake-3.6.4/deeplake/api/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1337,35 +1337,36 @@
         token: Optional[str] = None,
         connect_kwargs: Optional[Dict] = None,
         **dataset_kwargs,
     ) -> Dataset:
         """Ingest images and annotations in COCO format to a Deep Lake Dataset. The source data can be stored locally or in the cloud.
 
         Examples:
+            >>> # Ingest local data in COCO format to a Deep Lake dataset stored in Deep Lake storage.
             >>> ds = deeplake.ingest_coco(
-            >>>     "path/to/images/directory",
+            >>>     "<path/to/images/directory>",
             >>>     ["path/to/annotation/file1.json", "path/to/annotation/file2.json"],
             >>>     dest="hub://org_id/dataset",
             >>>     key_to_tensor_mapping={"category_id": "labels", "bbox": "boxes"},
             >>>     file_to_group_mapping={"file1.json": "group1", "file2.json": "group2"},
             >>>     ignore_keys=["area", "image_id", "id"],
-            >>>     token="my_activeloop_token",
             >>>     num_workers=4,
             >>> )
-            >>> # or ingest data from the cloud
+            >>> # Ingest data from your cloud into another Deep Lake dataset in your cloud, and connect that dataset to the Deep Lake backend.
             >>> ds = deeplake.ingest_coco(
             >>>     "s3://bucket/images/directory",
             >>>     "s3://bucket/annotation/file1.json",
-            >>>     dest="hub://org_id/dataset_name",
+            >>>     dest="s3://bucket/dataset_name",
             >>>     ignore_one_group=True,
             >>>     ignore_keys=["area", "image_id", "id"],
             >>>     image_settings={"name": "images", "htype": "link[image]", "sample_compression": "jpeg"},
-            >>>     image_creds_key="my_s3_managed_credentials"
+            >>>     image_creds_key="my_s3_managed_credentials",
             >>>     src_creds=aws_creds, # Can also be inferred from environment
-            >>>     token="my_activeloop_token",
+            >>>     dest_creds=aws_creds, # Can also be inferred from environment
+            >>>     connect_kwargs={"creds_key": "my_s3_managed_credentials", "org_id": "org_id"},
             >>>     num_workers=4,
             >>> )
 
         Args:
             images_directory (str, pathlib.Path): The path to the directory containing images.
             annotation_files (str, pathlib.Path, List[str]): Path to JSON annotation files in COCO format.
             dest (str, pathlib.Path):
@@ -1458,29 +1459,31 @@
         token: Optional[str] = None,
         connect_kwargs: Optional[Dict] = None,
         **dataset_kwargs,
     ) -> Dataset:
         """Ingest images and annotations (bounding boxes or polygons) in YOLO format to a Deep Lake Dataset. The source data can be stored locally or in the cloud.
 
         Examples:
+            >>> # Ingest local data in YOLO format to a Deep Lake dataset stored in Deep Lake storage.
             >>> ds = deeplake.ingest_yolo(
             >>>     "path/to/data/directory",
             >>>     dest="hub://org_id/dataset",
             >>>     allow_no_annotation=True,
             >>>     token="my_activeloop_token",
             >>>     num_workers=4,
             >>> )
-            >>> # or ingest data from the cloud
+            >>> # Ingest data from your cloud into another Deep Lake dataset in your cloud, and connect that dataset to the Deep Lake backend.
             >>> ds = deeplake.ingest_yolo(
             >>>     "s3://bucket/data_directory",
-            >>>     dest="hub://org_id/dataset",
+            >>>     dest="s3://bucket/dataset_name",
             >>>     image_params={"name": "image_links", "htype": "link[image]"},
             >>>     image_creds_key="my_s3_managed_credentials",
             >>>     src_creds=aws_creds, # Can also be inferred from environment
-            >>>     token="my_activeloop_token",
+            >>>     dest_creds=aws_creds, # Can also be inferred from environment
+            >>>     connect_kwargs={"creds_key": "my_s3_managed_credentials", "org_id": "org_id"},
             >>>     num_workers=4,
             >>> )
 
         Args:
             data_directory (str, pathlib.Path): The path to the directory containing the data (images files and annotation files(see 'annotations_directory' input for specifying annotations in a separate directory).
             dest (str, pathlib.Path):
                 - The full path to the dataset. Can be:
@@ -1815,31 +1818,56 @@
         token: Optional[str] = None,
         connect_kwargs: Optional[Dict] = None,
         **dataset_kwargs,
     ):
         """Convert pandas dataframe to a Deep Lake Dataset. The contents of the dataframe can be parsed literally, or can be treated as links to local or cloud files.
 
         Examples:
-            >>> ds = deeplake.dataframe(
+
+
+                    >>> # Ingest local data in COCO format to a Deep Lake dataset stored in Deep Lake storage.
+            >>> ds = deeplake.ingest_coco(
+            >>>     "<path/to/images/directory>",
+            >>>     ["path/to/annotation/file1.json", "path/to/annotation/file2.json"],
+            >>>     dest="hub://org_id/dataset",
+            >>>     key_to_tensor_mapping={"category_id": "labels", "bbox": "boxes"},
+            >>>     file_to_group_mapping={"file1.json": "group1", "file2.json": "group2"},
+            >>>     ignore_keys=["area", "image_id", "id"],
+            >>>     num_workers=4,
+            >>> )
+            >>> # Ingest data from your cloud into another Deep Lake dataset in your cloud, and connect that dataset to the Deep Lake backend.
+
+
+
+            >>> # Ingest data from a DataFrame into a Deep Lake dataset stored in Deep Lake storage.
+            >>> ds = deeplake.ingest_dataframe(
             >>>     df,
             >>>     dest="hub://org_id/dataset",
             >>> )
-            >>> # or ingest data as images from the cloud
-            >>> ds = deeplake.dataframe(
+            >>> # Ingest data from a DataFrame into a Deep Lake dataset stored in Deep Lake storage. The filenames in `df_column_with_cloud_paths` will be used as the filenames for loading data into the dataset.
+            >>> ds = deeplake.ingest_dataframe(
             >>>     df,
             >>>     dest="hub://org_id/dataset",
-            >>>     column_params={"df_column_with_cloud_paths": {"name": "images", "htype": "image"}}
+            >>>     column_params={"df_column_with_cloud_paths": {"name": "images", "htype": "image"}},
             >>>     src_creds=aws_creds
             >>> )
-            >>> # or ingest data as linked images in the cloud
-            >>> ds = deeplake.dataframe(
+            >>> # Ingest data from a DataFrame into a Deep Lake dataset stored in Deep Lake storage. The filenames in `df_column_with_cloud_paths` will be used as the filenames for linked data in the dataset.
+            >>> ds = deeplake.ingest_dataframe(
             >>>     df,
             >>>     dest="hub://org_id/dataset",
-            >>>     column_params={"df_column_with_cloud_paths": {"name": "image_links", "htype": "link[image]"}}
+            >>>     column_params={"df_column_with_cloud_paths": {"name": "image_links", "htype": "link[image]"}},
+            >>>     creds_key="my_s3_managed_credentials"
+            >>> )
+            >>> # Ingest data from a DataFrame into a Deep Lake dataset stored in your cloud, and connect that dataset to the Deep Lake backend. The filenames in `df_column_with_cloud_paths` will be used as the filenames for linked data in the dataset.
+            >>> ds = deeplake.ingest_dataframe(
+            >>>     df,
+            >>>     dest="s3://bucket/dataset_name",
+            >>>     column_params={"df_column_with_cloud_paths": {"name": "image_links", "htype": "link[image]"}},
             >>>     creds_key="my_s3_managed_credentials"
+            >>>     connect_kwargs={"creds_key": "my_s3_managed_credentials", "org_id": "org_id"},
             >>> )
 
         Args:
             src (pd.DataFrame): The pandas dataframe to be converted.
             dest (str, pathlib.Path):
                 - A Dataset or The full path to the dataset. Can be:
                 - a Deep Lake cloud path of the form ``hub://username/datasetname``. To write to Deep Lake cloud datasets, ensure that you are logged in to Deep Lake (use 'activeloop login' from command line)
```

### Comparing `deeplake-3.6.3/deeplake/api/info.py` & `deeplake-3.6.4/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/link.py` & `deeplake-3.6.4/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/link_tiled.py` & `deeplake-3.6.4/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/read.py` & `deeplake-3.6.4/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_access_method.py` & `deeplake-3.6.4/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_agreement.py` & `deeplake-3.6.4/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_api.py` & `deeplake-3.6.4/deeplake/api/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.6.4/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.6.4/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.6.4/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.6.4/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_dataset.py` & `deeplake-3.6.4/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_dicom.py` & `deeplake-3.6.4/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_downsample.py` & `deeplake-3.6.4/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_events.py` & `deeplake-3.6.4/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_grayscale.py` & `deeplake-3.6.4/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_info.py` & `deeplake-3.6.4/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.6.4/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_json.py` & `deeplake-3.6.4/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_link.py` & `deeplake-3.6.4/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.6.4/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_linking.py` & `deeplake-3.6.4/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_mesh.py` & `deeplake-3.6.4/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_meta.py` & `deeplake-3.6.4/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_nifti.py` & `deeplake-3.6.4/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_none.py` & `deeplake-3.6.4/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.6.4/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_pickle.py` & `deeplake-3.6.4/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.6.4/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_polygons.py` & `deeplake-3.6.4/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_pop.py` & `deeplake-3.6.4/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_readonly.py` & `deeplake-3.6.4/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_rechunk.py` & `deeplake-3.6.4/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_reset.py` & `deeplake-3.6.4/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_sample_info.py` & `deeplake-3.6.4/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_text.py` & `deeplake-3.6.4/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_update_samples.py` & `deeplake-3.6.4/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_video.py` & `deeplake-3.6.4/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tests/test_views.py` & `deeplake-3.6.4/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/api/tiled.py` & `deeplake-3.6.4/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/structured/base.py` & `deeplake-3.6.4/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/structured/dataframe.py` & `deeplake-3.6.4/deeplake/auto/structured/dataframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from collections import defaultdict
 from typing import DefaultDict, List, Union, Optional
 from deeplake.core.sample import Sample
 from deeplake.core.linked_sample import LinkedSample
 import pathlib
 
+import pandas as pd  # type: ignore
+
 
 from deeplake.client.log import logger
 
 
 class DataFrame(StructuredDataset):
     def __init__(self, source, column_params=None, creds=None, creds_key=None):
         """Convert a pandas dataframe to a Deep Lake dataset.
@@ -49,14 +51,20 @@
                     params["name"] = sanitize_tensor_name(key)
             else:
                 column_params[key] = {"name": sanitize_tensor_name(key)}
         self.column_params = column_params
 
     def _get_most_frequent_image_extension(self, fn_iterator):
         # TODO: Make this generic and work for any htype that requires compression
+
+        if len(fn_iterator) == 0:
+            raise IngestionError(
+                f"Cannot determine the most frequent image compression because no valid image files were provided."
+            )
+
         supported_image_extensions = tuple(
             "." + fmt for fmt in HTYPE_SUPPORTED_COMPRESSIONS["image"] + ["jpg"]
         )
         image_extensions: DefaultDict[str, int] = defaultdict(int)
         for file in fn_iterator:
             if file.lower().endswith(supported_image_extensions):
                 ext = file.rsplit(".", 1)[1]
@@ -71,66 +79,74 @@
 
     def _parse_tensor_params(self, key, inspect_limit=1000):
         """Parse the tensor parameters for a column. Required parameters that are not specified will be inferred by inspecting up to 'inspect_limit' rows in the data."""
 
         tensor_params: Dict = self.column_params[key]
 
         dtype = self.source[key].dtype
+
         if (
             "htype" not in tensor_params
         ):  # Auto-set some typing parameters if htype is not specified
             if dtype == np.dtype("object"):
-                types = [type(v) for v in self.source[key][0:inspect_limit].values]
+                types = [
+                    type(v)
+                    for v in self.source[key][0:inspect_limit].values
+                    if v is not None
+                ]  # Can be length 0 if all data is None
 
-                if len(set(types)) != 1:
+                if len(set(types)) > 1:
                     raise IngestionError(
                         f"Dataframe has different data types inside '{key}' column. Please make sure all data is given column is compatible with a single Deep Lake htype, or try specifying the htype manually."
                     )
 
-                if types[0] == str:
+                if len(types) > 0 and types[0] == str:
                     tensor_params.update(
                         htype="text"
                     )  # Use "text" htype for text data when the htype is not specified tensor_params
             else:
                 tensor_params.update(
                     dtype=dtype,
                     create_shape_tensor=tensor_params.get("create_shape_tensor", False),
-                )  # htype will be auto-inferred for numeric data unless the htype is specified in tensor_params
+                )
 
         # TODO: Make this more robust so it works for all htypes where sample_compression is required and should be inferred from the data itself
         if (
             "image" in tensor_params.get("htype", "")
             and "sample_compression" not in tensor_params
             and "chunk_compression" not in tensor_params
         ):
             tensor_params.update(
                 sample_compression=self._get_most_frequent_image_extension(
-                    self.source[key].values
+                    self.source[key][self.source[key].notnull()].values
                 )
             )
 
         return tensor_params
 
     def _get_extend_values(self, tensor_params: dict, key: str):  # type: ignore
         """Method creates a list of values to be extended to the tensor, based on the tensor parameters and the data in the dataframe column"""
 
+        column_data = self.source[key]
+        column_data = column_data.where(pd.notnull(column_data), None).values.tolist()
+
         extend_values: List[Optional[Union[Sample, LinkedSample, np.ndarray]]]
 
         if "htype" in tensor_params and "link[" in tensor_params["htype"]:
             extend_values = [
                 link(value, creds_key=self.creds_key) if value is not None else None
-                for value in self.source[key].values
+                for value in column_data
             ]
         elif "htype" in tensor_params and "image" in tensor_params["htype"]:
             extend_values = [
                 read(value, creds=self.creds) if value is not None else None
-                for value in self.source[key].values
+                for value in column_data
             ]
         else:
-            extend_values = self.source[key].values
+            extend_values = column_data
 
         return extend_values
 
     def fill_dataset(self, ds: Dataset, progressbar: bool = True) -> Dataset:
         """Fill dataset with data from the dataframe - one tensor per column
 
         Args:
@@ -156,8 +172,9 @@
                 if tensor_params["name"] not in ds.tensors:
                     ds.create_tensor(**tensor_params)
 
                 ds[tensor_params["name"]].extend(
                     self._get_extend_values(tensor_params, key),
                     progressbar=progressbar,
                 )
+
         return ds
```

### Comparing `deeplake-3.6.3/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.6.4/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.6.4/deeplake/auto/tests/test_ingestion.py`

 * *Files 6% similar despite different names*

```diff
@@ -301,57 +301,71 @@
     assert ds[df_keys[0]].meta.sample_compression == "jpeg"
 
     assert len(ds[df_keys[0]][0].numpy().shape) == 3
     assert ds[df_keys[2]][2].data()["text"][0] == df[df_keys[2]][2]
 
 
 def test_dataframe_array(memory_ds: Dataset):
-    # Create DataFrame
     data = {
-        "AA": ["Alice", "Bob", "Charlie", "Steve"],
+        "AA": ["Alice", "Bob", "Charlie", None],
         "BB": [
-            np.array([80, 75, 85]),
-            np.array([80, 22, 1]),
-            np.array([0, 565, 234]),
-            np.array([0, 565, 234]),
+            np.array([3, 22, 1, 3]),
+            np.array([1, 22, 10, 1]),
+            np.array([2, 22, 1, 2]),
+            np.array([0, 56, 34, 2]),
         ],
-        "CC": [45, 67, 88, 77],
+        "CC": [45, 67, 88, float("nan")],
+        "DD": [None, None, None, None],
+        "EE": [
+            None,
+            np.array([1, 22, 10, 1]),
+            None,
+            np.array([0, 56, 34]),
+        ],
+        "FF": [None, "Bob", "Charlie", "Dave"],
     }
 
     df = pd.DataFrame(data)
     df_keys = df.keys()
 
     ds = deeplake.ingest_dataframe(
         df,
-        memory_ds.path,
+        "mem://dummy",
         progressbar=False,
     )
     tensors_names = list(ds.tensors.keys())
 
-    assert tensors_names == [df_keys[0], df_keys[1], df_keys[2]]
+    assert tensors_names == df_keys.tolist()
     assert ds[df_keys[0]].htype == "text"
 
     np.testing.assert_array_equal(
         ds[df_keys[1]].numpy(), np.stack([arr for arr in df[df_keys[1]].values], axis=0)
     )
 
     np.testing.assert_array_equal(
         ds[df_keys[2]].numpy().reshape(-1), df[df_keys[2]].values
     )
     assert ds[df_keys[2]].dtype == df[df_keys[2]].dtype
 
+    data_key_4 = ds[df_keys[4]].numpy(aslist=True)
+    ds_data = [None if arr.shape[0] == 0 else arr for arr in data_key_4]
+    df_data = [arr for arr in df[df_keys[4]].values]
+
+    assert len(ds[df_keys[4]].numpy(aslist=True)) == 4
+    assert ds[df_keys[4]][0].numpy().tolist() == []
+    assert ds[df_keys[4]][0].numpy().shape[0] == 0
+    assert ds[df_keys[4]][1].numpy().shape[0] == 4
 
-def test_dataframe_array_bad(memory_ds: Dataset):
-    # Create DataFrame
 
+def test_dataframe_array_bad(memory_ds: Dataset):
     data = {
-        "AA": ["Alice", "Bob", "Charlie", "Steve"],
+        "AA": ["Alice", "Bob", "Charlie", None],
         "BB": [
-            np.array([80, 75, 85]),
-            np.array([80, 22, 1]),
+            np.array([80, 75, 85, 100]),
+            None,
             np.array([0, 565, 234]),
             "bad_data",
         ],
         "CC": [45, 67, 88, 77],
     }
 
     df = pd.DataFrame(data)
@@ -360,14 +374,37 @@
         ds = deeplake.ingest_dataframe(
             df,
             memory_ds.path,
             progressbar=False,
         )
 
 
+def test_dataframe_all_empty_images(memory_ds: Dataset):
+    data = {
+        "AA": ["Alice", "Bob", "Charlie", "Steve"],
+        "BB": [
+            None,
+            None,
+            None,
+            None,
+        ],
+        "CC": [45, 67, 88, 77],
+    }
+
+    df = pd.DataFrame(data)
+
+    with pytest.raises(IngestionError):
+        ds = deeplake.ingest_dataframe(
+            df,
+            "mem://dummy",
+            progressbar=False,
+            column_params={"BB": {"htype": "image"}},
+        )
+
+
 def test_dataframe_unsupported_file(memory_ds: Dataset, dataframe_ingestion_data):
     df = pd.read_csv(dataframe_ingestion_data["dataframe_w_bad_images_path"])
     df_keys = df.keys()
 
     df[df_keys[0]] = dataframe_ingestion_data["images_basepath"] + df[df_keys[0]]
 
     with pytest.raises(IngestionError):
```

### Comparing `deeplake-3.6.3/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.6.4/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.6.4/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/unstructured/base.py` & `deeplake-3.6.4/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.6.4/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.6.4/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.6.4/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.6.4/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.6.4/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.6.4/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/unstructured/util.py` & `deeplake-3.6.4/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.6.4/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.6.4/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/cli/auth.py` & `deeplake-3.6.4/deeplake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/cli/test_cli.py` & `deeplake-3.6.4/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/client/client.py` & `deeplake-3.6.4/deeplake/client/client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/client/config.py` & `deeplake-3.6.4/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/client/log.py` & `deeplake-3.6.4/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/client/test_client.py` & `deeplake-3.6.4/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/client/utils.py` & `deeplake-3.6.4/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/compression.py` & `deeplake-3.6.4/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/constants.py` & `deeplake-3.6.4/deeplake/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,15 @@
 DEFAULT_TRANSFORM_SAMPLE_CACHE_SIZE = 16
 TRANSFORM_CHUNK_CACHE_SIZE = 64 * MB
 
 DEFAULT_VECTORSTORE_DEEPLAKE_PATH = "./deeplake_vector_store"
 MAX_VECTORSTORE_INGESTION_RETRY_ATTEMPTS = 5
 MAX_CHECKPOINTING_INTERVAL = 100000
 VECTORSTORE_EXTEND_MAX_SIZE = 20000
+VECTORSTORE_EXTEND_MAX_SIZE_BY_HTYPE = {"image": 2000}
 DEFAULT_VECTORSTORE_TENSORS = [
     {
         "name": "text",
         "htype": "text",
         "create_id_tensor": False,
         "create_sample_info_tensor": False,
         "create_shape_tensor": False,
```

### Comparing `deeplake-3.6.3/deeplake/core/chunk/base_chunk.py` & `deeplake-3.6.4/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.6.4/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.6.4/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.6.4/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.6.4/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.6.4/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.6.4/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/chunk_engine.py` & `deeplake-3.6.4/deeplake/core/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/compression.py` & `deeplake-3.6.4/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/compute/process.py` & `deeplake-3.6.4/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/compute/provider.py` & `deeplake-3.6.4/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/compute/ray.py` & `deeplake-3.6.4/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/compute/serial.py` & `deeplake-3.6.4/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/compute/thread.py` & `deeplake-3.6.4/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/dataset/__init__.py` & `deeplake-3.6.4/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/dataset/dataset.py` & `deeplake-3.6.4/deeplake/core/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.6.4/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.6.4/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/dataset/deeplake_query_tensor.py` & `deeplake-3.6.4/deeplake/core/dataset/deeplake_query_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/dataset/invalid_view.py` & `deeplake-3.6.4/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/dataset/view_entry.py` & `deeplake-3.6.4/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/fast_forwarding.py` & `deeplake-3.6.4/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/index/index.py` & `deeplake-3.6.4/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/io.py` & `deeplake-3.6.4/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/ipc.py` & `deeplake-3.6.4/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/link_creds.py` & `deeplake-3.6.4/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/linked_chunk_engine.py` & `deeplake-3.6.4/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/linked_sample.py` & `deeplake-3.6.4/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/linked_tiled_sample.py` & `deeplake-3.6.4/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/lock.py` & `deeplake-3.6.4/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/dataset_meta.py` & `deeplake-3.6.4/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.6.4/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.6.4/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.6.4/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/encode/creds.py` & `deeplake-3.6.4/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/encode/pad.py` & `deeplake-3.6.4/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/encode/sequence.py` & `deeplake-3.6.4/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/encode/shape.py` & `deeplake-3.6.4/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.6.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.6.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.6.4/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.6.4/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.6.4/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/encode/tile.py` & `deeplake-3.6.4/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/meta/tensor_meta.py` & `deeplake-3.6.4/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/partial_reader.py` & `deeplake-3.6.4/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/partial_sample.py` & `deeplake-3.6.4/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/polygon.py` & `deeplake-3.6.4/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/query/autocomplete.py` & `deeplake-3.6.4/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/query/filter.py` & `deeplake-3.6.4/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/query/query.py` & `deeplake-3.6.4/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/sample.py` & `deeplake-3.6.4/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/serialize.py` & `deeplake-3.6.4/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/storage/azure.py` & `deeplake-3.6.4/deeplake/core/storage/azure.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.6.4/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/storage/gcs.py` & `deeplake-3.6.4/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/storage/google_drive.py` & `deeplake-3.6.4/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/storage/local.py` & `deeplake-3.6.4/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/storage/lru_cache.py` & `deeplake-3.6.4/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/storage/memory.py` & `deeplake-3.6.4/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/storage/provider.py` & `deeplake-3.6.4/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/storage/s3.py` & `deeplake-3.6.4/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tensor.py` & `deeplake-3.6.4/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tensor_link.py` & `deeplake-3.6.4/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/test_serialize.py` & `deeplake-3.6.4/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tests/test_compression.py` & `deeplake-3.6.4/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tests/test_compute.py` & `deeplake-3.6.4/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.6.4/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tests/test_io.py` & `deeplake-3.6.4/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tests/test_locking.py` & `deeplake-3.6.4/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tests/test_readonly.py` & `deeplake-3.6.4/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tests/test_serialize.py` & `deeplake-3.6.4/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tiling/deserialize.py` & `deeplake-3.6.4/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tiling/optimizer.py` & `deeplake-3.6.4/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.6.4/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tiling/serialize.py` & `deeplake-3.6.4/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.6.4/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/tiling/test_serialize.py` & `deeplake-3.6.4/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/transform/test_transform.py` & `deeplake-3.6.4/deeplake/core/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/transform/transform.py` & `deeplake-3.6.4/deeplake/core/transform/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/transform/transform_dataset.py` & `deeplake-3.6.4/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/transform/transform_tensor.py` & `deeplake-3.6.4/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/__init__.py` & `deeplake-3.6.4/deeplake/core/vectorstore/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,8 +7,9 @@
 )
 from deeplake.core.vectorstore.vector_search.python.search_algorithm import (
     search as python_search_algorithm,
 )
 from deeplake.core.vectorstore.vector_search.indra.search_algorithm import (
     search as indra_search_algorithm,
 )
+from deeplake.core.vectorstore.deeplake_vectorstore import VectorStore
 from deeplake.core.vectorstore.deeplake_vectorstore import DeepLakeVectorStore
```

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/deeplake_vectorstore.py` & `deeplake-3.6.4/deeplake/core/vectorstore/deeplake_vectorstore.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from deeplake.core.vectorstore.vector_search import filter as filter_utils
 
 from deeplake.util.bugout_reporter import feature_report_path, deeplake_reporter
 
 logger = logging.getLogger(__name__)
 
 
-class DeepLakeVectorStore:
+class VectorStore:
     """Base class for DeepLakeVectorStore"""
 
     def __init__(
         self,
         path: Union[str, pathlib.Path],
         tensor_params: List[Dict[str, object]] = DEFAULT_VECTORSTORE_TENSORS,
         embedding_function: Optional[Callable] = None,
@@ -72,16 +72,16 @@
                 - a Deep Lake cloud path of the form ``hub://org_id/dataset_name``. Requires registration with Deep Lake.
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             tensor_params (List[Dict[str, dict]], optional): List of dictionaries that contains information about tensors that user wants to create. See ``create_tensor`` in Deep Lake API docs for more information. Defaults to ``DEFAULT_VECTORSTORE_TENSORS``.
             embedding_function (Optional[callable], optional): Function that converts the embeddable data into embeddings. Defaults to None.
             read_only (bool, optional):  Opens dataset in read-only mode if True. Defaults to False.
-            ingestion_batch_size (int): Batch size used during ingestion. Defaults to 1024.
-            num_workers (int): The number of workers to use for ingesting data in parallel. Defaults to 0.
+            num_workers (int): Number of workers to use for parallel ingestion.
+            ingestion_batch_size (int): Batch size to use for parallel ingestion.
             exec_option (str): Default method for search execution. It could be either "python", "compute_engine" or "tensor_db". Defaults to "python".
                 - ``python`` - Pure-python implementation that runs on the client and can be used for data stored anywhere. WARNING: using this option with big datasets is discouraged because it can lead to memory issues.
                 - ``compute_engine`` - Performant C++ implementation of the Deep Lake Compute Engine that runs on the client and can be used for any data stored in or connected to Deep Lake. It cannot be used with in-memory or local datasets.
                 - ``tensor_db`` - Performant and fully-hosted Managed Tensor Database that is responsible for storage and query execution. Only available for data stored in the Deep Lake Managed Database. Store datasets in this database by specifying runtime = {"db_engine": True} during dataset creation.
             token (str, optional): Activeloop token, used for fetching user credentials. This is Optional, tokens are normally autogenerated. Defaults to None.
             overwrite (bool): If set to True this overwrites the Vector Store if it already exists. Defaults to False.
             verbose (bool): Whether to print summary of the dataset created. Defaults to True.
@@ -127,19 +127,21 @@
         self.embedding_function = embedding_function
         self.exec_option = exec_option
         self.verbose = verbose
         self.tensor_params = tensor_params
 
     def add(
         self,
-        embedding_function: Optional[Callable] = None,
-        embedding_data: Optional[List] = None,
-        embedding_tensor: Optional[str] = None,
+        embedding_function: Optional[Union[Callable, List[Callable]]] = None,
+        embedding_data: Optional[Union[List, List[List]]] = None,
+        embedding_tensor: Optional[Union[str, List[str]]] = None,
         total_samples_processed: int = 0,
         return_ids: bool = False,
+        num_workers: Optional[int] = None,
+        ingestion_batch_size: Optional[int] = None,
         **tensors,
     ) -> Optional[List[str]]:
         """Adding elements to deeplake vector store.
 
         Tensor names are specified as parameters, and data for each tensor is specified as parameter values. All data must of equal length.
 
         Examples:
@@ -178,14 +180,16 @@
 
         Args:
             embedding_function (Optional[Callable]): embedding function used to convert ``embedding_data`` into embeddings. Overrides the ``embedding_function`` specified when initializing the Vector Store.
             embedding_data (Optional[List]): Data to be converted into embeddings using the provided ``embedding_function``. Defaults to None.
             embedding_tensor (Optional[str]): Tensor where results from the embedding function will be stored. If None, the embedding tensors is automatically inferred (when possible). Defaults to None.
             total_samples_processed (int): Total number of samples processed before ingestion stopped. When specified.
             return_ids (bool): Whether to return added ids as an ouput of the method. Defaults to False.
+            num_workers (int): Number of workers to use for parallel ingestion. Overrides the ``num_workers`` specified when initializing the Vector Store.
+            ingestion_batch_size (int): Batch size to use for parallel ingestion. Defaults to 1000. Overrides the ``ingestion_batch_size`` specified when initializing the Vector Store.
             **tensors: Keyword arguments where the key is the tensor name, and the value is a list of samples that should be uploaded to that tensor.
 
         Returns:
             Optional[List[str]]: List of ids if ``return_ids`` is set to True. Otherwise, None.
         """
 
         deeplake_reporter.feature_report(
@@ -201,14 +205,23 @@
         )
 
         (
             embedding_function,
             embedding_data,
             embedding_tensor,
             tensors,
+        ) = utils.parse_tensors_kwargs(
+            tensors, embedding_function, embedding_data, embedding_tensor
+        )
+
+        (
+            embedding_function,
+            embedding_data,
+            embedding_tensor,
+            tensors,
         ) = utils.parse_add_arguments(
             dataset=self.dataset,
             initial_embedding_function=self.embedding_function,
             embedding_function=embedding_function,
             embedding_data=embedding_data,
             embedding_tensor=embedding_tensor,
             **tensors,
@@ -223,16 +236,16 @@
 
         dataset_utils.extend_or_ingest_dataset(
             processed_tensors=processed_tensors,
             dataset=self.dataset,
             embedding_function=embedding_function,
             embedding_data=embedding_data,
             embedding_tensor=embedding_tensor,
-            ingestion_batch_size=self.ingestion_batch_size,
-            num_workers=self.num_workers,
+            ingestion_batch_size=ingestion_batch_size or self.ingestion_batch_size,
+            num_workers=num_workers or self.num_workers,
             total_samples_processed=total_samples_processed,
             logger=logger,
         )
 
         self.dataset.commit(allow_empty=True)
         if self.verbose:
             self.dataset.summary()
@@ -344,14 +357,18 @@
         query_emb: Optional[Union[List[float], np.ndarray[Any, Any]]] = None
         if query is None:
             query_emb = dataset_utils.get_embedding(
                 embedding,
                 embedding_data,
                 embedding_function=embedding_function or self.embedding_function,
             )
+            if isinstance(query_emb, np.ndarray):
+                assert (
+                    query_emb.ndim == 1 or query_emb.shape[0] == 1
+                ), "Query embedding must be 1-dimensional. Please consider using another embedding function for converting query string to embedding."
 
         if not return_tensors:
             return_tensors = [
                 tensor for tensor in self.dataset.tensors if tensor != embedding_tensor
             ]
 
         return vector_search.search(
@@ -480,7 +497,10 @@
     def summary(self):
         """Prints a summary of the dataset"""
         return self.dataset.summary()
 
     def __len__(self):
         """Length of the dataset"""
         return len(self.dataset)
+
+
+DeepLakeVectorStore = VectorStore
```

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/test_deeplake_vectorstore.py` & `deeplake-3.6.4/deeplake/core/vectorstore/test_deeplake_vectorstore.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import numpy as np
 import pytest
 
 import deeplake
-from deeplake.core.vectorstore.deeplake_vectorstore import DeepLakeVectorStore
+from deeplake.core.vectorstore.deeplake_vectorstore import (
+    DeepLakeVectorStore,
+    VectorStore,
+)
 from deeplake.core.vectorstore import utils
 from deeplake.tests.common import requires_libdeeplake
 from deeplake.constants import (
     DEFAULT_VECTORSTORE_TENSORS,
 )
 
 from math import isclose
@@ -21,30 +24,34 @@
 
 query_embedding = np.random.uniform(low=-10, high=10, size=(EMBEDDING_DIM)).astype(
     np.float32
 )
 
 
 def embedding_fn(text, embedding_dim=EMBEDDING_DIM):
-    return np.zeros(len(text), EMBEDDING_DIM)  # pragma: no cover
+    return np.zeros((len(text), EMBEDDING_DIM))  # pragma: no cover
 
 
 def embedding_fn2(text, embedding_dim=EMBEDDING_DIM):
     pass  # pragma: no cover
 
 
 def embedding_fn3(text, embedding_dim=EMBEDDING_DIM):
     """Returns embedding in List[np.ndarray] format"""
     return [np.zeros(embedding_dim) for i in range(len(text))]
 
 
-def test_custom_tensors():
+def embedding_fn4(text, embedding_dim=EMBEDDING_DIM):
+    return np.zeros((1, EMBEDDING_DIM))  # pragma: no cover
+
+
+def test_custom_tensors(local_path):
     # initialize vector store object:
     vector_store = DeepLakeVectorStore(
-        path="./deeplake_vector_store",
+        path=local_path,
         overwrite=True,
         tensor_params=[
             {"name": "texts_custom", "htype": "text"},
             {"name": "emb_custom", "htype": "embedding"},
         ],
     )
 
@@ -64,19 +71,19 @@
         embedding=query_embedding, exec_option="python", embedding_tensor="emb_custom"
     )
     assert len(data.keys()) == 3
     assert "texts_custom" in data.keys() and "id" in data.keys()
 
 
 @requires_libdeeplake
-def test_search_basic(hub_cloud_dev_token):
+def test_search_basic(local_path, hub_cloud_dev_token):
     """Test basic search features"""
     # Initialize vector store object and add data
     vector_store = DeepLakeVectorStore(
-        path="./deeplake_vector_store",
+        path=local_path,
         overwrite=True,
         token=hub_cloud_dev_token,
     )
     vector_store.add(embedding=embeddings, text=texts, metadata=metadatas)
 
     # Check that default option works
     data_default = vector_store.search(
@@ -373,27 +380,27 @@
             for i in range(len(data_ce["score"]))
         ]
     )
     assert data_ce["text"] == data_db["text"]
     assert data_ce["ids"] == data_db["ids"]
 
 
-def test_delete(capsys):
+def test_delete(local_path, capsys):
     # initialize vector store object:
     vector_store = DeepLakeVectorStore(
-        path="./deeplake_vector_store",
+        path=local_path,
         overwrite=True,
         verbose=False,
     )
 
     # add data to the dataset:
     vector_store.add(id=ids, embedding=embeddings, text=texts, metadata=metadatas)
 
     output = (
-        "Dataset(path='./deeplake_vector_store', tensors=['embedding', 'id', 'metadata', 'text'])\n\n"
+        f"Dataset(path='{local_path}', tensors=['embedding', 'id', 'metadata', 'text'])\n\n"
         "  tensor      htype      shape     dtype  compression\n"
         "  -------    -------    -------   -------  ------- \n"
         " embedding  embedding  (10, 100)  float32   None   \n"
         "    id        text      (10, 1)     str     None   \n"
         " metadata     json      (10, 1)     str     None   \n"
         "   text       text      (10, 1)     str     None   \n"
     )
@@ -416,21 +423,21 @@
         vector_store.delete()
 
     tensors_before_delete = vector_store.dataset.tensors
     vector_store.delete(delete_all=True)
     assert len(vector_store.dataset) == 0
     assert vector_store.dataset.tensors.keys() == tensors_before_delete.keys()
 
-    vector_store.delete_by_path("./deeplake_vector_store")
+    vector_store.delete_by_path(local_path)
     dirs = os.listdir("./")
-    assert "./deeplake_vector_store" not in dirs
+    assert local_path not in dirs
 
     # backwards compatibility test:
     vector_store = DeepLakeVectorStore(
-        path="./deeplake_vector_store",
+        path=local_path,
         overwrite=True,
         tensor_params=[
             {
                 "name": "ids",
                 "htype": "text",
             },
             {
@@ -442,44 +449,44 @@
     # add data to the dataset:
     vector_store.add(ids=ids, docs=texts)
 
     # delete the data in the dataset by id:
     vector_store.delete(row_ids=[0])
     assert len(vector_store.dataset) == NUMBER_OF_DATA - 1
 
-    ds = deeplake.empty("local_ds", overwrite=True)
+    ds = deeplake.empty(local_path, overwrite=True)
     ds.create_tensor("ids", htype="text")
     ds.create_tensor("embedding", htype="embedding")
     ds.extend(
         {
             "ids": ids,
             "embedding": embeddings,
         }
     )
 
     vector_store = DeepLakeVectorStore(
-        path="local_ds",
+        path=local_path,
     )
     vector_store.delete(ids=ids[:3])
     assert len(vector_store) == NUMBER_OF_DATA - 3
 
     with pytest.raises(ValueError):
         vector_store.delete(ids=ids[5:7], exec_option="remote_tensor_db")
 
 
-def test_ingestion(capsys):
+def test_ingestion(local_path, capsys):
     # create data
     number_of_data = 1000
     texts, embeddings, ids, metadatas, _ = utils.create_data(
         number_of_data=number_of_data, embedding_dim=EMBEDDING_DIM
     )
 
     # initialize vector store object:
     vector_store = DeepLakeVectorStore(
-        path="./deeplake_vector_store",
+        path=local_path,
         overwrite=True,
         verbose=True,
     )
 
     with pytest.raises(Exception):
         # add data to the dataset:
         vector_store.add(
@@ -499,15 +506,15 @@
             something=texts[: number_of_data - 2],
         )
 
     vector_store.add(embedding=embeddings, text=texts, id=ids, metadata=metadatas)
     captured = capsys.readouterr()
 
     output = (
-        "Dataset(path='./deeplake_vector_store', tensors=['embedding', 'id', 'metadata', 'text'])\n\n"
+        f"Dataset(path='{local_path}', tensors=['embedding', 'id', 'metadata', 'text'])\n\n"
         "  tensor      htype       shape      dtype  compression\n"
         "  -------    -------     -------    -------  ------- \n"
         " embedding  embedding  (1000, 100)  float32   None   \n"
         "    id        text      (1000, 1)     str     None   \n"
         " metadata     json      (1000, 1)     str     None   \n"
         "   text       text      (1000, 1)     str     None   \n"
     )
@@ -533,15 +540,15 @@
         text=texts,
         id=ids,
         metadata=metadatas,
     )
     captured = capsys.readouterr()
 
     output = (
-        "Dataset(path='./deeplake_vector_store', tensors=['embedding', 'id', 'metadata', 'text'])\n\n"
+        f"Dataset(path='{local_path}', tensors=['embedding', 'id', 'metadata', 'text'])\n\n"
         "  tensor      htype       shape      dtype  compression\n"
         "  -------    -------     -------    -------  ------- \n"
         " embedding  embedding  (2000, 100)  float32   None   \n"
         "    id        text      (2000, 1)     str     None   \n"
         " metadata     json      (2000, 1)     str     None   \n"
         "   text       text      (2000, 1)     str     None   \n"
     )
@@ -560,15 +567,15 @@
         text=25 * texts,
         id=25 * ids,
         metadata=25 * metadatas,
     )
     captured = capsys.readouterr()
 
     output = (
-        "Dataset(path='./deeplake_vector_store', tensors=['embedding', 'id', 'metadata', 'text'])\n\n"
+        f"Dataset(path='{local_path}', tensors=['embedding', 'id', 'metadata', 'text'])\n\n"
         "  tensor      htype       shape       dtype  compression\n"
         "  -------    -------     -------     -------  ------- \n"
         " embedding  embedding  (27000, 100)  float32   None   \n"
         "    id        text      (27000, 1)     str     None   \n"
         " metadata     json      (27000, 1)     str     None   \n"
         "   text       text      (27000, 1)     str     None   \n"
     )
@@ -578,43 +585,43 @@
         "embedding",
         "id",
         "metadata",
         "text",
     ]
 
 
-def test_ingestion_images():
+def test_ingestion_images(local_path):
     tensor_params = [
         {"name": "image", "htype": "image", "sample_compression": "jpg"},
         {"name": "embedding", "htype": "embedding"},
     ]
 
     append_images = images
     append_images[0] = np.random.randint(0, 255, (100, 100, 3)).astype(
         np.uint8
     )  # Mix paths and images
 
     # initialize vector store object:
     vector_store = DeepLakeVectorStore(
-        path="./deeplake_vector_store",
+        path=local_path,
         tensor_params=tensor_params,
         overwrite=True,
         verbose=True,
     )
 
     ids = vector_store.add(image=images, embedding=embeddings, return_ids=True)
 
     assert "image" in vector_store.dataset.tensors
     assert "embedding" in vector_store.dataset.tensors
     assert len(vector_store.dataset.image[0].numpy().shape) == 3
     assert len(vector_store.dataset.image[1].numpy().shape) == 3
     assert len(ids) == 10
 
 
-def test_parse_add_arguments():
+def test_parse_add_arguments(local_path):
     deeplake_vector_store = DeepLakeVectorStore(
         path="mem://dummy",
         overwrite=True,
         embedding_function=embedding_fn,
     )
 
     with pytest.raises(ValueError):
@@ -763,16 +770,16 @@
         embedding_function=embedding_fn2,
         embedding_data=texts,
         embedding_tensor="embedding",
         text=texts,
         id=ids,
         metadata=metadatas,
     )
-    assert embedding_function is embedding_fn2
-    assert embedding_tensors == "embedding"
+    assert embedding_function[0] is embedding_fn2
+    assert embedding_tensors == ["embedding"]
     assert tensors == {
         "id": ids,
         "text": texts,
         "metadata": metadatas,
     }
 
     (
@@ -784,16 +791,16 @@
         dataset=deeplake_vector_store.dataset,
         embedding_function=embedding_fn2,
         embedding_data="text",
         embedding_tensor="embedding",
         text=texts,
         metadata=metadatas,
     )
-    assert embedding_function is embedding_fn2
-    assert embedding_tensors == "embedding"
+    assert embedding_function[0] is embedding_fn2
+    assert embedding_tensors == ["embedding"]
     assert len(tensors) == 2
 
     # Creating a vector store with two embedding tensors
     deeplake_vector_store = DeepLakeVectorStore(
         path="mem://dummy",
         overwrite=True,
         embedding_function=embedding_fn,
@@ -870,16 +877,16 @@
     ) = utils.parse_add_arguments(
         dataset=deeplake_vector_store.dataset,
         embedding_function=embedding_fn2,
         embedding_data=texts,
         text=texts,
     )
 
-    assert embedding_function is embedding_fn2
-    assert embedding_tensors == "embedding_1"
+    assert embedding_function[0] is embedding_fn2
+    assert embedding_tensors == ["embedding_1"]
     assert len(tensors) == 1
 
     deeplake_vector_store = DeepLakeVectorStore(
         path="mem://dummy",
         overwrite=True,
         embedding_function=embedding_fn,
     )
@@ -894,17 +901,17 @@
         initial_embedding_function=embedding_fn,
         text=texts,
         id=ids,
         metadata=metadatas,
         embedding_data=texts,
         embedding_tensor="embedding",
     )
-    assert embedding_function is embedding_fn
-    assert embedding_tensor == "embedding"
-    assert embedding_data == texts
+    assert embedding_function[0] is embedding_fn
+    assert embedding_tensor == ["embedding"]
+    assert embedding_data == [texts]
     assert tensors == {
         "id": ids,
         "text": texts,
         "metadata": metadatas,
     }
 
     with pytest.raises(ValueError):
@@ -947,15 +954,15 @@
             id=ids,
             metadata=metadatas,
             embedding=embeddings,
             new_tensor=texts,
         )
 
     with pytest.raises(ValueError):
-        dataset = deeplake.empty("local_ds", overwrite=True)
+        dataset = deeplake.empty(local_path, overwrite=True)
         dataset.create_tensor("embedding_1", htype="embedding")
         dataset.create_tensor("embedding_2", htype="embedding")
         dataset.create_tensor("id", htype="text")
         dataset.create_tensor("text", htype="text")
         dataset.create_tensor("metadata", htype="json")
 
         dataset.extend(
@@ -978,7 +985,163 @@
             text=texts,
             id=ids,
             metadata=metadatas,
             embedding_data=texts,
             embedding_function=embedding_fn3,
             embedding_2=embeddings,
         )
+
+
+def test_parse_tensors_kwargs():
+    tensors = {
+        "embedding_1": (embedding_fn, texts),
+        "embedding_2": (embedding_fn2, texts),
+        "custom_text": texts,
+    }
+    func, data, emb_tensor, new_tensors = utils.parse_tensors_kwargs(
+        tensors, None, None, None
+    )
+
+    assert func == [embedding_fn, embedding_fn2]
+    assert data == [texts, texts]
+    assert emb_tensor == ["embedding_1", "embedding_2"]
+    assert new_tensors == {"custom_text": texts}
+
+    with pytest.raises(ValueError):
+        utils.parse_tensors_kwargs(tensors, embedding_fn, None, None)
+
+    with pytest.raises(ValueError):
+        utils.parse_tensors_kwargs(tensors, None, texts, None)
+
+    with pytest.raises(ValueError):
+        utils.parse_tensors_kwargs(tensors, None, None, "embedding_1")
+
+
+def test_multiple_embeddings(local_path, capsys):
+    vector_store = DeepLakeVectorStore(
+        path=local_path,
+        overwrite=True,
+        tensor_params=[
+            {
+                "name": "text",
+                "htype": "text",
+            },
+            {
+                "name": "embedding_1",
+                "htype": "embedding",
+            },
+            {
+                "name": "embedding_2",
+                "htype": "embedding",
+            },
+        ],
+    )
+
+    with pytest.raises(AssertionError):
+        vector_store.add(
+            text=texts,
+            embedding_function=[embedding_fn, embedding_fn],
+            embedding_data=[texts],
+            embedding_tensor=["embedding_1", "embedding_2"],
+        )
+
+    with pytest.raises(AssertionError):
+        vector_store.add(
+            text=texts,
+            embedding_function=[embedding_fn, embedding_fn],
+            embedding_data=[texts, texts],
+            embedding_tensor=["embedding_1"],
+        )
+
+    with pytest.raises(AssertionError):
+        vector_store.add(
+            text=texts,
+            embedding_function=[embedding_fn],
+            embedding_data=[texts, texts],
+            embedding_tensor=["embedding_1", "embedding_2"],
+        )
+
+    vector_store.add(
+        text=texts,
+        embedding_function=[embedding_fn, embedding_fn],
+        embedding_data=[texts, texts],
+        embedding_tensor=["embedding_1", "embedding_2"],
+    )
+    vector_store.add(
+        text=texts, embedding_1=(embedding_fn, texts), embedding_2=(embedding_fn, texts)
+    )
+    vector_store.add(
+        text=texts,
+        embedding_function=embedding_fn,
+        embedding_data=[texts, texts],
+        embedding_tensor=["embedding_1", "embedding_2"],
+    )
+
+    # test with initial embedding function
+    vector_store.embedding_function = embedding_fn
+    vector_store.add(
+        text=texts,
+        embedding_data=[texts, texts],
+        embedding_tensor=["embedding_1", "embedding_2"],
+    )
+
+    number_of_data = 1000
+    _texts, embeddings, ids, metadatas, _ = utils.create_data(
+        number_of_data=number_of_data, embedding_dim=EMBEDDING_DIM
+    )
+    vector_store.add(
+        text=25 * _texts,
+        embedding_function=[embedding_fn3, embedding_fn3],
+        embedding_data=[25 * _texts, 25 * _texts],
+        embedding_tensor=["embedding_1", "embedding_2"],
+    )
+    vector_store.add(
+        text=25 * _texts,
+        embedding_1=(embedding_fn3, 25 * _texts),
+        embedding_2=(embedding_fn3, 25 * _texts),
+    )
+
+    assert len(vector_store.dataset) == 50040
+    assert len(vector_store.dataset.embedding_1) == 50040
+    assert len(vector_store.dataset.embedding_2) == 50040
+    assert len(vector_store.dataset.id) == 50040
+    assert len(vector_store.dataset.text) == 50040
+
+
+def test_extend_none(local_path):
+    vector_store = DeepLakeVectorStore(
+        path=local_path,
+        overwrite=True,
+        tensor_params=[
+            {"name": "text", "htype": "text"},
+            {"name": "embedding", "htype": "embedding"},
+            {
+                "name": "id",
+                "htype": "text",
+            },
+            {"name": "metadata", "htype": "json"},
+        ],
+    )
+
+    vector_store.add(text=texts, embedding=None, id=ids, metadata=None)
+    assert len(vector_store.dataset) == 10
+    assert len(vector_store.dataset.text) == 10
+    assert len(vector_store.dataset.embedding) == 10
+    assert len(vector_store.dataset.id) == 10
+    assert len(vector_store.dataset.metadata) == 10
+
+
+def test_query_dim(local_path):
+    vector_store = DeepLakeVectorStore(
+        path=local_path,
+        overwrite=True,
+        tensor_params=[
+            {"name": "text", "htype": "text"},
+            {"name": "embedding", "htype": "embedding"},
+        ],
+    )
+
+    vector_store.add(text=texts, embedding=embeddings)
+    with pytest.raises(AssertionError):
+        vector_store.search([texts[0], texts[0]], embedding_fn3, k=1)
+
+    vector_store.search([texts[0]], embedding_fn4, k=1)
```

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/dataset/dataset.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/dataset/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import uuid
 from typing import List, Dict, Any
 
 import numpy as np
+from math import ceil
 
 try:
     from indra import api  # type: ignore
 
     _INDRA_INSTALLED = True  # pragma: no cover
 except ImportError:  # pragma: no cover
     _INDRA_INSTALLED = False  # pragma: no cover
@@ -15,16 +16,16 @@
 from deeplake.core.vectorstore.vector_search import utils
 from deeplake.core.vectorstore.vector_search import dataset as dataset_utils
 from deeplake.core.vectorstore.vector_search.ingestion import ingest_data
 from deeplake.constants import (
     DEFAULT_VECTORSTORE_DEEPLAKE_PATH,
     VECTORSTORE_EXTEND_MAX_SIZE,
     DEFAULT_VECTORSTORE_TENSORS,
+    VECTORSTORE_EXTEND_MAX_SIZE_BY_HTYPE,
 )
-from deeplake.util.warnings import always_warn
 
 
 def create_or_load_dataset(
     tensor_params,
     dataset_path,
     token,
     creds,
@@ -230,34 +231,40 @@
 
     return embedding
 
 
 def preprocess_tensors(
     embedding_data=None, embedding_tensor=None, dataset=None, **tensors
 ):
-    first_item = next(iter(tensors))
-    ids_tensor = "ids" if "ids" in tensors else "id"
-    if ids_tensor not in tensors or ids_tensor is None:
-        id = [str(uuid.uuid1()) for _ in tensors[first_item]]
+    # generate id list equal to the length of the tensors
+    # dont use None tensors to get length of tensor
+    _tensors = {k: v for k, v in tensors.items() if v is not None}
+    first_item = next(iter(_tensors))
+    ids_tensor = "ids" if "ids" in _tensors else "id"
+    if ids_tensor not in _tensors or ids_tensor is None:
+        id = [str(uuid.uuid1()) for _ in _tensors[first_item]]
         tensors[ids_tensor] = id
 
     processed_tensors = {ids_tensor: tensors[ids_tensor]}
 
     for tensor_name, tensor_data in tensors.items():
-        if not isinstance(tensor_data, list):
+        if tensor_data is None:
+            tensor_data = [None] * len(tensors[ids_tensor])
+        elif not isinstance(tensor_data, list):
             tensor_data = list(tensor_data)
         if dataset and dataset[tensor_name].htype == "image":
             tensor_data = [
                 deeplake.read(data) if isinstance(data, str) else data
                 for data in tensor_data
             ]
         processed_tensors[tensor_name] = tensor_data
 
     if embedding_data:
-        processed_tensors[embedding_tensor] = embedding_data
+        for k, v in zip(embedding_tensor, embedding_data):
+            processed_tensors[k] = v
 
     return processed_tensors, tensors[ids_tensor]
 
 
 def create_elements(
     processed_tensors: Dict[str, List[Any]],
 ):
@@ -312,24 +319,45 @@
     embedding_data,
     ingestion_batch_size,
     num_workers,
     total_samples_processed,
     logger,
 ):
     first_item = next(iter(processed_tensors))
-    if len(processed_tensors[first_item]) <= VECTORSTORE_EXTEND_MAX_SIZE:
+
+    htypes = [
+        dataset[item].meta.htype for item in dataset.tensors
+    ]  # Inspect raw htype (not parsed htype like tensor.htype) in order to avoid parsing links and sequences separately.
+    threshold_by_htype = [
+        VECTORSTORE_EXTEND_MAX_SIZE_BY_HTYPE.get(h, int(1e10)) for h in htypes
+    ]
+    extend_threshold = min(threshold_by_htype + [VECTORSTORE_EXTEND_MAX_SIZE])
+
+    if len(processed_tensors[first_item]) <= extend_threshold:
         if embedding_function:
-            embedded_data = embedding_function(embedding_data)
-            embedded_data = np.array(embedded_data, dtype=np.float32)
-            processed_tensors[embedding_tensor] = embedded_data
+            for func, data, tensor in zip(
+                embedding_function, embedding_data, embedding_tensor
+            ):
+                embedded_data = func(data)
+                embedded_data = np.array(embedded_data, dtype=np.float32)
+                processed_tensors[tensor] = embedded_data
 
         dataset.extend(processed_tensors)
     else:
         elements = dataset_utils.create_elements(processed_tensors)
 
+        num_workers_auto = ceil(len(elements) / ingestion_batch_size)
+        if num_workers_auto < num_workers:
+            logger.warning(
+                f"Number of workers is {num_workers}, but {len(elements)} rows of data are being added and the ingestion_batch_size is {ingestion_batch_size}. "
+                f"Setting the number of workers to {num_workers_auto} instead, in order reduce overhead from excessive workers that will not accelerate ingestion."
+                f"If you want to parallelizing using more workers, please reduce ``ingestion_batch_size``."
+            )
+            num_workers = min(num_workers_auto, num_workers)
+
         ingest_data.run_data_ingestion(
             elements=elements,
             dataset=dataset,
             embedding_function=embedding_function,
             embedding_tensor=embedding_tensor,
             ingestion_batch_size=ingestion_batch_size,
             num_workers=num_workers,
```

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/filter/filter.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/filter/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/filter/test_filter.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/filter/test_filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/query.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/test_indra.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/test_indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/vector_search.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/indra/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 
 class DataIngestion:
     def __init__(
         self,
         elements: List[Dict[str, Any]],
         dataset: DeepLakeDataset,
-        embedding_function: Optional[Callable],
-        embedding_tensor: Optional[str],
+        embedding_function: Optional[List[Callable]],
+        embedding_tensor: Optional[List[str]],
         ingestion_batch_size: int,
         num_workers: int,
         retry_attempt: int,
         total_samples_processed: int,
         logger,
     ):
         self.elements = elements
@@ -153,22 +153,24 @@
     sample_out: list,
     embedding_function,
     embedding_tensor,
 ) -> None:
     embeds: List[Optional[np.ndarray]] = [None] * len(sample_in)
     if embedding_function:
         try:
-            embedding_data = [s[embedding_tensor] for s in sample_in]
-            embeddings = embedding_function(embedding_data)
+            for func, tensor in zip(embedding_function, embedding_tensor):
+                embedding_data = [s[tensor] for s in sample_in]
+                embeddings = func(embedding_data)
         except Exception as e:
             raise Exception(
                 "Could not use embedding function. Please try again with a different embedding function."
             )
         embeds = [np.array(e, dtype=np.float32) for e in embeddings]
 
     for s, emb in zip(sample_in, embeds):
         sample_in_i = {tensor_name: s[tensor_name] for tensor_name in s}
 
         if embedding_function:
-            sample_in_i[embedding_tensor] = np.array(emb, dtype=np.float32)
+            for tensor in embedding_tensor:
+                sample_in_i[tensor] = np.array(emb, dtype=np.float32)
 
         sample_out.append(sample_in_i)
```

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 
 
 def run_data_ingestion(
     elements: List[Dict[str, Any]],
     dataset: DeepLakeDataset,
     ingestion_batch_size: int,
     num_workers: int,
-    embedding_function: Optional[Callable] = None,
-    embedding_tensor: Optional[str] = None,
+    embedding_function: Optional[List[Callable]] = None,
+    embedding_tensor: Optional[List[str]] = None,
     retry_attempt: int = 0,
     total_samples_processed: int = 0,
     logger: Optional[logging.Logger] = None,
 ):
     """Running data ingestion into deeplake dataset.
 
     Args:
         elements (List[Dict[str, Any]]): List of dictionaries. Each dictionary contains mapping of
             names of 4 tensors (i.e. "embedding", "metadata", "ids", "text") to their corresponding values.
         dataset (DeepLakeDataset): deeplake dataset object.
-        embedding_function (Optional[Callable]): function used to convert query into an embedding.
-        embedding_tensor (Optional[str]) : tensor name where embedded data will be stored. Defaults to None.
+        embedding_function (Optional, List[Callable]]): function used to convert query into an embedding.
+        embedding_tensor (Optional, List[str]) : tensor name where embedded data will be stored. Defaults to None.
         ingestion_batch_size (int): The batch size to use during ingestion.
         num_workers (int): The number of workers to use for ingesting data in parallel.
         retry_attempt (int): The number of retry attempts already passed.
         total_samples_processed (int): The number of samples processed before transforms stopped. Defaults to 0.
         logger (Optional[logging.Logger]): logger where all warnings are logged. Defaults to None.
     """
```

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def corrupted_embedding_function(emb, threshold):
     p = random.uniform(0, 1)
     if p > threshold:
         raise Exception("CorruptedEmbeddingFunction")
     return np.zeros((len(emb), 1536), dtype=np.float32)
 
 
-def test_ingest_data():
+def test_ingest_data(local_path):
     data = [
         {
             "text": "a",
             "id": np.int64(1),
             "metadata": {"a": 1},
             "embedding": np.array([0.1, 0.2, 0.3, 0.4], dtype=np.float32),
         },
@@ -45,15 +45,15 @@
             "text": "d",
             "id": np.int64(4),
             "metadata": {"d": 4},
             "embedding": np.array([0.1, 0.2, 0.3, 0.4], dtype=np.float32),
         },
     ]
 
-    dataset = deeplake.empty("./xyzabc", overwrite=True)
+    dataset = deeplake.empty(local_path, overwrite=True)
     dataset.create_tensor(
         "text",
         htype="text",
         create_id_tensor=False,
         create_sample_info_tensor=False,
         create_shape_tensor=False,
         chunk_compression="lz4",
@@ -118,31 +118,31 @@
             "metadata": {"d": 4},
         },
     ]
 
     ingest_data.run_data_ingestion(
         dataset=dataset,
         elements=extended_data,
-        embedding_function=embedding_function,
+        embedding_function=[embedding_function],
         ingestion_batch_size=1024,
         num_workers=2,
-        embedding_tensor="embedding",
+        embedding_tensor=["embedding"],
     )
     assert len(dataset) == 20008
 
     extended_data = extended_data * 10
     embedding_function = partial(corrupted_embedding_function, threshold=0.95)
     with pytest.raises(FailedIngestionError):
         ingest_data.run_data_ingestion(
             dataset=dataset,
             elements=extended_data,
-            embedding_function=embedding_function,
+            embedding_function=[embedding_function],
             ingestion_batch_size=1024,
             num_workers=2,
-            embedding_tensor="embedding",
+            embedding_tensor=["embedding"],
         )
 
     with pytest.raises(FailedIngestionError):
         data = [
             {
                 "text": "a",
                 "id": np.int64(1),
@@ -165,22 +165,22 @@
         )
 
     extended_data = extended_data * 10
     with pytest.raises(FailedIngestionError):
         ingest_data.run_data_ingestion(
             dataset=dataset,
             elements=extended_data,
-            embedding_function=embedding_function,
+            embedding_function=[embedding_function],
             ingestion_batch_size=1024,
             num_workers=2,
-            embedding_tensor="embedding",
+            embedding_tensor=["embedding"],
         )
 
     with pytest.raises(ValueError):
         ingest_data.run_data_ingestion(
             dataset=dataset,
             elements=extended_data,
-            embedding_function=corrupted_embedding_function,
+            embedding_function=[corrupted_embedding_function],
             ingestion_batch_size=0,
             num_workers=2,
-            embedding_tensor="embedding",
+            embedding_tensor=["embedding"],
         )
```

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/search_algorithm.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/test_vector_search.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/test_vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/vector_search.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/python/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/utils.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,17 +12,15 @@
     "compute_engine": None,
     "python": None,
     "tensor_db": {"db_engine": True},
 }
 
 
 def parse_tensor_return(tensor):
-    data = tensor.data()["value"]
-
-    return data.tolist() if isinstance(data, np.ndarray) else data
+    return tensor.data(aslist=True)["value"]
 
 
 def check_indra_installation(exec_option, indra_installed):
     if exec_option == "compute_engine" and not indra_installed:
         raise raise_indra_installation_error(
             indra_import_error=False
         )  # pragma: no cover
@@ -135,44 +133,108 @@
 
         if kwargs["return_tensors"] and kwargs["query"]:
             raise ValueError(
                 f"return_tensors and query parameters cannot be specified simultaneously, becuase the data that is returned is directly specified in the query."
             )
 
 
+def parse_tensors_kwargs(tensors, embedding_function, embedding_data, embedding_tensor):
+    tensors = tensors.copy()
+
+    # embedding_tensor = (embedding_function, embedding_data) syntax
+    func_comma_data_style = (
+        lambda item: isinstance(item[1], tuple)
+        and len(item[1]) == 2
+        and callable(item[1][0])
+    )
+
+    funcs = []
+    data = []
+    tensors_ = []
+
+    filtered = dict(filter(func_comma_data_style, tensors.items()))
+
+    # cannot use both syntaxes (kwargs style and args style) at the same time
+    if len(filtered) > 0:
+        if embedding_function:
+            raise ValueError(
+                "Cannot specify embedding functions in both `tensors` and `embedding_function`."
+            )
+
+        if embedding_data:
+            raise ValueError(
+                "Cannot specify embedding data in both `tensors` and `embedding_data`."
+            )
+
+        if embedding_tensor:
+            raise ValueError(
+                "Cannot specify embedding tensors in both `tensors` and `embedding_tensor`."
+            )
+    else:
+        return embedding_function, embedding_data, embedding_tensor, tensors
+
+    # separate embedding functions, data and tensors
+    for k, v in filtered.items():
+        funcs.append(v[0])
+        data.append(v[1])
+        tensors_.append(k)
+        # remove embedding tensors (tuple format) from tensors
+        del tensors[k]
+
+    return funcs, data, tensors_, tensors
+
+
 def parse_add_arguments(
     dataset,
     embedding_function=None,
     initial_embedding_function=None,
     embedding_data=None,
     embedding_tensor=None,
     **tensors,
 ):
     """Parse the input argument to the Vector Store add function to infer whether they are a valid combination."""
+    if embedding_data and not isinstance(next(iter(embedding_data)), list):
+        embedding_data = [embedding_data]
+    if embedding_tensor and not isinstance(embedding_tensor, list):
+        embedding_tensor = [embedding_tensor]
 
     if embedding_function:
         if not embedding_data:
             raise ValueError(
                 f"embedding_data is not specified. When using embedding_function it is also necessary to specify the data that you want to embed"
             )
 
-        embedding_tensor = find_embedding_tensor(embedding_tensor, tensors, dataset)
+        # if single embedding function is specified, use it for all embedding data
+        if not isinstance(embedding_function, list):
+            embedding_function = [embedding_function] * len(embedding_data)
+
+        embedding_tensor = get_embedding_tensors(embedding_tensor, tensors, dataset)
+
+        assert len(embedding_function) == len(
+            embedding_data
+        ), "embedding_function and embedding_data must be of the same length"
+        assert len(embedding_function) == len(
+            embedding_tensor
+        ), "embedding_function and embedding_tensor must be of the same length"
 
         check_tensor_name_consistency(tensors, dataset.tensors, embedding_tensor)
         return (embedding_function, embedding_data, embedding_tensor, tensors)
 
     if initial_embedding_function:
         if not embedding_data:
             check_tensor_name_consistency(tensors, dataset.tensors, None)
             return (None, None, None, tensors)
 
-        embedding_tensor = find_embedding_tensor(embedding_tensor, tensors, dataset)
+        if not isinstance(initial_embedding_function, list):
+            initial_embedding_function = [initial_embedding_function] * len(
+                embedding_data
+            )
 
+        embedding_tensor = get_embedding_tensors(embedding_tensor, tensors, dataset)
         check_tensor_name_consistency(tensors, dataset.tensors, embedding_tensor)
-
         return (initial_embedding_function, embedding_data, embedding_tensor, tensors)
 
     if embedding_tensor:
         raise ValueError(
             f"`embedding_tensor` is specified while `embedding_function` is not specified. "
             "Either specify `embedding_function` during Vector Store initialization or during `add` call."
         )
@@ -187,15 +249,17 @@
     return (None, None, None, tensors)
 
 
 def check_tensor_name_consistency(tensors, dataset_tensors, embedding_tensor):
     """Check if the tensors specified in the add function are consistent with the tensors in the dataset and the automatically generated tensors (like id)"""
     id_str = "ids" if "ids" in dataset_tensors else "id"
     expected_tensor_length = len(dataset_tensors)
-    allowed_missing_tensors = [id_str, embedding_tensor]
+    if embedding_tensor is None:
+        embedding_tensor = []
+    allowed_missing_tensors = [id_str, *embedding_tensor]
 
     for allowed_missing_tensor in allowed_missing_tensors:
         if allowed_missing_tensor not in tensors and allowed_missing_tensor is not None:
             expected_tensor_length -= 1
 
     for tensor in tensors:
         if tensor not in dataset_tensors:
@@ -209,36 +273,38 @@
             if tensor not in tensors and tensor not in allowed_missing_tensors:
                 missing_tensors += f"`{tensor}`, "
         missing_tensors = missing_tensors[:-2]
 
         raise ValueError(f"{missing_tensors} tensor(s) is/are missing.")
 
 
-def find_embedding_tensor(embedding_tensor, tensor_args, dataset) -> str:
-    """Find the single embedding tensor to which embedding data should be uploaded. If there are none or multiple tensors, or if overlaps with the existing tensor arguments, raise an error."""
-
+def get_embedding_tensors(embedding_tensor, tensor_args, dataset) -> List[str]:
+    """Get the embedding tensors to which embedding data should be uploaded."""
     if not embedding_tensor:
-        embedding_tensors = find_embedding_tensors(dataset)
+        embedding_tensor = find_embedding_tensors(dataset)
 
-        if len(embedding_tensors) >= 2:
+        if len(embedding_tensor) == 0:
             raise ValueError(
-                f"embedding_function is specified but multiple embedding tensors were found in the Vector Store, so it it not clear to which tensor the embeddings should be appended. Please specify the `embedding_tensor` parameter for storing the embeddings."
+                f"embedding_function is specified but no embedding tensors were found in the Vector Store,"
+                " so the embeddings cannot be added. Please specify the `embedding_tensor` parameter for storing the embeddings."
             )
-        elif len(embedding_tensors) == 0:
+        elif len(embedding_tensor) > 1:
             raise ValueError(
-                f"embedding_function is specified but no embedding tensors were found in the Vector Store, so the embeddings cannot be added. Please specify the `embedding_tensor` parameter for storing the embeddings."
+                f"embedding_function is specified but multiple embedding tensors were found in the Vector Store,"
+                " so it is not clear to which tensor the embeddings should be added. Please specify the `embedding_tensor`"
+                " parameter for storing the embeddings."
             )
 
-        embedding_tensor = embedding_tensors[0]
-
-    if embedding_tensor in tensor_args:
-        raise ValueError(
-            f"{embedding_tensor} was specified as a tensor parameter for adding data, in addition to being specified as the `embedding_tensor' for storing embedding from the embedding_function."
-            f"Either `embedding_function` or `embedding_data` shouldn't be specified or `{embedding_tensor}` shouldn't be specified as a tensor for appending data."
-        )
+    # if same tensor is specified in both embedding_tensor and tensors, raise error
+    for tensor in embedding_tensor:
+        if tensor_args.get(tensor):
+            raise ValueError(
+                f"{tensor} was specified as a tensor parameter for adding data, in addition to being specified as an `embedding_tensor' for storing embedding from the embedding_function."
+                f"Either `embedding_function` or `embedding_data` shouldn't be specified or `{tensor}` shouldn't be specified as a tensor for appending data."
+            )
     return embedding_tensor
 
 
 def find_embedding_tensors(dataset) -> List[str]:
     """Find all the embedding tensors in a dataset."""
     matching_tensors = []
     for tensor in dataset.tensors:
```

### Comparing `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/vector_search.py` & `deeplake-3.6.4/deeplake/core/vectorstore/vector_search/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.6.4/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/version_control/commit_diff.py` & `deeplake-3.6.4/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/version_control/commit_node.py` & `deeplake-3.6.4/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.6.4/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/version_control/test_merge.py` & `deeplake-3.6.4/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/core/version_control/test_version_control.py` & `deeplake-3.6.4/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.6.4/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/enterprise/dataloader.py` & `deeplake-3.6.4/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.6.4/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.6.4/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/enterprise/test_pytorch.py` & `deeplake-3.6.4/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/enterprise/test_query.py` & `deeplake-3.6.4/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.6.4/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/enterprise/util.py` & `deeplake-3.6.4/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/hooks.py` & `deeplake-3.6.4/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/htype.py` & `deeplake-3.6.4/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.6.4/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.6.4/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.6.4/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.6.4/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/integrations/pytorch/common.py` & `deeplake-3.6.4/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.6.4/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.6.4/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.6.4/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/integrations/tf/common.py` & `deeplake-3.6.4/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.6.4/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.6.4/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/integrations/wandb/wandb.py` & `deeplake-3.6.4/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/tests/cache_fixtures.py` & `deeplake-3.6.4/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/tests/client_fixtures.py` & `deeplake-3.6.4/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/tests/common.py` & `deeplake-3.6.4/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/tests/dataset_fixtures.py` & `deeplake-3.6.4/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/tests/path_fixtures.py` & `deeplake-3.6.4/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/tests/storage_fixtures.py` & `deeplake-3.6.4/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/access_method.py` & `deeplake-3.6.4/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/agreement.py` & `deeplake-3.6.4/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/array_list.py` & `deeplake-3.6.4/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/assert_byte_indexes.py` & `deeplake-3.6.4/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/auto.py` & `deeplake-3.6.4/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/bugout_reporter.py` & `deeplake-3.6.4/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/cache_chain.py` & `deeplake-3.6.4/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/casting.py` & `deeplake-3.6.4/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/check_latest_version.py` & `deeplake-3.6.4/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/chunk_engine.py` & `deeplake-3.6.4/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/class_label.py` & `deeplake-3.6.4/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/compute.py` & `deeplake-3.6.4/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/connect_dataset.py` & `deeplake-3.6.4/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/dataset.py` & `deeplake-3.6.4/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/diff.py` & `deeplake-3.6.4/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/downsample.py` & `deeplake-3.6.4/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/encoder.py` & `deeplake-3.6.4/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/exceptions.py` & `deeplake-3.6.4/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/exif.py` & `deeplake-3.6.4/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/from_tfds.py` & `deeplake-3.6.4/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/htype.py` & `deeplake-3.6.4/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/image.py` & `deeplake-3.6.4/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/invalid_view_op.py` & `deeplake-3.6.4/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/iteration_warning.py` & `deeplake-3.6.4/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/json.py` & `deeplake-3.6.4/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/keys.py` & `deeplake-3.6.4/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/link.py` & `deeplake-3.6.4/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/logging.py` & `deeplake-3.6.4/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/merge.py` & `deeplake-3.6.4/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/modified.py` & `deeplake-3.6.4/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/notebook.py` & `deeplake-3.6.4/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/object_3d/mesh.py` & `deeplake-3.6.4/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.6.4/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.6.4/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.6.4/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.6.4/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.6.4/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.6.4/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.6.4/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.6.4/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.6.4/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/path.py` & `deeplake-3.6.4/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/pretty_print.py` & `deeplake-3.6.4/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/remove_cache.py` & `deeplake-3.6.4/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/scheduling.py` & `deeplake-3.6.4/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/shape_interval.py` & `deeplake-3.6.4/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/spinner.py` & `deeplake-3.6.4/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/split.py` & `deeplake-3.6.4/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/storage.py` & `deeplake-3.6.4/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/tag.py` & `deeplake-3.6.4/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/tensor_db.py` & `deeplake-3.6.4/deeplake/util/tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/testing.py` & `deeplake-3.6.4/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/tests/test_auto.py` & `deeplake-3.6.4/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.6.4/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.6.4/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/tests/test_read.py` & `deeplake-3.6.4/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.6.4/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/tests/test_split.py` & `deeplake-3.6.4/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/tests/test_tensor_db.py` & `deeplake-3.6.4/deeplake/util/tests/test_tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/tests/test_version_control.py` & `deeplake-3.6.4/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/transform.py` & `deeplake-3.6.4/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/version_control.py` & `deeplake-3.6.4/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/util/video.py` & `deeplake-3.6.4/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/visualizer/video_streaming.py` & `deeplake-3.6.4/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake/visualizer/visualizer.py` & `deeplake-3.6.4/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake.egg-info/PKG-INFO` & `deeplake-3.6.4/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.6.3
+Version: 3.6.4
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.6.3 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.4 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
 Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
```

### Comparing `deeplake-3.6.3/deeplake.egg-info/SOURCES.txt` & `deeplake-3.6.4/deeplake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/deeplake.egg-info/requires.txt` & `deeplake-3.6.4/deeplake.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.3/setup.py` & `deeplake-3.6.4/setup.py`

 * *Files identical despite different names*

