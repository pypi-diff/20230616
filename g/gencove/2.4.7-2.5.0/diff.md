# Comparing `tmp/gencove-2.4.7.tar.gz` & `tmp/gencove-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gencove-2.4.7.tar", last modified: Wed May 31 20:26:00 2023, max compression
+gzip compressed data, was "dist/gencove-2.5.0.tar", last modified: Fri Jun 16 14:34:43 2023, max compression
```

## Comparing `gencove-2.4.7.tar` & `gencove-2.5.0.tar`

### file list

```diff
@@ -1,301 +1,301 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-05-31 20:26:00.000000 gencove-2.4.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2085 2023-05-31 20:25:28.000000 gencove-2.4.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    32228 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6009 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/autoimports/
--rw-rw-rw-   0 root         (0) root         (0)       92 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1966 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/autoimports/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/create/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2536 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/create/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/biosamples/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/biosamples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/biosamples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/projects/
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_import/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_import/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1959 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_import/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_import/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_import/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1987 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/common_cli_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/download/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4611 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/download/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2104 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/download/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/download/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    14731 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/download/main.py
--rw-rw-rw-   0 root         (0) root         (0)    10579 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/download/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/files/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/files/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/files/main.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/files/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1682 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create/main.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/create_batch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create_batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create_batch/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2787 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create_batch/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/create_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1740 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create_merged_vcf/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/delete_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/delete_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/delete_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/delete_samples/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/get_batch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/get_batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      936 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/get_batch/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2769 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/get_batch/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/get_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/get_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/get_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/get_merged_vcf/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/import_existing_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/import_existing_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1843 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/import_existing_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/import_existing_samples/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2474 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/import_existing_samples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/import_existing_samples/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2859 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/list_batch_types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batch_types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      616 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batch_types/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2586 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batch_types/main.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batch_types/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/list_batches/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batches/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batches/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2504 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batches/main.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batches/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/main.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/list_pipelines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipelines/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1842 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipelines/main.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipelines/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/restore_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/restore_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/restore_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/restore_samples/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/run_prefix/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/run_prefix/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1881 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/run_prefix/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/run_prefix/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     5056 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/run_prefix/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/samples/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2454 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/samples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/samples/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/status_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/status_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/status_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2117 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/status_merged_vcf/main.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/status_merged_vcf/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/s3_imports/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/create/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2452 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/create/main.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/s3_imports/s3_import/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/s3_import/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/s3_import/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/s3_import/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2054 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/s3_import/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/samples/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/samples/download_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/download_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2911 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/download_file/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/download_file/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4930 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/download_file/main.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/download_file/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/samples/get_metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/get_metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      810 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/get_metadata/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/get_metadata/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/samples/set_metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/set_metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/set_metadata/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/set_metadata/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/upload/
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    16178 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3028 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/multi_file_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     7601 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/uploads/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/uploads/list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/list/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/webhook/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/webhook/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/webhook/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/webhook/verify/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/webhook/verify/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1011 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/webhook/verify/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/webhook/verify/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3691 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/description/
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/description/pypi_readme.md
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3205 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     7778 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/basespace/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6422 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/test_basespace_autoimports_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4249 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/test_basespace_autoimports_list.py
--rw-rw-rw-   0 root         (0) root         (0)     7257 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/test_basespace_biosamples_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6335 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/test_basespace_projects_import.py
--rw-rw-rw-   0 root         (0) root         (0)     5955 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/test_basespace_projects_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/basespace/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4675 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3328 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/download/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36754 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/download/test_cli_download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/download/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/download/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/download/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4371 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/files/test_file_types_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/files/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/files/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4519 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/projects/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6781 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_batch_get.py
--rw-rw-rw-   0 root         (0) root         (0)     4502 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_batch_types_list.py
--rw-rw-rw-   0 root         (0) root         (0)     8993 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_batches_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4601 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_batches_list.py
--rw-rw-rw-   0 root         (0) root         (0)     4380 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_create.py
--rw-rw-rw-   0 root         (0) root         (0)     9109 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_create_merged_vcf.py
--rw-rw-rw-   0 root         (0) root         (0)     8901 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_delete_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    12017 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_get_merged_vcf.py
--rw-rw-rw-   0 root         (0) root         (0)     6387 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_import_existing_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    10605 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6511 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_pipeline_capabilities_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_pipelines_list.py
--rw-rw-rw-   0 root         (0) root         (0)     7328 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_restore_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    13391 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_run_prefix.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_samples_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6469 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_status_merged_vcf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/projects/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11910 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/s3_imports/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/s3_imports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6470 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/s3_imports/test_s3_autoimports_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4163 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/s3_imports/test_s3_autoimports_list.py
--rw-rw-rw-   0 root         (0) root         (0)     5270 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/s3_imports/test_s3_uri_import.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/s3_imports/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/s3_imports/vcr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8865 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/samples/test_samples_download_file.py
--rw-rw-rw-   0 root         (0) root         (0)     7024 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/samples/test_samples_get_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/samples/test_samples_set_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/samples/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/samples/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/samples/vcr/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/test_logger.py
--rw-rw-rw-   0 root         (0) root         (0)    17615 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/upload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    35553 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/upload/test_cli_upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/upload/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/upload/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4000 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/upload/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/uploads/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/uploads/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4357 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/uploads/test_uploads_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/uploads/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/uploads/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      971 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/webhook/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/webhook/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3430 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/webhook/test_webhook_verify.py
--rw-rw-rw-   0 root         (0) root         (0)     5174 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/version/
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/version/A-major
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/version/B-minor
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/version/C-patch
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10251 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      127 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-31 20:26:00.000000 gencove-2.4.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1866 2023-05-31 20:25:28.000000 gencove-2.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-06-16 14:34:43.000000 gencove-2.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2023-06-16 14:34:08.000000 gencove-2.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    32627 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6009 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/autoimports/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/autoimports/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/basespace/autoimports/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1883 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/create/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/create/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/biosamples/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/biosamples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/biosamples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/projects/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_import/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_import/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_import/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_import/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_import/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/common_cli_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/download/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4611 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/download/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/download/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/download/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    14731 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/download/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    10579 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/download/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/files/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/files/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/files/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/files/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/create_batch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/create_batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create_batch/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create_batch/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/create_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/create_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create_merged_vcf/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/delete_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/delete_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/delete_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/delete_samples/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/get_batch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/get_batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/get_batch/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2769 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/get_batch/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/get_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/get_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/get_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/get_merged_vcf/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/import_existing_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/import_existing_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/import_existing_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/import_existing_samples/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/import_existing_samples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/import_existing_samples/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2859 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/list_batch_types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/list_batch_types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_batch_types/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_batch_types/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_batch_types/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/list_batches/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/list_batches/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_batches/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_batches/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_batches/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/list_pipelines/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/list_pipelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_pipelines/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1842 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_pipelines/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_pipelines/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/restore_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/restore_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/restore_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/restore_samples/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/run_prefix/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/run_prefix/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1953 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/run_prefix/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/run_prefix/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4918 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/run_prefix/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/samples/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2454 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/samples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/samples/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/status_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/status_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/status_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1813 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/status_merged_vcf/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/status_merged_vcf/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/s3_imports/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/create/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/create/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/s3_imports/s3_import/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/s3_imports/s3_import/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/s3_import/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/s3_import/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/s3_import/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/samples/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/samples/download_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/samples/download_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2911 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/download_file/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/download_file/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4930 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/download_file/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/download_file/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/samples/get_metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/samples/get_metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      810 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/get_metadata/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/get_metadata/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/samples/set_metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/samples/set_metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/set_metadata/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/set_metadata/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/upload/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    16788 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3028 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/multi_file_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     8819 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/uploads/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/uploads/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/uploads/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/uploads/list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/uploads/list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/uploads/list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/uploads/list/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/uploads/list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/uploads/list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/webhook/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/webhook/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/webhook/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/webhook/verify/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/webhook/verify/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/webhook/verify/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/webhook/verify/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3731 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/description/
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/description/pypi_readme.md
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3205 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     7984 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/basespace/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/basespace/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6374 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/basespace/test_basespace_autoimports_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4249 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/basespace/test_basespace_autoimports_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     7257 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/basespace/test_basespace_biosamples_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6334 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/basespace/test_basespace_projects_import.py
+-rw-rw-rw-   0 root         (0) root         (0)     5955 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/basespace/test_basespace_projects_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/basespace/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/basespace/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4675 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3328 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/download/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36754 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/download/test_cli_download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/download/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/download/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/download/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4371 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/files/test_file_types_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/files/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/files/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4519 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/projects/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/projects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6781 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_batch_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     4502 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_batch_types_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     8945 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_batches_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4601 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_batches_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     4380 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     9108 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_create_merged_vcf.py
+-rw-rw-rw-   0 root         (0) root         (0)     8901 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_delete_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    12016 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_get_merged_vcf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_import_existing_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    10605 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6511 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_pipeline_capabilities_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_pipelines_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     7212 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_restore_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    13390 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_run_prefix.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_samples_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6468 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_status_merged_vcf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/projects/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/projects/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11910 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/s3_imports/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/s3_imports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6422 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/s3_imports/test_s3_autoimports_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4163 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/s3_imports/test_s3_autoimports_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     5269 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/s3_imports/test_s3_uri_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/s3_imports/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/s3_imports/vcr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8865 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/samples/test_samples_download_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     7024 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/samples/test_samples_get_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/samples/test_samples_set_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/samples/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/samples/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      700 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/samples/vcr/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/test_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    22425 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/upload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42140 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/upload/test_cli_upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/upload/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/upload/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5281 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/upload/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/uploads/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/uploads/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4357 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/uploads/test_uploads_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/uploads/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/uploads/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      971 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/webhook/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/webhook/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3430 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/webhook/test_webhook_verify.py
+-rw-rw-rw-   0 root         (0) root         (0)     5174 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/version/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/version/A-major
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/version/B-minor
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/version/C-patch
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10251 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-16 14:34:43.000000 gencove-2.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2023-06-16 14:34:08.000000 gencove-2.5.0/setup.py
```

### Comparing `gencove-2.4.7/PKG-INFO` & `gencove-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gencove
-Version: 2.4.7
+Version: 2.5.0
 Summary: Gencove API and CLI tool
 Home-page: http://docs.gencove.com
 Author: Tomaz Berisa
 License: Apache 2.0
 Description: # The Gencove CLI
         
         [![PyPI Latest Release](https://img.shields.io/pypi/v/gencove.svg)](https://pypi.org/project/gencove/)
```

### Comparing `gencove-2.4.7/README.md` & `gencove-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/cli.py` & `gencove-2.5.0/gencove/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/client.py` & `gencove-2.5.0/gencove/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     S3ProjectImport,
     SampleDetails,
     SampleMetadata,
     SampleQC,
     SampleSheet,
     UploadCredentials,
     UploadSamples,
+    UploadURLImport,
     UploadsPostData,
 )
 from gencove.version import version as cli_version
 
 
 class CustomEncoder(json.JSONEncoder):
     """JSON encoder that knows how to encode `datetime`, `UUID`
@@ -237,15 +238,15 @@
                             ]
                         )
                     except AttributeError:
                         error_msg = "\n".join(response_json)
                     http_error_msg += f":\n{error_msg}"
 
         elif 500 <= response.status_code < 600:
-            http_error_msg = "Server Error: {response.reason}"
+            http_error_msg = f"Server Error: {response.reason}"
             if response.status_code == 503:
                 if response.text:
                     response_json = response.json()
                     if "maintenance" in response_json:
                         raise MaintenanceError(
                             message=response_json["maintenance_message"],
                             eta=response_json["maintenance_eta"],
@@ -963,14 +964,27 @@
         return self._post(
             self.endpoints.IMPORT_EXISTING_SAMPLES.value,
             payload,
             authorized=True,
             model=ImportExistingSamplesModel,
         )
 
+    def import_fastqs_from_url(self, gncv_file_path, url):
+        """POST fastq URL data to API"""
+        payload = {
+            "destination_path": gncv_file_path,
+            "source_url": url,
+        }
+        return self._post(
+            self.endpoints.UPLOAD_URL.value,
+            payload,
+            authorized=True,
+            model=UploadURLImport,
+        )
+
     def get_file_types(self, project_id=None):
         """List file types.
 
         Args:
             project_id (UUID, optional): project_id used to get all file types
                 for a project
         """
```

### Comparing `gencove-2.4.7/gencove/command/base.py` & `gencove-2.5.0/gencove/command/base.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/cli.py` & `gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/main.py` & `gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/utils.py` & `gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/basespace/autoimports/create/cli.py` & `gencove-2.5.0/gencove/command/basespace/autoimports/create/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Project autoimport Biosamples from BaseSpace projects shell command
 definition.
 """
 import click
 
 from gencove.command.common_cli_options import add_options, common_options
+from gencove.command.utils import validate_uuid
 from gencove.constants import Credentials
 
 from .constants import BaseSpaceAutoImportOptionals
 from .main import BaseSpaceAutoImport
 
 
 @click.command("create")
-@click.argument("project_id")
+@click.argument("project_id", callback=validate_uuid)
 @click.argument("identifier")
 @click.option(
     "--metadata-json",
     required=False,
     default=None,
     help=(
         "Add metadata to all samples that are to be imported from "
```

### Comparing `gencove-2.4.7/gencove/command/basespace/autoimports/create/main.py` & `gencove-2.5.0/gencove/command/basespace/autoimports/create/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """AutoImport Biosamples from BaseSpace projects to a project subcommand."""
 
 import json
 
 from ....base import Command
-from ....utils import is_valid_json, is_valid_uuid
+from ....utils import is_valid_json
 from ..... import client
 from .....exceptions import ValidationError
 
 
 class BaseSpaceAutoImport(Command):
     """BaseSpace autoimport command executor."""
 
@@ -23,16 +23,14 @@
 
     def validate(self):
         """Validate command input.
 
         Raises:
             ValidationError - if something is wrong with command parameters.
         """
-        if is_valid_uuid(self.project_id) is False:
-            raise ValidationError("Project ID is not valid. Exiting.")
         if self.metadata_json and is_valid_json(self.metadata_json) is False:
             raise ValidationError("Metadata JSON is not valid. Exiting.")
 
     # no retry for timeouts in order to avoid duplicate heavy operations on
     # the backend
     def execute(self):
         """Make a request to create a job to periodically import Biosamples
```

### Comparing `gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/cli.py` & `gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/main.py` & `gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/utils.py` & `gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/basespace/projects/basespace_import/cli.py` & `gencove-2.5.0/gencove/command/basespace/projects/basespace_import/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Project import Biosamples from BaseSpace projects shell command definition.
 """
 import click
 
 from gencove.command.common_cli_options import add_options, common_options
+from gencove.command.utils import validate_uuid
 from gencove.constants import Credentials
 from gencove.logger import echo_debug
 
 from .constants import BaseSpaceImportOptionals
 from .main import BaseSpaceImport
 
 
 @click.command("import")
 @click.argument("basespace_project_ids")
-@click.argument("project_id")
+@click.argument("project_id", callback=validate_uuid)
 @click.option(
     "--metadata-json",
     required=False,
     default=None,
     help=(
         "Add metadata to all samples that are to be imported from "
         "BaseSpace to a project."
```

### Comparing `gencove-2.4.7/gencove/command/basespace/projects/basespace_import/main.py` & `gencove-2.5.0/gencove/command/basespace/projects/basespace_import/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Import Biosamples from BaseSpace projects to a project subcommand."""
 
 import json
 
 from ....base import Command
-from ....utils import is_valid_json, is_valid_uuid
+from ....utils import is_valid_json
 from ..... import client
 from .....exceptions import ValidationError
 
 
 class BaseSpaceImport(Command):
     """BaseSpace import command executor."""
 
@@ -23,16 +23,14 @@
 
     def validate(self):
         """Validate command input.
 
         Raises:
             ValidationError - if something is wrong with command parameters.
         """
-        if is_valid_uuid(self.project_id) is False:
-            raise ValidationError("Project ID is not valid. Exiting.")
         if self.metadata_json and is_valid_json(self.metadata_json) is False:
             raise ValidationError("Metadata JSON is not valid. Exiting.")
 
     # no retry for timeouts in order to avoid duplicate heavy operations on
     # the backend
     def execute(self):
         """Make a request to import Biosamples from BaseSpace to a given
```

### Comparing `gencove-2.4.7/gencove/command/basespace/projects/basespace_list/cli.py` & `gencove-2.5.0/gencove/command/basespace/projects/basespace_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/basespace/projects/basespace_list/main.py` & `gencove-2.5.0/gencove/command/basespace/projects/basespace_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/basespace/projects/basespace_list/utils.py` & `gencove-2.5.0/gencove/command/basespace/projects/basespace_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/common_cli_options.py` & `gencove-2.5.0/gencove/command/common_cli_options.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/download/cli.py` & `gencove-2.5.0/gencove/command/download/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/download/constants.py` & `gencove-2.5.0/gencove/command/download/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/download/main.py` & `gencove-2.5.0/gencove/command/download/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/download/utils.py` & `gencove-2.5.0/gencove/command/download/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/files/cli.py` & `gencove-2.5.0/gencove/command/files/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/files/main.py` & `gencove-2.5.0/gencove/command/files/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/cli.py` & `gencove-2.5.0/gencove/command/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/create/cli.py` & `gencove-2.5.0/gencove/command/projects/create/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/create/main.py` & `gencove-2.5.0/gencove/command/projects/create/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/create_batch/cli.py` & `gencove-2.5.0/gencove/command/projects/create_batch/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 """Project batch types list shell command definition."""
 import click
 
 from gencove.command.common_cli_options import add_options, common_options
+from gencove.command.utils import validate_uuid, validate_uuid_list
 from gencove.constants import Credentials, Optionals
-from gencove.logger import echo_debug
 
 from .main import CreateBatch
 
 
 @click.command("create-batch")
-@click.argument("project_id")
+@click.argument("project_id", callback=validate_uuid)
 @click.option(
     "--batch-type",
     help="One of available project's batch types.\n"
     "Use `gencove projects list-batch-types` command to find out "
     "which batch types are available.",
 )
 @click.option("--batch-name", help="User defined batch name.")
 @click.option(
     "--sample-ids",
     default="",
     help="A comma separated list of sample ids for "
     "which to create a batch; if not specified use all samples in project",
+    callback=validate_uuid_list,
 )
 @add_options(common_options)
 def create_project_batch(  # pylint: disable=too-many-arguments
     project_id,
     batch_type,
     batch_name,
     sample_ids,
     host,
     email,
     password,
     api_key,
 ):
     """Create a batch in a project."""
-    if sample_ids:
-        sample_ids = [s_id.strip() for s_id in sample_ids.split(",")]
-        echo_debug(f"Sample ids translation: {sample_ids}")
-    else:
-        sample_ids = []
-
     CreateBatch(
         project_id,
         batch_type,
         batch_name,
         sample_ids,
         Credentials(email=email, password=password, api_key=api_key),
         Optionals(host=host),
```

### Comparing `gencove-2.4.7/gencove/command/projects/create_batch/main.py` & `gencove-2.5.0/gencove/command/projects/create_batch/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Create project's batch executor."""
 from gencove import client  # noqa: I100
 from gencove.command.base import Command
 from gencove.command.projects.list_batches.utils import get_line
-from gencove.command.utils import is_valid_uuid
 from gencove.exceptions import ValidationError
 
 
 class CreateBatch(Command):
     """Create project's batch executor."""
 
     # pylint: disable=too-many-arguments
@@ -37,21 +36,14 @@
         """
         if not self.batch_type:
             raise ValidationError("You must provide value for --batch-type. Exiting.")
 
         if not self.batch_name:
             raise ValidationError("You must provide value for --batch-name. Exiting.")
 
-        if is_valid_uuid(self.project_id) is False:
-            raise ValidationError("Project ID is not valid. Exiting.")
-
-        if self.sample_ids:
-            if not all(is_valid_uuid(s_id) for s_id in self.sample_ids):
-                raise ValidationError("Not all sample IDs are valid. Exiting.")
-
     # no retry for timeouts in order to avoid duplicate heavy operations on
     # the backend
     def execute(self):
         """Make a request to create a batch for given project."""
         self.echo_debug(
             f"Creating batch for project {self.project_id} and "
             f"batch key {self.batch_name}"
```

### Comparing `gencove-2.4.7/gencove/command/projects/create_merged_vcf/cli.py` & `gencove-2.5.0/gencove/command/projects/create_merged_vcf/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Project create merged VCF shell command definition."""
 import click
 
 from gencove.command.common_cli_options import add_options, common_options
+from gencove.command.utils import validate_uuid
 from gencove.constants import Credentials, Optionals
 
 from .main import CreateMergedVCF
 
 
 @click.command("create-merged-vcf")
-@click.argument("project_id")
+@click.argument("project_id", callback=validate_uuid)
 @add_options(common_options)
 def create_merged_vcf(
     project_id,
     host,
     email,
     password,
     api_key,
```

### Comparing `gencove-2.4.7/gencove/command/projects/create_merged_vcf/main.py` & `gencove-2.5.0/gencove/command/projects/create_merged_vcf/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Merge project's VCF files executor."""
 from ..status_merged_vcf.utils import get_line
 from ...base import Command
-from ...utils import is_valid_uuid
 from .... import client
-from ....exceptions import ValidationError
 
 
 class CreateMergedVCF(Command):
     """Merge project's VCF files executor."""
 
     def __init__(
         self,
@@ -19,21 +17,15 @@
         self.project_id = project_id
 
     def initialize(self):
         """Initialize subcommand."""
         self.login()
 
     def validate(self):
-        """Validate command input.
-
-        Raises:
-            ValidationError - if something is wrong with command parameters.
-        """
-        if is_valid_uuid(self.project_id) is False:
-            raise ValidationError("Project ID is not valid. Exiting.")
+        """Validate command input."""
 
     # no retry for timeouts in order to avoid duplicate heavy operations on
     # the backend
     def execute(self):
         """Make a request to merge VCF files for a given project."""
         self.echo_debug(f"Merging VCF files for project {self.project_id}")
         try:
```

### Comparing `gencove-2.4.7/gencove/command/projects/delete_samples/cli.py` & `gencove-2.5.0/gencove/command/projects/delete_samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/delete_samples/main.py` & `gencove-2.5.0/gencove/command/projects/delete_samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/get_batch/cli.py` & `gencove-2.5.0/gencove/command/projects/get_batch/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/get_batch/main.py` & `gencove-2.5.0/gencove/command/projects/get_batch/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/get_merged_vcf/cli.py` & `gencove-2.5.0/gencove/command/projects/get_merged_vcf/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Project get merged VCF shell command definition."""
 import click
 
 from gencove.command.common_cli_options import add_options, common_options
+from gencove.command.utils import validate_uuid
 from gencove.constants import Credentials, Optionals
 
 from .main import GetMergedVCF
 
 
 @click.command("get-merged-vcf")
-@click.argument("project_id")
+@click.argument("project_id", callback=validate_uuid)
 @click.option(
     "--output-filename",
     help="Output filename for merged VCF file.",
     type=click.Path(),
     required=False,
     default=None,
 )
```

### Comparing `gencove-2.4.7/gencove/command/projects/get_merged_vcf/main.py` & `gencove-2.5.0/gencove/command/projects/get_merged_vcf/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Download project's merged VCF file executor."""
 import backoff
 
 from ... import download
 from ...base import Command
-from ...utils import is_valid_uuid
 from .... import client
 from ....exceptions import ValidationError
 
 
 class GetMergedVCF(Command):
     """Download project's merged VCF file executor."""
 
@@ -26,21 +25,15 @@
         self.no_progress = no_progress
 
     def initialize(self):
         """Initialize subcommand."""
         self.login()
 
     def validate(self):
-        """Validate command input.
-
-        Raises:
-            ValidationError - if something is wrong with command parameters.
-        """
-        if is_valid_uuid(self.project_id) is False:
-            raise ValidationError("Project ID is not valid. Exiting.")
+        """Validate command input."""
 
     @backoff.on_exception(
         backoff.expo,
         (client.APIClientTimeout),
         max_tries=5,
         max_time=30,
     )
```

### Comparing `gencove-2.4.7/gencove/command/projects/import_existing_samples/cli.py` & `gencove-2.5.0/gencove/command/projects/import_existing_samples/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Import existing samples shell command definition."""
 import click
 
 from gencove.command.common_cli_options import add_options, common_options
+from gencove.command.utils import validate_uuid, validate_uuid_list
 from gencove.constants import Credentials
 from gencove.logger import echo_debug
 
 from .constants import ImportExistingSamplesOptionals
 from .main import ImportExistingSamples
 
 
 @click.command("import-existing-samples")
-@click.argument("project_id")
+@click.argument("project_id", callback=validate_uuid)
 @click.option(
     "--sample-ids",
     required=True,
     help="A comma separated list of sample ids to import into the provided project",
+    callback=validate_uuid_list,
 )
 @click.option(
     "--metadata-json",
     required=False,
     default=None,
     help="Add metadata to all samples that are to be imported into a project.",
 )
@@ -40,15 +42,14 @@
 
             gencove project import-existing-samples d9eaa54b-aaac-4b85-92b0-0b564be6d7db --sample-ids 59f5c1fd-cce0-4c4c-90e2-0b6c6c525d71,7edee497-12b5-4a1d-951f-34dc8dce1c1d
 
         Import samples with metadata:
 
             gencove project import-existing-samples d9eaa54b-aaac-4b85-92b0-0b564be6d7db --sample-ids 59f5c1fd-cce0-4c4c-90e2-0b6c6c525d71,7edee497-12b5-4a1d-951f-34dc8dce1c1d --metadata-json='{"batch": "batch1"}'
     """  # noqa: E501
-    sample_ids = [s_id.strip() for s_id in sample_ids.split(",")] if sample_ids else []
     echo_debug(f"Sample ids translation: {sample_ids}")
     ImportExistingSamples(
         project_id,
         sample_ids,
         Credentials(email=email, password=password, api_key=api_key),
         ImportExistingSamplesOptionals(host=host, metadata_json=metadata_json),
     ).run()
```

### Comparing `gencove-2.4.7/gencove/command/projects/import_existing_samples/main.py` & `gencove-2.5.0/gencove/command/projects/import_existing_samples/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Import existing samples to a project subcommand."""
 import json
 
 from .utils import get_line
 from ...base import Command
-from ...utils import is_valid_json, is_valid_uuid
+from ...utils import is_valid_json
 from .... import client
 from ....exceptions import ValidationError
 
 
 class ImportExistingSamples(Command):
     """Import existing samples command executor."""
 
@@ -23,18 +23,14 @@
 
     def validate(self):
         """Validate command input.
 
         Raises:
             ValidationError - if something is wrong with command parameters.
         """
-        if is_valid_uuid(self.project_id) is False:
-            raise ValidationError("Project ID is not valid. Exiting.")
-        if not all(is_valid_uuid(s_id) for s_id in self.sample_ids):
-            raise ValidationError("Not all sample IDs are valid. Exiting.")
         if self.metadata_json and is_valid_json(self.metadata_json) is False:
             raise ValidationError("Metadata JSON is not valid. Exiting.")
 
     def execute(self):
         """Import existing samples to the given project."""
         metadata = None
         if self.metadata_json is not None:
```

### Comparing `gencove-2.4.7/gencove/command/projects/list/main.py` & `gencove-2.5.0/gencove/command/projects/list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/list/utils.py` & `gencove-2.5.0/gencove/command/projects/list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/list_batch_types/cli.py` & `gencove-2.5.0/gencove/command/projects/list_batches/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-"""Project batch types list shell command definition."""
+"""Project batches list shell command definition."""
 import click
 
 from gencove.command.common_cli_options import add_options, common_options
+from gencove.command.utils import validate_uuid
 from gencove.constants import Credentials, Optionals
 
-from .main import ListBatchTypes
+from .main import ListBatches
 
 
-@click.command("list-batch-types")
-@click.argument("project_id")
+@click.command("list-batches")
+@click.argument("project_id", callback=validate_uuid)
 @add_options(common_options)
-def list_project_batch_types(project_id, host, email, password, api_key):
-    """List batch types that are available for a project."""
-    ListBatchTypes(
+def list_project_batches(project_id, host, email, password, api_key):
+    """List batches that are available for a project."""
+    ListBatches(
         project_id,
         Credentials(email=email, password=password, api_key=api_key),
         Optionals(host=host),
     ).run()
```

### Comparing `gencove-2.4.7/gencove/command/projects/list_batch_types/main.py` & `gencove-2.5.0/gencove/command/projects/list_batches/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,73 @@
-"""List project's batch types subcommand."""
+"""List project's batches subcommand."""
 
 import backoff
 
 # pylint: disable=wrong-import-order
 from gencove import client  # noqa: I100
 from gencove.command.base import Command
-from gencove.command.utils import is_valid_uuid
-from gencove.exceptions import ValidationError
 
 from .utils import get_line
 
 
-class ListBatchTypes(Command):
-    """List batch types command executor."""
+class ListBatches(Command):
+    """List batches command executor."""
 
     def __init__(self, project_id, credentials, options):
         super().__init__(credentials, options)
         self.project_id = project_id
 
     def initialize(self):
         """Initialize list subcommand."""
         self.login()
 
     def validate(self):
-        """Validate command input.
-
-        Raises:
-            ValidationError - if something is wrong with command parameters.
-        """
-
-        if is_valid_uuid(self.project_id) is False:
-            raise ValidationError("Project ID is not valid. Exiting.")
+        """Validate command input."""
 
     def execute(self):
-        self.echo_debug("Retrieving project's batch types:")
+        self.echo_debug("Retrieving project's batches:")
 
         try:
-            for batch_types in self.get_paginated_batch_types():
-                if not batch_types:
-                    self.echo_debug("No matching batch types were found.")
+            for batches in self.get_paginated_batches():
+                if not batches:
+                    self.echo_debug("No matching batches were found.")
                     return
 
-                for batch_type in batch_types:
-                    self.echo_data(get_line(batch_type))
-
+                for batch in batches:
+                    self.echo_data(get_line(batch))
         except client.APIClientError as err:
             self.echo_debug(err)
             if err.status_code == 400:
-                self.echo_warning("There was an error listing project batch types.")
+                self.echo_warning("There was an error listing project batches.")
                 self.echo_info("The following error was returned:")
                 self.echo_info(err.message)
             elif err.status_code == 404:
                 self.echo_warning(f"Project {self.project_id} does not exist.")
             else:
                 raise
 
-    def get_paginated_batch_types(self):
-        """Paginate over all batch types for the destination.
+    def get_paginated_batches(self):
+        """Paginate over all batches for the destination.
 
         Yields:
-            paginated lists of batch types
+            paginated lists of batches
         """
         more = True
         next_link = None
         while more:
-            self.echo_debug("Get batch types page")
-            resp = self.get_batch_types(next_link)
+            self.echo_debug("Get batches page")
+            resp = self.get_batches(next_link)
             yield resp.results
             next_link = resp.meta.next
             more = next_link is not None
 
     @backoff.on_exception(
         backoff.expo,
         (client.APIClientTimeout),
         max_tries=2,
         max_time=30,
     )
-    def get_batch_types(self, next_link=None):
-        """Get batch types page."""
-        return self.api_client.get_project_batch_types(
+    def get_batches(self, next_link=None):
+        """Get batches page."""
+        return self.api_client.get_project_batches(
             project_id=self.project_id, next_link=next_link
         )
```

### Comparing `gencove-2.4.7/gencove/command/projects/list_batches/cli.py` & `gencove-2.5.0/gencove/command/projects/status_merged_vcf/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,26 @@
-"""Project batches list shell command definition."""
+"""Project status merged VCF shell command definition."""
 import click
 
 from gencove.command.common_cli_options import add_options, common_options
+from gencove.command.utils import validate_uuid
 from gencove.constants import Credentials, Optionals
 
-from .main import ListBatches
+from .main import StatusMergedVCF
 
 
-@click.command("list-batches")
-@click.argument("project_id")
+@click.command("status-merged-vcf")
+@click.argument("project_id", callback=validate_uuid)
 @add_options(common_options)
-def list_project_batches(project_id, host, email, password, api_key):
-    """List batches that are available for a project."""
-    ListBatches(
+def status_merged_vcf(
+    project_id,
+    host,
+    email,
+    password,
+    api_key,
+):
+    """Get status of merge VCF files job in a project."""
+    StatusMergedVCF(
         project_id,
         Credentials(email=email, password=password, api_key=api_key),
         Optionals(host=host),
     ).run()
```

### Comparing `gencove-2.4.7/gencove/command/projects/list_batches/main.py` & `gencove-2.5.0/gencove/command/uploads/list/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,72 @@
-"""List project's batches subcommand."""
-
+"""List uploads subcommand."""
 import backoff
 
 # pylint: disable=wrong-import-order
-from gencove import client  # noqa: I100
+from gencove.client import APIClientError, APIClientTimeout  # noqa: I100
 from gencove.command.base import Command
-from gencove.command.utils import is_valid_uuid
-from gencove.exceptions import ValidationError
 
 from .utils import get_line
 
 
-class ListBatches(Command):
-    """List batches command executor."""
+class ListSampleSheet(Command):
+    """List sample sheet command executor."""
 
-    def __init__(self, project_id, credentials, options):
+    def __init__(self, credentials, options):
         super().__init__(credentials, options)
-        self.project_id = project_id
+        self.status = options.status
+        self.gncv_path = options.search
 
     def initialize(self):
         """Initialize list subcommand."""
         self.login()
 
     def validate(self):
-        """Validate command input.
-
-        Raises:
-            ValidationError - if something is wrong with command parameters.
-        """
-
-        if is_valid_uuid(self.project_id) is False:
-            raise ValidationError("Project ID is not valid. Exiting.")
+        """Validate command input."""
+        pass  # pylint: disable=unnecessary-pass
 
     def execute(self):
-        self.echo_debug("Retrieving project's batches:")
-
+        self.echo_debug(
+            "Retrieving sample sheet: "
+            f"status={self.status} search_term={self.gncv_path}"
+        )
         try:
-            for batches in self.get_paginated_batches():
-                if not batches:
-                    self.echo_debug("No matching batches were found.")
+            for uploads in self.get_paginated_sample_sheet():
+                if not uploads:
+                    self.echo_debug("No matching uploads found.")
                     return
 
-                for batch in batches:
-                    self.echo_data(get_line(batch))
-        except client.APIClientError as err:
-            self.echo_debug(err)
-            if err.status_code == 400:
-                self.echo_warning("There was an error listing project batches.")
-                self.echo_info("The following error was returned:")
-                self.echo_info(err.message)
-            elif err.status_code == 404:
-                self.echo_warning(f"Project {self.project_id} does not exist.")
-            else:
-                raise
+                for upload in uploads:
+                    self.echo_data(get_line(upload))
+        except APIClientError as err:
+            if err.status_code == 404:
+                self.echo_error("Uploads do not exist.")
+            raise
 
-    def get_paginated_batches(self):
-        """Paginate over all batches for the destination.
+    def get_paginated_sample_sheet(self):
+        """Paginate over all sample sheet pages.
 
         Yields:
-            paginated lists of batches
+            paginated lists of uploads
         """
         more = True
         next_link = None
         while more:
-            self.echo_debug("Get batches page")
-            resp = self.get_batches(next_link)
+            self.echo_debug("Get sample sheet page")
+            resp = self.get_sample_sheet(next_link)
             yield resp.results
             next_link = resp.meta.next
             more = next_link is not None
 
     @backoff.on_exception(
         backoff.expo,
-        (client.APIClientTimeout),
-        max_tries=2,
+        (APIClientTimeout),
+        max_tries=5,
         max_time=30,
     )
-    def get_batches(self, next_link=None):
-        """Get batches page."""
-        return self.api_client.get_project_batches(
-            project_id=self.project_id, next_link=next_link
+    def get_sample_sheet(self, next_link=None):
+        """Get sample sheet page."""
+        return self.api_client.get_sample_sheet(
+            gncv_path=self.gncv_path,
+            assigned_status=self.status,
+            next_link=next_link,
         )
```

### Comparing `gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/cli.py` & `gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/main.py` & `gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/list_pipelines/cli.py` & `gencove-2.5.0/gencove/command/projects/list_pipelines/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/list_pipelines/main.py` & `gencove-2.5.0/gencove/command/projects/list_pipelines/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/restore_samples/main.py` & `gencove-2.5.0/gencove/command/s3_imports/s3_import/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,58 @@
-"""Request project's samples restore."""
-from gencove import client  # noqa: I100
-from gencove.command.base import Command
-from gencove.command.utils import is_valid_uuid
-from gencove.exceptions import ValidationError
-
-
-class RestoreSamples(Command):
-    """Restore project's samples."""
-
-    # pylint: disable=too-many-arguments
-    def __init__(
-        self,
-        project_id,
-        sample_ids,
-        credentials,
-        options,
-    ):
+"""Import samples from S3 to a project subcommand."""
+
+import json
+
+from ...base import Command
+from ...utils import is_valid_json
+from .... import client
+from ....exceptions import ValidationError
+
+
+class S3Import(Command):
+    """S3 import command executor."""
+
+    def __init__(self, s3_uri, project_id, credentials, options):
         super().__init__(credentials, options)
+        self.s3_uri = s3_uri
         self.project_id = project_id
-        self.sample_ids = sample_ids
+        self.metadata_json = options.metadata_json
 
     def initialize(self):
-        """Initialize list subcommand."""
+        """Initialize s3-import subcommand."""
         self.login()
 
     def validate(self):
         """Validate command input.
 
         Raises:
             ValidationError - if something is wrong with command parameters.
         """
-        if is_valid_uuid(self.project_id) is False:
-            raise ValidationError("Project ID is not valid. Exiting.")
-
-        if self.sample_ids:
-            if not all(is_valid_uuid(s_id) for s_id in self.sample_ids):
-                raise ValidationError("Not all sample IDs are valid. Exiting.")
+        if self.metadata_json and is_valid_json(self.metadata_json) is False:
+            raise ValidationError("Metadata JSON is not valid. Exiting.")
 
     # no retry for timeouts in order to avoid duplicate heavy operations on
     # the backend
     def execute(self):
-        """Make a request to request samples restore for given project."""
+        """Make a request to import samples from S3 to a given
+        project.
+        """
         self.echo_debug(
-            "Requesting samples restore in project "
-            f"{self.project_id} for samples {self.sample_ids}"
+            f"Import samples from {self.s3_uri} to project {self.project_id}"
         )
 
         try:
-            restored_project_samples_details = self.api_client.restore_project_samples(
+            # prepare metadata
+            metadata = None
+            if self.metadata_json is not None:
+                metadata = json.loads(self.metadata_json)
+                self.echo_info("Assigning metadata to the imported samples.")
+            s3_uri_import = self.api_client.s3_uri_import(
+                s3_uri=self.s3_uri,
                 project_id=self.project_id,
-                sample_ids=self.sample_ids,
+                metadata=metadata,
             )
-            self.echo_debug(restored_project_samples_details)
-            self.echo_info("Request to restore samples accepted.")
-        except client.APIClientError as err:
-            self.echo_debug(err)
-            if err.status_code == 400:
-                self.echo_warning(
-                    "There was an error requesting project samples restore."
-                )
-                self.echo_info("The following error was returned:")
-                self.echo_info(err.message)
-            elif err.status_code == 404:
-                self.echo_warning(f"Project {self.project_id} does not exist.")
-            else:
-                raise
+            self.echo_debug(s3_uri_import)
+            self.echo_info("Request to import samples from S3 accepted.")
+        except client.APIClientError:
+            self.echo_error("There was an error importing from S3.")
+            raise
```

### Comparing `gencove-2.4.7/gencove/command/projects/run_prefix/cli.py` & `gencove-2.5.0/gencove/command/projects/run_prefix/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Project assign all uploads from a prefix shell command definition."""
 import click
 
 from gencove.command.common_cli_options import add_options, common_options
+from gencove.command.utils import validate_uuid
 from gencove.constants import Credentials, SampleAssignmentStatus
 from gencove.utils import enum_as_dict
 
 
 from .constants import RunPrefixOptionals
 from .main import RunPrefix
 
 
 @click.command("run-prefix")
-@click.argument("project_id")
+@click.argument("project_id", callback=validate_uuid)
 @click.argument("prefix")
 @click.option(
     "--metadata-json",
     required=False,
     default=None,
     help=("Add metadata to all uploads that are to be assigned to a project."),
 )
```

### Comparing `gencove-2.4.7/gencove/command/projects/run_prefix/main.py` & `gencove-2.5.0/gencove/command/projects/run_prefix/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Assign uploads from a prefix to a project subcommand."""
 
 import json
 
 import backoff
 
 from ...base import Command
-from ...utils import is_valid_json, is_valid_uuid
+from ...utils import is_valid_json
 from .... import client
 from ....constants import ASSIGN_BATCH_SIZE, UPLOAD_PREFIX
 from ....exceptions import ValidationError
 from ....utils import batchify
 
 
 class RunPrefix(Command):
@@ -28,16 +28,14 @@
 
     def validate(self):
         """Validate command input.
 
         Raises:
             ValidationError - if something is wrong with command parameters.
         """
-        if is_valid_uuid(self.project_id) is False:
-            raise ValidationError("Project ID is not valid. Exiting.")
         if self._valid_prefix() is False:
             raise ValidationError("Prefix is not valid. Exiting.")
         if self.metadata_json and is_valid_json(self.metadata_json) is False:
             raise ValidationError("Metadata JSON is not valid. Exiting.")
 
     def execute(self):
         """Assign samples to the project from the prefixed path."""
```

### Comparing `gencove-2.4.7/gencove/command/projects/samples/cli.py` & `gencove-2.5.0/gencove/command/projects/samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/samples/main.py` & `gencove-2.5.0/gencove/command/projects/samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/samples/utils.py` & `gencove-2.5.0/gencove/command/projects/samples/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/projects/status_merged_vcf/cli.py` & `gencove-2.5.0/gencove/command/projects/list_batch_types/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-"""Project status merged VCF shell command definition."""
+"""Project batch types list shell command definition."""
 import click
 
 from gencove.command.common_cli_options import add_options, common_options
+from gencove.command.utils import validate_uuid
 from gencove.constants import Credentials, Optionals
 
-from .main import StatusMergedVCF
+from .main import ListBatchTypes
 
 
-@click.command("status-merged-vcf")
-@click.argument("project_id")
+@click.command("list-batch-types")
+@click.argument("project_id", callback=validate_uuid)
 @add_options(common_options)
-def status_merged_vcf(
-    project_id,
-    host,
-    email,
-    password,
-    api_key,
-):
-    """Get status of merge VCF files job in a project."""
-    StatusMergedVCF(
+def list_project_batch_types(project_id, host, email, password, api_key):
+    """List batch types that are available for a project."""
+    ListBatchTypes(
         project_id,
         Credentials(email=email, password=password, api_key=api_key),
         Optionals(host=host),
     ).run()
```

### Comparing `gencove-2.4.7/gencove/command/projects/status_merged_vcf/main.py` & `gencove-2.5.0/gencove/command/projects/status_merged_vcf/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Merge project's VCF files executor."""
 import backoff
 
 from .utils import get_line
 from ...base import Command
-from ...utils import is_valid_uuid
 from .... import client
-from ....exceptions import ValidationError
 
 
 class StatusMergedVCF(Command):
     """Executor for retrieving the status of a job for merging project's VCF
     files.
     """
 
@@ -23,21 +21,15 @@
         self.project_id = project_id
 
     def initialize(self):
         """Initialize subcommand."""
         self.login()
 
     def validate(self):
-        """Validate command input.
-
-        Raises:
-            ValidationError - if something is wrong with command parameters.
-        """
-        if is_valid_uuid(self.project_id) is False:
-            raise ValidationError("Project ID is not valid. Exiting.")
+        """Validate command input."""
 
     @backoff.on_exception(
         backoff.expo,
         (client.APIClientTimeout),
         max_tries=5,
         max_time=30,
     )
```

### Comparing `gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/cli.py` & `gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/main.py` & `gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/s3_imports/autoimports/create/cli.py` & `gencove-2.5.0/gencove/command/s3_imports/autoimports/create/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Project autoimport from S3 shell command definition.
 """
 import click
 
 from gencove.command.common_cli_options import add_options, common_options
+from gencove.command.utils import validate_uuid
 from gencove.constants import Credentials
 
 from .constants import S3AutoImportOptionals
 from .main import S3AutoImport
 
 
 @click.command("create")
-@click.argument("project_id")
+@click.argument("project_id", callback=validate_uuid)
 @click.argument("s3_uri")
 @click.option(
     "--metadata-json",
     required=False,
     default=None,
     help=("Add metadata to all samples that are to be imported from S3 to a project."),
 )
```

### Comparing `gencove-2.4.7/gencove/command/s3_imports/autoimports/create/main.py` & `gencove-2.5.0/gencove/command/samples/set_metadata/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,58 @@
-"""AutoImport S3 URI to a project subcommand."""
+"""Set sample metadata subcommand."""
 
 import json
 
-from ..... import client
-from .....exceptions import ValidationError
-from ....base import Command  # noqa: I100
-from ....utils import is_valid_json, is_valid_uuid
+from ...base import Command
+from ...utils import is_valid_json, is_valid_uuid
+from .... import client
+from ....exceptions import ValidationError
 
 
-class S3AutoImport(Command):
-    """S3AutoImport autoimport command executor."""
+class SetMetadata(Command):
+    """Set metadata command executor."""
 
-    def __init__(self, project_id, s3_uri, credentials, options):
+    def __init__(self, sample_id, json_metadata, credentials, options):
         super().__init__(credentials, options)
-        self.project_id = project_id
-        self.s3_uri = s3_uri
-        self.metadata_json = options.metadata_json
+        self.sample_id = sample_id
+        self.json_metadata = json_metadata
 
     def initialize(self):
-        """Initialize s3-autoimport subcommand."""
+        """Initialize set-metadata subcommand."""
         self.login()
 
     def validate(self):
         """Validate command input.
 
         Raises:
             ValidationError - if something is wrong with command parameters.
         """
-        if is_valid_uuid(self.project_id) is False:
-            raise ValidationError("Project ID is not valid. Exiting.")
-        if self.metadata_json and is_valid_json(self.metadata_json) is False:
+
+        if is_valid_uuid(self.sample_id) is False:
+            raise ValidationError("Sample ID is not valid. Exiting.")
+
+        if is_valid_json(self.json_metadata) is False:
             raise ValidationError("Metadata JSON is not valid. Exiting.")
 
     # no retry for timeouts in order to avoid duplicate heavy operations on
     # the backend
     def execute(self):
-        """Make a request to create a job to automatically import
-        from S3 URI to a Gencove project.
-        """
-        self.echo_debug(
-            "Create AutoImport job from "
-            f"s3_uri {self.s3_uri} to project {self.project_id}"
-        )
+        """Make a request to assign given metadata to a specified sample."""
+
+        self.echo_debug(f"Assigning metadata to a sample {self.sample_id}")
 
         try:
-            # prepare metadata
-            metadata = None
-            if self.metadata_json is not None:
-                metadata = json.loads(self.metadata_json)
-                self.echo_info("Metadata will be assigned to the imported Biosamples.")
-            autoimport_from_s3 = self.api_client.autoimport_from_s3(
-                project_id=self.project_id,
-                s3_uri=self.s3_uri,
-                metadata=metadata,
-            )
-            self.echo_info(
-                "Request to create a periodic import job from"
-                "S3 URI to project accepted."
-            )
-            self.echo_data(
-                "\t".join(
-                    [
-                        str(autoimport_from_s3.id),
-                        autoimport_from_s3.topic_arn,
-                    ]
-                )
+            metadata_api = None
+            if self.json_metadata is not None:
+                metadata_api = json.loads(self.json_metadata)
+            assigned_metadata = self.api_client.set_metadata(
+                self.sample_id, metadata_api
             )
-        except client.APIClientError:
-            self.echo_error("There was an error creating an import job of S3 URI.")
+            self.echo_debug(assigned_metadata)
+            self.echo_info(f"Assigned metadata to a sample {self.sample_id}")
+        except client.APIClientError as err:
+            self.echo_debug(err)
+            if err.status_code == 400:
+                self.echo_error("There was an error assigning metadata.")
+            elif err.status_code == 404:
+                self.echo_error(f"Sample {self.sample_id} does not exist.")
             raise
```

### Comparing `gencove-2.4.7/gencove/command/s3_imports/s3_import/cli.py` & `gencove-2.5.0/gencove/command/s3_imports/s3_import/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Project import samples from S3 URI to projects shell command definition.
 """
 import click
 
 from gencove.command.common_cli_options import add_options, common_options
+from gencove.command.utils import validate_uuid
 from gencove.constants import Credentials
 
 from .constants import S3ImportOptionals
 from .main import S3Import
 
 
 @click.command("import")
 @click.argument("s3_uri")
-@click.argument("project_id")
+@click.argument("project_id", callback=validate_uuid)
 @click.option(
     "--metadata-json",
     required=False,
     default=None,
     help=("Add metadata to all samples that are to be imported from S3 to a project."),
 )
 @add_options(common_options)
```

### Comparing `gencove-2.4.7/gencove/command/s3_imports/s3_import/main.py` & `gencove-2.5.0/gencove/command/s3_imports/autoimports/create/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,69 @@
-"""Import samples from S3 to a project subcommand."""
+"""AutoImport S3 URI to a project subcommand."""
 
 import json
 
-from ...base import Command
-from ...utils import is_valid_json, is_valid_uuid
-from .... import client
-from ....exceptions import ValidationError
+from ..... import client
+from .....exceptions import ValidationError
+from ....base import Command  # noqa: I100
+from ....utils import is_valid_json
 
 
-class S3Import(Command):
-    """S3 import command executor."""
+class S3AutoImport(Command):
+    """S3AutoImport autoimport command executor."""
 
-    def __init__(self, s3_uri, project_id, credentials, options):
+    def __init__(self, project_id, s3_uri, credentials, options):
         super().__init__(credentials, options)
-        self.s3_uri = s3_uri
         self.project_id = project_id
+        self.s3_uri = s3_uri
         self.metadata_json = options.metadata_json
 
     def initialize(self):
-        """Initialize s3-import subcommand."""
+        """Initialize s3-autoimport subcommand."""
         self.login()
 
     def validate(self):
         """Validate command input.
 
         Raises:
             ValidationError - if something is wrong with command parameters.
         """
-        if is_valid_uuid(self.project_id) is False:
-            raise ValidationError("Project ID is not valid. Exiting.")
         if self.metadata_json and is_valid_json(self.metadata_json) is False:
             raise ValidationError("Metadata JSON is not valid. Exiting.")
 
     # no retry for timeouts in order to avoid duplicate heavy operations on
     # the backend
     def execute(self):
-        """Make a request to import samples from S3 to a given
-        project.
+        """Make a request to create a job to automatically import
+        from S3 URI to a Gencove project.
         """
         self.echo_debug(
-            f"Import samples from {self.s3_uri} to project {self.project_id}"
+            "Create AutoImport job from "
+            f"s3_uri {self.s3_uri} to project {self.project_id}"
         )
 
         try:
             # prepare metadata
             metadata = None
             if self.metadata_json is not None:
                 metadata = json.loads(self.metadata_json)
-                self.echo_info("Assigning metadata to the imported samples.")
-            s3_uri_import = self.api_client.s3_uri_import(
-                s3_uri=self.s3_uri,
+                self.echo_info("Metadata will be assigned to the imported Biosamples.")
+            autoimport_from_s3 = self.api_client.autoimport_from_s3(
                 project_id=self.project_id,
+                s3_uri=self.s3_uri,
                 metadata=metadata,
             )
-            self.echo_debug(s3_uri_import)
-            self.echo_info("Request to import samples from S3 accepted.")
+            self.echo_info(
+                "Request to create a periodic import job from"
+                "S3 URI to project accepted."
+            )
+            self.echo_data(
+                "\t".join(
+                    [
+                        str(autoimport_from_s3.id),
+                        autoimport_from_s3.topic_arn,
+                    ]
+                )
+            )
         except client.APIClientError:
-            self.echo_error("There was an error importing from S3.")
+            self.echo_error("There was an error creating an import job of S3 URI.")
             raise
```

### Comparing `gencove-2.4.7/gencove/command/samples/download_file/cli.py` & `gencove-2.5.0/gencove/command/samples/download_file/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/samples/download_file/main.py` & `gencove-2.5.0/gencove/command/samples/download_file/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/samples/download_file/utils.py` & `gencove-2.5.0/gencove/command/samples/download_file/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/samples/get_metadata/cli.py` & `gencove-2.5.0/gencove/command/samples/get_metadata/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/samples/get_metadata/main.py` & `gencove-2.5.0/gencove/command/samples/get_metadata/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/samples/set_metadata/cli.py` & `gencove-2.5.0/gencove/command/samples/set_metadata/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/upload/cli.py` & `gencove-2.5.0/gencove/command/upload/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/upload/constants.py` & `gencove-2.5.0/gencove/command/upload/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/upload/main.py` & `gencove-2.5.0/gencove/command/upload/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 )
 from .exceptions import SampleSheetError, UploadError, UploadNotFound
 from .multi_file_reader import MultiFileReader
 from .utils import (
     get_filename_from_path,
     get_get_upload_details_retry_predicate,
     get_gncv_path,
+    looks_like_url,
     parse_fastqs_map_file,
     seek_files_to_upload,
     upload_file,
     upload_multi_file,
 )
 from ..utils import is_valid_json
 from ...constants import ASSIGN_BATCH_SIZE
@@ -151,14 +152,15 @@
     def execute(self):
         """Upload fastq files from host system to Gencove cloud.
 
         If project id was provided, all fastq files will
         be assigned to this project, after upload.
         """
         s3_client = get_s3_client_refreshable(self.api_client.get_upload_credentials)
+
         try:
             if self.fastqs:
                 self.upload_from_source(s3_client)
             elif self.fastqs_map:
                 self.upload_from_map_file(s3_client)
         except UploadError:
             return
@@ -179,19 +181,34 @@
                 self.upload_ids.add(upload.id)
 
         self.echo_info("All files were successfully uploaded.")
 
     def upload_from_map_file(self, s3_client):
         """Upload fastq files from a csv file."""
         for key, fastqs in self.fastqs_map.items():
-            upload = self.concatenate_and_upload_fastqs(key, fastqs, s3_client)
+            if all((looks_like_url(f) for f in fastqs)):
+                upload = self.post_fastq_url(key, fastqs)
+            else:
+                upload = self.concatenate_and_upload_fastqs(key, fastqs, s3_client)
+
             if self.project_id and upload:
                 self.upload_ids.add(upload.id)
 
-        self.echo_info("All files were successfully uploaded.")
+        self.echo_info("All files were successfully processed.")
+
+    def post_fastq_url(self, key, fastqs):
+        """Post FASTQ URL to API endpoint"""
+        client_id, r_notation = key
+        gncv_path = self.destination + get_gncv_path(client_id, r_notation)
+        self.echo_debug(f"Calculated gncv path: {gncv_path}")
+        upload_url_details = self.api_client.import_fastqs_from_url(
+            gncv_file_path=gncv_path,
+            url=next(iter(fastqs)),
+        )
+        return upload_url_details
 
     def concatenate_and_upload_fastqs(self, key, fastqs, s3_client):
         """Upload fastqs parts as one file."""
         client_id, r_notation = key
         self.echo_debug(
             f"Uploading fastq. client_id={client_id} r_notation={r_notation}"
         )
```

### Comparing `gencove-2.4.7/gencove/command/upload/multi_file_reader.py` & `gencove-2.5.0/gencove/command/upload/multi_file_reader.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/upload/utils.py` & `gencove-2.5.0/gencove/command/upload/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Utils for upload command."""
 import csv
 import os
 import platform
+import re
+import urllib.parse
 from collections import defaultdict
+from urllib.parse import urlparse
 
 from boto3.s3.transfer import TransferConfig
 
 from botocore.exceptions import ClientError
 
 from gencove.exceptions import ValidationError
 from gencove.logger import echo_debug, echo_info
@@ -128,14 +131,15 @@
     Args:
         pbar: progressbar.ProgressBar instance
 
     Returns:
         a function that in turn accepts chunk that is used to update the
         progressbar.
     """
+
     # noqa: D202
     def _update_pbar(chunk_uploaded_in_bytes):
         pbar.update(pbar.value + chunk_uploaded_in_bytes)
 
     return _update_pbar
 
 
@@ -174,23 +178,30 @@
     Args:
         fastq (FastQ): fastq object
     Returns:
         None if all good
     Raises:
         ValidationError if fastq is not valid
     """
-    if not fastq.path.lower().endswith(FASTQ_EXTENSIONS):
-        echo_info(f"Unsupported file type found: {fastq.path}")
-        raise ValidationError(f"Bad file extension in path: {fastq.path}")
+    if looks_like_url(fastq.path):
+        if not valid_fastq_file_name_in_url(fastq.path):
+            raise ValidationError(
+                f"Could not determine FASTQ file name from supplied URL {fastq.path}"
+            )
+    else:
+        if not fastq.path.lower().endswith(FASTQ_EXTENSIONS):
+            echo_info(f"Unsupported file type found: {fastq.path}")
+            raise ValidationError(f"Bad file extension in path: {fastq.path}")
+        if not os.path.exists(fastq.path):
+            echo_info(f"Path does not exist: {fastq.path}")
+            raise ValidationError(f"Could not find: {fastq.path}")
+
     if "_" in fastq.client_id:
         echo_info("Underscore is not allowed in client id")
         raise ValidationError("Underscore is not allowed in client id")
-    if not os.path.exists(fastq.path):
-        echo_info(f"Path does not exist: {fastq.path}")
-        raise ValidationError(f"Could not find: {fastq.path}")
     if fastq.r_notation not in R_NOTATION_MAP:
         echo_info(f"Wrong R notation: {fastq.r_notation}")
         echo_info(f"Valid R notations are: {R_NOTATION_MAP.keys()}")
         raise ValidationError(f"Wrong R notation: {fastq.r_notation}")
 
 
 def _validate_header(header):
@@ -204,14 +215,16 @@
 
 def parse_fastqs_map_file(fastqs_map_path):
     """Parse fastq map file.
 
     Map file has to have following columns/headers:
         client_id, r_notation, path
 
+    Note this map file also supports URLs under the path column
+
     Example fastqs map file:
         client_id,r_notation,path
         sample1,R1,dir1/sample1_L001_R1.fastq.gz
         sample1,R1,dir1/sample1_L002_R1.fastq.gz
         sample2,R2,dir2/sample1_L001_R2.fastq.gz
 
     Args:
@@ -250,7 +263,38 @@
     """
     return PATH_TEMPLATE.format(
         **{
             PathTemplateParts.client_id.value: client_id,
             PathTemplateParts.r_notation.value: r_notation,
         }
     )
+
+
+def looks_like_url(value):
+    """Detects if input value appears to be a URL
+
+    Args:
+        value (str): value to test
+
+    Returns:
+        bool: True if URL-like, False otherwise
+    """
+    try:
+        result = urlparse(value)
+        if result.scheme in ["http", "https"]:
+            if result.netloc:
+                return True
+    except ValueError:
+        return False
+    return False
+
+
+def valid_fastq_file_name_in_url(value):
+    """Attempt to detect FASTQ file name in URL"""
+    path = urllib.parse.urlparse(value).path
+    fastq_extensions_regex = [x.replace(".", r"\.") for x in FASTQ_EXTENSIONS]
+    re_fastq_extensions = "|".join(fastq_extensions_regex)
+    re_pattern = rf"/([^/]*?({re_fastq_extensions}))$"
+    match = re.search(re_pattern, path)
+    if match:
+        return True
+    return False
```

### Comparing `gencove-2.4.7/gencove/command/uploads/list/cli.py` & `gencove-2.5.0/gencove/command/uploads/list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/uploads/list/utils.py` & `gencove-2.5.0/gencove/command/uploads/list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/utils.py` & `gencove-2.5.0/gencove/command/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/webhook/verify/cli.py` & `gencove-2.5.0/gencove/command/webhook/verify/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/command/webhook/verify/utils.py` & `gencove-2.5.0/gencove/command/webhook/verify/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/constants.py` & `gencove-2.5.0/gencove/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 @unique
 class ApiEndpoints(Enum):
     """ApiEndpoints enum"""
 
     GET_JWT = "/api/v2/jwt-create/"
     REFRESH_JWT = "/api/v2/jwt-refresh/"
     UPLOAD_DETAILS = "/api/v2/uploads-post-data/"
+    UPLOAD_URL = "/api/v2/uploads-url/"
     GET_UPLOAD_CREDENTIALS = "/api/v2/upload-credentials/"
     PROJECT_SAMPLES = "/api/v2/project-samples/{id}"
     SAMPLE_DETAILS = "/api/v2/samples/{id}"
     SAMPLE_QC_METRICS = "/api/v2/sample-quality-controls/{id}"
     SAMPLE_SHEET = "/api/v2/sample-sheet/"
     PROJECTS = "/api/v2/projects/"
     PIPELINE_CAPABILITES = "/api/v2/pipeline-capabilities/{id}"
```

### Comparing `gencove-2.4.7/gencove/description/pypi_readme.md` & `gencove-2.5.0/gencove/description/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/logger.py` & `gencove-2.5.0/gencove/logger.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/models.py` & `gencove-2.5.0/gencove/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,7 +371,16 @@
 
 
 class Pipelines(BaseModel):
     """Pipeline model"""
 
     meta: ResponseMeta
     results: Optional[List[Pipeline]]
+
+
+class UploadURLImport(GencoveBaseModel):
+    """URL import moodel"""
+
+    s3: Optional[S3Object]
+    last_status: Optional[GencoveStatus]
+    destination_path: Optional[str]
+    source_url: Optional[str]
```

### Comparing `gencove-2.4.7/gencove/tests/basespace/test_basespace_autoimports_create.py` & `gencove-2.5.0/gencove/tests/basespace/test_basespace_autoimports_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from click.testing import CliRunner
 
 from gencove.client import APIClient, APIClientError
 from gencove.command.basespace.autoimports.create.cli import (
     create,
 )
-from gencove.tests.decorators import assert_authorization
+from gencove.tests.decorators import assert_authorization, assert_no_requests
 from gencove.tests.filters import filter_jwt, replace_gencove_url_vcr
 from gencove.tests.utils import MOCK_UUID
 
 import pytest
 
 from vcr import VCR
 
@@ -37,17 +37,15 @@
         ],
         "before_record_response": [
             filter_jwt,
         ],
     }
 
 
-@pytest.mark.default_cassette("jwt-create.yaml")
-@pytest.mark.vcr
-@assert_authorization
+@assert_no_requests
 def test_basespace_autoimport_create_project_id_not_uuid(
     credentials,
     mocker,
 ):
     """Test that project id is valid UUID when creating an automated import."""
     runner = CliRunner()
```

### Comparing `gencove-2.4.7/gencove/tests/basespace/test_basespace_autoimports_list.py` & `gencove-2.5.0/gencove/tests/basespace/test_basespace_autoimports_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/basespace/test_basespace_biosamples_list.py` & `gencove-2.5.0/gencove/tests/basespace/test_basespace_biosamples_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/basespace/test_basespace_projects_import.py` & `gencove-2.5.0/gencove/tests/basespace/test_basespace_projects_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             "--email",
             "foo@bar.com",
             "--password",
             "123",
         ],
     )
     assert res.exit_code == 1
-    mocked_login.assert_called_once()
+    mocked_login.assert_not_called()
     mocked_import_basespace_projects.assert_not_called()
     assert "Project ID is not valid" in res.output
 
 
 def test_basespace_import__bad_json(mocker):
     """Test BaseSpace import when bad JSON is used."""
     runner = CliRunner()
```

### Comparing `gencove-2.4.7/gencove/tests/basespace/test_basespace_projects_list.py` & `gencove-2.5.0/gencove/tests/basespace/test_basespace_projects_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/conftest.py` & `gencove-2.5.0/gencove/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/decorators.py` & `gencove-2.5.0/gencove/tests/decorators.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/download/test_cli_download.py` & `gencove-2.5.0/gencove/tests/download/test_cli_download.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/download/vcr/filters.py` & `gencove-2.5.0/gencove/tests/download/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/files/test_file_types_list.py` & `gencove-2.5.0/gencove/tests/files/test_file_types_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/filters.py` & `gencove-2.5.0/gencove/tests/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_batch_get.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_batch_get.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_batch_types_list.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_batch_types_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_batches_create.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_batches_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from click import echo
 from click.testing import CliRunner
 
 from gencove.client import APIClient, APIClientError  # noqa: I100
 from gencove.command.projects.cli import create_project_batch
 from gencove.models import ProjectBatches
-from gencove.tests.decorators import assert_authorization
+from gencove.tests.decorators import assert_authorization, assert_no_requests
 from gencove.tests.filters import filter_jwt, replace_gencove_url_vcr
 from gencove.tests.projects.vcr.filters import (
     filter_project_batches_request,
     filter_project_batches_response,
 )
 from gencove.tests.upload.vcr.filters import filter_volatile_dates
 from gencove.tests.utils import get_vcr_response
@@ -91,17 +91,15 @@
         ],
     )
     assert res.exit_code == 1
     mocked_create_project_batch.assert_not_called()
     assert "You must provide value for --batch-name" in res.output
 
 
-@pytest.mark.default_cassette("jwt-create.yaml")
-@pytest.mark.vcr
-@assert_authorization
+@assert_no_requests
 def test_create_project_batches__bad_project_id(credentials, mocker):
     """Test batch creation failure when non-uuid string is used as project
     id.
     """
     runner = CliRunner()
     mocked_create_project_batch = mocker.patch.object(
         APIClient,
```

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_batches_list.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_batches_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_create.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_create_merged_vcf.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_create_merged_vcf.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             "foo@bar.com",
             "--password",
             "123",
         ],
     )
 
     assert res.exit_code == 1
-    mocked_login.assert_called_once()
+    mocked_login.assert_not_called()
     mocked_create_merged_vcf.assert_not_called()
     assert "Project ID is not valid" in res.output
 
 
 def test_create_merged_vcf__not_owned_project(mocker):
     """Test create merged file failure when project is not owned."""
     mocked_response = {"detail": "Not found."}
```

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_delete_samples.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_delete_samples.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_get_merged_vcf.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_get_merged_vcf.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             "foo@bar.com",
             "--password",
             "123",
         ],
     )
 
     assert res.exit_code == 1
-    mocked_login.assert_called_once()
+    mocked_login.assert_not_called()
     mocked_get_project.assert_not_called()
     assert "Project ID is not valid" in res.output
 
 
 def test_get_merged_vcf__not_owned_project(mocker):
     """Test get merged file failure when project is not owned."""
     mocked_response = {"detail": "Not found."}
```

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_import_existing_samples.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_import_existing_samples.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from uuid import uuid4
 
 from click.testing import CliRunner
 
 from gencove.client import APIClient, APIClientError
 from gencove.command.projects.cli import import_existing_project_samples
 from gencove.models import ImportExistingSamplesModel
-from gencove.tests.decorators import assert_authorization
+from gencove.tests.decorators import assert_authorization, assert_no_requests
 from gencove.tests.filters import filter_jwt, replace_gencove_url_vcr
 from gencove.tests.projects.vcr.filters import (
     filter_import_existing_samples_request,
     filter_import_existing_samples_response,
 )
 from gencove.tests.utils import MOCK_UUID, get_vcr_response
 
@@ -45,17 +45,15 @@
         "before_record_response": [
             filter_jwt,
             filter_import_existing_samples_response,
         ],
     }
 
 
-@pytest.mark.default_cassette("jwt-create.yaml")
-@pytest.mark.vcr
-@assert_authorization
+@assert_no_requests
 def test_import_existing_project_samples__bad_project_id(mocker, credentials):
     """Test import existing project samples failure when non-uuid string is used as
     project id.
     """
     runner = CliRunner()
 
     mocked_import_existing_samples = mocker.patch.object(
@@ -64,27 +62,25 @@
     )
 
     res = runner.invoke(
         import_existing_project_samples,
         [
             "1111111",
             "--sample-ids",
-            "1111111,2222222",
+            f"{str(uuid4())},{str(uuid4())}",
             *credentials,
         ],
     )
 
     assert res.exit_code == 1
     mocked_import_existing_samples.assert_not_called()
     assert "Project ID is not valid" in res.output
 
 
-@pytest.mark.default_cassette("jwt-create.yaml")
-@pytest.mark.vcr
-@assert_authorization
+@assert_no_requests
 def test_import_existing_project_samples__bad_sample_ids(mocker, credentials):
     """Test import existing project samples failure when sample_ids are bad."""
     runner = CliRunner()
 
     mocked_import_existing_samples = mocker.patch.object(
         APIClient,
         "import_existing_samples",
```

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_list.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_pipeline_capabilities_list.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_pipeline_capabilities_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_pipelines_list.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_pipelines_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_restore_samples.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_restore_samples.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from click.testing import CliRunner
 
 from gencove.client import (
     APIClient,
     APIClientError,
 )  # noqa: I100
 from gencove.command.projects.cli import restore_project_samples
-from gencove.tests.decorators import assert_authorization
+from gencove.tests.decorators import assert_authorization, assert_no_requests
 from gencove.tests.filters import filter_jwt, replace_gencove_url_vcr
 from gencove.tests.projects.vcr.filters import (
     filter_post_project_restore_samples,
 )
 from gencove.tests.upload.vcr.filters import filter_volatile_dates
 from gencove.tests.utils import get_vcr_response
 
@@ -46,17 +46,15 @@
         "before_record_response": [
             filter_jwt,
             filter_volatile_dates,
         ],
     }
 
 
-@pytest.mark.default_cassette("jwt-create.yaml")
-@pytest.mark.vcr
-@assert_authorization
+@assert_no_requests
 def test_restore_project_samples__bad_project_id(mocker, credentials):
     """Test restore project samples when non-uuid string is used as project
     id."""
     runner = CliRunner()
     mocked_restore_project_samples = mocker.patch.object(
         APIClient,
         "restore_project_samples",
@@ -133,17 +131,15 @@
         ],
     )
     assert res.exit_code == 0
     if not recording:
         mocked_restore_project_samples.assert_called_once()
 
 
-@pytest.mark.default_cassette("jwt-create.yaml")
-@pytest.mark.vcr
-@assert_authorization
+@assert_no_requests
 def test_restore_project_samples__invalid_sample_ids(credentials, mocker):
     """Test restore project samples failure when an empty list of sample ids
     is sent."""
 
     runner = CliRunner()
     mocked_restore_project_samples = mocker.patch.object(
         APIClient, "restore_project_samples"
```

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_run_prefix.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_run_prefix.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             "--email",
             "foo@bar.com",
             "--password",
             "123",
         ],
     )
     assert res.exit_code == 1
-    mocked_login.assert_called_once()
+    mocked_login.assert_not_called()
     mocked_get_sample_sheet.assert_not_called()
     assert "Project ID is not valid" in res.output
 
 
 def test_run_prefix__bad_prefix(mocker):
     """Test run prefix when bad prefix string is used."""
     runner = CliRunner()
```

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_samples_list.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_samples_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/projects/test_projects_status_merged_vcf.py` & `gencove-2.5.0/gencove/tests/projects/test_projects_status_merged_vcf.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             "foo@bar.com",
             "--password",
             "123",
         ],
     )
 
     assert res.exit_code == 1
-    mocked_login.assert_called_once()
+    mocked_login.assert_not_called()
     mocked_retrieve_merged_vcf.assert_not_called()
     assert "Project ID is not valid" in res.output
 
 
 def test_status_merged_vcf__empty(mocker):
     """Test create merged file failure when project is responding empty.
     This can be due to no merged files or no permission required for the
```

### Comparing `gencove-2.4.7/gencove/tests/projects/vcr/filters.py` & `gencove-2.5.0/gencove/tests/projects/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/s3_imports/test_s3_autoimports_create.py` & `gencove-2.5.0/gencove/tests/s3_imports/test_s3_autoimports_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from uuid import uuid4
 
 import pytest
 from click.testing import CliRunner  # noqa: I100,I201
 from gencove.client import APIClient, APIClientError  # noqa: I201
 from gencove.command.s3_imports.autoimports.create.cli import create
 from gencove.models import S3AutoimportTopic
-from gencove.tests.decorators import assert_authorization
+from gencove.tests.decorators import assert_authorization, assert_no_requests
 from gencove.tests.filters import filter_jwt, replace_gencove_url_vcr
 
 from vcr import VCR
 
 
 @pytest.fixture(scope="module")
 def vcr_config():
@@ -35,17 +35,15 @@
         ],
         "before_record_response": [
             filter_jwt,
         ],
     }
 
 
-@pytest.mark.default_cassette("jwt-create.yaml")
-@pytest.mark.vcr
-@assert_authorization
+@assert_no_requests
 def test_s3_autoimport_create_project_id_not_uuid(
     credentials,
     mocker,
 ):
     """Test that project id is valid UUID when creating an automated import."""
     runner = CliRunner()
```

### Comparing `gencove-2.4.7/gencove/tests/s3_imports/test_s3_autoimports_list.py` & `gencove-2.5.0/gencove/tests/s3_imports/test_s3_autoimports_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/s3_imports/test_s3_uri_import.py` & `gencove-2.5.0/gencove/tests/s3_imports/test_s3_uri_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             "--email",
             "foo@bar.com",
             "--password",
             "123",
         ],
     )
     assert res.exit_code == 1
-    mocked_login.assert_called_once()
+    mocked_login.assert_not_called()
     mocked_import_s3_projects.assert_not_called()
     assert "Project ID is not valid" in res.output
 
 
 def test_s3_import__bad_json(mocker):
     """Test S3 import when bad JSON is used."""
     runner = CliRunner()
```

### Comparing `gencove-2.4.7/gencove/tests/samples/test_samples_download_file.py` & `gencove-2.5.0/gencove/tests/samples/test_samples_download_file.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/samples/test_samples_get_metadata.py` & `gencove-2.5.0/gencove/tests/samples/test_samples_get_metadata.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/samples/test_samples_set_metadata.py` & `gencove-2.5.0/gencove/tests/samples/test_samples_set_metadata.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/samples/vcr/filters.py` & `gencove-2.5.0/gencove/tests/samples/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/test_logger.py` & `gencove-2.5.0/gencove/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/test_utils.py` & `gencove-2.5.0/gencove/tests/test_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 from gencove.command.download.utils import (
     _get_prefix_parts,
     build_file_path,
     get_download_template_format_params,
 )
 from gencove.command.upload.utils import (
     _validate_header,
+    looks_like_url,
     parse_fastqs_map_file,
     upload_file,
+    valid_fastq_file_name_in_url,
 )
 from gencove.command.utils import is_valid_uuid, validate_uuid, validate_uuid_list
 from gencove.constants import (
     ApiEndpoints,
     Credentials,
     DOWNLOAD_TEMPLATE,
     DownloadTemplateParts,
@@ -288,14 +290,106 @@
             )
         try:
             parse_fastqs_map_file("test_map.csv")
         except ValidationError as err:
             assert "Unexpected CSV header" in err.args[0]
 
 
+def test_parse_fastqs_map_file_with_urls():
+    """Test parsing of map file with URLs into dict"""
+    runner = CliRunner()
+    with runner.isolated_filesystem():
+        with open("test_url_map.fastq-map.csv", "w", encoding="utf-8") as map_file:
+            writer = csv.writer(map_file)
+            writer.writerows(
+                [
+                    ["client_id", "r_notation", "path"],
+                    ["barid", "r1", "https://s3.amazonaws.com/samples/1/R1.fastq.gz"],
+                    ["barid", "r2", "https://s3.amazonaws.com/samples/1/R2.fastq.gz"],
+                    [
+                        "barid",
+                        "r1",
+                        "https://storage.googleapis.com/samples/2/R1.fastq.gz",
+                    ],
+                ]
+            )
+
+        fastqs = parse_fastqs_map_file("test_url_map.fastq-map.csv")
+        assert len(fastqs) == 2
+        assert ("barid", "R1") in fastqs
+        assert ("barid", "R2") in fastqs
+        assert len(fastqs[("barid", "R1")]) == 2
+        assert (
+            fastqs[("barid", "R1")][0]
+            == "https://s3.amazonaws.com/samples/1/R1.fastq.gz"
+        )
+        assert (
+            fastqs[("barid", "R1")][1]
+            == "https://storage.googleapis.com/samples/2/R1.fastq.gz"
+        )
+
+
+def test_parse_fastqs_map_file_with_urls_and_s3():
+    """Test parsing of map file with URLs into dict"""
+    runner = CliRunner()
+    fastq_file_path = "barid-R2.fastq.gz"
+    with runner.isolated_filesystem():
+        with open(fastq_file_path, "w", encoding="utf-8") as fastq_file:
+            fastq_file.write("AAABBB")
+
+        with open("test_url_map.fastq-map.csv", "w", encoding="utf-8") as map_file:
+            writer = csv.writer(map_file)
+            writer.writerows(
+                [
+                    ["client_id", "r_notation", "path"],
+                    [
+                        "barid",
+                        "r1",
+                        "https://s3.amazonaws.com/samples/1/barid-R1.fastq.gz",
+                    ],
+                    ["barid", "r2", fastq_file_path],
+                ]
+            )
+
+        fastqs = parse_fastqs_map_file("test_url_map.fastq-map.csv")
+        assert len(fastqs) == 2
+        assert ("barid", "R1") in fastqs
+        assert ("barid", "R2") in fastqs
+        assert len(fastqs[("barid", "R1")]) == 1
+        assert (
+            fastqs[("barid", "R1")][0]
+            == "https://s3.amazonaws.com/samples/1/barid-R1.fastq.gz"
+        )
+        assert fastqs[("barid", "R2")][0] == fastq_file_path
+
+
+def test_parse_fastqs_map_file_with_urls_invalid():
+    """Test parsing of map file with URLs into dict, invalid URLs"""
+    runner = CliRunner()
+    with runner.isolated_filesystem():
+        with open("test_url_map.fastq-map.csv", "w", encoding="utf-8") as map_file:
+            writer = csv.writer(map_file)
+            writer.writerows(
+                [
+                    ["client_id", "r_notation", "path"],
+                    ["barid", "r1", "https://s3.amazonaws.com/samples/1/invalid"],
+                    ["barid", "r2", "https://s3.amazonaws.com/samples/1/invalid"],
+                    [
+                        "barid",
+                        "r1",
+                        "https://storage.googleapis.com/samples/2/invalid",
+                    ],
+                ]
+            )
+        try:
+            parse_fastqs_map_file("test_url_map.fastq-map.csv")
+        except ValidationError as err:
+            assert "Could not determine FASTQ file" in err.args[0]
+
+
 def test__validate_header():
     """Test that header is validated properly."""
     header_row = dict(foo="foo", bar="bar")
     try:
         _validate_header(header_row)
     except ValidationError:
         pass
@@ -480,7 +574,47 @@
     param = Option(["-sample_ids"], nargs=1, multiple=False, default=None)
     valid_uuid_list = fake.pylist(nb_elements=3, value_types=("uuid4",))
     valid_uuids_string = ",".join(valid_uuid_list)
     uuids_string = f"{valid_uuids_string},{invalid_uuid}"
 
     with pytest.raises(Abort):
         validate_uuid_list(None, param, uuids_string)
+
+
+@pytest.mark.parametrize(
+    "url,expected",
+    [
+        ("http://example.com/file.fastq.bgz", True),
+        ("http://example.com/file.fastq.gz", True),
+        ("http://example.com/file.fq.bgz", True),
+        ("http://example.com/file.fq.gz", True),
+        ("http://example.com/file.txt", False),
+        ("http://example.com/file", False),
+        ("http://example.com/file.fastq", False),
+        ("http://example.com/.fastq", False),
+        ("http://example.com/", False),
+        ("foo", False),
+    ],
+)
+def test_file_name_in_url(url, expected):
+    """Test multiple cases to ensure valid FASTQ file detected"""
+    assert valid_fastq_file_name_in_url(url) == expected
+
+
+@pytest.mark.parametrize(
+    "value,expected",
+    [
+        ("http://example.com", True),
+        ("https://example.com", True),
+        ("http://example.com/file.fastq", True),
+        ("https://www.example.com", True),
+        ("http://", False),
+        ("https://", False),
+        ("example.com", False),
+        ("ftp://example.com", False),
+        ("foo", False),
+        ("", False),
+    ],
+)
+def test_looks_like_url(value, expected):
+    """Test multiple cases of URL strings"""
+    assert looks_like_url(value) == expected
```

### Comparing `gencove-2.4.7/gencove/tests/upload/test_cli_upload.py` & `gencove-2.5.0/gencove/tests/upload/test_cli_upload.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 """Tests upload command of Gencove CLI."""
 
 # pylint: disable=too-many-lines, import-error
 
+import csv
 import json
 import operator
 import os
 from uuid import uuid4
 
 from click.testing import CliRunner
 
-
 from gencove.cli import upload
 from gencove.client import APIClient, APIClientError, APIClientTimeout
 from gencove.command.upload.utils import upload_file
 from gencove.constants import ApiEndpoints, UPLOAD_PREFIX
-from gencove.models import SampleSheet, UploadSamples, UploadsPostData
+from gencove.models import SampleSheet, UploadSamples, UploadURLImport, UploadsPostData
 from gencove.tests.decorators import assert_authorization
 from gencove.tests.filters import (
     filter_aws_headers,
     filter_jwt,
     replace_gencove_url_vcr,
 )
 from gencove.tests.upload.vcr.filters import (
+    filter_import_fastqs_from_url_response,
     filter_project_samples_request,
     filter_project_samples_response,
     filter_sample_sheet_response,
     filter_upload_credentials_response,
     filter_upload_post_data_response,
     filter_upload_request,
+    filter_upload_url_request,
     filter_volatile_dates,
 )
 from gencove.tests.utils import get_vcr_response
 from gencove.utils import get_regular_progress_bar, get_s3_client_refreshable
 
 import pytest  # pylint: disable=wrong-import-order
 
@@ -56,17 +58,19 @@
         ],
         "filter_query_parameters": [("search", "gncv://cli-mock/test.fastq.gz")],
         "match_on": ["method", "scheme", "port", "path", "query"],
         "path_transformer": VCR.ensure_suffix(".yaml"),
         "before_record_request": [
             replace_gencove_url_vcr,
             filter_upload_request,
+            filter_upload_url_request,
             filter_project_samples_request,
         ],
         "before_record_response": [
+            filter_import_fastqs_from_url_response,
             filter_jwt,
             filter_upload_credentials_response,
             filter_upload_post_data_response,
             filter_volatile_dates,
             filter_aws_headers,
             filter_sample_sheet_response,
             filter_project_samples_response,
@@ -963,7 +967,186 @@
 
         assert res.exit_code == 0
         mocked_login.assert_called_once()
         mocked_get_credentials.assert_called_once()
         # Call count = upload details + refresh jwt + retry upload details
         assert mocked_request.call_count == 3
         assert force_refresh_jwt is False
+
+
+@pytest.mark.vcr
+@assert_authorization
+def test_upload_url(credentials, vcr, recording, mocker):
+    """Basic check of uploading URL"""
+    runner = CliRunner()
+    with runner.isolated_filesystem():
+        os.mkdir("cli_test_data")
+        map_file_path = "cli_test_data/test_url_map.fastq-map.csv"
+        with open(map_file_path, "w", encoding="utf-8") as map_file:
+            writer = csv.writer(map_file)
+            writer.writerows(
+                [
+                    ["client_id", "r_notation", "path"],
+                    [
+                        "some-id",
+                        "r1",
+                        "https://s3.amazonaws.com/example/client-id_R1.fastq.gz",
+                    ],
+                ]
+            )
+        mocked_get_credentials = mocker.patch(
+            "gencove.command.upload.main.get_s3_client_refreshable",
+            side_effect=get_s3_client_refreshable,
+        )
+
+        if not recording:
+            response = get_vcr_response("/api/v2/uploads-url/", vcr)
+            mocked_import_fastqs_from_url = mocker.patch.object(
+                APIClient,
+                "import_fastqs_from_url",
+                return_value=UploadURLImport(**response),
+            )
+
+        res = runner.invoke(
+            upload,
+            [map_file_path, *credentials],
+        )
+        assert not res.exception
+        assert res.exit_code == 0
+        if not recording:
+            mocked_import_fastqs_from_url.assert_called_once()
+        mocked_get_credentials.assert_called_once()
+        assert "All files were successfully processed" in res.output
+
+
+@pytest.mark.vcr
+@assert_authorization
+def test_upload_url_with_local(credentials, vcr, recording, mocker):
+    """Basic check of uploading URL"""
+    # pylint: disable=too-many-locals
+
+    runner = CliRunner()
+    with runner.isolated_filesystem():
+        os.mkdir("cli_test_data")
+        map_file_path = "cli_test_data/test_url_map.fastq-map.csv"
+
+        fastq_file_path = "cli_test_data/test.fastq.gz"
+
+        with open(fastq_file_path, "w", encoding="utf-8") as fastq_file:
+            fastq_file.write("AAABBB")
+
+        with open(map_file_path, "w", encoding="utf-8") as map_file:
+            writer = csv.writer(map_file)
+            writer.writerows(
+                [
+                    ["client_id", "r_notation", "path"],
+                    [
+                        "foo",
+                        "r1",
+                        "https://s3.amazonaws.com/example/client-id_R1.fastq.gz",
+                    ],
+                    [
+                        "bar",
+                        "r1",
+                        fastq_file_path,
+                    ],
+                ]
+            )
+
+        mocked_get_credentials = mocker.patch(
+            "gencove.command.upload.main.get_s3_client_refreshable",
+            side_effect=get_s3_client_refreshable,
+        )
+
+        if not recording:
+            url_response = get_vcr_response("/api/v2/uploads-url/", vcr)
+            mocked_import_fastqs_from_url = mocker.patch.object(
+                APIClient,
+                "import_fastqs_from_url",
+                return_value=UploadURLImport(**url_response),
+            )
+
+            upload_response = get_vcr_response("/api/v2/uploads-post-data/", vcr)
+            mocked_get_upload_details = mocker.patch.object(
+                APIClient,
+                "get_upload_details",
+                return_value=UploadsPostData(**upload_response),
+            )
+
+        res = runner.invoke(
+            upload,
+            [map_file_path, *credentials],
+        )
+        assert not res.exception
+        assert res.exit_code == 0
+        if not recording:
+            mocked_import_fastqs_from_url.assert_called_once()
+            mocked_get_upload_details.assert_called_once()
+        mocked_get_credentials.assert_called_once()
+        assert "All files were successfully processed" in res.output
+
+
+@pytest.mark.vcr
+@assert_authorization
+def test_upload_url_and_run_immediately(
+    credentials, vcr, recording, mocker, project_id
+):
+    """Test uploading then running in project"""
+    # pylint: disable=too-many-locals
+
+    runner = CliRunner()
+    with runner.isolated_filesystem():
+        os.mkdir("cli_test_data")
+        map_file_path = "cli_test_data/test_url_map.fastq-map.csv"
+
+        with open(map_file_path, "w", encoding="utf-8") as map_file:
+            writer = csv.writer(map_file)
+            writer.writerows(
+                [
+                    ["client_id", "r_notation", "path"],
+                    [
+                        "some-id",
+                        "r1",
+                        "https://s3.amazonaws.com/example/client-id_R1.fastq.gz",
+                    ],
+                ]
+            )
+
+        if not recording:
+            response = get_vcr_response("/api/v2/uploads-url/", vcr)
+            mocked_import_fastqs_from_url = mocker.patch.object(
+                APIClient,
+                "import_fastqs_from_url",
+                return_value=UploadURLImport(**response),
+            )
+            sample_sheet_response = get_vcr_response("/api/v2/sample-sheet/", vcr)
+            mocked_get_sample_sheet = mocker.patch.object(
+                APIClient,
+                "get_sample_sheet",
+                return_value=SampleSheet(**sample_sheet_response),
+            )
+            project_sample_response = get_vcr_response(
+                "/api/v2/project-samples/", vcr, operator.contains
+            )
+            mocked_assign_sample = mocker.patch.object(
+                APIClient,
+                "add_samples_to_project",
+                return_value=UploadSamples(**project_sample_response),
+            )
+        mocked_regular_progress_bar = mocker.patch(
+            "gencove.command.upload.main.get_regular_progress_bar",
+            side_effect=get_regular_progress_bar,
+        )
+        res = runner.invoke(
+            upload,
+            [map_file_path, "--run-project-id", project_id, *credentials],
+        )
+
+        assert not res.exception
+        assert res.exit_code == 0
+        assert "All files were successfully processed" in res.output
+        if not recording:
+            mocked_import_fastqs_from_url.assert_called_once()
+            mocked_get_sample_sheet.assert_called()
+            mocked_assign_sample.assert_called_once()
+
+        mocked_regular_progress_bar.assert_called_once()
```

### Comparing `gencove-2.4.7/gencove/tests/upload/vcr/filters.py` & `gencove-2.5.0/gencove/tests/upload/vcr/filters.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,22 @@
     if "uploads-post-data" in request.path:
         request.body = '{"destination_path": "gncv://cli-mock/test.fastq.gz"}'
     if "s3.amazonaws.com" in request.uri:
         request.uri = f"https://s3.amazonaws.com/mock_bucket/organization/{MOCK_UUID}/user/{MOCK_UUID}/uploads/{MOCK_UUID}.fastq-r1"  # noqa: E501 line too long pylint: disable=line-too-long
     return request
 
 
+def filter_upload_url_request(request):
+    """Removes destination path and aws url from request."""
+    request = copy.deepcopy(request)
+    if "uploads-url" in request.path:
+        request.body = '{"destination_path": "gncv://cli-mock/test.fastq.gz", "source_url": "https://s3.amazonaws.com/example/client-id_R1.fastq.gz"}'  # noqa: E501 pylint: disable=line-too-long
+    return request
+
+
 def filter_project_samples_request(request):
     """Filter sample sheet sensitive data from request."""
     request = copy.deepcopy(request)
     if "project-samples" in request.path:
         try:
             body = json.loads(request.body)
             for upload in body["uploads"]:
@@ -57,14 +65,35 @@
         }
     if "last_status" in json_response:
         json_response["last_status"]["id"] = MOCK_UUID
     return response, json_response
 
 
 @parse_response_to_json
+def filter_import_fastqs_from_url_response(response, json_response):
+    """Removes sensitive data from POST to uploads-post-data."""
+    if "id" in json_response:
+        json_response["id"] = MOCK_UUID
+    if "destination_path" in json_response:
+        json_response["destination_path"] = "gncv://cli-mock/test.fastq.gz"
+    if "s3" in json_response:
+        json_response["s3"] = {
+            "bucket": "mock_bucket",
+            "object_name": f"organization/{MOCK_UUID}/user/{MOCK_UUID}/uploads/{MOCK_UUID}.fastq-r1",  # noqa: E501 pylint: disable=line-too-long
+        }
+    if "last_status" in json_response:
+        json_response["last_status"]["id"] = MOCK_UUID
+    if "source_url" in json_response:
+        json_response[
+            "source_url"
+        ] = "https://s3.amazonaws.com/example/client-id_R1.fastq.gz"
+    return response, json_response
+
+
+@parse_response_to_json
 def filter_volatile_dates(response, json_response):
     """Patches volatile dates, and push them into the future, otherwise
     the app will think the token/whatever is expired.
     """
     if "expiry_time" in json_response:
         json_response["expiry_time"] = "2050-09-03T00:00:00+00:00"
     return response, json_response
```

### Comparing `gencove-2.4.7/gencove/tests/uploads/test_uploads_list.py` & `gencove-2.5.0/gencove/tests/uploads/test_uploads_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/utils.py` & `gencove-2.5.0/gencove/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/tests/webhook/test_webhook_verify.py` & `gencove-2.5.0/gencove/tests/webhook/test_webhook_verify.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove/utils.py` & `gencove-2.5.0/gencove/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/gencove.egg-info/PKG-INFO` & `gencove-2.5.0/gencove.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gencove
-Version: 2.4.7
+Version: 2.5.0
 Summary: Gencove API and CLI tool
 Home-page: http://docs.gencove.com
 Author: Tomaz Berisa
 License: Apache 2.0
 Description: # The Gencove CLI
         
         [![PyPI Latest Release](https://img.shields.io/pypi/v/gencove.svg)](https://pypi.org/project/gencove/)
```

### Comparing `gencove-2.4.7/gencove.egg-info/SOURCES.txt` & `gencove-2.5.0/gencove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gencove-2.4.7/setup.py` & `gencove-2.5.0/setup.py`

 * *Files identical despite different names*

