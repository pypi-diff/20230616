# Comparing `tmp/metamist-6.0.3.tar.gz` & `tmp/metamist-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamist-6.0.3.tar", last modified: Fri May 19 02:37:25 2023, max compression
+gzip compressed data, was "metamist-6.0.4.tar", last modified: Thu Jun 15 22:32:25 2023, max compression
```

## Comparing `metamist-6.0.3.tar` & `metamist-6.0.4.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.122965 metamist-6.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-19 02:31:41.000000 metamist-6.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 02:31:41.000000 metamist-6.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-05-19 02:37:25.118965 metamist-6.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-05-19 02:31:41.000000 metamist-6.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.058964 metamist-6.0.3/metamist/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.070964 metamist-6.0.3/metamist/api/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55799 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/api/analysis_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33060 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/api/assay_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/api/enums_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28817 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/api/family_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41903 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/participant_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28288 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53117 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/sample_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46958 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/seqr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/sequencing_group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18066 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/web_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.070964 metamist-6.0.3/metamist/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17054 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.074964 metamist-6.0.3/metamist/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-19 02:31:41.000000 metamist-6.0.3/metamist/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-19 02:34:36.000000 metamist-6.0.3/metamist/graphql/schema.graphql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.094965 metamist-6.0.3/metamist/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/analysis_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/analysis_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/analysis_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/assay.py
--rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/assay_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/body_get_assays_by_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/body_get_latest_complete_analysis_for_type_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/body_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/body_get_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/export_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/extra_participant_importer_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/family_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/family_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/family_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/meta_search_entity_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/nested_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/nested_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/nested_sequencing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/paging_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/participant_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/participant_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/project_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/sample_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/sample_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/search_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/search_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/search_response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/sequencing_group_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/web_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    82230 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.094965 metamist-6.0.3/metamist/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.098965 metamist-6.0.3/metamist/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 02:31:41.000000 metamist-6.0.3/metamist/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-19 02:31:41.000000 metamist-6.0.3/metamist/parser/cloudhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)    31027 2023-05-19 02:31:41.000000 metamist-6.0.3/metamist/parser/generic_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    50764 2023-05-19 02:31:41.000000 metamist-6.0.3/metamist/parser/generic_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-19 02:31:41.000000 metamist-6.0.3/metamist/parser/sample_file_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.062964 metamist-6.0.3/metamist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-05-19 02:37:24.000000 metamist-6.0.3/metamist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-19 02:37:25.000000 metamist-6.0.3/metamist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 02:37:24.000000 metamist-6.0.3/metamist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 02:37:24.000000 metamist-6.0.3/metamist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-19 02:37:24.000000 metamist-6.0.3/metamist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 02:37:24.000000 metamist-6.0.3/metamist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-19 02:31:41.000000 metamist-6.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 02:37:25.122965 metamist-6.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-19 02:31:41.000000 metamist-6.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.118965 metamist-6.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_assay.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_generic_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_import_individual_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_metamist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_parse_existing_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_parse_file_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_parse_generic_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_parse_ont_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_parse_ont_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_sequencing_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    19216 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-19 02:31:41.000000 metamist-6.0.3/test/testbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:32:25.797434 metamist-6.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 22:27:11.000000 metamist-6.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:27:11.000000 metamist-6.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-06-15 22:32:25.797434 metamist-6.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-06-15 22:27:11.000000 metamist-6.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:32:25.781433 metamist-6.0.4/metamist/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:32:25.781433 metamist-6.0.4/metamist/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55799 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/api/analysis_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33060 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/api/assay_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/api/enums_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28817 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/api/family_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41903 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/api/participant_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28288 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53117 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/api/sample_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46958 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/api/seqr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/api/sequencing_group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18066 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/api/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:32:25.781433 metamist-6.0.4/metamist/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17054 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:32:25.785433 metamist-6.0.4/metamist/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-15 22:27:11.000000 metamist-6.0.4/metamist/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-15 22:29:54.000000 metamist-6.0.4/metamist/graphql/schema.graphql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:32:25.789434 metamist-6.0.4/metamist/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-06-15 22:29:48.000000 metamist-6.0.4/metamist/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-06-15 22:29:48.000000 metamist-6.0.4/metamist/model/analysis_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-15 22:29:48.000000 metamist-6.0.4/metamist/model/analysis_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/analysis_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/assay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/assay_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/body_get_assays_by_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/body_get_latest_complete_analysis_for_type_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/body_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/body_get_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/export_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/extra_participant_importer_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/family_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/family_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/family_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/meta_search_entity_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/nested_participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/nested_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/nested_sequencing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/paging_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/participant_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/participant_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/project_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/sample_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/sample_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/search_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/search_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/search_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/sequencing_group_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/sequencing_group_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model/web_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82230 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:32:25.789434 metamist-6.0.4/metamist/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:32:25.789434 metamist-6.0.4/metamist/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 22:27:11.000000 metamist-6.0.4/metamist/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-06-15 22:27:11.000000 metamist-6.0.4/metamist/parser/cloudhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31027 2023-06-15 22:27:11.000000 metamist-6.0.4/metamist/parser/generic_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-06-15 22:27:11.000000 metamist-6.0.4/metamist/parser/generic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-15 22:27:11.000000 metamist-6.0.4/metamist/parser/sample_file_map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-06-15 22:29:49.000000 metamist-6.0.4/metamist/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:32:25.781433 metamist-6.0.4/metamist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-06-15 22:32:25.000000 metamist-6.0.4/metamist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-15 22:32:25.000000 metamist-6.0.4/metamist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:32:25.000000 metamist-6.0.4/metamist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:32:25.000000 metamist-6.0.4/metamist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 22:32:25.000000 metamist-6.0.4/metamist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 22:32:25.000000 metamist-6.0.4/metamist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 22:27:11.000000 metamist-6.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:32:25.797434 metamist-6.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-15 22:27:11.000000 metamist-6.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:32:25.797434 metamist-6.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_assay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_generic_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_import_individual_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_metamist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_parse_existing_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_parse_file_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_parse_generic_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_parse_ont_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_parse_ont_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_sequencing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-06-15 22:27:11.000000 metamist-6.0.4/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-15 22:27:11.000000 metamist-6.0.4/test/testbase.py
```

### Comparing `metamist-6.0.3/LICENSE` & `metamist-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/PKG-INFO` & `metamist-6.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.0.3
+Version: 6.0.4
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-6.0.3/README.md` & `metamist-6.0.4/README.md`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/metamist/__init__.py` & `metamist-6.0.4/metamist/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `metamist-6.0.3/metamist/api/analysis_api.py` & `metamist-6.0.4/metamist/api/analysis_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/api/assay_api.py` & `metamist-6.0.4/metamist/api/assay_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/api/enums_api.py` & `metamist-6.0.4/metamist/api/enums_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/api/family_api.py` & `metamist-6.0.4/metamist/api/family_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/api/import_api.py` & `metamist-6.0.4/metamist/api/import_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/api/participant_api.py` & `metamist-6.0.4/metamist/api/participant_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/api/project_api.py` & `metamist-6.0.4/metamist/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/api/sample_api.py` & `metamist-6.0.4/metamist/api/sample_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/api/seqr_api.py` & `metamist-6.0.4/metamist/api/seqr_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/api/sequencing_group_api.py` & `metamist-6.0.4/metamist/api/sequencing_group_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/api/web_api.py` & `metamist-6.0.4/metamist/api/web_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/api_client.py` & `metamist-6.0.4/metamist/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
```

### Comparing `metamist-6.0.3/metamist/apis/__init__.py` & `metamist-6.0.4/metamist/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/metamist/configuration.py` & `metamist-6.0.4/metamist/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 from os import getenv
 import json
 import copy
@@ -401,15 +401,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 6.0.3\n"\
+               "Version of the API: 6.0.4\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `metamist-6.0.3/metamist/exceptions.py` & `metamist-6.0.4/metamist/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `metamist-6.0.3/metamist/graphql/__init__.py` & `metamist-6.0.4/metamist/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/metamist/graphql/schema.graphql` & `metamist-6.0.4/metamist/graphql/schema.graphql`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,17 @@
   participants: [GraphQLParticipant!]!
 }
 
 type GraphQLParticipant {
   id: Int!
   externalId: String!
   meta: JSON!
+  reportedSex: Int
+  reportedGender: String
+  karyotype: String
   samples(type: StrGraphQLFilter = null, meta: JSON = null, active: BoolGraphQLFilter = null): [GraphQLSample!]!
   families: [GraphQLFamily!]!
   project: GraphQLProject!
 }
 
 type GraphQLProject {
   id: Int!
@@ -89,24 +92,24 @@
   active: Boolean!
   meta: JSON!
   type: String!
   author: String
   participant: GraphQLParticipant
   assays(type: StrGraphQLFilter = null): [GraphQLAssay!]!
   project: GraphQLProject!
-  sequencingGroups(type: StrGraphQLFilter = null, technology: StrGraphQLFilter = null, platform: StrGraphQLFilter = null, meta: JSON = null, activeOnly: BoolGraphQLFilter = null): [GraphQLSequencingGroup!]!
+  sequencingGroups(id: StrGraphQLFilter = null, type: StrGraphQLFilter = null, technology: StrGraphQLFilter = null, platform: StrGraphQLFilter = null, meta: JSON = null, activeOnly: BoolGraphQLFilter = null): [GraphQLSequencingGroup!]!
 }
 
 type GraphQLSequencingGroup {
   id: String!
   type: String!
   technology: String!
   platform: String!
   meta: JSON!
-  externalIds: JSON!
+  externalIds: JSON
   sample: GraphQLSample!
   analyses(status: AnalysisStatusGraphQLFilter = null, type: StrGraphQLFilter = null, meta: JSON = null, active: BoolGraphQLFilter = null): [GraphQLAnalysis!]!
   assays: [GraphQLAssay!]!
 }
 
 """Filter for GraphQL queries"""
 input IntGraphQLFilter {
```

### Comparing `metamist-6.0.3/metamist/model/analysis.py` & `metamist-6.0.4/metamist/model/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/analysis_query_model.py` & `metamist-6.0.4/metamist/model/analysis_query_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/analysis_status.py` & `metamist-6.0.4/metamist/model/analysis_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/analysis_update_model.py` & `metamist-6.0.4/metamist/model/analysis_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/assay.py` & `metamist-6.0.4/metamist/model/assay.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/assay_upsert.py` & `metamist-6.0.4/metamist/model/assay_upsert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/body_get_assays_by_criteria.py` & `metamist-6.0.4/metamist/model/body_get_assays_by_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/body_get_latest_complete_analysis_for_type_post.py` & `metamist-6.0.4/metamist/model/body_get_latest_complete_analysis_for_type_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/body_get_participants.py` & `metamist-6.0.4/metamist/model/body_get_participants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/body_get_samples.py` & `metamist-6.0.4/metamist/model/body_get_samples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/error_response.py` & `metamist-6.0.4/metamist/model/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/export_type.py` & `metamist-6.0.4/metamist/model/export_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/extra_participant_importer_handler.py` & `metamist-6.0.4/metamist/model/extra_participant_importer_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/family_search_response_data.py` & `metamist-6.0.4/metamist/model/family_search_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/family_simple.py` & `metamist-6.0.4/metamist/model/family_simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/family_update_model.py` & `metamist-6.0.4/metamist/model/family_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/http_validation_error.py` & `metamist-6.0.4/metamist/model/http_validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/meta_search_entity_prefix.py` & `metamist-6.0.4/metamist/model/meta_search_entity_prefix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/nested_participant.py` & `metamist-6.0.4/metamist/model/nested_participant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/nested_sample.py` & `metamist-6.0.4/metamist/model/nested_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/nested_sequencing_group.py` & `metamist-6.0.4/metamist/model/nested_sequencing_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/paging_links.py` & `metamist-6.0.4/metamist/model/paging_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/participant_search_response_data.py` & `metamist-6.0.4/metamist/model/participant_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/participant_upsert.py` & `metamist-6.0.4/metamist/model/participant_upsert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/project.py` & `metamist-6.0.4/metamist/model/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/project_summary.py` & `metamist-6.0.4/metamist/model/project_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/sample_search_response_data.py` & `metamist-6.0.4/metamist/model/sample_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/sample_upsert.py` & `metamist-6.0.4/metamist/model/sample_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/search_item.py` & `metamist-6.0.4/metamist/model/search_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/search_response.py` & `metamist-6.0.4/metamist/model/search_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/search_response_model.py` & `metamist-6.0.4/metamist/model/search_response_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/search_response_type.py` & `metamist-6.0.4/metamist/model/search_response_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -51,14 +51,15 @@
     """
 
     allowed_values = {
         ('value',): {
             'FAMILY': "family",
             'PARTICIPANT': "participant",
             'SAMPLE': "sample",
+            'SEQUENCING-GROUP': "sequencing-group",
             'ERROR': "error",
         },
     }
 
     validations = {
     }
 
@@ -103,18 +104,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """SearchResponseType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Define types of search results., must be one of ["family", "participant", "sample", "error", ]  # noqa: E501
+            args[0] (str): Define types of search results., must be one of ["family", "participant", "sample", "sequencing-group", "error", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Define types of search results., must be one of ["family", "participant", "sample", "error", ]  # noqa: E501
+            value (str): Define types of search results., must be one of ["family", "participant", "sample", "sequencing-group", "error", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -193,18 +194,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """SearchResponseType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Define types of search results., must be one of ["family", "participant", "sample", "error", ]  # noqa: E501
+            args[0] (str): Define types of search results., must be one of ["family", "participant", "sample", "sequencing-group", "error", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Define types of search results., must be one of ["family", "participant", "sample", "error", ]  # noqa: E501
+            value (str): Define types of search results., must be one of ["family", "participant", "sample", "sequencing-group", "error", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `metamist-6.0.3/metamist/model/sequencing_group_upsert.py` & `metamist-6.0.4/metamist/model/sequencing_group_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/validation_error.py` & `metamist-6.0.4/metamist/model/validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model/web_project.py` & `metamist-6.0.4/metamist/model/web_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.3/metamist/model_utils.py` & `metamist-6.0.4/metamist/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `metamist-6.0.3/metamist/models/__init__.py` & `metamist-6.0.4/metamist/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,10 +37,11 @@
 from metamist.model.project_summary import ProjectSummary
 from metamist.model.sample_search_response_data import SampleSearchResponseData
 from metamist.model.sample_upsert import SampleUpsert
 from metamist.model.search_item import SearchItem
 from metamist.model.search_response import SearchResponse
 from metamist.model.search_response_model import SearchResponseModel
 from metamist.model.search_response_type import SearchResponseType
+from metamist.model.sequencing_group_search_response_data import SequencingGroupSearchResponseData
 from metamist.model.sequencing_group_upsert import SequencingGroupUpsert
 from metamist.model.validation_error import ValidationError
 from metamist.model.web_project import WebProject
```

### Comparing `metamist-6.0.3/metamist/parser/cloudhelper.py` & `metamist-6.0.4/metamist/parser/cloudhelper.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/metamist/parser/generic_metadata_parser.py` & `metamist-6.0.4/metamist/parser/generic_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/metamist/parser/generic_parser.py` & `metamist-6.0.4/metamist/parser/generic_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,16 +124,17 @@
 )
 QUERY_MATCH_ASSAYS = gql(
     """
 query GetSampleEidMapQuery($project: String!) {
   project(name: $project) {
     samples {
       assays {
-        externalIds
         id
+        externalIds
+        meta
       }
     }
   }
 }
 """
 )
 
@@ -791,15 +792,15 @@
                 raise TypeError(f'Unformmatted reads (expected file object): {reads}')
             raise ValueError(f'Unknown type {reads}')
 
         filename_meta_map = {
             reads_to_key(assay['meta']['reads']): assay['id']
             for sample in values['project']['samples']
             for assay in sample['assays']
-            if assay.get('meta', {}).get('reads')
+            if assay['meta'].get('reads')
         }
 
         def _map_assay(assay: ParsedAssay):
             # put it in a function so we can return early
 
             # external IDs match
             for exid in (assay.external_ids or {}).values():
```

### Comparing `metamist-6.0.3/metamist/parser/sample_file_map_parser.py` & `metamist-6.0.4/metamist/parser/sample_file_map_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/metamist/rest.py` & `metamist-6.0.4/metamist/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.3
+    The version of the OpenAPI document: 6.0.4
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `metamist-6.0.3/metamist.egg-info/PKG-INFO` & `metamist-6.0.4/metamist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.0.3
+Version: 6.0.4
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-6.0.3/metamist.egg-info/SOURCES.txt` & `metamist-6.0.4/metamist.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 metamist/model/project_summary.py
 metamist/model/sample_search_response_data.py
 metamist/model/sample_upsert.py
 metamist/model/search_item.py
 metamist/model/search_response.py
 metamist/model/search_response_model.py
 metamist/model/search_response_type.py
+metamist/model/sequencing_group_search_response_data.py
 metamist/model/sequencing_group_upsert.py
 metamist/model/validation_error.py
 metamist/model/web_project.py
 metamist/models/__init__.py
 metamist/parser/__init__.py
 metamist/parser/cloudhelper.py
 metamist/parser/generic_metadata_parser.py
```

### Comparing `metamist-6.0.3/setup.py` & `metamist-6.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='6.0.3',
+    version='6.0.4',
     description='Python API for interacting with the Sample API system',
     long_description=readme,
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/sample-metadata',
     license='MIT',
     packages=all_packages,
     install_requires=[
```

### Comparing `metamist-6.0.3/test/test_analysis.py` & `metamist-6.0.4/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_assay.py` & `metamist-6.0.4/test/test_assay.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_generate_data.py` & `metamist-6.0.4/test/test_generate_data.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_generic_filters.py` & `metamist-6.0.4/test/test_generic_filters.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_get_participants.py` & `metamist-6.0.4/test/test_get_participants.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_graphql.py` & `metamist-6.0.4/test/test_graphql.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,79 @@
 from test.testbase import DbIsolatedTest, run_as_sync
 from graphql.error import GraphQLError, GraphQLSyntaxError
 
-from db.python.layers import ParticipantLayer
+import api.graphql.schema
+from db.python.layers import ParticipantLayer, AnalysisLayer
 from models.models import (
     SampleUpsertInternal,
     ParticipantUpsertInternal,
     SequencingGroupUpsertInternal,
     AssayUpsertInternal,
+    AnalysisInternal,
 )
-import api.graphql.schema
+from models.utils.sequencing_group_id_format import sequencing_group_id_format
+from models.enums import AnalysisStatus
+
 from metamist.graphql import gql, validate, configure_sync_client
 
 
 default_assay_meta = {
     'sequencing_type': 'genome',
     'sequencing_technology': 'short-read',
     'sequencing_platform': 'illumina',
 }
 
-SINGLE_PARTICIPANT_UPSERT = ParticipantUpsertInternal(
-    external_id='Demeter',
-    meta={},
-    samples=[
-        SampleUpsertInternal(
-            external_id='sample_id001',
-            meta={},
-            type='blood',
-            sequencing_groups=[
-                SequencingGroupUpsertInternal(
-                    type='genome',
-                    technology='short-read',
-                    platform='illumina',
-                    assays=[
-                        AssayUpsertInternal(
-                            type='sequencing',
-                            meta={
-                                'reads': [
-                                    [
-                                        {
-                                            'basename': 'sample_id001.filename-R1.fastq.gz',
-                                            'checksum': None,
-                                            'class': 'File',
-                                            'location': '/path/to/sample_id001.filename-R1.fastq.gz',
-                                            'size': 111,
-                                        },
-                                        {
-                                            'basename': 'sample_id001.filename-R2.fastq.gz',
-                                            'checksum': None,
-                                            'class': 'File',
-                                            'location': '/path/to/sample_id001.filename-R2.fastq.gz',
-                                            'size': 111,
-                                        },
-                                    ]
-                                ],
-                                'reads_type': 'fastq',
-                                'batch': 'M001',
-                                **default_assay_meta,
-                            },
-                        ),
-                    ],
-                )
-            ],
-        )
-    ],
-)
+
+def _get_single_participant_upsert():
+
+    return ParticipantUpsertInternal(
+        external_id='Demeter',
+        meta={},
+        samples=[
+            SampleUpsertInternal(
+                external_id='sample_id001',
+                meta={},
+                type='blood',
+                sequencing_groups=[
+                    SequencingGroupUpsertInternal(
+                        type='genome',
+                        technology='short-read',
+                        platform='illumina',
+                        assays=[
+                            AssayUpsertInternal(
+                                type='sequencing',
+                                meta={
+                                    'reads': [
+                                            {
+                                                'basename': 'sample_id001.filename-R1.fastq.gz',
+                                                'checksum': None,
+                                                'class': 'File',
+                                                'location': '/path/to/sample_id001.filename-R1.fastq.gz',
+                                                'size': 111,
+                                            },
+                                            {
+                                                'basename': 'sample_id001.filename-R2.fastq.gz',
+                                                'checksum': None,
+                                                'class': 'File',
+                                                'location': '/path/to/sample_id001.filename-R2.fastq.gz',
+                                                'size': 111,
+                                            },
+                                    ],
+                                    'reads_type': 'fastq',
+                                    'batch': 'M001',
+                                    **default_assay_meta,
+                                },
+                            ),
+                        ],
+                    )
+                ],
+            )
+        ],
+    )
+
 
 TEST_QUERY = gql(
     """
 query MyQuery($project: String!) {
   project(name: $project) {
     participants {
       id
@@ -137,15 +143,17 @@
         )
         with self.assertRaises(GraphQLError):
             validate(query, use_local_schema=True)
 
     @run_as_sync
     async def test_basic_graphql_query(self):
         """Test getting the summary for a project"""
-        p = (await self.player.upsert_participants([SINGLE_PARTICIPANT_UPSERT]))[0]
+        p = (await self.player.upsert_participants([_get_single_participant_upsert()]))[
+            0
+        ]
 
         query = """
 query MyQuery($project: String!) {
   project(name: $project) {
     participants {
       id
       samples {
@@ -179,7 +187,47 @@
         assays = sequencing_groups[0]['assays']
         self.assertEqual(
             1, len(participants[0]['samples'][0]['sequencingGroups'][0]['assays'])
         )
         self.assertEqual(
             p.samples[0].sequencing_groups[0].assays[0].id, assays[0]['id']
         )
+
+    @run_as_sync
+    async def test_sg_analyses_query(self):
+        """Example graphql query of analyses from sequencing-group"""
+        p = await self.player.upsert_participant(_get_single_participant_upsert())
+        sg_id = p.samples[0].sequencing_groups[0].id
+
+        alayer = AnalysisLayer(self.connection)
+        await alayer.create_analysis(
+            AnalysisInternal(
+                sequencing_group_ids=[sg_id],
+                type='cram',
+                status=AnalysisStatus.COMPLETED,
+                meta={},
+                output='some-output',
+            )
+        )
+
+        q = """
+query MyQuery($sg_id: String!) {
+  sequencingGroups(id: {in_: [$sg_id]}) {
+    analyses {
+      id
+      meta
+      output
+    }
+  }
+}"""
+
+        resp = await self.run_graphql_query_async(
+            q, {'sg_id': sequencing_group_id_format(sg_id)}
+        )
+        self.assertIn('sequencingGroups', resp)
+        self.assertEqual(1, len(resp['sequencingGroups']))
+        self.assertIn('analyses', resp['sequencingGroups'][0])
+        self.assertEqual(1, len(resp['sequencingGroups'][0]['analyses']))
+        analyses = resp['sequencingGroups'][0]['analyses']
+        self.assertIn('id', analyses[0])
+        self.assertIn('meta', analyses[0])
+        self.assertIn('output', analyses[0])
```

### Comparing `metamist-6.0.3/test/test_import_individual_metadata.py` & `metamist-6.0.4/test/test_import_individual_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_metamist.py` & `metamist-6.0.4/test/test_metamist.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_models.py` & `metamist-6.0.4/test/test_models.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_parse_existing_cohort.py` & `metamist-6.0.4/test/test_parse_existing_cohort.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_parse_file_map.py` & `metamist-6.0.4/test/test_parse_file_map.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_parse_generic_metadata.py` & `metamist-6.0.4/test/test_parse_generic_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,89 @@
 import unittest
 from datetime import datetime
 from io import StringIO
 from unittest.mock import patch
 
 from test.testbase import run_as_sync, DbIsolatedTest
 
+import api.graphql.schema
+from db.python.layers import ParticipantLayer
+from models.models import (
+    ParticipantUpsertInternal,
+    SampleUpsertInternal,
+    SequencingGroupUpsertInternal,
+    AssayUpsertInternal,
+)
+from models.utils.sample_id_format import sample_id_format
+from models.utils.sequencing_group_id_format import sequencing_group_id_format
+
 from metamist.graphql import validate, configure_sync_client
 from metamist.parser.generic_parser import (
     ParsedParticipant,
     ParsedSample,
     QUERY_MATCH_PARTICIPANTS,
     QUERY_MATCH_SAMPLES,
     QUERY_MATCH_SEQUENCING_GROUPS,
     QUERY_MATCH_ASSAYS,
+    ParsedSequencingGroup,
 )
 from metamist.parser.generic_metadata_parser import GenericMetadataParser
 
-import api.graphql.schema
+
+def _get_basic_participant_to_upsert():
+    default_assay_meta = {
+        'sequencing_type': 'genome',
+        'sequencing_technology': 'short-read',
+        'sequencing_platform': 'illumina',
+    }
+
+    return ParticipantUpsertInternal(
+        external_id='Demeter',
+        meta={},
+        samples=[
+            SampleUpsertInternal(
+                external_id='sample_id001',
+                meta={},
+                type='blood',
+                sequencing_groups=[
+                    SequencingGroupUpsertInternal(
+                        type='genome',
+                        technology='short-read',
+                        platform='illumina',
+                        assays=[
+                            AssayUpsertInternal(
+                                type='sequencing',
+                                meta={
+                                    'reads': [
+                                        {
+                                            'basename': 'sample_id001.filename-R1.fastq.gz',
+                                            'checksum': None,
+                                            'class': 'File',
+                                            'location': '/path/to/sample_id001.filename-R1.fastq.gz',
+                                            'size': 111,
+                                        },
+                                        {
+                                            'basename': 'sample_id001.filename-R2.fastq.gz',
+                                            'checksum': None,
+                                            'class': 'File',
+                                            'location': '/path/to/sample_id001.filename-R2.fastq.gz',
+                                            'size': 111,
+                                        },
+                                    ],
+                                    'reads_type': 'fastq',
+                                    'batch': 'M001',
+                                    **default_assay_meta,
+                                },
+                            ),
+                        ],
+                    )
+                ],
+            )
+        ],
+    )
 
 
 class TestValidateParserQueries(unittest.TestCase):
     """
     Validate queries used by the GenericParser
     """
 
@@ -667,14 +730,88 @@
                 StringIO(file_contents), delimiter='\t', dry_run=True
             )
         self.assertEqual(
             'Multiple reference assemblies were defined for sample_id003: ref.fa, ref2.fa',
             str(ctx.exception),
         )
 
+    @run_as_sync
+    @patch('metamist.parser.generic_parser.query_async')
+    @patch('metamist.parser.cloudhelper.CloudHelper.datetime_added')
+    @patch('metamist.parser.cloudhelper.CloudHelper.file_exists')
+    @patch('metamist.parser.cloudhelper.CloudHelper.file_size')
+    async def test_matching_sequencing_groups_and_assays(
+        self, mock_filesize, mock_fileexists, mock_datetime_added, mock_graphql_query
+    ):
+        """Test basic import with data that exists in the database"""
+        mock_graphql_query.side_effect = self.run_graphql_query_async
+        mock_filesize.return_value = 111
+        mock_fileexists.return_value = False
+        mock_datetime_added.return_value = datetime.fromisoformat('2022-02-02T22:22:22')
+
+        player = ParticipantLayer(self.connection)
+        participant = await player.upsert_participant(_get_basic_participant_to_upsert())
+
+        filenames = [
+            'sample_id001.filename-R1.fastq.gz',
+            'sample_id001.filename-R2.fastq.gz',
+        ]
+
+        rows = [
+            'Participant ID\tSample ID\tFilename',
+            f'Demeter\tsample_id001\t{filenames[0]}',
+            f'Demeter\tsample_id001\t{filenames[1]}',
+        ]
+
+        parser = GenericMetadataParser(
+            search_locations=[],
+            participant_column='Participant ID',
+            sample_name_column='Sample ID',
+            reads_column='Filename',
+            participant_meta_map={},
+            sample_meta_map={},
+            assay_meta_map={},
+            qc_meta_map={},
+            # doesn't matter, we're going to mock the call anyway
+            project=self.project_name,
+        )
+
+        parser.filename_map = {f: '/path/to/' + f for f in filenames}
+
+        summary, parsed_files = await parser.parse_manifest(
+            StringIO('\n'.join(rows)), delimiter='\t', dry_run=True
+        )
+
+        self.assertEqual(1, summary['participants']['update'])
+        self.assertEqual(1, summary['samples']['update'])
+        self.assertEqual(1, summary['sequencing_groups']['update'])
+        self.assertEqual(1, summary['assays']['update'])
+        self.assertEqual(0, summary['participants']['insert'])
+        self.assertEqual(0, summary['samples']['insert'])
+        self.assertEqual(0, summary['sequencing_groups']['insert'])
+        self.assertEqual(0, summary['assays']['insert'])
+
+        parsed_p: ParsedParticipant = parsed_files[0]
+        self.assertEqual(participant.id, parsed_p.internal_pid)
+        self.assertEqual(
+            sample_id_format(participant.samples[0].id),
+            parsed_p.samples[0].internal_sid,
+        )
+
+        sg: SequencingGroupUpsertInternal = participant.samples[0].sequencing_groups[0]
+        sg_parsed: ParsedSequencingGroup = (
+            parsed_files[0].samples[0].sequencing_groups[0]
+        )
+
+        self.assertEqual(
+            sequencing_group_id_format(sg.id), sg_parsed.internal_seqgroup_id
+        )
+        self.assertEqual(len(sg.assays), len(sg_parsed.assays))
+        self.assertEqual(sg.assays[0].id, sg_parsed.assays[0].internal_id)
+
 
 class FastqPairMatcher(unittest.TestCase):
     """Test Fastq pair matching logic explictly"""
 
     def test_simple(self):
         """Simple fastq pair matching case"""
         entries = [
```

### Comparing `metamist-6.0.3/test/test_parse_ont_processor.py` & `metamist-6.0.4/test/test_parse_ont_processor.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_parse_ont_sheet.py` & `metamist-6.0.4/test/test_parse_ont_sheet.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_pedigree.py` & `metamist-6.0.4/test/test_pedigree.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_sample.py` & `metamist-6.0.4/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_search.py` & `metamist-6.0.4/test/test_search.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from test.testbase import DbIsolatedTest, run_as_sync
 
 from db.python.layers.participant import ParticipantLayer
 from db.python.layers.sample import SampleLayer
 from db.python.layers.search import SearchLayer
 from db.python.layers.family import FamilyLayer
+from db.python.layers.sequencing_group import SequencingGroupLayer
 from db.python.tables.family_participant import FamilyParticipantTable
 
 from models.enums import SearchResponseType
 from models.models.family import PedRowInternal
 from models.models.sample import sample_id_format, SampleUpsertInternal
 from models.models.participant import ParticipantUpsertInternal
+from models.models.sequencing_group import SequencingGroupUpsertInternal, sequencing_group_id_format
+from models.models.assay import AssayUpsertInternal
 
 
 class TestSample(DbIsolatedTest):
     """Test sample class"""
 
     # tests run in 'sorted by ascii' order
     @run_as_sync
     async def setUp(self) -> None:
         super().setUp()
 
         self.schlay = SearchLayer(self.connection)
         self.slayer = SampleLayer(self.connection)
         self.player = ParticipantLayer(self.connection)
         self.flayer = FamilyLayer(self.connection)
+        self.sglayer = SequencingGroupLayer(self.connection)
 
     @run_as_sync
     async def test_search_non_existent_sample_by_internal_id(self):
         """
         Search by CPG sample ID that doesn't exist
         """
         cpg_id = sample_id_format(9_999_999_999)
@@ -63,14 +67,55 @@
 
         self.assertEqual(1, len(results))
         self.assertEqual(cpg_id, results[0].title)
         self.assertEqual(cpg_id, results[0].data.id)
         self.assertListEqual(['EX001'], results[0].data.sample_external_ids)
 
     @run_as_sync
+    async def test_search_isolated_sequencing_group_by_id(self):
+        """
+        Search by valid CPG sequencing group ID (special case)
+        """
+        sample = await self.slayer.upsert_sample(
+            SampleUpsertInternal(external_id='EXS001', type='blood')
+        )
+        sg = await self.sglayer.upsert_sequencing_groups(
+            [
+                SequencingGroupUpsertInternal(
+                    sample_id=sample.id,
+                    technology='long-read',
+                    platform='illumina',
+                    meta={
+                        'sequencing_type': 'transcriptome',
+                        'sequencing_technology': 'long-read',
+                        'sequencing_platform': 'illumina',
+                    },
+                    type='transcriptome',
+                    assays=[
+                        AssayUpsertInternal(
+                            type='sequencing',
+                            meta={
+                                'sequencing_type': 'transcriptome',
+                                'sequencing_technology': 'long-read',
+                                'sequencing_platform': 'illumina',
+                            }
+                        )
+                    ]
+                )
+            ]
+        )
+        cpg_sg_id = sequencing_group_id_format(sg[0].id)
+        results = await self.schlay.search(query=cpg_sg_id, project_ids=[self.project_id])
+
+        self.assertEqual(1, len(results))
+        self.assertEqual(cpg_sg_id, results[0].title)
+        self.assertEqual(cpg_sg_id, results[0].data.id)
+        self.assertEqual(cpg_sg_id, results[0].data.sg_external_id)
+
+    @run_as_sync
     async def test_search_isolated_sample_by_external_id(self):
         """
         Search by External sample ID with no participant / family,
         should only return one result
         """
         sample = await self.slayer.upsert_sample(
             SampleUpsertInternal(external_id='EX001', type='blood')
```

### Comparing `metamist-6.0.3/test/test_sequencing_groups.py` & `metamist-6.0.4/test/test_sequencing_groups.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_upsert.py` & `metamist-6.0.4/test/test_upsert.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.3/test/test_web.py` & `metamist-6.0.4/test/test_web.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,30 +67,28 @@
                         technology='short-read',
                         platform='illumina',
                         assays=[
                             AssayUpsertInternal(
                                 type='sequencing',
                                 meta={
                                     'reads': [
-                                        [
                                             {
                                                 'basename': 'sample_id001.filename-R1.fastq.gz',
                                                 'checksum': None,
                                                 'class': 'File',
                                                 'location': '/path/to/sample_id001.filename-R1.fastq.gz',
                                                 'size': 111,
                                             },
                                             {
                                                 'basename': 'sample_id001.filename-R2.fastq.gz',
                                                 'checksum': None,
                                                 'class': 'File',
                                                 'location': '/path/to/sample_id001.filename-R2.fastq.gz',
                                                 'size': 111,
                                             },
-                                        ]
                                     ],
                                     'reads_type': 'fastq',
                                     'batch': 'M001',
                                     **default_assay_meta,
                                 },
                             ),
                         ],
@@ -170,19 +168,20 @@
     sample_keys=[
         ('id', 'Sample ID'),
         ('external_id', 'External Sample ID'),
         ('created_date', 'Created date'),
     ],
     sequencing_group_keys=[
         ('id', 'Sequencing Group ID'),
-        ('created_date', 'Created date'),
+        ('platform', 'Platform'),
+        ('technology', 'Technology'),
+        ('type', 'Type'),
     ],
     assay_keys=[
         ('type', 'type'),
-        ('technology', 'technology'),
         ('meta.batch', 'batch'),
         ('meta.reads_type', 'reads_type'),
     ],
     seqr_links={},
     seqr_sync_types=[],
 )
 
@@ -357,19 +356,20 @@
             sample_keys=[
                 ('id', 'Sample ID'),
                 ('external_id', 'External Sample ID'),
                 ('created_date', 'Created date'),
             ],
             sequencing_group_keys=[
                 ('id', 'Sequencing Group ID'),
-                ('created_date', 'Created date'),
+                ('platform', 'Platform'),
+                ('technology', 'Technology'),
+                ('type', 'Type'),
             ],
             assay_keys=[
                 ('type', 'type'),
-                ('technology', 'technology'),
                 ('meta.batch', 'batch'),
                 ('meta.field with spaces', 'field with spaces'),
                 ('meta.reads_type', 'reads_type'),
             ],
             seqr_links={},
             seqr_sync_types=[],
         )
@@ -409,19 +409,20 @@
             sample_keys=[
                 ('id', 'Sample ID'),
                 ('external_id', 'External Sample ID'),
                 ('created_date', 'Created date'),
             ],
             sequencing_group_keys=[
                 ('id', 'Sequencing Group ID'),
-                ('created_date', 'Created date'),
+                ('platform', 'Platform'),
+                ('technology', 'Technology'),
+                ('type', 'Type'),
             ],
             assay_keys=[
                 ('type', 'type'),
-                ('technology', 'technology'),
                 ('meta.batch', 'batch'),
                 ('meta.field with spaces', 'field with spaces'),
                 ('meta.reads_type', 'reads_type'),
             ],
             seqr_links={},
             seqr_sync_types=[],
         )
@@ -486,19 +487,20 @@
             sample_keys=[
                 ('id', 'Sample ID'),
                 ('external_id', 'External Sample ID'),
                 ('created_date', 'Created date'),
             ],
             sequencing_group_keys=[
                 ('id', 'Sequencing Group ID'),
-                ('created_date', 'Created date'),
+                ('platform', 'Platform'),
+                ('technology', 'Technology'),
+                ('type', 'Type'),
             ],
             assay_keys=[
                 ('type', 'type'),
-                ('technology', 'technology'),
                 ('meta.batch', 'batch'),
                 ('meta.field with spaces', 'field with spaces'),
                 ('meta.reads_type', 'reads_type'),
             ],
             seqr_links={},
             seqr_sync_types=[],
         )
```

### Comparing `metamist-6.0.3/test/testbase.py` & `metamist-6.0.4/test/testbase.py`

 * *Files identical despite different names*

