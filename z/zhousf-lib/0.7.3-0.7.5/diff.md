# Comparing `tmp/zhousf-lib-0.7.3.tar.gz` & `tmp/zhousf-lib-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhousf-lib-0.7.3.tar", last modified: Wed Jun 14 09:42:39 2023, max compression
+gzip compressed data, was "zhousf-lib-0.7.5.tar", last modified: Fri Jun 16 06:03:02 2023, max compression
```

## Comparing `zhousf-lib-0.7.3.tar` & `zhousf-lib-0.7.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.455414 zhousf-lib-0.7.3/
--rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.7.3/LICENSE
--rw-rw-rw-   0        0        0     2073 2023-06-14 09:42:39.454413 zhousf-lib-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     1179 2023-06-09 06:54:16.000000 zhousf-lib-0.7.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 09:42:39.455414 zhousf-lib-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0     4289 2023-06-14 09:42:06.000000 zhousf-lib-0.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.392414 zhousf-lib-0.7.3/zhousf_lib.egg-info/
--rw-rw-rw-   0        0        0     2073 2023-06-14 09:42:39.000000 zhousf-lib-0.7.3/zhousf_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-06-14 09:42:39.000000 zhousf-lib-0.7.3/zhousf_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:42:39.000000 zhousf-lib-0.7.3/zhousf_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-14 09:42:39.000000 zhousf-lib-0.7.3/zhousf_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.393413 zhousf-lib-0.7.3/zhousflib/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.7.3/zhousflib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.394414 zhousf-lib-0.7.3/zhousflib/datasets/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.7.3/zhousflib/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.396415 zhousf-lib-0.7.3/zhousflib/datasets/classification/
--rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.7.3/zhousflib/datasets/classification/__init__.py
--rw-rw-rw-   0        0        0     4895 2023-06-13 08:58:42.000000 zhousf-lib-0.7.3/zhousflib/datasets/classification/classification_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.402414 zhousf-lib-0.7.3/zhousflib/datasets/coco/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.3/zhousflib/datasets/coco/__init__.py
--rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.7.3/zhousflib/datasets/coco/coco_bbox_extract.py
--rw-rw-rw-   0        0        0     5484 2023-06-12 06:00:08.000000 zhousf-lib-0.7.3/zhousflib/datasets/coco/coco_bbox_update.py
--rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.7.3/zhousflib/datasets/coco/coco_bbox_vis.py
--rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.7.3/zhousflib/datasets/coco/coco_dataset_merge.py
--rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.7.3/zhousflib/datasets/coco/coco_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.407414 zhousf-lib-0.7.3/zhousflib/datasets/labelme/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.3/zhousflib/datasets/labelme/__init__.py
--rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.7.3/zhousflib/datasets/labelme/labelme_clip.py
--rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.7.3/zhousflib/datasets/labelme/labelme_convert_coco.py
--rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.7.3/zhousflib/datasets/labelme/labelme_convert_seg.py
--rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.7.3/zhousflib/datasets/labelme/labelme_dataset_clip.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.408443 zhousf-lib-0.7.3/zhousflib/datasets/segmentation/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.3/zhousflib/datasets/segmentation/__init__.py
--rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.7.3/zhousflib/datasets/segmentation/seg_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.410413 zhousf-lib-0.7.3/zhousflib/db/
--rw-rw-rw-   0        0        0       62 2023-06-08 02:33:01.000000 zhousf-lib-0.7.3/zhousflib/db/__init__.py
--rw-rw-rw-   0        0        0     2345 2023-06-09 06:00:56.000000 zhousf-lib-0.7.3/zhousflib/db/lmdb_master.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.413413 zhousf-lib-0.7.3/zhousflib/decorator/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.3/zhousflib/decorator/__init__.py
--rw-rw-rw-   0        0        0      466 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/decorator/except_util.py
--rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/decorator/interceptor_util.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.427413 zhousf-lib-0.7.3/zhousflib/font/
--rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.7.3/zhousflib/font/SimSun.ttf
--rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.7.3/zhousflib/font/Symbola.ttf
--rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.7.3/zhousflib/font/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.429414 zhousf-lib-0.7.3/zhousflib/locust/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/locust/__init__.py
--rw-rw-rw-   0        0        0     1544 2023-06-09 06:20:55.000000 zhousf-lib-0.7.3/zhousflib/locust/locust_demo.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.432414 zhousf-lib-0.7.3/zhousflib/pandas/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.7.3/zhousflib/pandas/__init__.py
--rw-rw-rw-   0        0        0     3768 2023-06-14 09:41:15.000000 zhousf-lib-0.7.3/zhousflib/pandas/openpyxl_util.py
--rw-rw-rw-   0        0        0     5833 2023-06-14 09:41:15.000000 zhousf-lib-0.7.3/zhousflib/pandas/pandas_util.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.435441 zhousf-lib-0.7.3/zhousflib/pdf/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/pdf/__init__.py
--rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/pdf/export_image.py
--rw-rw-rw-   0        0        0     1467 2023-06-08 02:34:30.000000 zhousf-lib-0.7.3/zhousflib/pdf/pdfplumber_util.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.449413 zhousf-lib-0.7.3/zhousflib/util/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/util/__init__.py
--rw-rw-rw-   0        0        0     2770 2023-06-07 01:49:13.000000 zhousf-lib-0.7.3/zhousflib/util/calculater_util.py
--rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/util/cv_util.py
--rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.7.3/zhousflib/util/encrypt_util.py
--rw-rw-rw-   0        0        0     1592 2023-06-14 06:14:27.000000 zhousf-lib-0.7.3/zhousflib/util/img_util.py
--rw-rw-rw-   0        0        0    12930 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/util/iou_util.py
--rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/util/json_util.py
--rw-rw-rw-   0        0        0      749 2023-06-13 08:44:02.000000 zhousf-lib-0.7.3/zhousflib/util/list_util.py
--rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/util/permission_util.py
--rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.7.3/zhousflib/util/poly_util.py
--rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/util/re_util.py
--rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/util/singleton.py
--rw-rw-rw-   0        0        0     4989 2023-06-14 07:42:54.000000 zhousf-lib-0.7.3/zhousflib/util/string_util.py
--rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.7.3/zhousflib/util/time_util.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:42:39.453415 zhousf-lib-0.7.3/zhousflib/web/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/web/__init__.py
--rw-rw-rw-   0        0        0     4355 2023-06-07 01:49:13.000000 zhousf-lib-0.7.3/zhousflib/web/config.py
--rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.7.3/zhousflib/web/log_util.py
--rw-rw-rw-   0        0        0     2860 2023-06-07 01:49:13.000000 zhousf-lib-0.7.3/zhousflib/web/logger.py
--rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.7.3/zhousflib/web/response.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.944036 zhousf-lib-0.7.5/
+-rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.7.5/LICENSE
+-rw-rw-rw-   0        0        0     2073 2023-06-16 06:03:02.944036 zhousf-lib-0.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1179 2023-06-09 06:54:16.000000 zhousf-lib-0.7.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 06:03:02.944036 zhousf-lib-0.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     4289 2023-06-16 06:02:45.000000 zhousf-lib-0.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.408104 zhousf-lib-0.7.5/zhousf_lib.egg-info/
+-rw-rw-rw-   0        0        0     2073 2023-06-16 06:03:01.000000 zhousf-lib-0.7.5/zhousf_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1929 2023-06-16 06:03:02.000000 zhousf-lib-0.7.5/zhousf_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 06:03:01.000000 zhousf-lib-0.7.5/zhousf_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 06:03:01.000000 zhousf-lib-0.7.5/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.409104 zhousf-lib-0.7.5/zhousflib/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.7.5/zhousflib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.411104 zhousf-lib-0.7.5/zhousflib/datasets/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.7.5/zhousflib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.413104 zhousf-lib-0.7.5/zhousflib/datasets/classification/
+-rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.7.5/zhousflib/datasets/classification/__init__.py
+-rw-rw-rw-   0        0        0     4895 2023-06-13 08:58:42.000000 zhousf-lib-0.7.5/zhousflib/datasets/classification/classification_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.481547 zhousf-lib-0.7.5/zhousflib/datasets/coco/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.5/zhousflib/datasets/coco/__init__.py
+-rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.7.5/zhousflib/datasets/coco/coco_bbox_extract.py
+-rw-rw-rw-   0        0        0     5484 2023-06-12 06:00:08.000000 zhousf-lib-0.7.5/zhousflib/datasets/coco/coco_bbox_update.py
+-rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.7.5/zhousflib/datasets/coco/coco_bbox_vis.py
+-rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.7.5/zhousflib/datasets/coco/coco_dataset_merge.py
+-rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.7.5/zhousflib/datasets/coco/coco_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.546175 zhousf-lib-0.7.5/zhousflib/datasets/labelme/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.5/zhousflib/datasets/labelme/__init__.py
+-rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.7.5/zhousflib/datasets/labelme/labelme_clip.py
+-rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.7.5/zhousflib/datasets/labelme/labelme_convert_coco.py
+-rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.7.5/zhousflib/datasets/labelme/labelme_convert_seg.py
+-rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.7.5/zhousflib/datasets/labelme/labelme_dataset_clip.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.555349 zhousf-lib-0.7.5/zhousflib/datasets/segmentation/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.5/zhousflib/datasets/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.7.5/zhousflib/datasets/segmentation/seg_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.567321 zhousf-lib-0.7.5/zhousflib/db/
+-rw-rw-rw-   0        0        0       60 2023-06-15 07:08:53.000000 zhousf-lib-0.7.5/zhousflib/db/__init__.py
+-rw-rw-rw-   0        0        0     2343 2023-06-15 07:08:53.000000 zhousf-lib-0.7.5/zhousflib/db/lmdb_master.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.581472 zhousf-lib-0.7.5/zhousflib/decorator/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.7.5/zhousflib/decorator/__init__.py
+-rw-rw-rw-   0        0        0      466 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/decorator/except_util.py
+-rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/decorator/interceptor_util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.707121 zhousf-lib-0.7.5/zhousflib/font/
+-rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.7.5/zhousflib/font/SimSun.ttf
+-rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.7.5/zhousflib/font/Symbola.ttf
+-rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.7.5/zhousflib/font/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.718126 zhousf-lib-0.7.5/zhousflib/locust/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/locust/__init__.py
+-rw-rw-rw-   0        0        0     1521 2023-06-15 07:08:53.000000 zhousf-lib-0.7.5/zhousflib/locust/locust_demo.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.730414 zhousf-lib-0.7.5/zhousflib/pandas/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.7.5/zhousflib/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4088 2023-06-16 06:02:45.000000 zhousf-lib-0.7.5/zhousflib/pandas/openpyxl_util.py
+-rw-rw-rw-   0        0        0     6066 2023-06-16 06:01:36.000000 zhousf-lib-0.7.5/zhousflib/pandas/pandas_util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.771006 zhousf-lib-0.7.5/zhousflib/pdf/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/pdf/export_image.py
+-rw-rw-rw-   0        0        0     1465 2023-06-15 07:08:53.000000 zhousf-lib-0.7.5/zhousflib/pdf/pdfplumber_util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.894673 zhousf-lib-0.7.5/zhousflib/util/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/util/__init__.py
+-rw-rw-rw-   0        0        0     2770 2023-06-07 01:49:13.000000 zhousf-lib-0.7.5/zhousflib/util/calculater_util.py
+-rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/util/cv_util.py
+-rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.7.5/zhousflib/util/encrypt_util.py
+-rw-rw-rw-   0        0        0     1592 2023-06-14 06:14:27.000000 zhousf-lib-0.7.5/zhousflib/util/img_util.py
+-rw-rw-rw-   0        0        0    12930 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/util/iou_util.py
+-rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/util/json_util.py
+-rw-rw-rw-   0        0        0      749 2023-06-13 08:44:02.000000 zhousf-lib-0.7.5/zhousflib/util/list_util.py
+-rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/util/permission_util.py
+-rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.7.5/zhousflib/util/poly_util.py
+-rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/util/re_util.py
+-rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/util/singleton.py
+-rw-rw-rw-   0        0        0     4989 2023-06-14 07:42:54.000000 zhousf-lib-0.7.5/zhousflib/util/string_util.py
+-rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.7.5/zhousflib/util/time_util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:03:02.939875 zhousf-lib-0.7.5/zhousflib/web/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/web/__init__.py
+-rw-rw-rw-   0        0        0     4355 2023-06-07 01:49:13.000000 zhousf-lib-0.7.5/zhousflib/web/config.py
+-rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.7.5/zhousflib/web/log_util.py
+-rw-rw-rw-   0        0        0     2860 2023-06-07 01:49:13.000000 zhousf-lib-0.7.5/zhousflib/web/logger.py
+-rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.7.5/zhousflib/web/response.py
```

### Comparing `zhousf-lib-0.7.3/LICENSE` & `zhousf-lib-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/PKG-INFO` & `zhousf-lib-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.7.3
+Version: 0.7.5
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.7.3/README.md` & `zhousf-lib-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/setup.py` & `zhousf-lib-0.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # 打包：python setup.py upload
 NAME = 'zhousf-lib'
 DESCRIPTION = 'a python library of zhousf'
 URL = 'https://github.com/MrZhousf/ZhousfLib'
 EMAIL = '442553199@qq.com'
 AUTHOR = 'zhousf'
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '0.7.3'
+VERSION = '0.7.5'
 PACKAGE_DATA = {'': ['*.yaml', '*.ttf', '*.txt', '*.md']}
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 # What packages are required for this module to be executed?
```

### Comparing `zhousf-lib-0.7.3/zhousf_lib.egg-info/PKG-INFO` & `zhousf-lib-0.7.5/zhousf_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.7.3
+Version: 0.7.5
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.7.3/zhousf_lib.egg-info/SOURCES.txt` & `zhousf-lib-0.7.5/zhousf_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/datasets/classification/classification_dataset_split.py` & `zhousf-lib-0.7.5/zhousflib/datasets/classification/classification_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/datasets/coco/coco_bbox_extract.py` & `zhousf-lib-0.7.5/zhousflib/datasets/coco/coco_bbox_extract.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/datasets/coco/coco_bbox_update.py` & `zhousf-lib-0.7.5/zhousflib/datasets/coco/coco_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/datasets/coco/coco_bbox_vis.py` & `zhousf-lib-0.7.5/zhousflib/datasets/coco/coco_bbox_vis.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/datasets/coco/coco_dataset_merge.py` & `zhousf-lib-0.7.5/zhousflib/datasets/coco/coco_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/datasets/coco/coco_dataset_split.py` & `zhousf-lib-0.7.5/zhousflib/datasets/coco/coco_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/datasets/labelme/labelme_clip.py` & `zhousf-lib-0.7.5/zhousflib/datasets/labelme/labelme_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/datasets/labelme/labelme_convert_coco.py` & `zhousf-lib-0.7.5/zhousflib/datasets/labelme/labelme_convert_coco.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/datasets/labelme/labelme_convert_seg.py` & `zhousf-lib-0.7.5/zhousflib/datasets/labelme/labelme_convert_seg.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/datasets/labelme/labelme_dataset_clip.py` & `zhousf-lib-0.7.5/zhousflib/datasets/labelme/labelme_dataset_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/datasets/segmentation/seg_dataset_split.py` & `zhousf-lib-0.7.5/zhousflib/datasets/segmentation/seg_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/db/lmdb_master.py` & `zhousf-lib-0.7.5/zhousflib/db/lmdb_master.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# @Author  : zhousf-a
+# @Author  : zhousf
 # @Function: lmdb (Lightning Memory-Mapped Database) 快如闪电的内存映射数据库
 # pip install lmdb
 import pickle
 import lmdb
 from pathlib import Path
 
 """
```

### Comparing `zhousf-lib-0.7.3/zhousflib/decorator/interceptor_util.py` & `zhousf-lib-0.7.5/zhousflib/decorator/interceptor_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/font/SimSun.ttf` & `zhousf-lib-0.7.5/zhousflib/font/SimSun.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/font/Symbola.ttf` & `zhousf-lib-0.7.5/zhousflib/font/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/font/__init__.py` & `zhousf-lib-0.7.5/zhousflib/font/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/locust/locust_demo.py` & `zhousf-lib-0.7.5/zhousflib/locust/locust_demo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding:utf-8 -*-
 # Author:  zhousf
-# Date:    2022-10-21
 # Description: 并发测试工具
 # pip install locust
 import os
 import time
 from locust import HttpUser, task, TaskSet
 
 HOST = "http://127.0.0.1:5000"
```

### Comparing `zhousf-lib-0.7.3/zhousflib/pandas/openpyxl_util.py` & `zhousf-lib-0.7.5/zhousflib/pandas/openpyxl_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# @Author  : zhousf-a
+# @Author  : zhousf
 # @Function:
 import openpyxl
 from pathlib import Path
 from zhousflib.util import re_util
 
 
 def unmerge_and_fill_cells(excel_file: Path, merged_cell_rate=2/3, delete_duplicates=True, tmp_excel: Path = None,
@@ -45,17 +45,19 @@
                 cell.value = merged_cell.value
         """
         找到符合拆分合并单元格条件的单元格rows
         """
         need_fill = []
         for i in rows_deal:
             column_count = rows_deal.get(i)
-            if column_count >= merged_cell_rate * worksheet.max_column:
-                need_fill.append(i)
-                contain_merge_cells = True
+            # if column_count >= merged_cell_rate * worksheet.max_column:
+            #     need_fill.append(i)
+            #     contain_merge_cells = True
+            need_fill.append(i)
+            contain_merge_cells = True
         """
         拆分合并单元格后，对空单元格赋予有效值
         """
         for cells in worksheet.iter_rows():
             for cell in cells:
                 row = cell.row
                 column = cell.column
@@ -65,26 +67,32 @@
                         if not cell.value and next_cell.value:
                             cell.value = next_cell.value
                         if cell.value and not next_cell.value:
                             next_cell.value = cell.value
         """
         拆分合并单元格后会有重复的两条，这里去重一下
         """
+        if len(need_fill) > 0:
+            need_fill.sort(key=lambda x: x[0], reverse=False)
         if delete_duplicates:
+            # 偏移量，记录删除row的个数
+            offset = 0
             for fill in need_fill:
                 data = []
+                fill = (fill[0]-offset, fill[1]-offset)
                 for row_cells in worksheet.iter_rows(min_row=min(fill), max_row=max(fill)):
                     data.append([cell.value for cell in row_cells])
-                if len(data) > 1:
-                    first_row_value = data[0]
-                    first_row_index = min(fill)
-                    first_row_index += 1
-                    for i in range(1, len(data)):
-                        if data[i] == first_row_value:
-                            worksheet.delete_rows(idx=first_row_index)
+                if len(data) < 2:
+                    continue
+                first_row_index = min(fill) + 1
+                for i in range(1, len(data)):
+                    first_row_value = data[i-1]
+                    if data[i] == first_row_value:
+                        worksheet.delete_rows(idx=first_row_index)
+                        offset += 1
     if tmp_excel:
         wb.save(str(tmp_excel))
         wb.close()
         return tmp_excel
     else:
         if contain_merge_cells:
             wb.save(str(excel_file))
```

### Comparing `zhousf-lib-0.7.3/zhousflib/pandas/pandas_util.py` & `zhousf-lib-0.7.5/zhousflib/pandas/pandas_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,8 +162,11 @@
     """
     with open(csv_path, "w") as file:
         writer = csv.writer(file)
         writer.writerows(data)
 
 
 if __name__ == "__main__":
+    read_excel_merge_cell(file_path=Path(r"C:\Users\zhousf-a\Desktop\2_ocr_data.xlsx"),
+                          tmp_excel=Path(r"C:\Users\zhousf-a\Desktop\2_ocr_data-tmp.xlsx"),
+                          delete_duplicates=True)
     pass
```

### Comparing `zhousf-lib-0.7.3/zhousflib/pdf/export_image.py` & `zhousf-lib-0.7.5/zhousflib/pdf/export_image.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/pdf/pdfplumber_util.py` & `zhousf-lib-0.7.5/zhousflib/pdf/pdfplumber_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding:utf-8 -*-
-# Author:  zhousf-a
+# Author:  zhousf
 # Description: pdf表格还原工具
 # pip install pdfplumber
 import pdfplumber
 import pandas as pd
 
 
 def pdf_to_excel(pdf_file, save_file):
```

### Comparing `zhousf-lib-0.7.3/zhousflib/util/calculater_util.py` & `zhousf-lib-0.7.5/zhousflib/util/calculater_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/util/cv_util.py` & `zhousf-lib-0.7.5/zhousflib/util/cv_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/util/encrypt_util.py` & `zhousf-lib-0.7.5/zhousflib/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/util/img_util.py` & `zhousf-lib-0.7.5/zhousflib/util/img_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/util/iou_util.py` & `zhousf-lib-0.7.5/zhousflib/util/iou_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/util/json_util.py` & `zhousf-lib-0.7.5/zhousflib/util/json_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/util/list_util.py` & `zhousf-lib-0.7.5/zhousflib/util/list_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/util/permission_util.py` & `zhousf-lib-0.7.5/zhousflib/util/permission_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/util/poly_util.py` & `zhousf-lib-0.7.5/zhousflib/util/poly_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/util/re_util.py` & `zhousf-lib-0.7.5/zhousflib/util/re_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/util/singleton.py` & `zhousf-lib-0.7.5/zhousflib/util/singleton.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/util/string_util.py` & `zhousf-lib-0.7.5/zhousflib/util/string_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/util/time_util.py` & `zhousf-lib-0.7.5/zhousflib/util/time_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/web/config.py` & `zhousf-lib-0.7.5/zhousflib/web/config.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/web/log_util.py` & `zhousf-lib-0.7.5/zhousflib/web/log_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/web/logger.py` & `zhousf-lib-0.7.5/zhousflib/web/logger.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.7.3/zhousflib/web/response.py` & `zhousf-lib-0.7.5/zhousflib/web/response.py`

 * *Files identical despite different names*

