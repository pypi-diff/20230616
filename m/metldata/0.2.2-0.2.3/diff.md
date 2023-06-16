# Comparing `tmp/metldata-0.2.2.tar.gz` & `tmp/metldata-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metldata-0.2.2.tar", last modified: Wed Jun 14 12:15:48 2023, max compression
+gzip compressed data, was "metldata-0.2.3.tar", last modified: Fri Jun 16 12:30:14 2023, max compression
```

## Comparing `metldata-0.2.2.tar` & `metldata-0.2.3.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.476115 metldata-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-14 12:15:36.000000 metldata-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-06-14 12:15:48.476115 metldata-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-06-14 12:15:36.000000 metldata-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.444115 metldata-0.2.2/metldata/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.448115 metldata-0.2.2/metldata/accession_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/accession_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/accession_registry/accession_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/accession_registry/accession_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/accession_registry/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.448115 metldata-0.2.2/metldata/artifacts_rest/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/artifacts_rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/artifacts_rest/api_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/artifacts_rest/artifact_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/artifacts_rest/artifact_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/artifacts_rest/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/artifacts_rest/load_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/artifacts_rest/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/artifacts_rest/query_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.448115 metldata-0.2.2/metldata/builtin_transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.448115 metldata-0.2.2/metldata/builtin_transformations/add_accessions/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/add_accessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/add_accessions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/add_accessions/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/add_accessions/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/add_accessions/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.452115 metldata-0.2.2/metldata/builtin_transformations/custom_embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/custom_embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/custom_embeddings/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/custom_embeddings/embedding_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/custom_embeddings/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/custom_embeddings/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/custom_embeddings/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.452115 metldata-0.2.2/metldata/builtin_transformations/delete_slots/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/delete_slots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/delete_slots/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/delete_slots/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/delete_slots/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/delete_slots/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/delete_slots/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.456115 metldata-0.2.2/metldata/builtin_transformations/infer_references/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/infer_references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/infer_references/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/infer_references/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/infer_references/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/infer_references/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.456115 metldata-0.2.2/metldata/builtin_transformations/infer_references/path/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/infer_references/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/infer_references/path/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/infer_references/path/path_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/infer_references/path/path_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/infer_references/path/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/infer_references/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.460115 metldata-0.2.2/metldata/builtin_transformations/merge_slots/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/merge_slots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/merge_slots/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/merge_slots/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/merge_slots/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/merge_slots/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/merge_slots/model_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_transformations/merge_slots/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.460115 metldata-0.2.2/metldata/builtin_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/builtin_workflows/ghga_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/custom_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.460115 metldata-0.2.2/metldata/event_handling/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/event_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/event_handling/artifact_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/event_handling/event_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/event_handling/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/event_handling/submission_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.464115 metldata-0.2.2/metldata/load/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/load/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/load/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/load/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/load/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/load/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/load/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/load/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/load/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.464115 metldata-0.2.2/metldata/model_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/model_utils/anchors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/model_utils/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/model_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/model_utils/essentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/model_utils/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/model_utils/manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/model_utils/metadata_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.464115 metldata-0.2.2/metldata/submission_registry/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/submission_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/submission_registry/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/submission_registry/event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/submission_registry/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/submission_registry/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/submission_registry/submission_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/submission_registry/submission_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.468115 metldata-0.2.2/metldata/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/transform/artifact_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/transform/handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/transform/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-14 12:15:36.000000 metldata-0.2.2/metldata/transform/source_event_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.444115 metldata-0.2.2/metldata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-06-14 12:15:48.000000 metldata-0.2.2/metldata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-14 12:15:48.000000 metldata-0.2.2/metldata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:15:48.000000 metldata-0.2.2/metldata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-14 12:15:48.000000 metldata-0.2.2/metldata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:15:48.000000 metldata-0.2.2/metldata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-14 12:15:48.000000 metldata-0.2.2/metldata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 12:15:48.000000 metldata-0.2.2/metldata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-14 12:15:48.480115 metldata-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-14 12:15:36.000000 metldata-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.468115 metldata-0.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.468115 metldata-0.2.2/tests/accession_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/accession_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/accession_registry/test_accession_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/accession_registry/test_accession_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.468115 metldata-0.2.2/tests/artifact_rest/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/artifact_rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/artifact_rest/test_api_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/artifact_rest/test_artifact_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/artifact_rest/test_load_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/artifact_rest/test_query_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.468115 metldata-0.2.2/tests/builtin_tranformations/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/builtin_tranformations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.468115 metldata-0.2.2/tests/builtin_tranformations/infer_references/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/builtin_tranformations/infer_references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.472115 metldata-0.2.2/tests/builtin_tranformations/infer_references/path/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/builtin_tranformations/infer_references/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/builtin_tranformations/infer_references/path/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/builtin_tranformations/infer_references/path/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/builtin_tranformations/infer_references/path/test_path_str.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.472115 metldata-0.2.2/tests/builtin_tranformations/merge_slots/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/builtin_tranformations/merge_slots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/builtin_tranformations/merge_slots/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/builtin_tranformations/merge_slots/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/builtin_tranformations/test_happy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.472115 metldata-0.2.2/tests/builtin_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/builtin_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/builtin_workflows/test_happy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.472115 metldata-0.2.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/fixtures/artifact_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/fixtures/event_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/fixtures/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/fixtures/metadata_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/fixtures/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/fixtures/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.476115 metldata-0.2.2/tests/load/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/load/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/load/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.476115 metldata-0.2.2/tests/model_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/model_utils/test_anchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/model_utils/test_assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/model_utils/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/model_utils/test_essentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/model_utils/test_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/model_utils/test_manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/model_utils/test_metadata_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.476115 metldata-0.2.2/tests/submission_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/submission_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/submission_registry/test_event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/submission_registry/test_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/submission_registry/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/submission_registry/test_submission_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/submission_registry/test_submission_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/test_event_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/test_metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:15:48.476115 metldata-0.2.2/tests/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/transform/test_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-14 12:15:36.000000 metldata-0.2.2/tests/transform/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.143061 metldata-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-16 12:30:04.000000 metldata-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-06-16 12:30:14.143061 metldata-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-06-16 12:30:04.000000 metldata-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.123061 metldata-0.2.3/metldata/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.123061 metldata-0.2.3/metldata/accession_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/accession_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/accession_registry/accession_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/accession_registry/accession_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/accession_registry/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.123061 metldata-0.2.3/metldata/artifacts_rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/artifacts_rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/artifacts_rest/api_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/artifacts_rest/artifact_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/artifacts_rest/artifact_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/artifacts_rest/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/artifacts_rest/load_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/artifacts_rest/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/artifacts_rest/query_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.127061 metldata-0.2.3/metldata/builtin_transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.127061 metldata-0.2.3/metldata/builtin_transformations/add_accessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/add_accessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/add_accessions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/add_accessions/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/add_accessions/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/add_accessions/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.127061 metldata-0.2.3/metldata/builtin_transformations/custom_embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/custom_embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/custom_embeddings/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/custom_embeddings/embedding_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/custom_embeddings/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/custom_embeddings/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/custom_embeddings/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.127061 metldata-0.2.3/metldata/builtin_transformations/delete_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/delete_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/delete_slots/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/delete_slots/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/delete_slots/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/delete_slots/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/delete_slots/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.127061 metldata-0.2.3/metldata/builtin_transformations/infer_references/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/infer_references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/infer_references/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/infer_references/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/infer_references/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/infer_references/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.127061 metldata-0.2.3/metldata/builtin_transformations/infer_references/path/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/infer_references/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/infer_references/path/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/infer_references/path/path_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/infer_references/path/path_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/infer_references/path/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/infer_references/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.131061 metldata-0.2.3/metldata/builtin_transformations/merge_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/merge_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/merge_slots/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/merge_slots/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/merge_slots/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/merge_slots/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/merge_slots/model_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_transformations/merge_slots/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.131061 metldata-0.2.3/metldata/builtin_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/builtin_workflows/ghga_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/custom_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.131061 metldata-0.2.3/metldata/event_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/event_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/event_handling/artifact_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/event_handling/event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/event_handling/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/event_handling/submission_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.131061 metldata-0.2.3/metldata/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/load/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/load/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/load/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/load/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/load/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/load/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/load/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/load/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.131061 metldata-0.2.3/metldata/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/model_utils/anchors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/model_utils/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/model_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/model_utils/essentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/model_utils/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/model_utils/manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/model_utils/metadata_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.135061 metldata-0.2.3/metldata/submission_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/submission_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/submission_registry/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/submission_registry/event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/submission_registry/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/submission_registry/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/submission_registry/submission_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/submission_registry/submission_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.135061 metldata-0.2.3/metldata/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/transform/artifact_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/transform/handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/transform/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-16 12:30:04.000000 metldata-0.2.3/metldata/transform/source_event_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.123061 metldata-0.2.3/metldata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-06-16 12:30:14.000000 metldata-0.2.3/metldata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-16 12:30:14.000000 metldata-0.2.3/metldata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:30:14.000000 metldata-0.2.3/metldata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 12:30:14.000000 metldata-0.2.3/metldata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:30:13.000000 metldata-0.2.3/metldata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-16 12:30:14.000000 metldata-0.2.3/metldata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 12:30:14.000000 metldata-0.2.3/metldata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-16 12:30:14.143061 metldata-0.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-16 12:30:04.000000 metldata-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.135061 metldata-0.2.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.135061 metldata-0.2.3/tests/accession_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/accession_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/accession_registry/test_accession_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/accession_registry/test_accession_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.135061 metldata-0.2.3/tests/artifact_rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/artifact_rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/artifact_rest/test_api_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/artifact_rest/test_artifact_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/artifact_rest/test_load_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/artifact_rest/test_query_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.135061 metldata-0.2.3/tests/builtin_tranformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/builtin_tranformations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.135061 metldata-0.2.3/tests/builtin_tranformations/infer_references/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/builtin_tranformations/infer_references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.139061 metldata-0.2.3/tests/builtin_tranformations/infer_references/path/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/builtin_tranformations/infer_references/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/builtin_tranformations/infer_references/path/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/builtin_tranformations/infer_references/path/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/builtin_tranformations/infer_references/path/test_path_str.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.139061 metldata-0.2.3/tests/builtin_tranformations/merge_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/builtin_tranformations/merge_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/builtin_tranformations/merge_slots/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/builtin_tranformations/merge_slots/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/builtin_tranformations/test_happy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.139061 metldata-0.2.3/tests/builtin_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/builtin_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/builtin_workflows/test_happy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.139061 metldata-0.2.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/fixtures/artifact_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/fixtures/event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/fixtures/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/fixtures/metadata_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/fixtures/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/fixtures/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.139061 metldata-0.2.3/tests/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/load/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/load/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.139061 metldata-0.2.3/tests/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/model_utils/test_anchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/model_utils/test_assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/model_utils/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/model_utils/test_essentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/model_utils/test_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/model_utils/test_manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/model_utils/test_metadata_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.143061 metldata-0.2.3/tests/submission_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/submission_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/submission_registry/test_event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/submission_registry/test_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/submission_registry/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/submission_registry/test_submission_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/submission_registry/test_submission_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/test_event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/test_metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:30:14.143061 metldata-0.2.3/tests/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/transform/test_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-16 12:30:04.000000 metldata-0.2.3/tests/transform/test_main.py
```

### Comparing `metldata-0.2.2/LICENSE` & `metldata-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/PKG-INFO` & `metldata-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metldata
-Version: 0.2.2
+Version: 0.2.3
 Summary: metldata - A framework for handling metadata based on ETL, CQRS, and event sourcing.
 Home-page: https://github.com/ghga-de/metldata
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -76,29 +76,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/metldata):
 ```bash
-docker pull ghga/metldata:0.2.2
+docker pull ghga/metldata:0.2.3
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/metldata:0.2.2 .
+docker build -t ghga/metldata:0.2.3 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/metldata:0.2.2 --help
+docker run -p 8080:8080 ghga/metldata:0.2.3 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `metldata-0.2.2/README.md` & `metldata-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,29 +58,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/metldata):
 ```bash
-docker pull ghga/metldata:0.2.2
+docker pull ghga/metldata:0.2.3
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/metldata:0.2.2 .
+docker build -t ghga/metldata:0.2.3 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/metldata:0.2.2 --help
+docker run -p 8080:8080 ghga/metldata:0.2.3 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `metldata-0.2.2/metldata/__init__.py` & `metldata-0.2.3/metldata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Short description of package"""  # Please adapt to package
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
```

### Comparing `metldata-0.2.2/metldata/__main__.py` & `metldata-0.2.3/metldata/__main__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/accession_registry/__init__.py` & `metldata-0.2.3/metldata/accession_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/accession_registry/accession_registry.py` & `metldata-0.2.3/metldata/accession_registry/accession_registry.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/accession_registry/accession_store.py` & `metldata-0.2.3/metldata/accession_registry/accession_store.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/accession_registry/config.py` & `metldata-0.2.3/metldata/accession_registry/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/artifacts_rest/__init__.py` & `metldata-0.2.3/metldata/artifacts_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/artifacts_rest/api_factory.py` & `metldata-0.2.3/metldata/artifacts_rest/api_factory.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/artifacts_rest/artifact_dao.py` & `metldata-0.2.3/metldata/artifacts_rest/artifact_dao.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/artifacts_rest/artifact_info.py` & `metldata-0.2.3/metldata/artifacts_rest/artifact_info.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/artifacts_rest/config.py` & `metldata-0.2.3/metldata/artifacts_rest/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/artifacts_rest/load_resources.py` & `metldata-0.2.3/metldata/artifacts_rest/load_resources.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/artifacts_rest/models.py` & `metldata-0.2.3/metldata/artifacts_rest/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/artifacts_rest/query_resources.py` & `metldata-0.2.3/metldata/artifacts_rest/query_resources.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/__init__.py` & `metldata-0.2.3/metldata/builtin_transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/add_accessions/__init__.py` & `metldata-0.2.3/metldata/builtin_transformations/add_accessions/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/add_accessions/config.py` & `metldata-0.2.3/metldata/builtin_transformations/add_accessions/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/add_accessions/main.py` & `metldata-0.2.3/metldata/builtin_transformations/add_accessions/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/add_accessions/metadata_transform.py` & `metldata-0.2.3/metldata/builtin_transformations/add_accessions/metadata_transform.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from collections import defaultdict
 
 from pydantic import Json
 from typing_extensions import TypeAlias
 
 from metldata.metadata_utils import lookup_self_id
-from metldata.model_utils.anchors import AnchorPoint
+from metldata.model_utils.anchors import AnchorPoint, lookup_anchor_point
 from metldata.model_utils.essentials import MetadataModel
 from metldata.submission_registry.models import AccessionMap
 from metldata.transform.base import MetadataTransformationError
 
 # A type for specifying references between anchored classes in a given model:
 # The first key is the name of the class that is anchored, the second key is the
 # the name of the slot of that class that contains the references.
@@ -48,20 +48,26 @@
             if slot.range in anchor_points_by_target:
                 references[source_class_name][slot.name] = slot.range
 
     return references
 
 
 def lookup_accession(
-    *, target_class: str, old_identifier: str, accession_map: AccessionMap
+    *,
+    target_class: str,
+    old_identifier: str,
+    accession_map: AccessionMap,
+    anchor_points_by_target: dict[str, AnchorPoint],
 ) -> str:
     """Lookup the accession for the a resource with the given identifier of the given
     class."""
-
-    accession = accession_map.get(target_class, {}).get(old_identifier)
+    anchor_point = lookup_anchor_point(
+        class_name=target_class, anchor_points_by_target=anchor_points_by_target
+    )
+    accession = accession_map.get(anchor_point.root_slot, {}).get(old_identifier)
     if not accession:
         raise MetadataTransformationError(
             f"Could not find accession for '{old_identifier}' of class"
             + f" '{target_class}."
         )
     return accession
 
@@ -70,14 +76,15 @@
     *,
     resource: Json,
     class_name: str,
     old_identifier_slot: str,
     accession_slot_name: str,
     accession_map: AccessionMap,
     references: dict[str, str],
+    anchor_points_by_target: dict[str, AnchorPoint],
 ) -> Json:
     """Add an accession to a resource.
 
     Args:
         resource:
             The resource to which accessions should be added.
         old_identifier_slot:
@@ -99,35 +106,38 @@
     old_identifier = lookup_self_id(
         resource=resource, identifier_slot=old_identifier_slot
     )
     new_identifier = lookup_accession(
         target_class=class_name,
         old_identifier=old_identifier,
         accession_map=accession_map,
+        anchor_points_by_target=anchor_points_by_target,
     )
 
     new_resource: Json = {accession_slot_name: new_identifier}
 
     for slot_name, slot_value in resource.items():
         if slot_name in references:
             referenced_class = references[slot_name]
             if isinstance(slot_value, list):
                 new_resource[slot_name] = [
                     lookup_accession(
                         target_class=referenced_class,
                         old_identifier=reference_old_identifier,
                         accession_map=accession_map,
+                        anchor_points_by_target=anchor_points_by_target,
                     )
                     for reference_old_identifier in slot_value
                 ]
             else:
                 new_resource[slot_name] = lookup_accession(
                     target_class=referenced_class,
                     old_identifier=slot_value,
                     accession_map=accession_map,
+                    anchor_points_by_target=anchor_points_by_target,
                 )
         else:
             new_resource[slot_name] = slot_value
 
     return new_resource
 
 
@@ -146,28 +156,29 @@
             if the transformation of the metadata fails.
     """
 
     modified_metadata = {}
 
     for target_class_name, anchor_point in anchor_points_by_target.items():
         target_resources = []
-        target_accession_map = accession_map.get(target_class_name)
+        target_accession_map = accession_map.get(anchor_point.root_slot)
         if target_accession_map is None:
             raise MetadataTransformationError(
                 "Could not find accession mapping for target class"
                 + f" {target_class_name}."
             )
 
         for old_resource in metadata[anchor_point.root_slot]:
             new_resource = add_accession_to_resource(
                 resource=old_resource,
                 class_name=target_class_name,
                 old_identifier_slot=anchor_point.identifier_slot,
                 accession_slot_name=accession_slot_name,
                 accession_map=accession_map,
                 references=references[target_class_name],
+                anchor_points_by_target=anchor_points_by_target,
             )
             target_resources.append(new_resource)
 
         modified_metadata[anchor_point.root_slot] = target_resources
 
     return modified_metadata
```

### Comparing `metldata-0.2.2/metldata/builtin_transformations/add_accessions/model_transform.py` & `metldata-0.2.3/metldata/builtin_transformations/add_accessions/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/custom_embeddings/__init__.py` & `metldata-0.2.3/metldata/builtin_transformations/custom_embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/custom_embeddings/config.py` & `metldata-0.2.3/metldata/builtin_transformations/custom_embeddings/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/custom_embeddings/embedding_profile.py` & `metldata-0.2.3/metldata/builtin_transformations/custom_embeddings/embedding_profile.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/custom_embeddings/main.py` & `metldata-0.2.3/metldata/builtin_transformations/custom_embeddings/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/custom_embeddings/metadata_transform.py` & `metldata-0.2.3/metldata/builtin_transformations/custom_embeddings/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/custom_embeddings/model_transform.py` & `metldata-0.2.3/metldata/builtin_transformations/custom_embeddings/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/delete_slots/__init__.py` & `metldata-0.2.3/metldata/builtin_transformations/delete_slots/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/delete_slots/assumptions.py` & `metldata-0.2.3/metldata/builtin_transformations/delete_slots/assumptions.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/delete_slots/config.py` & `metldata-0.2.3/metldata/builtin_transformations/delete_slots/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/delete_slots/main.py` & `metldata-0.2.3/metldata/builtin_transformations/delete_slots/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/delete_slots/metadata_transform.py` & `metldata-0.2.3/metldata/builtin_transformations/delete_slots/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/delete_slots/model_transform.py` & `metldata-0.2.3/metldata/builtin_transformations/delete_slots/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/infer_references/__init__.py` & `metldata-0.2.3/metldata/builtin_transformations/infer_references/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/infer_references/config.py` & `metldata-0.2.3/metldata/builtin_transformations/infer_references/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/infer_references/main.py` & `metldata-0.2.3/metldata/builtin_transformations/infer_references/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/infer_references/metadata_transform.py` & `metldata-0.2.3/metldata/builtin_transformations/infer_references/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/infer_references/model_transform.py` & `metldata-0.2.3/metldata/builtin_transformations/infer_references/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/infer_references/path/__init__.py` & `metldata-0.2.3/metldata/builtin_transformations/infer_references/path/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/infer_references/path/path.py` & `metldata-0.2.3/metldata/builtin_transformations/infer_references/path/path.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/infer_references/path/path_elements.py` & `metldata-0.2.3/metldata/builtin_transformations/infer_references/path/path_elements.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/infer_references/path/path_str.py` & `metldata-0.2.3/metldata/builtin_transformations/infer_references/path/path_str.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/infer_references/path/resolve.py` & `metldata-0.2.3/metldata/builtin_transformations/infer_references/path/resolve.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/infer_references/reference.py` & `metldata-0.2.3/metldata/builtin_transformations/infer_references/reference.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/merge_slots/__init__.py` & `metldata-0.2.3/metldata/builtin_transformations/merge_slots/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/merge_slots/assumptions.py` & `metldata-0.2.3/metldata/builtin_transformations/merge_slots/assumptions.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/merge_slots/config.py` & `metldata-0.2.3/metldata/builtin_transformations/merge_slots/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/merge_slots/main.py` & `metldata-0.2.3/metldata/builtin_transformations/merge_slots/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/merge_slots/metadata_transform.py` & `metldata-0.2.3/metldata/builtin_transformations/merge_slots/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/merge_slots/model_transform.py` & `metldata-0.2.3/metldata/builtin_transformations/merge_slots/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_transformations/merge_slots/models.py` & `metldata-0.2.3/metldata/builtin_transformations/merge_slots/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_workflows/__init__.py` & `metldata-0.2.3/metldata/builtin_workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/builtin_workflows/ghga_archive.py` & `metldata-0.2.3/metldata/builtin_workflows/ghga_archive.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/cli.py` & `metldata-0.2.3/metldata/cli.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/config.py` & `metldata-0.2.3/metldata/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/custom_types.py` & `metldata-0.2.3/metldata/custom_types.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/event_handling/__init__.py` & `metldata-0.2.3/metldata/event_handling/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/event_handling/artifact_events.py` & `metldata-0.2.3/metldata/event_handling/artifact_events.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/event_handling/event_handling.py` & `metldata-0.2.3/metldata/event_handling/event_handling.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/event_handling/models.py` & `metldata-0.2.3/metldata/event_handling/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/event_handling/submission_events.py` & `metldata-0.2.3/metldata/event_handling/submission_events.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/load/__init__.py` & `metldata-0.2.3/metldata/load/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/load/api.py` & `metldata-0.2.3/metldata/load/api.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/load/auth.py` & `metldata-0.2.3/metldata/load/auth.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/load/client.py` & `metldata-0.2.3/metldata/load/client.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/load/collect.py` & `metldata-0.2.3/metldata/load/collect.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/load/config.py` & `metldata-0.2.3/metldata/load/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/load/load.py` & `metldata-0.2.3/metldata/load/load.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/load/main.py` & `metldata-0.2.3/metldata/load/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/load/models.py` & `metldata-0.2.3/metldata/load/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/metadata_utils.py` & `metldata-0.2.3/metldata/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/model_utils/__init__.py` & `metldata-0.2.3/metldata/model_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/model_utils/anchors.py` & `metldata-0.2.3/metldata/model_utils/anchors.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/model_utils/assumptions.py` & `metldata-0.2.3/metldata/model_utils/assumptions.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/model_utils/config.py` & `metldata-0.2.3/metldata/model_utils/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/model_utils/essentials.py` & `metldata-0.2.3/metldata/model_utils/essentials.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/model_utils/identifiers.py` & `metldata-0.2.3/metldata/model_utils/identifiers.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/model_utils/manipulate.py` & `metldata-0.2.3/metldata/model_utils/manipulate.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/model_utils/metadata_validator.py` & `metldata-0.2.3/metldata/model_utils/metadata_validator.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/submission_registry/__init__.py` & `metldata-0.2.3/metldata/submission_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/submission_registry/config.py` & `metldata-0.2.3/metldata/submission_registry/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/submission_registry/event_publisher.py` & `metldata-0.2.3/metldata/submission_registry/event_publisher.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 """Logic for the publication of source events."""
 
 import asyncio
 import json
 
 from hexkit.protocols.eventpub import EventPublisherProtocol
 
+from metldata.event_handling.models import SubmissionAnnotation, SubmissionEventPayload
 from metldata.event_handling.submission_events import SourceEventConfig
 from metldata.submission_registry import models
 
 
 class SourceEventPublisherConfig(SourceEventConfig):
     """Config parameters and their defaults."""
 
@@ -42,16 +43,21 @@
 
     def publish_submission(self, submission: models.Submission):
         """Publish the current submission as source event"""
 
         if submission.content is None:
             raise ValueError("Submission content must be defined.")
 
-        payload = json.loads(submission.json())
+        payload = SubmissionEventPayload(
+            submission_id=submission.id,
+            content=submission.content,
+            annotation=SubmissionAnnotation(accession_map=submission.accession_map),
+        )
+
         asyncio.run(
             self._provider.publish(
                 topic=self._config.source_event_topic,
                 type_=self._config.source_event_type,
                 key=submission.id,
-                payload=payload,
+                payload=json.loads(payload.json()),
             )
         )
```

### Comparing `metldata-0.2.2/metldata/submission_registry/identifiers.py` & `metldata-0.2.3/metldata/submission_registry/identifiers.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/submission_registry/models.py` & `metldata-0.2.3/metldata/submission_registry/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/submission_registry/submission_registry.py` & `metldata-0.2.3/metldata/submission_registry/submission_registry.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/submission_registry/submission_store.py` & `metldata-0.2.3/metldata/submission_registry/submission_store.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/transform/__init__.py` & `metldata-0.2.3/metldata/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/transform/artifact_publisher.py` & `metldata-0.2.3/metldata/transform/artifact_publisher.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/transform/base.py` & `metldata-0.2.3/metldata/transform/base.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/transform/config.py` & `metldata-0.2.3/metldata/transform/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/transform/handling.py` & `metldata-0.2.3/metldata/transform/handling.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/transform/main.py` & `metldata-0.2.3/metldata/transform/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata/transform/source_event_subscriber.py` & `metldata-0.2.3/metldata/transform/source_event_subscriber.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/metldata.egg-info/PKG-INFO` & `metldata-0.2.3/metldata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metldata
-Version: 0.2.2
+Version: 0.2.3
 Summary: metldata - A framework for handling metadata based on ETL, CQRS, and event sourcing.
 Home-page: https://github.com/ghga-de/metldata
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -76,29 +76,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/metldata):
 ```bash
-docker pull ghga/metldata:0.2.2
+docker pull ghga/metldata:0.2.3
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/metldata:0.2.2 .
+docker build -t ghga/metldata:0.2.3 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/metldata:0.2.2 --help
+docker run -p 8080:8080 ghga/metldata:0.2.3 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `metldata-0.2.2/metldata.egg-info/SOURCES.txt` & `metldata-0.2.3/metldata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/setup.cfg` & `metldata-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/setup.py` & `metldata-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/accession_registry/__init__.py` & `metldata-0.2.3/tests/accession_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/accession_registry/test_accession_registry.py` & `metldata-0.2.3/tests/accession_registry/test_accession_registry.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/accession_registry/test_accession_store.py` & `metldata-0.2.3/tests/accession_registry/test_accession_store.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/artifact_rest/__init__.py` & `metldata-0.2.3/tests/artifact_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/artifact_rest/test_api_factory.py` & `metldata-0.2.3/tests/artifact_rest/test_api_factory.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/artifact_rest/test_artifact_info.py` & `metldata-0.2.3/tests/artifact_rest/test_artifact_info.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/artifact_rest/test_load_artifacts.py` & `metldata-0.2.3/tests/artifact_rest/test_load_artifacts.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/artifact_rest/test_query_resources.py` & `metldata-0.2.3/tests/artifact_rest/test_query_resources.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/builtin_tranformations/__init__.py` & `metldata-0.2.3/tests/builtin_tranformations/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/builtin_tranformations/infer_references/__init__.py` & `metldata-0.2.3/tests/builtin_tranformations/infer_references/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/builtin_tranformations/infer_references/path/__init__.py` & `metldata-0.2.3/tests/builtin_tranformations/infer_references/path/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/builtin_tranformations/infer_references/path/test_config.py` & `metldata-0.2.3/tests/builtin_tranformations/infer_references/path/test_config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/builtin_tranformations/infer_references/path/test_path.py` & `metldata-0.2.3/tests/builtin_tranformations/infer_references/path/test_path.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/builtin_tranformations/infer_references/path/test_path_str.py` & `metldata-0.2.3/tests/builtin_tranformations/infer_references/path/test_path_str.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/builtin_tranformations/merge_slots/__init__.py` & `metldata-0.2.3/tests/builtin_tranformations/merge_slots/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/builtin_tranformations/merge_slots/test_config.py` & `metldata-0.2.3/tests/builtin_tranformations/merge_slots/test_config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/builtin_tranformations/merge_slots/test_models.py` & `metldata-0.2.3/tests/builtin_tranformations/merge_slots/test_models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/builtin_tranformations/test_happy.py` & `metldata-0.2.3/tests/builtin_tranformations/test_happy.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/builtin_workflows/__init__.py` & `metldata-0.2.3/tests/builtin_workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/builtin_workflows/test_happy.py` & `metldata-0.2.3/tests/builtin_workflows/test_happy.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/fixtures/__init__.py` & `metldata-0.2.3/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/fixtures/artifact_info.py` & `metldata-0.2.3/tests/fixtures/artifact_info.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/fixtures/config.py` & `metldata-0.2.3/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/fixtures/event_handling.py` & `metldata-0.2.3/tests/fixtures/event_handling.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/fixtures/metadata.py` & `metldata-0.2.3/tests/fixtures/metadata.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/fixtures/metadata_models.py` & `metldata-0.2.3/tests/fixtures/metadata_models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/fixtures/transformations.py` & `metldata-0.2.3/tests/fixtures/transformations.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/fixtures/utils.py` & `metldata-0.2.3/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/fixtures/workflows.py` & `metldata-0.2.3/tests/fixtures/workflows.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/load/__init__.py` & `metldata-0.2.3/tests/load/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/load/test_client.py` & `metldata-0.2.3/tests/load/test_client.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/load/test_main.py` & `metldata-0.2.3/tests/load/test_main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/model_utils/__init__.py` & `metldata-0.2.3/tests/model_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/model_utils/test_anchor.py` & `metldata-0.2.3/tests/model_utils/test_anchor.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/model_utils/test_assumptions.py` & `metldata-0.2.3/tests/model_utils/test_assumptions.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/model_utils/test_config.py` & `metldata-0.2.3/tests/model_utils/test_config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/model_utils/test_essentials.py` & `metldata-0.2.3/tests/model_utils/test_essentials.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/model_utils/test_identifiers.py` & `metldata-0.2.3/tests/model_utils/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/model_utils/test_manipulate.py` & `metldata-0.2.3/tests/model_utils/test_manipulate.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/model_utils/test_metadata_validator.py` & `metldata-0.2.3/tests/model_utils/test_metadata_validator.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/submission_registry/__init__.py` & `metldata-0.2.3/tests/submission_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/submission_registry/test_event_publisher.py` & `metldata-0.2.3/tests/submission_registry/test_event_publisher.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import json
 
 from ghga_service_commons.utils.utc_dates import now_as_utc
 
 from metldata.config import SubmissionConfig
 from metldata.event_handling.event_handling import FileSystemEventPublisher
+from metldata.event_handling.models import SubmissionAnnotation, SubmissionEventPayload
 from metldata.submission_registry import models
 from metldata.submission_registry.event_publisher import SourceEventPublisher
 from tests.fixtures.config import config_sub_fixture  # noqa: F401
 from tests.fixtures.event_handling import file_system_event_fixture  # noqa: F401
 from tests.fixtures.event_handling import Event, FileSystemEventFixture
 
 
@@ -43,15 +44,23 @@
     """
 
     expected_events = [
         Event(
             topic=source_event_topic,
             type_=source_event_type,
             key=expected_submission.id,
-            payload=json.loads(expected_submission.json()),
+            payload=json.loads(
+                SubmissionEventPayload(
+                    submission_id=expected_submission.id,
+                    content=expected_submission.content,
+                    annotation=SubmissionAnnotation(
+                        accession_map=expected_submission.accession_map
+                    ),
+                ).json()
+            ),
         )
         for expected_submission in expected_submissions
     ]
 
     file_system_event_fixture.expect_events(expected_events=expected_events)
```

### Comparing `metldata-0.2.2/tests/submission_registry/test_identifiers.py` & `metldata-0.2.3/tests/submission_registry/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/submission_registry/test_models.py` & `metldata-0.2.3/tests/submission_registry/test_models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/submission_registry/test_submission_registry.py` & `metldata-0.2.3/tests/submission_registry/test_submission_registry.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/submission_registry/test_submission_store.py` & `metldata-0.2.3/tests/submission_registry/test_submission_store.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/test_event_handling.py` & `metldata-0.2.3/tests/test_event_handling.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/test_metadata_utils.py` & `metldata-0.2.3/tests/test_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/transform/__init__.py` & `metldata-0.2.3/tests/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/transform/test_base.py` & `metldata-0.2.3/tests/transform/test_base.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/transform/test_handling.py` & `metldata-0.2.3/tests/transform/test_handling.py`

 * *Files identical despite different names*

### Comparing `metldata-0.2.2/tests/transform/test_main.py` & `metldata-0.2.3/tests/transform/test_main.py`

 * *Files identical despite different names*

